# Comparing `tmp/tree-of-thoughts-0.1.5.tar.gz` & `tmp/tree-of-thoughts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.1.5.tar", last modified: Mon May 22 15:49:43 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.1.6.tar", last modified: Mon May 22 15:58:09 2023, max compression
```

## Comparing `tree-of-thoughts-0.1.5.tar` & `tree-of-thoughts-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:49:43.612428 tree-of-thoughts-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 15:49:28.000000 tree-of-thoughts-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 15:49:43.608428 tree-of-thoughts-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-22 15:49:28.000000 tree-of-thoughts-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:49:43.612428 tree-of-thoughts-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-22 15:49:28.000000 tree-of-thoughts-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:49:43.608428 tree-of-thoughts-0.1.5/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 15:49:28.000000 tree-of-thoughts-0.1.5/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-05-22 15:49:28.000000 tree-of-thoughts-0.1.5/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:49:43.608428 tree-of-thoughts-0.1.5/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 15:49:43.000000 tree-of-thoughts-0.1.5/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 15:49:43.000000 tree-of-thoughts-0.1.5/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:49:43.000000 tree-of-thoughts-0.1.5/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 15:49:43.000000 tree-of-thoughts-0.1.5/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 15:49:43.000000 tree-of-thoughts-0.1.5/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.1.5/LICENSE` & `tree-of-thoughts-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.1.5/PKG-INFO` & `tree-of-thoughts-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.1.5/README.md` & `tree-of-thoughts-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.1.5/setup.py` & `tree-of-thoughts-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.1.5',
+  version = '0.1.6',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.1.5/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.1.6/tree_of_thoughts/treeofthoughts.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,18 +107,14 @@
     def parallel_evaluate_states(self, states):
         with concurrent.futures.ThreadPoolExecutor() as executor:
             state_values = list(executor.map(self.evaluate_states, states))
             print(f"Parallel evaluated state values: {state_values}")
         return state_values
     
 
-# model = OptimizedOpenAILanguageModel('your_openai_api_key_here')
-# model = OptimizedOpenAILanguageModel('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')
-
-#update tree of thoughts to use optimized models mehtods
 
 class TreeofThoughts:
     """
     1. Thought Decomposition --> based on problem properties
 
     2. Thought Generator -> create a thought generator function G(p0, s, k) with 2 strategies a sample iid thoughts from a cot prompt b. propose thoughts
     sequentially using a propose prompt
@@ -215,15 +211,15 @@
             return False
 
         dfs(x, 1)
         return max(output, key=lambda x: x[1]) if output else None
 
 
 class OptimizedTreeofThoughts(TreeofThoughts):
-    def solve(self, x, k, T, b, vth, timeout=None, confidence_threshold=None, max_iterations=None, convergence_threshold=None, convergence_count=None):
+    def solve(self, x, k, T, b, vth, timeout=None, confidence_threshold=0.9, max_iterations=10, convergence_threshold=0.1, convergence_count=5):
         start_time = time.time()
         if self.search_algorithm == 'BFS':
             while timeout is None or time.time() - start_time < timeout:
                 result = self.tot_bfs(x, k, T, b)
                 if result:
                     return result
         elif self.search_algorithm == 'DFS':
@@ -235,36 +231,40 @@
             raise ValueError("Invalid search algorithm. Choose 'BFS' or 'DFS'.")
 
 search_algorithm = "DFS"
 strategy = "cot"
 evaluation_strategy="vote"
 
 #create instance
-model = OptimizedOpenAILanguageModel('api-key')
+model = OptimizedOpenAILanguageModel('api key')
 
 
 tree_of_thoughts = OptimizedTreeofThoughts(model, search_algorithm)
 
-input_problem = "What is 3032 * 322 - 1"
+
+input_problem = "What are next generation reasoning methods for Large Language Models"
 k = 5
 T = 3
 b = 5
 vth = 0.5
-timeout = 10
 
-# Optimal nominal values for the stopping conditions
-confidence = 0.9 #HIGH QUALITY SOLIUTION FOUND
-max_iterations = 5 # MAX ITERATIONS 10
-convergence_threshold = 0.01 #Convergence Check: Monitor the change in evaluation values between consecutive iterations. If the change in evaluation values is below a certain threshold for a specified number of consecutive iterations, the algorithm can stop and return the solution.
-convergence_count = 5
+# # Optimal nominal values for the stopping conditions
+
+# confidence = 0.9 #HIGH QUALITY SOLIUTION FOUND
+
+# max_iterations = 5 # MAX ITERATIONS 10
+
+# convergence_threshold = 0.01 #Convergence Check: Monitor the change in evaluation values between consecutive iterations. If the change in evaluation values is below a certain threshold for a specified number of consecutive iterations, the algorithm can stop and return the solution.
+
+# convergence_count = 5
 
 #call the solve method with the input problem and other params
-solution = tree_of_thoughts.solve(input_problem, k, T, b, vth=vth, confidence_threshold=confidence, max_iterations=max_iterations, convergence_threshold=convergence_threshold, convergence_count=convergence_count)
+solution = tree_of_thoughts.solve(input_problem, k, T, b, vth)
 
-#use the solution in env
+#use the solution in yes
 print(f"solution: {solution}")
 
 """
 should return something like this:
 
 ['1. Utilizing reinforcement learning techniques to train large language models can be an effective approach to advancing them.\n2. Developing methods to better incorporate contextual information into large language models can help in their advancement.\n3. Incorpor', '1. Utilizing reinforcement learning techniques to allow for more efficient training of large language models.\n2. Incorporating transfer learning to leverage existing language models for faster and more accurate inference.\n3. Exploring the use of distributed', '1. Identifying and understanding key components of large language models such as natural language processing and machine learning algorithms.\n2. Utilizing methods such as transfer learning to quickly and efficiently train large language models.\n3. Incorporating', '1. Utilizing reinforcement learning techniques to train large language models can be an effective method of advancing them.\n2. Incorporating techniques such as transfer learning and data augmentation can help improve the performance of large language models.', '1. Identifying and understanding the underlying structure of language is essential to advancing large language models.\n2. Developing methods to effectively capture and represent the complexities of language is necessary for the advancement of large language models.\n3. Ut']
 0.8
```

### Comparing `tree-of-thoughts-0.1.5/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

