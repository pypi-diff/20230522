# Comparing `tmp/bayanpy-0.7.2.tar.gz` & `tmp/bayanpy-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.7.2.tar", last modified: Thu May 11 16:47:04 2023, max compression
+gzip compressed data, was "bayanpy-0.7.3.tar", last modified: Mon May 22 15:34:46 2023, max compression
```

## Comparing `bayanpy-0.7.2.tar` & `bayanpy-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:47:04.403252 bayanpy-0.7.2/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.2/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-11 16:47:04.403252 bayanpy-0.7.2/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.2/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:47:04.403252 bayanpy-0.7.2/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57757 2023-05-11 16:44:44.000000 bayanpy-0.7.2/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.2/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:47:04.403252 bayanpy-0.7.2/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-11 16:47:04.403252 bayanpy-0.7.2/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-11 16:46:44.000000 bayanpy-0.7.2/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-22 15:34:46.476622 bayanpy-0.7.3/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.3/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-22 15:34:46.476622 bayanpy-0.7.3/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.3/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-22 15:34:46.476622 bayanpy-0.7.3/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    59427 2023-05-20 16:15:23.000000 bayanpy-0.7.3/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.3/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-22 15:34:46.476622 bayanpy-0.7.3/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-22 15:34:46.476622 bayanpy-0.7.3/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-22 15:34:21.000000 bayanpy-0.7.3/setup.py
```

### Comparing `bayanpy-0.7.2/LICENSE` & `bayanpy-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.2/README.md` & `bayanpy-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.2/bayanpy/BayanImplied.py` & `bayanpy-0.7.3/bayanpy/BayanImplied.py`

 * *Files 2% similar despite different names*

```diff
@@ -605,14 +605,30 @@
         if len(item)>1:
             for i in range(0,len(item)):
                 for j in range(i+1,len(item)):
                     OFV = OFV + 2*(ModularityMatrix[item[i],item[j]])
 #     OFV = OFV + ModularityMatrix.trace()[0,0]
     OFV = OFV + ModularityMatrix.trace()
     return np.round(OFV/(np.sum(AdjacencyMatrix)), 8)
+    
+def calculate_weighted_modularity(community, Graph, resolution):
+    """
+    Method that calculates weighted modularity for input community partition on input Graph
+    """
+    ModularityMatrix = get_weighted_modularity_matrix(Graph, resolution, weight="weight")
+    AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="weight")
+    OFV=0
+    for item in community:
+        if len(item)>1:
+            for i in range(0,len(item)):
+                for j in range(i+1,len(item)):
+                    OFV = OFV + 2*(ModularityMatrix[item[i],item[j]])
+#     OFV = OFV + ModularityMatrix.trace()[0,0]
+    OFV = OFV + ModularityMatrix.trace()
+    return np.round(OFV/(np.sum(AdjacencyMatrix)), 8)
 
 def find_violating_triples(Graph, var_vals, list_of_cut_triads):
     """
     Returns a dictionary whose key is a violated constrained and value is the sum
     """
     violated_triples_sums = {}
 #     list_of_tuples=list(combinations(np.sort(list((Graph).nodes())),3))
@@ -983,25 +999,39 @@
 def get_modularity_matrix(Graph, resolution):
     AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="actual_weight")
     ModularityMatrix = np.empty(AdjacencyMatrix.shape)
     for i in Graph.nodes():
         for j in Graph.nodes():
             deg_i = Graph.degree(i, weight="actual_weight") - AdjacencyMatrix[i, i]
             deg_j = Graph.degree(j, weight="actual_weight") - AdjacencyMatrix[j, j]
