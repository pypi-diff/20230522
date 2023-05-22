# Comparing `tmp/tree-of-thoughts-0.1.3.tar.gz` & `tmp/tree-of-thoughts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.1.3.tar", last modified: Mon May 22 12:13:22 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.1.4.tar", last modified: Mon May 22 14:18:19 2023, max compression
```

## Comparing `tree-of-thoughts-0.1.3.tar` & `tree-of-thoughts-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:18:19.393773 tree-of-thoughts-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 14:18:05.000000 tree-of-thoughts-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 14:18:19.393773 tree-of-thoughts-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-22 14:18:05.000000 tree-of-thoughts-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:18:19.393773 tree-of-thoughts-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-22 14:18:05.000000 tree-of-thoughts-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:18:19.393773 tree-of-thoughts-0.1.4/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 14:18:05.000000 tree-of-thoughts-0.1.4/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-05-22 14:18:05.000000 tree-of-thoughts-0.1.4/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:18:19.393773 tree-of-thoughts-0.1.4/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 14:18:19.000000 tree-of-thoughts-0.1.4/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 14:18:19.000000 tree-of-thoughts-0.1.4/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:18:19.000000 tree-of-thoughts-0.1.4/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 14:18:19.000000 tree-of-thoughts-0.1.4/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 14:18:19.000000 tree-of-thoughts-0.1.4/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.1.3/LICENSE` & `tree-of-thoughts-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.1.3/PKG-INFO` & `tree-of-thoughts-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.1.3/README.md` & `tree-of-thoughts-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -179,14 +179,23 @@
 Provide ready to use generate thoughts function -- done
 
 Provide ready to use evaluate states function -- done
 
 now
 Implement a more sophisticated prompt engineering strategy to guide the model's reasoning process more effectively.
 
+Make TreeofThoughts class completely customizable with a config yml file with params like
+chatbot:
+    type: "openai"
+    max_context_length: 8000
+    include_chat_history_in_query: false
+openai:
+    model: <model_name>
+    api_key: <your_open_ai_api_key>
+
 
 Script that generates an dataset based on a topic input, -> set of questions are asked, then multiple trees of thoughts are run concurrently to generate the decision making rich dataset
 
 
 Introduce a reinforcement learning, distillment, and finetuning scripts to finely tune the model based on feedback from the Tree of Thoughts algorithm.
 
 Integrate heuristics that autonomously determine the search algorithm based on indicators
```

### Comparing `tree-of-thoughts-0.1.3/setup.py` & `tree-of-thoughts-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.1.3',
+  version = '0.1.4',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.1.3/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.1.4/tree_of_thoughts/treeofthoughts.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
             prompt=prompt,
             n=k,
             max_tokens=50,
             stop=None,
             temperature=0.5,
         )
         thoughts = [choice.text.strip() for choice in response.choices]
-        print(thoughts)
+        # print(thoughts)
+        print(f"Generated thoughts: {thoughts}")
         return thoughts
 
     def evaluate_states(self, states):
         if self.evaluation_strategy == 'value':
             state_values = {}
             for state in states:
                 state_text = ' '.join(state)
@@ -56,17 +57,18 @@
                     prompt=prompt,
                     n=1,
                     max_tokens=10,
                     stop=None,
                     temperature=0.5,
                 )
                 try:
-                    print(response.choices[0].text.strip())
+                    value_text = response.choices[0].text.strip()
+                    print(f"Value text {value_text}")
                     value = float(response.choices[0].text.strip())
-                    print(value)
+                    print(f"value: {value}")
                 except ValueError:
                     value = 0  # Assign a default value if the conversion fails
                 state_values[state] = value
             return state_values
 
         elif self.evaluation_strategy == 'vote':
             states_text = '\n'.join([' '.join(state) for state in states])
@@ -76,15 +78,15 @@
                 prompt=prompt,
                 n=1,
                 max_tokens=50,
                 stop=None,
                 temperature=0.5,
             )
             best_state_text = response.choices[0].text.strip()
-            print(best_state_text)
+            print(f"Best state text: {best_state_text}")
             best_state = tuple(best_state_text.split())
             return {state: 1 if state == best_state else 0 for state in states}
 
         else:
             raise ValueError("Invalid evaluation strategy. Choose 'value' or 'vote'.")
 
 class OptimizedOpenAILanguageModel(OpenAILanguageModel):
@@ -93,21 +95,21 @@
         self.cache_enabled = cache_enabled
         self.thought_cache = {}
         self.state_evaluation_cache = {}
 
     def parallel_generate_thoughts(self, states, k):
         with concurrent.futures.ThreadPoolExecutor() as executor:
             thoughts = list(executor.map(lambda state: self.generate_thoughts(state, k), states))
-            print(thoughts)
+            print(f"Parallel generated thoughts: {thoughts}")
         return thoughts
 
     def parallel_evaluate_states(self, states):
         with concurrent.futures.ThreadPoolExecutor() as executor:
             state_values = list(executor.map(self.evaluate_states, states))
-            print(state_values)
+            print(f"Parallel evaluated state values: {state_values}")
         return state_values
     
 
 # model = OptimizedOpenAILanguageModel('your_openai_api_key_here')
 
 #update tree of thoughts to use optimized models mehtods
```

### Comparing `tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.1.4/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

