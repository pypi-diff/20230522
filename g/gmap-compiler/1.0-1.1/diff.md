# Comparing `tmp/gmap-compiler-1.0.tar.gz` & `tmp/gmap-compiler-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmap-compiler-1.0.tar", last modified: Tue May  9 19:40:56 2023, max compression
+gzip compressed data, was "gmap-compiler-1.1.tar", last modified: Mon May 22 13:20:07 2023, max compression
```

## Comparing `gmap-compiler-1.0.tar` & `gmap-compiler-1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jimmyweber   (501) staff       (20)        0 2023-05-09 19:40:56.987720 gmap-compiler-1.0/
--rw-r--r--   0 jimmyweber   (501) staff       (20)     1089 2023-04-20 10:38:31.000000 gmap-compiler-1.0/LICENSE
--rw-r--r--   0 jimmyweber   (501) staff       (20)      376 2023-05-09 19:40:56.987629 gmap-compiler-1.0/PKG-INFO
--rw-r--r--   0 jimmyweber   (501) staff       (20)     3101 2023-05-09 19:38:08.000000 gmap-compiler-1.0/README.md
-drwxr-xr-x   0 jimmyweber   (501) staff       (20)        0 2023-05-09 19:40:56.986264 gmap-compiler-1.0/gmap/
--rw-r--r--   0 jimmyweber   (501) staff       (20)        2 2023-04-20 10:38:31.000000 gmap-compiler-1.0/gmap/__init__.py
--rw-r--r--   0 jimmyweber   (501) staff       (20)    13037 2023-05-09 19:18:31.000000 gmap-compiler-1.0/gmap/compiler.py
--rw-r--r--   0 jimmyweber   (501) staff       (20)     7043 2023-05-09 18:42:11.000000 gmap-compiler-1.0/gmap/hardware.py
-drwxr-xr-x   0 jimmyweber   (501) staff       (20)        0 2023-05-09 19:40:56.986781 gmap-compiler-1.0/gmap/matrix/
--rw-r--r--   0 jimmyweber   (501) staff       (20)        0 2023-05-09 12:14:59.000000 gmap-compiler-1.0/gmap/matrix/__init__.py
--rw-r--r--   0 jimmyweber   (501) staff       (20)     9010 2023-05-09 15:41:57.000000 gmap-compiler-1.0/gmap/matrix/generator.py
--rw-r--r--   0 jimmyweber   (501) staff       (20)     4589 2023-05-09 16:12:51.000000 gmap-compiler-1.0/gmap/matrix/utils.py
-drwxr-xr-x   0 jimmyweber   (501) staff       (20)        0 2023-05-09 19:40:56.987491 gmap-compiler-1.0/gmap_compiler.egg-info/
--rw-r--r--   0 jimmyweber   (501) staff       (20)      376 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/PKG-INFO
--rw-r--r--   0 jimmyweber   (501) staff       (20)      331 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/SOURCES.txt
--rw-r--r--   0 jimmyweber   (501) staff       (20)        1 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/dependency_links.txt
--rw-r--r--   0 jimmyweber   (501) staff       (20)       48 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/requires.txt
--rw-r--r--   0 jimmyweber   (501) staff       (20)        5 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/top_level.txt
--rw-r--r--   0 jimmyweber   (501) staff       (20)       38 2023-05-09 19:40:56.987760 gmap-compiler-1.0/setup.cfg
--rw-r--r--   0 jimmyweber   (501) staff       (20)      658 2023-05-09 19:40:54.000000 gmap-compiler-1.0/setup.py
+drwxr-xr-x   0 jimmy      (501) staff       (20)        0 2023-05-22 13:20:07.581626 gmap-compiler-1.1/
+-rw-r--r--   0 jimmy      (501) staff       (20)     1089 2023-03-30 02:05:47.000000 gmap-compiler-1.1/LICENSE
+-rw-r--r--   0 jimmy      (501) staff       (20)      331 2023-05-22 13:20:07.578677 gmap-compiler-1.1/PKG-INFO
+-rw-r--r--   0 jimmy      (501) staff       (20)     3101 2023-05-22 09:32:52.000000 gmap-compiler-1.1/README.md
+drwxr-xr-x   0 jimmy      (501) staff       (20)        0 2023-05-22 13:20:07.568929 gmap-compiler-1.1/gmap/
+-rw-r--r--   0 jimmy      (501) staff       (20)     7022 2023-05-22 13:15:00.000000 gmap-compiler-1.1/gmap/Hardware.py
+-rw-r--r--   0 jimmy      (501) staff       (20)        2 2023-03-31 17:03:09.000000 gmap-compiler-1.1/gmap/__init__.py
+-rw-r--r--   0 jimmy      (501) staff       (20)    11937 2023-05-22 12:25:54.000000 gmap-compiler-1.1/gmap/compiler.py
+-rw-r--r--   0 jimmy      (501) staff       (20)     3237 2023-05-22 11:06:06.000000 gmap-compiler-1.1/gmap/mapping.py
+drwxr-xr-x   0 jimmy      (501) staff       (20)        0 2023-05-22 13:20:07.572052 gmap-compiler-1.1/gmap/matrix/
+-rw-r--r--   0 jimmy      (501) staff       (20)        0 2023-05-22 09:32:52.000000 gmap-compiler-1.1/gmap/matrix/__init__.py
+-rw-r--r--   0 jimmy      (501) staff       (20)     9010 2023-05-22 09:32:52.000000 gmap-compiler-1.1/gmap/matrix/generator.py
+-rw-r--r--   0 jimmy      (501) staff       (20)     3259 2023-05-22 10:56:35.000000 gmap-compiler-1.1/gmap/matrix/utils.py
+drwxr-xr-x   0 jimmy      (501) staff       (20)        0 2023-05-22 13:20:07.577498 gmap-compiler-1.1/gmap_compiler.egg-info/
+-rw-r--r--   0 jimmy      (501) staff       (20)      331 2023-05-22 13:20:07.000000 gmap-compiler-1.1/gmap_compiler.egg-info/PKG-INFO
+-rw-r--r--   0 jimmy      (501) staff       (20)      364 2023-05-22 13:20:07.000000 gmap-compiler-1.1/gmap_compiler.egg-info/SOURCES.txt
+-rw-r--r--   0 jimmy      (501) staff       (20)        1 2023-05-22 13:20:07.000000 gmap-compiler-1.1/gmap_compiler.egg-info/dependency_links.txt
+-rw-r--r--   0 jimmy      (501) staff       (20)       48 2023-05-22 13:20:07.000000 gmap-compiler-1.1/gmap_compiler.egg-info/requires.txt
+-rw-r--r--   0 jimmy      (501) staff       (20)        5 2023-05-22 13:20:07.000000 gmap-compiler-1.1/gmap_compiler.egg-info/top_level.txt
+-rw-r--r--   0 jimmy      (501) staff       (20)       38 2023-05-22 13:20:07.583798 gmap-compiler-1.1/setup.cfg
+-rw-r--r--   0 jimmy      (501) staff       (20)      658 2023-05-22 13:19:57.000000 gmap-compiler-1.1/setup.py
```

### Comparing `gmap-compiler-1.0/LICENSE` & `gmap-compiler-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmap-compiler-1.0/README.md` & `gmap-compiler-1.1/README.md`

 * *Files identical despite different names*

### Comparing `gmap-compiler-1.0/gmap/compiler.py` & `gmap-compiler-1.1/gmap/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import copy
 import random
 from simanneal import Annealer
