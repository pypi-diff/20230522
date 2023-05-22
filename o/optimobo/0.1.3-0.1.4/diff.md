# Comparing `tmp/optimobo-0.1.3.tar.gz` & `tmp/optimobo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimobo-0.1.3.tar", last modified: Mon May 22 12:09:36 2023, max compression
+gzip compressed data, was "optimobo-0.1.4.tar", last modified: Mon May 22 12:39:54 2023, max compression
```

## Comparing `optimobo-0.1.3.tar` & `optimobo-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:09:36.771198 optimobo-0.1.3/
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     1063 2023-05-20 14:55:19.000000 optimobo-0.1.3/LICENSE
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     3689 2023-05-22 12:09:36.767198 optimobo-0.1.3/PKG-INFO
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     3443 2023-05-20 19:14:19.000000 optimobo-0.1.3/README.md
-drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:09:36.767198 optimobo-0.1.3/optimobo/
--rw-rw-r--   0 lecky     (1000) lecky     (1000)        0 2023-05-22 11:49:17.000000 optimobo-0.1.3/optimobo/__init__.py
--rw-rw-r--   0 lecky     (1000) lecky     (1000)    16114 2023-05-20 15:16:09.000000 optimobo-0.1.3/optimobo/optimisers.py
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     7822 2023-05-20 14:58:32.000000 optimobo-0.1.3/optimobo/scalarisations.py
--rw-rw-r--   0 lecky     (1000) lecky     (1000)    11483 2023-05-18 23:42:13.000000 optimobo-0.1.3/optimobo/util_functions.py
-drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:09:36.767198 optimobo-0.1.3/optimobo.egg-info/
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     3689 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/PKG-INFO
--rw-rw-r--   0 lecky     (1000) lecky     (1000)      300 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/SOURCES.txt
--rw-rw-r--   0 lecky     (1000) lecky     (1000)        1 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/dependency_links.txt
--rw-rw-r--   0 lecky     (1000) lecky     (1000)       73 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/requires.txt
--rw-rw-r--   0 lecky     (1000) lecky     (1000)        9 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/top_level.txt
--rw-rw-r--   0 lecky     (1000) lecky     (1000)       38 2023-05-22 12:09:36.771198 optimobo-0.1.3/setup.cfg
--rw-rw-r--   0 lecky     (1000) lecky     (1000)      634 2023-05-22 12:09:33.000000 optimobo-0.1.3/setup.py
-drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:09:36.767198 optimobo-0.1.3/tests/
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     6837 2023-05-20 18:55:15.000000 optimobo-0.1.3/tests/testing.py
+drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:39:54.945690 optimobo-0.1.4/
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     1063 2023-05-20 14:55:19.000000 optimobo-0.1.4/LICENSE
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     3689 2023-05-22 12:39:54.945690 optimobo-0.1.4/PKG-INFO
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     3443 2023-05-20 19:14:19.000000 optimobo-0.1.4/README.md
+drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:39:54.945690 optimobo-0.1.4/optimobo/
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)        0 2023-05-22 11:49:17.000000 optimobo-0.1.4/optimobo/__init__.py
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)    16214 2023-05-22 12:39:04.000000 optimobo-0.1.4/optimobo/optimisers.py
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     7822 2023-05-20 14:58:32.000000 optimobo-0.1.4/optimobo/scalarisations.py
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)    11483 2023-05-18 23:42:13.000000 optimobo-0.1.4/optimobo/util_functions.py
+drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:39:54.945690 optimobo-0.1.4/optimobo.egg-info/
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     3689 2023-05-22 12:39:54.000000 optimobo-0.1.4/optimobo.egg-info/PKG-INFO
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)      300 2023-05-22 12:39:54.000000 optimobo-0.1.4/optimobo.egg-info/SOURCES.txt
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)        1 2023-05-22 12:39:54.000000 optimobo-0.1.4/optimobo.egg-info/dependency_links.txt
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)       73 2023-05-22 12:39:54.000000 optimobo-0.1.4/optimobo.egg-info/requires.txt
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)        9 2023-05-22 12:39:54.000000 optimobo-0.1.4/optimobo.egg-info/top_level.txt
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)       38 2023-05-22 12:39:54.945690 optimobo-0.1.4/setup.cfg
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)      634 2023-05-22 12:39:49.000000 optimobo-0.1.4/setup.py
+drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:39:54.945690 optimobo-0.1.4/tests/
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     6837 2023-05-20 18:55:15.000000 optimobo-0.1.4/tests/testing.py
```

### Comparing `optimobo-0.1.3/LICENSE` & `optimobo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.3/PKG-INFO` & `optimobo-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimobo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Solve multi-objective problems using Bayesian optimisation.
 Author: aje220
 Author-email: aje220@exeter.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `optimobo-0.1.3/README.md` & `optimobo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.3/optimobo/optimisers.py` & `optimobo-0.1.4/optimobo/optimisers.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn.gaussian_process import GaussianProcessRegressor
 from scipy.stats import qmc
 from scipy.stats import norm
 from scipy.optimize import differential_evolution
 from pymoo.util.ref_dirs import get_reference_directions
-from pymoo.indicators.hv import HV
-from pymoo.core.problem import ElementwiseProblem
+# from pymoo.indicators.hv import HV
+# from pymoo.core.problem import ElementwiseProblem
 
 
-from util_functions import EHVI, calc_pf, EIPBI, EITCH, expected_decomposition
-from scalarisations import ExponentialWeightedCriterion, IPBI, PBI, Tchebicheff, WeightedNorm, WeightedPower, WeightedProduct, AugmentedTchebicheff, ModifiedTchebicheff
+# from util_functions import EHVI, calc_pf, expected_decomposition
+from . import util_functions
+
+
+# from scalarisations import ExponentialWeightedCriterion, IPBI, PBI, Tchebicheff, WeightedNorm, WeightedPower, WeightedProduct, AugmentedTchebicheff, ModifiedTchebicheff
 
 
 class MultiSurrogateOptimiser:
     """
     Class that allows optimisation of multi-objective problems using a multi-surrogate methodology.
     This method creates multiple probabalistic models, one for each objective.
     Constraints not supported.
@@ -162,19 +165,19 @@
 
             # With each iteration we select a random weight vector, this is to improve diversity.
             ref_dir = np.asarray(ref_dirs[np.random.randint(0,len(ref_dirs))])
 
             # Retrieve the next sample point.
             X_next = None
             if acquisition_func is None:
-                pf = calc_pf(ysample)
-                X_next, _, = self._get_proposed_EHVI(EHVI, models, self.ideal_point, self.max_point, pf, cached_samples)
+                pf = util_functions.calc_pf(ysample)
+                X_next, _, = self._get_proposed_EHVI(util_functions.EHVI, models, self.ideal_point, self.max_point, pf, cached_samples)
             else:
                 min_scalar =  np.min([acquisition_func(y, ref_dir) for y in ysample])
-                X_next, _, _ = self._get_proposed_scalarisation(expected_decomposition, models, min_scalar, acquisition_func, ref_dir, cached_samples)
+                X_next, _, _ = self._get_proposed_scalarisation(util_functions.expected_decomposition, models, min_scalar, acquisition_func, ref_dir, cached_samples)
 
 
             # expected_decomposition([1,1], models, ref_dir, acquisition_func, min_scalar, cached_samples)
 
             # Evaluate the next input.
             y_next = self._objective_function(problem, X_next)
 
@@ -185,15 +188,15 @@
             Xsample = np.vstack((Xsample, X_next))
 
         # Get hypervolume metric.
         # ref_point = self.max_point
         # HV_ind = HV(ref_point=ref_point)
         # hv = HV_ind(ysample)
 
-        pf_approx = calc_pf(ysample)
+        pf_approx = util_functions.calc_pf(ysample)
 
         if display_pareto_front:
             plt.scatter(ysample[5:,0], ysample[5:,1], color="red", label="Samples.")
             plt.scatter(ysample[0:n_init_samples,0], ysample[0:n_init_samples,1], color="blue", label="Initial samples.")
             plt.scatter(pf_approx[:,0], pf_approx[:,1], color="green", label="PF approximation.")
             plt.scatter(ysample[-1:-5:-1,0], ysample[-1:-5:-1,1], color="black", label="Last 5 samples.")
             plt.xlabel(r"$f_1(x)$")
@@ -358,15 +361,15 @@
             agg = aggregation_func(next_y, ref_dir)
 
             aggregated_samples = np.append(aggregated_samples, agg)
 
             # Add the variables into the archives.
             Xsample = np.vstack((Xsample, next_X))
         
-        pf_approx = calc_pf(ysample)
+        pf_approx = util_functions.calc_pf(ysample)
 
         if display_pareto_front:
             plt.scatter(ysample[5:,0], ysample[5:,1], color="red", label="Samples.")
             plt.scatter(ysample[0:n_init_samples,0], ysample[0:n_init_samples,1], color="blue", label="Initial samples.")
             plt.scatter(pf_approx[:,0], pf_approx[:,1], color="green", label="PF approximation.")
             plt.scatter(ysample[-1:-5:-1,0], ysample[-1:-5:-1,1], color="black", label="Last 5 samples.", zorder=10)
             plt.xlabel(r"$f_1(x)$")
```

### Comparing `optimobo-0.1.3/optimobo/scalarisations.py` & `optimobo-0.1.4/optimobo/scalarisations.py`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.3/optimobo/util_functions.py` & `optimobo-0.1.4/optimobo/util_functions.py`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.3/optimobo.egg-info/PKG-INFO` & `optimobo-0.1.4/optimobo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimobo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Solve multi-objective problems using Bayesian optimisation.
 Author: aje220
 Author-email: aje220@exeter.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `optimobo-0.1.3/setup.py` & `optimobo-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
    name='optimobo',
-   version='0.1.3',
+   version='0.1.4',
    license='MIT',
    description='Solve multi-objective problems using Bayesian optimisation.',
    long_description=long_description,
    long_description_content_type='text/markdown',
    author='aje220',
    author_email='aje220@exeter.ac.uk',
    packages=['optimobo'],  #same as name
```

### Comparing `optimobo-0.1.3/tests/testing.py` & `optimobo-0.1.4/tests/testing.py`

 * *Files identical despite different names*

