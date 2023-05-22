# Comparing `tmp/arulespy-0.1.0.tar.gz` & `tmp/arulespy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arulespy-0.1.0.tar", last modified: Sun May 21 01:35:21 2023, max compression
+gzip compressed data, was "arulespy-0.1.1.tar", last modified: Mon May 22 18:09:37 2023, max compression
```

## Comparing `arulespy-0.1.0.tar` & `arulespy-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.281930 arulespy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-21 01:35:07.000000 arulespy-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-21 01:35:07.000000 arulespy-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-05-21 01:35:21.281930 arulespy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-21 01:35:07.000000 arulespy-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 01:35:07.000000 arulespy-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 01:35:21.281930 arulespy-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-21 01:35:07.000000 arulespy-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.273930 arulespy-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.277930 arulespy-0.1.0/src/arulespy/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-21 01:35:07.000000 arulespy-0.1.0/src/arulespy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-05-21 01:35:07.000000 arulespy-0.1.0/src/arulespy/arules.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 01:35:07.000000 arulespy-0.1.0/src/arulespy/arulesViz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.281930 arulespy-0.1.0/src/arulespy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.281930 arulespy-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-21 01:35:07.000000 arulespy-0.1.0/tests/test_arules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-22 18:09:24.000000 arulespy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 18:09:24.000000 arulespy-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-22 18:09:37.122646 arulespy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-22 18:09:24.000000 arulespy-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 18:09:24.000000 arulespy-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 18:09:37.122646 arulespy-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-22 18:09:24.000000 arulespy-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/src/arulespy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-22 18:09:24.000000 arulespy-0.1.1/src/arulespy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-22 18:09:24.000000 arulespy-0.1.1/src/arulespy/arules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-22 18:09:24.000000 arulespy-0.1.1/src/arulespy/arulesViz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/src/arulespy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-22 18:09:24.000000 arulespy-0.1.1/tests/test_arules.py
```

### Comparing `arulespy-0.1.0/LICENSE` & `arulespy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arulespy-0.1.0/PKG-INFO` & `arulespy-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arulespy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python interface to the R package arules
 Home-page: https://github.com/mhahsler/arulespy
 Author: Michael Hahsler
 Author-email: mhahsler@lyle.smu.edu
 Project-URL: Documentation, https://github.com/mhahsler/arulespy
 Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
 Project-URL: Source Code, https://github.com/mhahsler/arulespy
@@ -55,20 +55,20 @@
 -   `Rules`: Association rules
 -   `Itemsets`: Itemsets
 -   `ItemMatrix`: sparse matrix representation of sets of items.
 
 with Phyton-style slicing and `len()`. 
 
 Most arules functions are
