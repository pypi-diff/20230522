# Comparing `tmp/hypothesis-rdkit-0.1.tar.gz` & `tmp/hypothesis-rdkit-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis-rdkit-0.1.tar", last modified: Mon Feb 20 00:21:09 2023, max compression
+gzip compressed data, was "hypothesis-rdkit-0.3.tar", last modified: Mon May 22 11:13:14 2023, max compression
```

## Comparing `hypothesis-rdkit-0.1.tar` & `hypothesis-rdkit-0.3.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.1/MANIFEST.in
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1269 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      829 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.1/README.md
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/hypothesis_rdkit/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       24 2023-02-19 23:11:07.000000 hypothesis-rdkit-0.1/hypothesis_rdkit/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)   441809 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.1/hypothesis_rdkit/fragments.smi
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      199 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.1/hypothesis_rdkit/hook.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     6131 2023-02-19 23:39:15.000000 hypothesis-rdkit-0.1/hypothesis_rdkit/strategy.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1269 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      386 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/SOURCES.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/dependency_links.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       62 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/entry_points.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/requires.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/top_level.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/setup.cfg
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      768 2023-02-20 00:20:56.000000 hypothesis-rdkit-0.1/setup.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-22 11:13:14.984404 hypothesis-rdkit-0.3/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1081 2023-03-06 20:54:00.000000 hypothesis-rdkit-0.3/LICENSE
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.3/MANIFEST.in
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1475 2023-05-22 11:13:14.984404 hypothesis-rdkit-0.3/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      829 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.3/README.md
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-22 11:13:14.984404 hypothesis-rdkit-0.3/hypothesis_rdkit/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       24 2023-02-19 23:11:07.000000 hypothesis-rdkit-0.3/hypothesis_rdkit/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)   441944 2023-03-23 14:59:34.000000 hypothesis-rdkit-0.3/hypothesis_rdkit/fragments.smi
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      199 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.3/hypothesis_rdkit/hook.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     8995 2023-03-24 09:26:52.000000 hypothesis-rdkit-0.3/hypothesis_rdkit/strategy.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-22 11:13:14.984404 hypothesis-rdkit-0.3/hypothesis_rdkit.egg-info/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1475 2023-05-22 11:13:14.000000 hypothesis-rdkit-0.3/hypothesis_rdkit.egg-info/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      459 2023-05-22 11:13:14.000000 hypothesis-rdkit-0.3/hypothesis_rdkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-05-22 11:13:14.000000 hypothesis-rdkit-0.3/hypothesis_rdkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       62 2023-05-22 11:13:14.000000 hypothesis-rdkit-0.3/hypothesis_rdkit.egg-info/entry_points.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       30 2023-05-22 11:13:14.000000 hypothesis-rdkit-0.3/hypothesis_rdkit.egg-info/requires.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-05-22 11:13:14.000000 hypothesis-rdkit-0.3/hypothesis_rdkit.egg-info/top_level.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-05-22 11:13:14.984404 hypothesis-rdkit-0.3/setup.cfg
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1006 2023-05-22 11:08:22.000000 hypothesis-rdkit-0.3/setup.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-22 11:13:14.984404 hypothesis-rdkit-0.3/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      648 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.3/tests/test_mol_blocks.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      784 2023-03-22 19:40:08.000000 hypothesis-rdkit-0.3/tests/test_mols.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      607 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.3/tests/test_smiles.py
```

### Comparing `hypothesis-rdkit-0.1/PKG-INFO` & `hypothesis-rdkit-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: hypothesis-rdkit
-Version: 0.1
+Version: 0.3
 Home-page: https://github.com/shirte/hypothesis-rdkit
 Maintainer: Steffen Hirte
 Maintainer-email: shirte@users.noreply.github.com
+License: MIT
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Framework :: Hypothesis
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
 # hypothesis-rdkit
 
 ## Installation
 
 ```sh
 pip install -U hypothesis-rdkit
```

