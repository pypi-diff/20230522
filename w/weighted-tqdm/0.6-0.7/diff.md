# Comparing `tmp/weighted_tqdm-0.6.tar.gz` & `tmp/weighted_tqdm-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_tqdm-0.6.tar", last modified: Thu Apr 27 21:16:28 2023, max compression
+gzip compressed data, was "weighted_tqdm-0.7.tar", last modified: Mon May 22 14:15:13 2023, max compression
```

## Comparing `weighted_tqdm-0.6.tar` & `weighted_tqdm-0.7.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.288491 weighted_tqdm-0.6/
--rw-rw-rw-   0        0        0     1096 2023-04-27 21:16:24.000000 weighted_tqdm-0.6/LICENSE
--rw-rw-rw-   0        0        0     2967 2023-04-27 21:16:28.289490 weighted_tqdm-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2023-04-27 21:16:24.000000 weighted_tqdm-0.6/README.md
--rw-rw-rw-   0        0        0      516 2023-04-27 21:16:28.290489 weighted_tqdm-0.6/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-04-27 21:16:24.000000 weighted_tqdm-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.260590 weighted_tqdm-0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.267574 weighted_tqdm-0.6/src/weighted_tqdm/
--rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.6/src/weighted_tqdm/__init__.py
--rw-rw-rw-   0        0        0    14675 2023-04-27 18:40:16.000000 weighted_tqdm-0.6/src/weighted_tqdm/weighted_tqdm.py
-drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.282490 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/
--rw-rw-rw-   0        0        0     2967 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.287491 weighted_tqdm-0.6/test/
--rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 weighted_tqdm-0.6/test/test_JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 weighted_tqdm-0.6/test/test_kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:15:13.466488 weighted_tqdm-0.7/
+-rw-rw-rw-   0        0        0     1096 2023-05-22 14:14:29.000000 weighted_tqdm-0.7/LICENSE
+-rw-rw-rw-   0        0        0     2967 2023-05-22 14:15:13.467996 weighted_tqdm-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2023-05-22 14:14:29.000000 weighted_tqdm-0.7/README.md
+-rw-rw-rw-   0        0        0      516 2023-05-22 14:15:13.470555 weighted_tqdm-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-05-22 14:14:29.000000 weighted_tqdm-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:15:13.426646 weighted_tqdm-0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:15:13.437609 weighted_tqdm-0.7/src/weighted_tqdm/
+-rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.7/src/weighted_tqdm/__init__.py
+-rw-rw-rw-   0        0        0    16117 2023-05-22 12:47:17.000000 weighted_tqdm-0.7/src/weighted_tqdm/weighted_tqdm.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:15:13.465489 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/
+-rw-rw-rw-   0        0        0     2967 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/top_level.txt
```

### Comparing `weighted_tqdm-0.6/LICENSE` & `weighted_tqdm-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.6/PKG-INFO` & `weighted_tqdm-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: weighted_tqdm
-Version: 0.6
+Version: 0.7
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.6.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.7.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `weighted_tqdm-0.6/README.md` & `weighted_tqdm-0.7/README.md`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.6/setup.cfg` & `weighted_tqdm-0.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 360d  ..version = 0.6.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 370d  ..version = 0.7.
 00000030: 0a61 7574 686f 7220 3d20 4d69 6368 6165  .author = Michae
 00000040: 6c20 5363 6869 6c6c 696e 670d 0a61 7574  l Schilling..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d69 6368  hor_email = mich
 00000060: 6165 6c40 6e74 726f 7069 632e 6465 0d0a  ael@ntropic.de..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 7765  description = we
 00000080: 6967 6874 6564 5f74 7164 6d20 616c 6c6f  ighted_tqdm allo
 00000090: 7773 2066 6f72 2077 6569 6768 7465 6420  ws for weighted 
@@ -15,15 +15,15 @@
 000000e0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 000000f0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
 00000100: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
 00000110: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
 00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
 00000130: 7472 6f70 6963 2f77 6569 6768 7465 645f  tropic/weighted_
 00000140: 7471 646d 2f61 7263 6869 7665 2f72 6566  tqdm/archive/ref
-00000150: 732f 7461 6773 2f76 302e 362e 7461 722e  s/tags/v0.6.tar.
+00000150: 732f 7461 6773 2f76 302e 372e 7461 722e  s/tags/v0.7.tar.
 00000160: 677a 0d0a 5072 6f67 7261 6d6d 696e 6720  gz..Programming 
 00000170: 4c61 6e67 7561 6765 203d 203a 2050 7974  Language = : Pyt
 00000180: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
 00000190: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
 000001a0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
 000001b0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
 000001c0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
