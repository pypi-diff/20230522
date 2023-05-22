# Comparing `tmp/torchmd-0.0.4.tar.gz` & `tmp/torchmd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmd-0.0.4.tar", last modified: Wed Apr 12 18:04:38 2023, max compression
+gzip compressed data, was "torchmd-1.0.0.tar", last modified: Mon May 22 17:03:54 2023, max compression
```

## Comparing `torchmd-0.0.4.tar` & `torchmd-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.820437 torchmd-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-12 18:04:01.000000 torchmd-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 18:04:01.000000 torchmd-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-12 18:04:38.820437 torchmd-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-12 18:04:01.000000 torchmd-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 18:04:01.000000 torchmd-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:04:38.820437 torchmd-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 18:04:01.000000 torchmd-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.816437 torchmd-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-04-12 18:04:01.000000 torchmd-0.0.4/tests/test_torchmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.820437 torchmd-0.0.4/torchmd/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 18:04:38.820437 torchmd-0.0.4/torchmd/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.820437 torchmd-0.0.4/torchmd/forcefields/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forcefields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forcefields/ff_parmed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forcefields/ff_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forcefields/forcefield.py
--rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/minimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/mycalc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/neighbourlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.820437 torchmd-0.0.4/torchmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.839715 torchmd-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-22 17:03:11.000000 torchmd-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 17:03:11.000000 torchmd-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-22 17:03:54.839715 torchmd-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-22 17:03:11.000000 torchmd-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 17:03:11.000000 torchmd-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:03:54.839715 torchmd-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 17:03:11.000000 torchmd-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.831715 torchmd-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-05-22 17:03:12.000000 torchmd-1.0.0/tests/test_torchmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.839715 torchmd-1.0.0/torchmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-22 17:03:54.839715 torchmd-1.0.0/torchmd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.839715 torchmd-1.0.0/torchmd/forcefields/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forcefields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forcefields/ff_parmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forcefields/ff_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forcefields/forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/minimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/mycalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/neighbourlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.839715 torchmd-1.0.0/torchmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/top_level.txt
```

### Comparing `torchmd-0.0.4/LICENSE.md` & `torchmd-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/PKG-INFO` & `torchmd-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmd
-Version: 0.0.4
+Version: 1.0.0
 Summary: TorchMD. Molecular dynamics with pytorch
 Author-email: Acellera <info@acellera.com>
 License: Copyright (c) 2020 Acellera
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,15 +20,17 @@
 
 # TorchMD
 
 ## About
 
 TorchMD intends to provide a simple to use API for performing molecular dynamics using PyTorch. This enables researchers to more rapidly do research in force-field development as well as integrate seamlessly neural network potentials into the dynamics, with the simplicity and power of PyTorch.
 
-TorchMD is currently WIP so feel free to provide feedback on the API or potential bugs in the GitHub issue tracker.
+TorchMD is currently WIP so feel free to provide feedback on the API or potential bugs in the GitHub issue tracker. 
+
+Also check TorchMD-Net for fast and accurate neural network potentials https://github.com/torchmd/torchmd-net/
 
 ## Citation
 
 Please cite:
 
 ```
 @misc{doerr2020torchmd,
```

### Comparing `torchmd-0.0.4/README.md` & `torchmd-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # TorchMD
 
 ## About
 
 TorchMD intends to provide a simple to use API for performing molecular dynamics using PyTorch. This enables researchers to more rapidly do research in force-field development as well as integrate seamlessly neural network potentials into the dynamics, with the simplicity and power of PyTorch.
 
-TorchMD is currently WIP so feel free to provide feedback on the API or potential bugs in the GitHub issue tracker.
+TorchMD is currently WIP so feel free to provide feedback on the API or potential bugs in the GitHub issue tracker. 
+
+Also check TorchMD-Net for fast and accurate neural network potentials https://github.com/torchmd/torchmd-net/
 
 ## Citation
 
 Please cite:
 
 ```
 @misc{doerr2020torchmd,
```

### Comparing `torchmd-0.0.4/pyproject.toml` & `torchmd-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/tests/test_torchmd.py` & `torchmd-1.0.0/tests/test_torchmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,28 +295,24 @@
         from glob import glob
         import parmed
         import os
         import logging
 
         logging.getLogger("parmed.structure").setLevel("ERROR")
 