### Comparing `hypothesis-rdkit-0.1/README.md` & `hypothesis-rdkit-0.3/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.1/hypothesis_rdkit/fragments.smi` & `hypothesis-rdkit-0.3/hypothesis_rdkit/fragments.smi`

 * *Files 1% similar despite different names*

```diff
@@ -1630,14 +1630,30 @@
 Nc1ccc2c(O)c(/N=N/c3ccc4c(O)cc(S(=O)(=O)O)cc4c3)c(S(=O)(=O)O)cc2c1
 CCCCCCCC(=O)/N=c1\c2c3c(ccc2cc2n1CCc1cc4c(cc1-2)OCO4)OCO3
 CC1=C(C)C(=O)O[C@@H]([C@]2(C)OC(=O)[C@]34CC[C@H]5[C@@H](C[C@H]6O[C@]67[C@@H](O)CCC(=O)[C@]57C)[C@@H]3CC[C@H]24)C1
 C=C(C)[C@@H]1CC[C@]2(C)CC[C@]3(C)[C@H](CC[C@@H]4[C@@]5(C)Cc6c([nH]c7ccc(Cl)cc67)C(C)(C)[C@@H]5CC[C@]43C)[C@@H]12
 C=C(C)[C@@H]1CC[C@]2(C)CC[C@]3(C)[C@H](CC[C@@H]4[C@@]5(C)CC[C@H](N(O)c6ccccc6)C(C)(C)[C@@H]5CC[C@]43C)[C@@H]12
 C[C@]12C(=O)C[C@@H](O)C=C1C=C[C@@H]1[C@@H]2CC[C@]2(O)C(=O)O[C@@]3(C)[C@H]4C[C@]5(C)[C@@H](CO[C@@]16O[C@@]32[C@H]5C6=O)C(=O)O4
 C[C@@H]1C(=O)O[C@H]2[C@@H]1O[C@]13O[C@@]4(CC[C@]5(C)C(=O)[C@](C)(O)[C@@]2(O)[C@H]15)C[C@]12OC(=O)C[C@H]1OC(C)(C)[C@@H]2[C@@H](O)C[C@H]4C3=O
+[1*][H]
+[2*][H]
+[3*][H]
+[4*][H]
+[5*][H]
+[6*][H]
+[7*][H]
+[8*][H]
+[9*][H]
+[10*][H]
+[11*][H]
+[12*][H]
+[13*][H]
+[14*][H]
+[15*][H]
+[16*][H]
 [4*]CC
 [3*]ON
 [5*]NC
 [7*]CC
 [8*]CO
 [8*]CF
 [8*]CS
```

### Comparing `hypothesis-rdkit-0.1/hypothesis_rdkit/strategy.py` & `hypothesis-rdkit-0.3/hypothesis_rdkit/strategy.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,27 +9,36 @@
     CombineMols,
     Mol,
     MolFromSmiles,
     MolToMolBlock,
     MolToSmiles,
     RemoveHs,
     SanitizeMol,
+    rdMolDescriptors,
+    BondType,
 )
 from rdkit.Chem.BRICS import reverseReactions
 
 __all__ = ["mols", "smiles", "mol_blocks"]
 
 
+# load a set of fragments (encoded as smiles) from a file
 with pkg_resources.resource_stream(__name__, "fragments.smi") as f:
-    fragments = [MolFromSmiles(line) for line in f]
+
+    def _parse_line(line):
+        m = MolFromSmiles(line)
+        rotatable_bonds = rdMolDescriptors.CalcNumRotatableBonds(m)
+        return m, rotatable_bonds
+
+    fragments = [_parse_line(line) for line in f]
 
 possible_dummy_labels = set(
     [
         a.GetIsotope()
-        for fragment in fragments
+        for fragment, _ in fragments
         for a in fragment.GetAtoms()
         if a.GetSymbol() == "*"
     ]
 )
 
 
 def has_dummy_atom(fragment, dummy_label):
@@ -58,90 +67,143 @@
         if has_dummy_atom(r._matchers[1], dummy_label)
     ]
     for dummy_label in possible_dummy_labels
 }
 
 # mapping dummy atom d to fragments containing d
 compatible_fragments = defaultdict(list)