-            mod = AdjacencyMatrix[i, j] - (((deg_i*deg_j)/(np.sum(AdjacencyMatrix)))*resolution)
+            mod = AdjacencyMatrix[i, j] - (resolution*((deg_i*deg_j)/(np.sum(AdjacencyMatrix))))
+            ModularityMatrix[i, j] = mod
+    return ModularityMatrix
+
+def get_weighted_modularity_matrix(Graph, resolution, weight):
+    AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="weight")
+    ModularityMatrix = np.empty(AdjacencyMatrix.shape)
+    for i in Graph.nodes():
+        for j in Graph.nodes():
+            deg_i = Graph.degree(i, weight="weight") - AdjacencyMatrix[i, i]
+            deg_j = Graph.degree(j, weight="weight") - AdjacencyMatrix[j, j]
+            mod = AdjacencyMatrix[i, j] - (resolution*((deg_i*deg_j)/(np.sum(AdjacencyMatrix))))
             ModularityMatrix[i, j] = mod
     return ModularityMatrix
 
 
 def output(develop, state, lower_bound, upper_bound, communities, preprocessing_time, formulation_time, solve_time):
 
     if develop:
         out = state, lower_bound, upper_bound, communities, preprocessing_time, formulation_time, solve_time
     else:
-        gap = (upper_bound - lower_bound) / upper_bound
+        if upper_bound == 0:
+            gap = 0
+        else:
+            gap = (upper_bound - lower_bound) / upper_bound
         out = lower_bound, gap, communities, preprocessing_time+formulation_time, solve_time
     return out
 
 
 def bayan(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4, develop_mode=False):
     # Running Bayan for a network with multiple connected components
     optimal_partition = []
@@ -1009,22 +1039,26 @@
     n_sub = len(list_of_subgraphs)
     sub_results = {}
     total_gap = 0
     total_modeling_time = 0
     total_solve_time = 0
     total_preprocessing_time = 0
     total_formulation_time = 0
-    threshold_sub = threshold / n_sub
+    total_w_edge = np.sum(nx.adjacency_matrix(G, weight="actual_weight"))
+    threshold_sub = threshold / float(n_sub)
     for sub_inx, sub_graph in enumerate(list_of_subgraphs):
+        if sub_graph.number_of_edges() == 0:
+            optimal_partition.append([a for a in sub_graph.nodes()])
+            continue
 
         sub_graph = nx.convert_node_labels_to_integers(sub_graph, label_attribute="original_label")
         mapping = nx.get_node_attributes(sub_graph, 'original_label')
-
+        sub_resolution = resolution * np.sum(nx.adjacency_matrix(sub_graph, weight="actual_weight"))/ total_w_edge
         bayan_output = alg(sub_graph, threshold=threshold_sub, time_allowed=time_allowed, delta=delta,
-              resolution=resolution, lp_method=lp_method, develop_mode=develop_mode)
+              resolution=sub_resolution, lp_method=lp_method, develop_mode=develop_mode)
 
         if develop_mode:
             sub_results[sub_inx] = bayan_output
             optimal_partition += [[mapping[i] for i in com] for com in bayan_output[3]]
             total_preprocessing_time += bayan_output[4]
             total_formulation_time += bayan_output[5]
             total_solve_time += bayan_output[6]
@@ -1036,16 +1070,15 @@
             total_solve_time += bayan_output[4]
     # print(optimal_partition)
 
     G = nx.convert_node_labels_to_integers(G, label_attribute="original_label")
     mapping = nx.get_node_attributes(G, 'original_label')
     mapping ={val: key for key, val in mapping.items()}
     int_optimal_partition = [[mapping[i] for i in com] for com in optimal_partition]
-    lower_bound = calculate_modularity(int_optimal_partition, G, resolution)
-
+    lower_bound = calculate_weighted_modularity(int_optimal_partition, G, resolution)
 
     if develop_mode:
         for sub_inx, sub_graph in enumerate(list_of_subgraphs):
             print(f"Connected component {sub_inx}")
             print(sub_results[sub_inx])
         out = lower_bound, optimal_partition,  total_preprocessing_time, total_formulation_time,total_solve_time
     else:
```

### Comparing `bayanpy-0.7.2/setup.py` & `bayanpy-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.7.2",
+    version="0.7.3",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