```

### Comparing `weighted_tqdm-0.6/setup.py` & `weighted_tqdm-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "weighted_tqdm",
-    version      = "0.6",
+    version       = "0.7",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "weighted_tqdm allows for weighted iterations in tqdm progress bars.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.6.tar.gz",
+    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.7.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `weighted_tqdm-0.6/src/weighted_tqdm/weighted_tqdm.py` & `weighted_tqdm-0.7/src/weighted_tqdm/weighted_tqdm.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,37 +31,42 @@
             weights = [int(i/min_weight) for i in weight_vals]
             weight_sum = sum(weights)
     else:
         weight_sum = total
         weights = [1]*total
     return weights, weight_sum
 
-def weighted_tqdm(iterable, weights=None, name='', print_val=False, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', **kwargs):
+def weighted_tqdm(iterable, weights=None, name='', print_val=False, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', max_rate=30, **kwargs):
     total = determine_length_of_iterable(iterable, weights, **kwargs)
     weights_var, weight_sum = make_weight_list(iterable, total, weights)
     # create a new tqdm object, then with every iteration yield the next weight in weight_vals
     pbar = tqdm(total=weight_sum, bar_format=bar_format, **kwargs)
+    start_time = time.time()
+    min_time = 1/max_rate 
     i = 1
     if len(name):
         name += ': '
     # with every iteration 
     iterator = iter(iterable)
     elem = next(iterator)
     if print_val:
         pbar.set_description(name+str(elem)+' (' +str(i) + '/' + str(total) + ')')
     else:
         pbar.set_description(name+'(' +str(i) + '/' + str(total) + ')')
     yield elem
     for weight in weights_var[:-1]:
         i += 1
         elem = next(iterator)
-        if print_val:
-            pbar.set_description(name+str(elem)+' (' +str(i) + '/' + str(total) + ')')
-        else:
-            pbar.set_description(name+'(' +str(i) + '/' + str(total) + ')')
+        new_time = time.time()
+        if new_time - start_time > min_time:
+            if print_val:
+                pbar.set_description(name+str(elem)+' (' +str(i) + '/' + str(total) + ')')
+            else:
+                pbar.set_description(name+'(' +str(i) + '/' + str(total) + ')')
+            start_time = new_time
         pbar.update(weight)
         yield elem
     #pbar.set_description('(Done)')
     pbar.update(weights_var[-1])
     pbar.close()
 
 def qudit_tqdm(iterable, dit=2, exp=3, name='qubits', print_val=False, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', **kwargs):
@@ -72,25 +77,27 @@
 # which is then used to create progress bars, which can be split between different loops
 ## for example:
 # p = progress()# for i in p.tqdm(range(10)):
 #    for j in p.tqdm(range(10)):
 #       pass
 ## this will create a progress bar where every iteration of j is counted as 1/10th of an iteration of i
 class progress:
-    def __init__(self, total=1000, print_val=False, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', **kwargs):
+    def __init__(self, total=1000, print_val=False, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', max_rate=30, **kwargs):
         self.total = total # separate these steps dynamically
         self.levels = 0
         self.weight_by_level = []
         self.ind_by_level = []
         self.current_count = 0
         self.current_count_float = 0.0
         self.pbar = None
         self.print_val = print_val
         self.bar_format = bar_format
         self.names = []
+        self.min_time = 1/max_rate
+        self.time = time.time()
         
     def weighted_tqdm(self, iterable, weights=None, name='', **kwargs):
         how_many = determine_length_of_iterable(iterable, weights, **kwargs)
         # add to total levels of the progress bar
         # add the weight of the new level to the weight_by_level list
         if len(name):
             name += ': '
@@ -127,18 +134,21 @@
             # then yield the next item
             elem = next(iterator)
             if my_level == self.levels: # no sub-call -> update pbar
                 self.current_count_float += self.weight_by_level[-1][ind]
                 ind += 1
                 new_count = round(self.current_count_float*self.total)
                 diff_count = new_count - self.current_count
-                if self.print_val:
-                    self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind) + '/' + str(how_many) + ')')
-                else:
-                    self.pbar.set_description(self.names[-1]+'(' +str(ind) + '/' + str(how_many) + ')')
+                new_time = time.time()
+                if new_time - self.time > self.min_time:
+                    if self.print_val:
+                        self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind) + '/' + str(how_many) + ')')
+                    else:
+                        self.pbar.set_description(self.names[-1]+'(' +str(ind) + '/' + str(how_many) + ')')
+                    self.time = new_time
                 self.pbar.update(diff_count)
                 self.current_count = new_count
                 destroyed_subcall_last = 0
             else: # there was a subcall -> destroy it
                 ind += 1
                 self.levels -= 1
                 self.weight_by_level.pop()
@@ -148,66 +158,79 @@
             self.ind_by_level[my_level-1] = ind
             yield elem
         if not destroyed_subcall_last: # if there was a subcall, the progress bar was already updated
             self.current_count_float += self.weight_by_level[-1][ind]
             new_count = round(self.current_count_float*self.total)
             diff_count = new_count - self.current_count
             self.current_count = new_count
+            new_time = time.time()
+            if new_time - self.time > self.min_time:
+                if self.print_val:
+                    self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind+1) + '/' + str(how_many) + ')')
+                else:
+                    self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
+                self.time = new_time
+            self.pbar.update(diff_count)
+        # finished iterating through the iterable
+        if my_level == 1:  # reset the object
             if self.print_val:
                 self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind+1) + '/' + str(how_many) + ')')
             else:
                 self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
-            self.pbar.update(diff_count)
-        # finished iterating through the iterable
-        if my_level == 1:  # reset the object
+            self.time = new_time
             self.pbar.close()
             self.pbar = None
             self.current_count = 0
             self.current_count_float = 0.0
             self.weight_by_level = []
             self.names = []
-            self.levels = 0    
-            if self.print_val:
-                self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind+1) + '/' + str(how_many) + ')')
-            else:
-                self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
-
+            self.levels = 0   
+            new_time = time.time()
+            if new_time - self.time > self.min_time: 
+                if self.print_val:
+                    self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind+1) + '/' + str(how_many) + ')')
+                else:
+                    self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
+                self.time = new_time
             
     def tqdm(self, iterable, **kwargs):
         return self.weighted_tqdm(iterable, **kwargs)
     
     def qudit_tqdm(self, iterable, dit=2, exp=3, **kwargs):
         return self.weighted_tqdm(iterable, weights=lambda i: (dit**i)**exp, **kwargs)
       
 #p = progress(total=1000)
 #for i in p.weighted_tqdm(range(5), weights=lambda i: (i+1), name='outer'):
 #    for j in p.tqdm((1,2,3,4,5), name='inner'):
 #        time.sleep(0.1*(i+1))      
 
 class weighted_kronbinations_tqdm:
-    def __init__(self, list_of_iterators, list_of_weights, total=1000, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', **kwargs):
+    def __init__(self, list_of_iterators, list_of_weights, total=1000, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', max_rate=30, **kwargs):
         # this function takes a list of iterators and weights and returns a generator that iterates through the kronecker product of the iterators
         # Prepare data
         lengths = []
         weights = []
         for i, w in zip(list_of_iterators, list_of_weights):
             lengths.append(determine_length_of_iterable(i, w, **kwargs))
             weights_var, sum_weights = make_weight_list(i, lengths[-1], w)
             weights.append([j/sum_weights for j in weights_var])
         self.lengths = lengths
+        self.total_length = np.prod(lengths)
         self.weights = weights
         self.total = total
         # Variables for subincrements 
         # similar to progress class but lowest level is kronbinations level and 
         # treated differently
         self.levels = 0
         self.weight_by_level = []
         self.ind_by_level = []
         self.names = []
         self.bar_format = bar_format
+        self.last_update_time = time.time()
+        self.min_t = 1/max_rate
         
     def init(self, indexes, **kwargs):
         # indexes is a 2d array of indexes, where each row is an index and each column is an iterator
         # Construct a pbar object, and find the total weight  of all indexes to renormalize for the pbar
         # find sum_of_weights = sum([weight of every index]), with weight of an index being the product of the weights of the iterators that make up that index
         weights = []
         for ind in indexes:
@@ -277,27 +300,32 @@
         else:
             self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
                 
     def increment(self):
         # increment 
         curr_weight = self.curr_weights[self.curr_ind]
         self.curr_ind += 1
-        #self.pbar.set_description('(' +str(i) + '/' + str(self.len_indexes) + ')')
+        new_time = time.time()
+        if new_time - self.last_update_time > self.min_t:
+            self.pbar.set_description('(' +str(self.curr_ind) + '/' + str(self.total_length) + ')')
+            self.last_update_time = new_time
         if self.levels == 0:
             self.cumm_weight += curr_weight 
             new_index = round(self.cumm_weight)
             diff = new_index - self.curr_pbar_index
             self.curr_pbar_index = new_index
             self.pbar.update(diff)
         else: # reset sublevels
             self.levels = 0
             self.weight_by_level = []
             self.ind_by_level = []
             self.names = []
             
     def close(self):
+        self.pbar.set_description('(' +str(self.curr_ind) + '/' + str(self.total_length) + ')')
+        self.pbar.update(0)
         self.pbar.close()
         
     def all_indexes(self):
         list_of_indexes = [list(np.arange(0, len(l))) for l in list_of_iterators]
         return np.array(list(itertools.product(*list_of_indexes)))
```

### Comparing `weighted_tqdm-0.6/src/weighted_tqdm.egg-info/PKG-INFO` & `weighted_tqdm-0.7/src/weighted_tqdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: weighted-tqdm
-Version: 0.6
+Version: 0.7
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.6.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.7.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