-        # for d in glob(os.path.join("test-data", "*", "")):
-        # for d in [
-        #     "test-data/prod_alanine_dipeptide_amber/",
-        # ]:
         terms = [
             "bonds",
             "angles",
             "dihedrals",
             "impropers",
             "1-4",
             "electrostatics",
             "lj",
         ]
-        for d in glob(os.path.join("test-data", "*", "")):
+        for d in glob(os.path.join("tests/data", "*", "")):
             with self.subTest(system=d):
                 print("\nRunning test:", d)
                 testname = os.path.basename(os.path.abspath(d))
                 if testname == "thrombin-ligand-amber":
                     abstol = 1e-1
                 elif testname == "waterbox":
                     abstol = 1e-3
@@ -385,15 +381,15 @@
                         keepForces(prm, struct, mol, forces=forceOMM)
                     elif len(prmtopFile):
                         struct = parmed.load_file(prmtopFile[0])
                         prm = parmed.amber.AmberParameterSet().from_structure(struct)
                         keepForces(prm, struct, mol, forces=forceOMM)
                         keepForcesAmber(struct, mol, forces=forceOMM)
 
-                    if d == "test-data/waterbox/":
+                    if d == "tests/data/waterbox/":
                         # I don't support multi-frame evaluation yet
                         mol.dropFrames(keep=0)
 
                     ff = ForceField.create(mol, prm)
                     parameters = Parameters(ff, mol, precision=precision, device=device)
                     system = getTorchMDSystem(mol, device, precision)
                     forces = Forces(
@@ -468,15 +464,15 @@
     def test_replicas(self):
         from moleculekit.molecule import Molecule
         from torchmd.systems import System
         import os
 
         n_replicas = 2
 
-        testdir = os.path.join("test-data", "prod_alanine_dipeptide_amber")
+        testdir = os.path.join("tests/data", "prod_alanine_dipeptide_amber")
         mol = Molecule(os.path.join(testdir, "structure.prmtop"))
         mol.read(os.path.join(testdir, "input.coor"))
         struct = parmed.load_file(os.path.join(testdir, "structure.prmtop"))
         prm = parmed.amber.AmberParameterSet().from_structure(struct)
         terms = [
             "bonds",
             "angles",
```

### Comparing `torchmd-0.0.4/torchmd/forcefields/ff_parmed.py` & `torchmd-1.0.0/torchmd/forcefields/ff_parmed.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/forcefields/ff_yaml.py` & `torchmd-1.0.0/torchmd/forcefields/ff_yaml.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/forcefields/forcefield.py` & `torchmd-1.0.0/torchmd/forcefields/forcefield.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/forces.py` & `torchmd-1.0.0/torchmd/forces.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/integrator.py` & `torchmd-1.0.0/torchmd/integrator.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/minimizers.py` & `torchmd-1.0.0/torchmd/minimizers.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/mycalc.py` & `torchmd-1.0.0/torchmd/mycalc.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/neighbourlist.py` & `torchmd-1.0.0/torchmd/neighbourlist.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/parameters.py` & `torchmd-1.0.0/torchmd/parameters.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/run.py` & `torchmd-1.0.0/torchmd/run.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/systems.py` & `torchmd-1.0.0/torchmd/systems.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/utils.py` & `torchmd-1.0.0/torchmd/utils.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd/wrapper.py` & `torchmd-1.0.0/torchmd/wrapper.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.4/torchmd.egg-info/PKG-INFO` & `torchmd-1.0.0/torchmd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmd
-Version: 0.0.4
+Version: 1.0.0
 Summary: TorchMD. Molecular dynamics with pytorch
 Author-email: Acellera <info@acellera.com>
 License: Copyright (c) 2020 Acellera
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,15 +20,17 @@
 
 # TorchMD
 
 ## About
 
 TorchMD intends to provide a simple to use API for performing molecular dynamics using PyTorch. This enables researchers to more rapidly do research in force-field development as well as integrate seamlessly neural network potentials into the dynamics, with the simplicity and power of PyTorch.
 
-TorchMD is currently WIP so feel free to provide feedback on the API or potential bugs in the GitHub issue tracker.
+TorchMD is currently WIP so feel free to provide feedback on the API or potential bugs in the GitHub issue tracker. 
+
+Also check TorchMD-Net for fast and accurate neural network potentials https://github.com/torchmd/torchmd-net/
 
 ## Citation
 
 Please cite:
 
 ```
 @misc{doerr2020torchmd,
```

### Comparing `torchmd-0.0.4/torchmd.egg-info/SOURCES.txt` & `torchmd-1.0.0/torchmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