+
+from gmap.mapping import Mapping
 from gmap.matrix.utils import *
 import time
 import math
 
 
 class Hardware_Annealer(Annealer):
     """ Hardware annealer is an annealer designed specifically to anneal hardware.
 
      Parameters:
-        mapping (Mapping) : The network to anneal
+        mapping (gmap.mapping.Mapping) : The network to anneal
         update_move(mapping, i, j) (callable): The function to call at each swap of neurons i and j and that returns dE
         cost(mapping) (callable): The function that returns the energy of a mapping, i.e. the number of violated constraints
     """
 
     def __init__(self, mapping, update_move, cost, get_temperature, debug):
         self.update_move = update_move
         self.cost = cost
@@ -156,44 +157,17 @@
         if self.save_state_on_exit:
             self.save_state()
 
         # Return best mapping and energy
         return self.best_mapping, self.best_energy
 
     def energy(self):
-        return self.cost(self.state)
-
-
-class Mapping:
-    """
-    mapping contains the actual data useful for a mapping
-
-    Parameters:
-    order (np.array): The order to apply to connectivity_matrix and to weight_matrix to get the mapping
-    connectivity_matrix (2D np.array): The original unordered connectivity matrix of the network
-    weight_matrix (2D np.array): The original unordered weight matrix of the network
-    cost_tracker : Any object that help to track the actual cost of the actual mapping
-
-    """
-
-    def __init__(self, connectivity_matrix, weight_matrix, cost_tracker=None):
-        self.order = np.arange(len(connectivity_matrix))
-        self.connectivity_matrix = connectivity_matrix
-        self.weight_matrix = weight_matrix
-        self.cost_tracker = cost_tracker
-
-    def copy(self):
-        """
-        Only the order and the cost_tracker has to be copied. They depend on the mapping.
-        The connectivity_matrix and th  weight_matrix are the original unordered ones.
-        """
-        new = Mapping(self.connectivity_matrix, self.weight_matrix)
-        new.order = copy.deepcopy(self.order)
-        new.cost_tracker = copy.deepcopy(self.cost_tracker)
-        return new
+        cost = self.cost(self.state)
+        self.state.cost = cost
+        return cost
 
 
 class Hardware:
     """
     Class to define a hardware regarding its constrains.
     """
 
@@ -286,17 +260,22 @@
 
         # Swap the mapping
         mapping.order[i], mapping.order[j] = mapping.order[j], mapping.order[i]
 
         # Update the mapping accordingly.
         self.update_cost_tracker(mapping, i, j)
 