-interfaced with conversion from the R data structures to Python.
+interfaced as methods for the four classes with conversion from the R data structures to Python.
 Documentation is avaialible in Python via `help()`. Detailed online documentation
 for the R package is available [here](https://mhahsler.r-universe.dev/arules/doc/manual.html). 
 
 Low-level `arules` functions can also be directly used in the form 
-`arules.r.<arules R function>()`. The result will be a `rpy2` data type.
+`R.<arules R function>()`. The result will be a `rpy2` data type.
 Transactions, itemsets and rules can manually be converted to Python
 classes using the helper function `a2p()`.
 
 ## Installation
 
 `arulespy` is based on the python package `rpy2` which requires an R installation. Here are the installation steps:
 
@@ -98,52 +98,49 @@
 This will lead the python kernel to die or exit without explanation when the package `arulespy` is imported.
 Check `python -m rpy2.situation` to see if R and R's libraries are found.
 Details can be found [here](https://pypi.org/project/rpy2/).
 
 
 ## Example
 
-``` python
-from arulespy import arules
+```python
+from arulespy.arules import Transactions, apriori, parameters
 import pandas as pd
 
 # define the data as a pandas dataframe
 df = pd.DataFrame (
     [
         [True,True, True],
         [True, False,False],
         [True, True, True],
         [True, False, False],
         [True, True, True]
     ],
     columns=list ('ABC')) 
 
 # convert dataframe to transactions
-trans = arules.transactions(df)
+trans = transactions.from_df(df)
 
 # mine association rules
-rules = arules.apriori(trans,
-                    parameter = arules.parameters({"supp": 0.1, "conf": 0.8}), 
-                    control = arules.parameters({"verbose": False}))  
+rules = apriori(trans,
+                    parameter = parameters({"supp": 0.1, "conf": 0.8}), 
+                    control = parameters({"verbose": False}))  
 
 # display the rules as a pandas dataframe
 rules.as_df()
 ```
 
-```
-	LHS	    RHS     support	confidence	coverage	lift	count
-1	{}      {A}	    1.0     1.0	        1.0	        1.000000	5
-2	{B}     {C}	    0.6	    1.0	        0.6	        1.666667	3
-3	{C}     {B}	    0.6	    1.0	        0.6	        1.666667	3
-4	{B}     {A}	    0.6	    1.0	        0.6	        1.000000	3
-5	{C}     {A}	    0.6	    1.0	        0.6	        1.000000	3
-6	{B,C}   {A}	    0.6	    1.0	        0.6	        1.000000	3
-7	{A,B}   {C}	    0.6	    1.0	        0.6	        1.666667	3
-8	{A,C}   {B}	    0.6	    1.0	        0.6	        1.666667	3
-```
+|    | LHS   | RHS   |   support |   confidence |   coverage |   lift |   count |
+|---:|:------|:------|----------:|-------------:|-----------:|-------:|--------:|
+|  1 | {}    | {A}   |       0.8 |          0.8 |        1   |   1    |       8 |
+|  2 | {}    | {C}   |       0.8 |          0.8 |        1   |   1    |       8 |
+|  3 | {B}   | {A}   |       0.4 |          0.8 |        0.5 |   1    |       4 |
+|  4 | {B}   | {C}   |       0.5 |          1   |        0.5 |   1.25 |       5 |
+|  5 | {A,B} | {C}   |       0.4 |          1   |        0.4 |   1.25 |       4 |
+|  6 | {B,C} | {A}   |       0.4 |          0.8 |        0.5 |   1    |       4 |
 
 Complete examples:
   * [Using arules](https://mhahsler.github.io/arulespy/examples/arules.html)
   * [Using arulesViz](https://mhahsler.github.io/arulespy/examples/arulesViz.html)
 
 
 ## References
```

### Comparing `arulespy-0.1.0/README.md` & `arulespy-0.1.1/src/arulespy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: arulespy
+Version: 0.1.1
+Summary: Python interface to the R package arules
+Home-page: https://github.com/mhahsler/arulespy
+Author: Michael Hahsler
+Author-email: mhahsler@lyle.smu.edu
+Project-URL: Documentation, https://github.com/mhahsler/arulespy
+Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
+Project-URL: Source Code, https://github.com/mhahsler/arulespy
+Keywords: association rules,frequent itemsets
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: R
+Classifier: Programming Language :: C++
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Python interface to the R package arules
 
 [![PyPI
 package](https://img.shields.io/badge/pip%20install-arulespy-brightgreen)](https://pypi.org/project/arulespy/)
 [![version
 number](https://img.shields.io/pypi/v/arulespy?color=green&label=version)](https://github.com/mhahsler/arulespy/releases)
 [![Actions
@@ -30,20 +55,20 @@
 -   `Rules`: Association rules
 -   `Itemsets`: Itemsets
 -   `ItemMatrix`: sparse matrix representation of sets of items.
 
 with Phyton-style slicing and `len()`. 
 
 Most arules functions are
-interfaced with conversion from the R data structures to Python.
+interfaced as methods for the four classes with conversion from the R data structures to Python.
 Documentation is avaialible in Python via `help()`. Detailed online documentation
 for the R package is available [here](https://mhahsler.r-universe.dev/arules/doc/manual.html). 
 
 Low-level `arules` functions can also be directly used in the form 
-`arules.r.<arules R function>()`. The result will be a `rpy2` data type.
+`R.<arules R function>()`. The result will be a `rpy2` data type.
 Transactions, itemsets and rules can manually be converted to Python
 classes using the helper function `a2p()`.
 
 ## Installation
 
 `arulespy` is based on the python package `rpy2` which requires an R installation. Here are the installation steps:
 
@@ -73,52 +98,49 @@
 This will lead the python kernel to die or exit without explanation when the package `arulespy` is imported.
 Check `python -m rpy2.situation` to see if R and R's libraries are found.
 Details can be found [here](https://pypi.org/project/rpy2/).
 
 
 ## Example
 
-``` python
-from arulespy import arules
+```python
+from arulespy.arules import Transactions, apriori, parameters
 import pandas as pd
 
 # define the data as a pandas dataframe
 df = pd.DataFrame (
     [
         [True,True, True],
         [True, False,False],
         [True, True, True],
         [True, False, False],
         [True, True, True]
     ],
     columns=list ('ABC')) 
 
 # convert dataframe to transactions
-trans = arules.transactions(df)
+trans = transactions.from_df(df)
 
 # mine association rules
-rules = arules.apriori(trans,
-                    parameter = arules.parameters({"supp": 0.1, "conf": 0.8}), 
-                    control = arules.parameters({"verbose": False}))  
+rules = apriori(trans,
+                    parameter = parameters({"supp": 0.1, "conf": 0.8}), 
+                    control = parameters({"verbose": False}))  
 
 # display the rules as a pandas dataframe
 rules.as_df()
 ```
 
-```
-	LHS	    RHS     support	confidence	coverage	lift	count
-1	{}      {A}	    1.0     1.0	        1.0	        1.000000	5
-2	{B}     {C}	    0.6	    1.0	        0.6	        1.666667	3
-3	{C}     {B}	    0.6	    1.0	        0.6	        1.666667	3
-4	{B}     {A}	    0.6	    1.0	        0.6	        1.000000	3
-5	{C}     {A}	    0.6	    1.0	        0.6	        1.000000	3
-6	{B,C}   {A}	    0.6	    1.0	        0.6	        1.000000	3
-7	{A,B}   {C}	    0.6	    1.0	        0.6	        1.666667	3
-8	{A,C}   {B}	    0.6	    1.0	        0.6	        1.666667	3
-```
+|    | LHS   | RHS   |   support |   confidence |   coverage |   lift |   count |
+|---:|:------|:------|----------:|-------------:|-----------:|-------:|--------:|
+|  1 | {}    | {A}   |       0.8 |          0.8 |        1   |   1    |       8 |
+|  2 | {}    | {C}   |       0.8 |          0.8 |        1   |   1    |       8 |
+|  3 | {B}   | {A}   |       0.4 |          0.8 |        0.5 |   1    |       4 |
+|  4 | {B}   | {C}   |       0.5 |          1   |        0.5 |   1.25 |       5 |
+|  5 | {A,B} | {C}   |       0.4 |          1   |        0.4 |   1.25 |       4 |
+|  6 | {B,C} | {A}   |       0.4 |          0.8 |        0.5 |   1    |       4 |
 
 Complete examples:
   * [Using arules](https://mhahsler.github.io/arulespy/examples/arules.html)
   * [Using arulesViz](https://mhahsler.github.io/arulespy/examples/arulesViz.html)
 
 
 ## References
```

### Comparing `arulespy-0.1.0/setup.py` & `arulespy-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `arulespy-0.1.0/src/arulespy/__init__.py` & `arulespy-0.1.1/src/arulespy/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import rpy2.robjects as ro
 import rpy2.robjects.packages as packages
 import os
 
 os.makedirs(ro.r('Sys.getenv("R_LIBS_USER")')[0], exist_ok=True)
 ro.r('.libPaths(c(Sys.getenv("R_LIBS_USER"), .libPaths()))')
@@ -17,10 +17,10 @@
 
 if not ro.packages.isinstalled('arulesViz'):
     print("Installing R package arulesViz (plus dependencies).")
     utils.install_packages('arulesViz', 
                            repos='https://cloud.r-project.org/',
                            lib = ro.r('Sys.getenv("R_LIBS_USER")[1]'))
 
-
-from .arules import parameters, set, Associations, ItemMatrix, Rules, Itemsets, Transactions, R, a2p, encode, concat, apriori, eclat, discretizeDF, random_transactions                 
+              
+from .arules import parameters, Associations, ItemMatrix, Rules, Itemsets, Transactions, R, a2py, concat, apriori, eclat, discretizeDF
 from .arulesViz import plot, inspectDT
```

### Comparing `arulespy-0.1.0/src/arulespy/arules.py` & `arulespy-0.1.1/src/arulespy/arules.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,71 +9,60 @@
 
 ### activate automatic conversion of pandas dataframes to R dataframes
 #pandas2ri.activate()
 
 # install arules if necessary. Note: the system path is probably not writable for the user.
 # we try to create the directory so install.packages does not ask
 
-
 ### import the R arules package
 R = packages.importr('arules')
 methods = packages.importr('methods')
 base = packages.importr('base')
 
 ### arules interface code 
 
 def parameters(x):
     """define parameters for apriori and eclat"""
 
     return ro.ListVector(x)
 
-def set(x):
-    """define a set of items"""
-
-    return ro.StrVector(x)
 
 class ItemMatrix(ro.RS4):
     """Class for arules itemMatrix object"""
     
+    @staticmethod
+    def from_list(items, itemLabels):
+        items = [ro.StrVector(x) for x in items]
+        return ItemMatrix(R.encode(items, itemLabels))
+
     def as_df(self):
         """convert to pandas dataframe"""
         if type(self) != ro.vectors.DataFrame:
             self  = R.DATAFRAME(self)
         with (ro.default_converter + pandas2ri.converter).context():
             pd_df = ro.conversion.get_conversion().rpy2py(self)
         return pd_df
     
     def as_matrix(self):
         """convert to numpy matrix
-        
-        Args:
-            what: can be "items", "lhs", "rhs"
         """
+
         return np.array(ro.r('function(x) as(x, "matrix")')(self))
 
-    ### convert arules associations (rules/itemsets) into a dictionary (what can be "items", "lhs", "rhs")
     def as_dict(self):
         """convert to dictionary
-        
-        Args:
-            what can be "items", "lhs", "rhs"
         """
 
         l = ro.r('function(x) as(x, "list")')(self)
         l.names = [*range(0, len(l))]
         return dict(zip(l.names, map(list,list(l))))
       
     def as_list(self):
         """convert to list"""
         return list(self.as_dict().values())  
-    
-    @staticmethod
-    def from_list(items, itemLabels):
-        items = [ro.StrVector(x) for x in items]
-        return ItemMatrix(R.encode(items, itemLabels))
 
     def __getitem__(self, key):
         # prepare subset selection
         if isinstance(key, slice):
             key = list(range(key.stop)[key])  
         
         key = np.array(key)
@@ -104,119 +93,110 @@
     def sort(self, by = "lift", decreasing = True):
         """sort
         
         Args:
             by: the interest measure from the quality slot
             decreasing: sort decreasingly?
         """
-        if decreasing:
-            decreasing = "TRUE"
-        else:
-            decreasing = "FALSE"
-
-        return a2p(ro.r('function(x) sort(x, by = "' + by + '", decreasing = ' + decreasing + ')')(self))
+        decreasing  = ro.vectors.BoolVector([decreasing])
+        return a2py(ro.r('function(x, by, decreasing) sort(x, by = by, decreasing = decreasing)')(self, by, decreasing))
 
     def unique(self):
         """return unique elements"""
-        return a2p(ro.r('function(x) unique(x)')(self))
+        return a2py(ro.r('function(x) unique(x)')(self))
     
-    def sample(self, size = 1):
+    def sample(self, size = 1, replace = False):
         """sample from the set
         
         Args:
             size: number of samples
         """
-        return a2p(ro.r('function(x) sample(x, size = ' + str(size) + ')')(self))
+        replace = ro.vectors.BoolVector([replace])
+        return a2py(ro.r('function(x, size, replace) sample(x, size = size, replace = replace)')(self, size, replace))
     
     def items(self):
         """return items"""
-        return a2p(ro.r('function(x) items(x)')(self))
+        return ItemMatrix(ro.r('function(x) items(x)')(self))
     
     def itemFrequency(self, type = "absolute"):
         """return item frequency
         
         Args:
             type: "absolute" or "relative"
         """
-        return np.array(a2p(ro.r('function(x, type) itemFrequency(x, type)')(self, type)))
+        return np.array(a2py(ro.r('function(x, type) itemFrequency(x, type)')(self, type)))
     
     def itemInfo(self):
         """return item info as dataframe"""
-        return r2df(ro.r('function(x) itemInfo(x)')(self))
+        return a2py(ro.r('function(x) itemInfo(x)')(self))
     
     def labels(self):
         """returns a list of labels for the sets"""
-        return r2list(ro.r('function(x) labels(x)')(self))
+        return a2py(ro.r('function(x) labels(x)')(self))
     
     def is_subset(self, x, sparse = False):
         """check if x is a subset of self
         
         Args:
             x: the other set
             sparse: return sparse matrix representation?
         """    
-        if sparse:
-            sparse = "TRUE"
-        else:
-            sparse = "FALSE"
+        sparse = ro.vectors.BoolVector([sparse])
         return ro.r('function(x, y, sparse) is.subset(x, y, sparse)')(self, x, sparse)
     
     def is_superset(self, x, sparse = False):
         """check if x is a superset of self
         
         Args:
             x: the other set
             sparse: return sparse matrix representation?
         """
-        if sparse:
-            sparse = "TRUE"
-        else:
-            sparse = "FALSE"
+        sparse = ro.vectors.BoolVector([sparse])
         return ro.r('function(x, y, sparse) is.superset(x, y, sparse)')(self, x, sparse)
             
 
 class Associations(ItemMatrix):
     """Superclass for arules associations (rules/itemsets)"""
 
     def quality(self):
         """return quality measures as dataframe"""
-        return r2df(ro.r('function(x) quality(x)')(self))
+        return a2py(ro.r('function(x) quality(x)')(self))
 
     def is_closed(self):
         """return closedness as boolean vector"""
-        return r2list(ro.r('function(x) is.closed(x)')(self))
+        return a2py(ro.r('function(x) is.closed(x)')(self))
     
     def is_maximal(self):
         """return maximality as boolean vector"""
-        return r2list(ro.r('function(x) is.maximal(x)')(self))
+        return a2py(ro.r('function(x) is.maximal(x)')(self))
     
     def is_generator(self):
         """return generator as boolean vector"""
-        return r2list(ro.r('function(x) is.generator(x)')(self))
+        return a2py(ro.r('function(x) is.generator(x)')(self))
     
     def is_redundant(self):
         """return redundent rules as boolean vector"""
-        return r2list(ro.r('function(x) is.redundant(x)')(self))
+        return a2py(ro.r('function(x) is.redundant(x)')(self))
     
     def is_significant(self):
         """return significant rules as boolean vector"""
-        return r2list(ro.r('function(x) is.significant(x)')(self))
+        return a2py(ro.r('function(x) is.significant(x)')(self))
     
     def interestMeasure(self, measure = ["support", "confidence", "lift"], 
                         transactions = None):
         """calculate additional interest measures
         
         Args:
             measure: a list of interest measures (see: https://mhahsler.github.io/arules/docs/measures)
             transactions: the transactions to use (optional)
         """
         if transactions == None:
             transactions = ro.r('NULL')
-        return r2df(ro.r('function(x, measure, transactions) interestMeasure(x, measure, transactions)')
-                    (self, measure, transactions), column_names=measure)
+        return a2py(ro.r('function(x, measure, transactions) interestMeasure(x, measure, transactions)')
+                    (self, measure, transactions))
 
     def addQuality(self, df):
         """add quality measures to the associations.
         
         Args:
             df: a pandas dataframe with the same number of rows as the associations
         """
@@ -240,127 +220,109 @@
     def lhs(self):
         """return lhs as an itemMatrix"""
         return ItemMatrix(ro.r('function(x) lhs(x)')(self))
     
     def rhs(self):
         """return rhs as an itemMatrix"""
         return ItemMatrix(ro.r('function(x) rhs(x)')(self))
-
-    def as_matrix(self, what = "items"):
-        """return lhs/rhs as numpy matrix
-        
-        Args:
-            what: "lhs", "rhs", or "items"
-        """
-        return ItemMatrix(ro.r('function(x) ' + what + '(x)')(self)).as_matrix()
-    
-    def as_dict(self, what = "items"):
-        """return lhs/rhs as a dictionary
-        
-        Args:
-            what: "lhs", "rhs", or "items"
-        """
-        return ItemMatrix(ro.r('function(x) ' + what + '(x)')(self)).as_dict()
     
 
 
 class Itemsets(Associations):
     """Class for arules itemsets object"""
     
     @staticmethod
     def new(items, quality = None):
 
         if quality == None:
-             return a2p(methods.new("itemsets", items))
+             return a2py(methods.new("itemsets", items))
         else:
-            return a2p(methods.new("itemsets", items, quality))
+            return a2py(methods.new("itemsets", items, quality))
+    
+    def items(self):
+        """return items as an itemMatrix"""
+        return ItemMatrix(ro.r('function(x) lhs(x)')(self))
+
 
 class Transactions(ItemMatrix):
     """Class for arules transactions object"""
     
     @staticmethod
     def new(items):
         return Transactions(methods.new("transactions", items))
     
+    @staticmethod
     def from_df(x, itemLabels = None):
         """convert pandas dataframe into an arules transactions object"""
     
         with (ro.default_converter + ro.pandas2ri.converter).context():
             x_r = ro.conversion.get_conversion().py2rpy(x)
     
         if itemLabels == None:
             return Transactions(R.transactions(x_r))
         else:
             return Transactions(R.transactions(x_r, itemLabels))
 
 ### Conversion functions
 
-def a2p(x):
-    """convert arules S4 object to python object"""
+def a2py(x):
+    """convert arules S4 object to python object
+    
+    Conversion rules:
+    - rules: Python Rules object
+    - itemsets: Python Itemsets object
+    - transactions: Python Transactions object
+    - itemMatrix: Python ItemMatrix object
+    - data.frame: pandas dataframe
+    - character: string list
+    - integer: int list
+    - numeric: float list
+    - matrix: numpy matrix
+    """
 
     if x.rclass[0] == "rules":
         return Rules(x)
     elif x.rclass[0] == "itemsets":
         return Itemsets(x)
     elif x.rclass[0] == "transactions":
         return Transactions(x)
     elif x.rclass[0] == "itemMatrix":
         return ItemMatrix(x)
-    else:
-        return x
-
-def r2df(x, column_names = None):
-    """convert R dataframe to pandas dataframe"""
-
-    with (ro.default_converter + ro.pandas2ri.converter).context():
-        pd_df = ro.conversion.get_conversion().rpy2py(x)
-
-    if type(pd_df) != pd.core.frame.DataFrame:
-        pd_df = pd.DataFrame(pd_df, columns= column_names)   ### set column name!
-    return pd_df   
+    elif x.rclass[0] == "data.frame":
+        colnames = list(x.colnames)
+        with (ro.default_converter + ro.pandas2ri.converter).context():
+            pd_df = ro.conversion.get_conversion().rpy2py(x)
 
-def r2list(x):  
-    return list(x) 
+        if type(pd_df) != pd.core.frame.DataFrame:
+            pd_df = pd.DataFrame(pd_df, columns= colnames)   ### set column name!
+        return pd_df   
+    elif x.rclass[0] == "character" or x.rclass[0] == "integer" or x.rclass[0] == "numeric":
+        return list(x)
+    elif x.rclass[0] == "matrix":
+        return np.array(x)
 
-def r2df_decor(function):
-    """decorator to convert R dataframes to pandas dataframes"""
+    else:
+        return x
 
-    def wrapper(*args, **kwargs):
-        return r2df(function(*args, **kwargs))
-    return wrapper
 
-def r2list_decor(function):
-    """decorator to convert R lists to Python lists"""
+def a2py_decor(function):
+    """decorator to convert arules S4 objects to python objects"""
 
     def wrapper(*args, **kwargs):
-        return r2list(function(*args, **kwargs))
+        return a2py(function(*args, **kwargs))
     return wrapper
 
-def a2p_decor(function):
-    """decorator to convert arules S4 objects to python objects"""
 
-    def wrapper(*args, **kwargs):
-        return a2p(function(*args, **kwargs))
-    return wrapper
+# package functions
+discretizeDF = a2py_decor(R.discretizeDF)
+discretizeDF.__doc__ = R.discretizeDF.__doc__   
 
 
-apriori = a2p_decor(R.apriori)
+apriori = a2py_decor(R.apriori)
 apriori.__doc__ = R.apriori.__doc__
 
-eclat = a2p_decor(R.eclat)
+eclat = a2py_decor(R.eclat)
 eclat.__doc__ = R.eclat.__doc__
 
-
-### static functions
-encode = a2p_decor(R.encode)
-encode.__doc__ = R.encode.__doc__
-
 def concat(list):
     conc = methods.selectMethod("c", tuple(list[0].rclass)[0])
-    return a2p(conc(*list))
-
-discretizeDF = r2df_decor(R.discretizeDF)
-discretizeDF.__doc__ = R.discretizeDF.__doc__   
-
-random_transactions = a2p_decor(R.random_transactions)
-random_transactions.__doc__ = R.random_transactions.__doc__
-
+    return a2py(conc(*list))
```

### Comparing `arulespy-0.1.0/src/arulespy.egg-info/PKG-INFO` & `arulespy-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: arulespy
-Version: 0.1.0
-Summary: Python interface to the R package arules
-Home-page: https://github.com/mhahsler/arulespy
-Author: Michael Hahsler
-Author-email: mhahsler@lyle.smu.edu
-Project-URL: Documentation, https://github.com/mhahsler/arulespy
-Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
-Project-URL: Source Code, https://github.com/mhahsler/arulespy
-Keywords: association rules,frequent itemsets
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: R
-Classifier: Programming Language :: C++
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Python interface to the R package arules
 
 [![PyPI
 package](https://img.shields.io/badge/pip%20install-arulespy-brightgreen)](https://pypi.org/project/arulespy/)
 [![version
 number](https://img.shields.io/pypi/v/arulespy?color=green&label=version)](https://github.com/mhahsler/arulespy/releases)
 [![Actions
@@ -55,20 +30,20 @@
 -   `Rules`: Association rules
 -   `Itemsets`: Itemsets
 -   `ItemMatrix`: sparse matrix representation of sets of items.
 
 with Phyton-style slicing and `len()`. 
 
 Most arules functions are
-interfaced with conversion from the R data structures to Python.
+interfaced as methods for the four classes with conversion from the R data structures to Python.
 Documentation is avaialible in Python via `help()`. Detailed online documentation
 for the R package is available [here](https://mhahsler.r-universe.dev/arules/doc/manual.html). 
 
 Low-level `arules` functions can also be directly used in the form 
-`arules.r.<arules R function>()`. The result will be a `rpy2` data type.
+`R.<arules R function>()`. The result will be a `rpy2` data type.
 Transactions, itemsets and rules can manually be converted to Python
 classes using the helper function `a2p()`.
 
 ## Installation
 
 `arulespy` is based on the python package `rpy2` which requires an R installation. Here are the installation steps:
 
@@ -98,52 +73,49 @@
 This will lead the python kernel to die or exit without explanation when the package `arulespy` is imported.
 Check `python -m rpy2.situation` to see if R and R's libraries are found.
 Details can be found [here](https://pypi.org/project/rpy2/).
 
 
 ## Example
 
-``` python
-from arulespy import arules
+```python
+from arulespy.arules import Transactions, apriori, parameters
 import pandas as pd
 
 # define the data as a pandas dataframe
 df = pd.DataFrame (
     [
         [True,True, True],
         [True, False,False],
         [True, True, True],
         [True, False, False],
         [True, True, True]
     ],
     columns=list ('ABC')) 
 
 # convert dataframe to transactions
-trans = arules.transactions(df)
+trans = transactions.from_df(df)
 
 # mine association rules
-rules = arules.apriori(trans,
-                    parameter = arules.parameters({"supp": 0.1, "conf": 0.8}), 
-                    control = arules.parameters({"verbose": False}))  
+rules = apriori(trans,
+                    parameter = parameters({"supp": 0.1, "conf": 0.8}), 
+                    control = parameters({"verbose": False}))  
 
 # display the rules as a pandas dataframe
 rules.as_df()
 ```
 
-```
-	LHS	    RHS     support	confidence	coverage	lift	count
-1	{}      {A}	    1.0     1.0	        1.0	        1.000000	5
-2	{B}     {C}	    0.6	    1.0	        0.6	        1.666667	3
-3	{C}     {B}	    0.6	    1.0	        0.6	        1.666667	3
-4	{B}     {A}	    0.6	    1.0	        0.6	        1.000000	3
-5	{C}     {A}	    0.6	    1.0	        0.6	        1.000000	3
-6	{B,C}   {A}	    0.6	    1.0	        0.6	        1.000000	3
-7	{A,B}   {C}	    0.6	    1.0	        0.6	        1.666667	3
-8	{A,C}   {B}	    0.6	    1.0	        0.6	        1.666667	3
-```
+|    | LHS   | RHS   |   support |   confidence |   coverage |   lift |   count |
+|---:|:------|:------|----------:|-------------:|-----------:|-------:|--------:|
+|  1 | {}    | {A}   |       0.8 |          0.8 |        1   |   1    |       8 |
+|  2 | {}    | {C}   |       0.8 |          0.8 |        1   |   1    |       8 |
+|  3 | {B}   | {A}   |       0.4 |          0.8 |        0.5 |   1    |       4 |
+|  4 | {B}   | {C}   |       0.5 |          1   |        0.5 |   1.25 |       5 |
+|  5 | {A,B} | {C}   |       0.4 |          1   |        0.4 |   1.25 |       4 |
+|  6 | {B,C} | {A}   |       0.4 |          0.8 |        0.5 |   1    |       4 |
 
 Complete examples:
   * [Using arules](https://mhahsler.github.io/arulespy/examples/arules.html)
   * [Using arulesViz](https://mhahsler.github.io/arulespy/examples/arulesViz.html)
 
 
 ## References
```

### Comparing `arulespy-0.1.0/tests/test_arules.py` & `arulespy-0.1.1/tests/test_arules.py`

 * *Files identical despite different names*