-for fragment in fragments:
+for fragment, n in fragments:
     for a in fragment.GetAtoms():
         if a.GetSymbol() == "*":
             dummy_label = a.GetIsotope()
-            compatible_fragments[dummy_label].append(fragment)
+            compatible_fragments[dummy_label].append((fragment, n))
+
 
 # sort the lists in each key by number of dummy atoms in the fragment and fragment size
 def num_dummy_atoms(mol):
     return sum([1 for a in mol.GetAtoms() if a.GetSymbol() == "*"])
 
 
 for dummy_label in possible_dummy_labels:
     compatible_fragments[dummy_label] = sorted(
         compatible_fragments[dummy_label],
-        key=lambda x: (num_dummy_atoms(x), x.GetNumAtoms()),
+        key=lambda x: (num_dummy_atoms(x[0]), x[0].GetNumAtoms()),
     )
 
 
 dummy_pattern = MolFromSmiles("[*]")
 
 
 @st.composite
 def mols(
     draw,
     name=st.text(alphabet=list(string.ascii_lowercase), min_size=1),
+    max_rotatable_bonds=st.just(10),
     n_connected_components=st.just(1),
 ):
     """Strategy for generating random molecules.
 
     Parameters
     ----------
     name : str or hypothesis.strategies.SearchStrategy
         Name of the molecule.
+    max_rotatable_bonds : int or hypothesis.strategies.SearchStrategy
+        Maximum number of rotatable bonds in the molecule. If
+        n_connected_components > 1, each individual component will have less
+        rotatable bonds than max_rotatable_bonds.
     n_connected_components : int or hypothesis.strategies.SearchStrategy
         Number of connected components in the molecule.
     """
     if isinstance(name, str):
         name = st.just(name)
     if isinstance(n_connected_components, int):
         n_connected_components = st.just(n_connected_components)
+    if isinstance(max_rotatable_bonds, int):
+        max_rotatable_bonds = st.just(max_rotatable_bonds)
 
+    max_rotatable_bonds = draw(max_rotatable_bonds)
     n_connected_components = draw(n_connected_components)
 
     # draw connected components independently
     if n_connected_components > 1:
         components = [
-            draw(mols(n_connected_components=1)) for _ in range(n_connected_components)
+            draw(
+                mols(
+                    max_rotatable_bonds=max_rotatable_bonds,
+                    n_connected_components=1,
+                )
+            )
+            for _ in range(n_connected_components)
         ]
         seed = reduce(CombineMols, components)
     else:
         # repeat this process until a valid molecule is drawn
         while True:
             # start by drawing a random fragment and use it as seed
-            seed = draw(st.sampled_from(fragments))
+            # make sure that the seed has less rotatable bonds than max_rotatable_bonds
+            suitable_seeds = [
+                (f, n) for (f, n) in fragments if n <= max_rotatable_bonds
+            ]
+            seed, n_rotatable_bonds_current = draw(st.sampled_from(suitable_seeds))
+            display(seed)
 
             # extend the seed by running compatible reactions on the seed
             # stop when molecule has no dummy atoms anymore (i.e. is fully built)
+            rep = 0
             while seed.HasSubstructMatch(dummy_pattern):
+                if rep > 10:
+                    raise ValueError("Could not build molecule")
                 while True:
                     # find a free substitution site
                     for atom in seed.GetAtoms():
                         if atom.GetSymbol() == "*":
                             dummy_label = atom.GetIsotope()
                             break
 
-                    # draw a random reaction and fragment compatible with the substitution site
-                    # note: compatible_mapping[dummy_label] was sorted by number of dummy atoms and size
-                    #       --> shrinking is done automatically
-                    # run the reaction and collect the products
+                    # draw a random reaction compatible with the chosen dummy atom
                     reaction, right = draw(
                         st.sampled_from(compatible_reactions[dummy_label])
                     )
                     other_label = (
                         reaction._matchers[int(right)].GetAtomWithIdx(0).GetIsotope()
                     )