-        # Compute the difference of cost.
-        return self.cost(mapping) - E_ini
+        # Cost of the un-mutated mapping.
+        E_fin = self.cost(mapping)
+
+        # Update the mapping cost
+        mapping.cost = E_fin
 
+        # Compute the difference of cost.
+        return E_fin - E_ini
 
     def map(self, weight_matrix, minutes=1, debug=False, params=None, greedy_ratio=0.2):
         """
         Map a network defined by its weight matrix onto this Hardware.
 
         Parameters:
         weight_matrix (2D np.array) : The network to map
@@ -315,18 +294,17 @@
         # Pre-check the size of the network that has to be smaller than the hardware
         if len(weight_matrix) > self.n_total:
             return weight_matrix, float('inf')
 
         # Pre-treatment. Zero-pad the network matrix.
         pad = self.n_total - len(weight_matrix)
         weight_matrix = np.pad(weight_matrix, [(0, pad), (0, pad)], mode='constant')
-        connectivity_matrix = 1 * (weight_matrix > 0)
 
         # Initiating the solver
-        initial_mapping = Mapping(connectivity_matrix, weight_matrix)
+        initial_mapping = Mapping(weight_matrix)
         sa = Hardware_Annealer(initial_mapping, self.update_move, self.cost, self.get_temperature, debug=debug)
         sa.copy_strategy = 'method'
         if debug: print("Initial cost : ", self.cost(initial_mapping))
 
         if params is None:
             if debug: print("Searching for the good optimization parameters...")
             # Searching for the good params
@@ -342,8 +320,8 @@
 
         if debug:
             if violated_constrains == 0:
                 print("Mappable !")
             else:
                 print("Not Mappable, violated : ", violated_constrains)
 
-        return mapping.order, reorder(mapping.order, weight_matrix), violated_constrains
+        return mapping
```

### Comparing `gmap-compiler-1.0/gmap/hardware.py` & `gmap-compiler-1.1/gmap/Hardware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from gmap.compiler import Hardware
-from gmap.matrix.utils import reorder, expected_cost_difference_line
+from gmap.matrix.utils import expected_cost_difference_line
 from gmap.matrix.generator import create_multicore_mask
 import numpy as np
 import math
 import scipy.stats as stats
 
 
 class Multicore(Hardware):
@@ -154,9 +154,9 @@
             # Compare it with the actual max number of tags.
             violated_K += (max_K - self.K) * (max_K > self.K)
 
         return violated_K
 
     def cost(self, mapping):
         # Non optimized way of computing the constraints violated. Complexity of O(N**2).
-        actual_connectivity_matrix = reorder(mapping.order, mapping.connectivity_matrix)
+        actual_connectivity_matrix = mapping.reordered_connectivity_matrix()
         return self.violated_mem_sender(actual_connectivity_matrix) + self.violated_mem_receiver(actual_connectivity_matrix)
```

### Comparing `gmap-compiler-1.0/gmap/matrix/generator.py` & `gmap-compiler-1.1/gmap/matrix/generator.py`

 * *Files identical despite different names*

### Comparing `gmap-compiler-1.0/gmap/matrix/utils.py` & `gmap-compiler-1.1/gmap/matrix/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -63,63 +63,14 @@
     plt.figure()
     degree_hist = nx.degree_histogram(G)
     plt.plot(degree_hist)
     plt.xlabel("Degree")
     plt.ylabel("Frequency")
 
 
-def reorder(order, A):
-    """
-    A function that reorders the rows and columns of a matrix according
-    to a given order.
-
-    Args:
-    order (array-like): The desired order of the rows and columns.
-    A (array-like): The input matrix to be reordered.
-
-    Returns:
-    A_new (array-like): The reordered matrix.
-    """
-
-    # Reorder the rows of the input matrix according to the given order.
-    A_new = A.take(order, axis=0)
-
-    # Reorder the columns of the reordered matrix according to the given order.
-    A_new = A_new.take(order, axis=1)
-
-    # Return the reordered matrix.
-    return A_new
-
-
-# Shuffle the label of a network. The network remains the same but not its incidency matrix.
-def shuffle(A):
-    """
-    A function that shuffles the rows and columns of a matrix randomly.
-
-    Args:
-    A (array-like): The input matrix to be shuffled.
-
-    Returns:
-    A_new (array-like): The shuffled matrix.
-    """
-
-    # Create a copy of the input matrix to avoid modifying the original.
-    A_new = np.copy(A)
-
-    # Generate a random permutation of indices for the rows and columns.
-    arr = np.arange(len(A_new))
-    np.random.shuffle(arr)
-
-    # Reorder the rows and columns of the matrix according to the random permutation.
-    A_new = reorder(arr, A_new)
-
-    # Return the shuffled matrix.
-    return A_new
-
-
 def expected_cost_difference_line(n, p, func_cost_line):
     """
     Computes the expectation of the difference of cost between two random lines or two random columns
     when the difference is negative.
 
     Args:
         n: The number of lines/columns.
```

### Comparing `gmap-compiler-1.0/setup.py` & `gmap-compiler-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gmap-compiler',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'matplotlib',
         'networkx',
         'numba',
         'scipy',
```