-                    fragment = draw(st.sampled_from(compatible_fragments[other_label]))
+                    reaction_adds_rotatable_bond = (
+                        reaction.GetProducts()[0].GetBondWithIdx(0).GetBondType()
+                        != BondType.DOUBLE
+                    )
+
+                    # draw a random fragment compatible with the drawn reaction
+                    # (but filter all fragments that would exceed the maximum number of rotatable bonds)
+                    # note: compatible_mapping[dummy_label] was sorted by number of dummy atoms and size
+                    #       --> shrinking is done automatically
+                    def _induced_rotatable_bonds(fragment, n):
+                        # IF reaction adds a rotatable bond AND fragment has more than 2 atoms
+                        # --> add 1 to the number of rotatable bonds
+                        # note: this is only an approximation
+                        # ... but: the actual number of rotatable bonds will be less
+                        #          than this estimate
+                        return n + (
+                            reaction_adds_rotatable_bond
+                            and (fragment.GetNumAtoms() > 2)
+                        )
+
+                    n_remaining_rotatable_bonds = (
+                        max_rotatable_bonds - n_rotatable_bonds_current
+                    )
+                    feasible_fragments = [
+                        (f, n_induced)
+                        for (f, n) in compatible_fragments[other_label]
+                        if (n_induced := _induced_rotatable_bonds(f, n))
+                        <= n_remaining_rotatable_bonds
+                    ]
+                    fragment, n = draw(st.sampled_from(feasible_fragments))
+                    print("fragment")
+                    display(fragment)
+
+                    # run the reaction and collect the products
                     if right:
                         products = reaction.RunReactants((seed, fragment))
                     else:
                         products = reaction.RunReactants((fragment, seed))
 
                     # remove duplicate products
                     unique_smiles = set()
@@ -157,28 +219,32 @@
                     if len(results) == 0:
                         continue
 
                     # if reactions were successful, pick a random product and use it as the new seed
                     # note: shrinking is not applicable here, because all products have the same size
                     seed = draw(st.sampled_from(results))
 
+                    # update the number of rotatable bonds
+                    n_rotatable_bonds_current += n
+
                     break
 
             try:
                 seed.UpdatePropertyCache()
                 SanitizeMol(seed)
                 seed = RemoveHs(seed)
-                break
             except:
                 continue
 
     name = draw(name)
     if name is not None:
         seed.SetProp("_Name", name)
 
+    # TODO: create conformer
+
     return seed
 
 
 @st.composite
 def smiles(draw, **kwargs):
     mol = draw(mols(**kwargs))
```

### Comparing `hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/PKG-INFO` & `hypothesis-rdkit-0.3/hypothesis_rdkit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: hypothesis-rdkit
-Version: 0.1
+Version: 0.3
 Home-page: https://github.com/shirte/hypothesis-rdkit
 Maintainer: Steffen Hirte
 Maintainer-email: shirte@users.noreply.github.com
+License: MIT
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Framework :: Hypothesis
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
 # hypothesis-rdkit
 
 ## Installation
 
 ```sh
 pip install -U hypothesis-rdkit
```

### Comparing `hypothesis-rdkit-0.1/setup.py` & `hypothesis-rdkit-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="hypothesis-rdkit",
-    version="0.1",
+    version="0.3",
     maintainer="Steffen Hirte",
     maintainer_email="shirte@users.noreply.github.com",
     packages=find_packages(),
     url="https://github.com/shirte/hypothesis-rdkit",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    install_requires=["hypothesis", "rdkit"],
+    license="MIT",
+    license_files=("LICENSE",),
+    install_requires=["hypothesis"],
+    extras_require={"dev": ["black", "isort"]},
     entry_points={"hypothesis": {"_ = hypothesis_rdkit.hook:_hypothesis_setup_hook"}},
     include_package_data=True,
     classifiers=[
+        "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Testing",
+        "Topic :: Scientific/Engineering :: Chemistry",
         "Framework :: Hypothesis",
+        "License :: OSI Approved :: MIT License",
     ],
 )
```

