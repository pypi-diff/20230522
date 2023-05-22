# Comparing `tmp/ito_diffusions-1.3.0.tar.gz` & `tmp/ito_diffusions-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ito_diffusions-1.3.0.tar", last modified: Mon Jul 25 18:44:49 2022, max compression
+gzip compressed data, was "ito_diffusions-1.4.0.tar", last modified: Mon May 22 08:43:24 2023, max compression
```

## Comparing `ito_diffusions-1.3.0.tar` & `ito_diffusions-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1001)        0 2022-07-25 18:44:49.959915 ito_diffusions-1.3.0/
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    35129 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/LICENSE.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     1249 2022-07-25 18:44:49.959915 ito_diffusions-1.3.0/PKG-INFO
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)      937 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/README.md
-drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1001)        0 2022-07-25 18:44:49.955915 ito_diffusions-1.3.0/ito_diffusions/
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)      235 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/ito_diffusions/__init__.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     6410 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/ito_diffusions/ito_diffusion.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    35786 2022-07-25 18:39:08.000000 ito_diffusions-1.3.0/ito_diffusions/ito_diffusion_1d.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    21063 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/ito_diffusions/ito_diffusion_multi_d.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    12583 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/ito_diffusions/ito_diffusion_sheaf.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     6218 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/ito_diffusions/noise.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     3807 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/ito_diffusions/pdmp.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     3818 2022-07-25 18:41:31.000000 ito_diffusions-1.3.0/ito_diffusions/pdmp_1d.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     5185 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/ito_diffusions/saw.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     3503 2022-07-25 18:38:28.000000 ito_diffusions-1.3.0/ito_diffusions/sle.py
-drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1001)        0 2022-07-25 18:44:49.959915 ito_diffusions-1.3.0/ito_diffusions.egg-info/
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     1249 2022-07-25 18:44:49.000000 ito_diffusions-1.3.0/ito_diffusions.egg-info/PKG-INFO
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)      508 2022-07-25 18:44:49.000000 ito_diffusions-1.3.0/ito_diffusions.egg-info/SOURCES.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)        1 2022-07-25 18:44:49.000000 ito_diffusions-1.3.0/ito_diffusions.egg-info/dependency_links.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)       31 2022-07-25 18:44:49.000000 ito_diffusions-1.3.0/ito_diffusions.egg-info/requires.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)       15 2022-07-25 18:44:49.000000 ito_diffusions-1.3.0/ito_diffusions.egg-info/top_level.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)       38 2022-07-25 18:44:49.959915 ito_diffusions-1.3.0/setup.cfg
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)      563 2022-07-25 18:42:38.000000 ito_diffusions-1.3.0/setup.py
+drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1001)        0 2023-05-22 08:43:24.367065 ito_diffusions-1.4.0/
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    35129 2022-09-27 21:41:13.000000 ito_diffusions-1.4.0/LICENSE.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     1390 2023-05-22 08:43:24.367065 ito_diffusions-1.4.0/PKG-INFO
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     1078 2023-05-22 08:41:10.000000 ito_diffusions-1.4.0/README.md
+drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1001)        0 2023-05-22 08:43:24.367065 ito_diffusions-1.4.0/ito_diffusions/
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)      310 2023-05-21 12:33:44.000000 ito_diffusions-1.4.0/ito_diffusions/__init__.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     6727 2023-05-21 12:34:43.000000 ito_diffusions-1.4.0/ito_diffusions/ito_diffusion.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    35992 2023-05-21 12:33:57.000000 ito_diffusions-1.4.0/ito_diffusions/ito_diffusion_1d.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    20667 2023-05-21 12:34:19.000000 ito_diffusions-1.4.0/ito_diffusions/ito_diffusion_multi_d.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    12600 2023-05-21 12:35:02.000000 ito_diffusions-1.4.0/ito_diffusions/ito_diffusion_sheaf.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     6200 2023-05-21 12:33:33.000000 ito_diffusions-1.4.0/ito_diffusions/noise.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     3853 2023-05-21 12:35:34.000000 ito_diffusions-1.4.0/ito_diffusions/pdmp.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     3924 2023-05-21 12:35:25.000000 ito_diffusions-1.4.0/ito_diffusions/pdmp_1d.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     5237 2023-05-21 12:35:49.000000 ito_diffusions-1.4.0/ito_diffusions/saw.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     3555 2023-05-21 12:36:01.000000 ito_diffusions-1.4.0/ito_diffusions/sle.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)    21135 2023-05-22 08:18:52.000000 ito_diffusions-1.4.0/ito_diffusions/time_series.py
+drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1001)        0 2023-05-22 08:43:24.367065 ito_diffusions-1.4.0/ito_diffusions.egg-info/
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)     1390 2023-05-22 08:43:24.000000 ito_diffusions-1.4.0/ito_diffusions.egg-info/PKG-INFO
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)      538 2023-05-22 08:43:24.000000 ito_diffusions-1.4.0/ito_diffusions.egg-info/SOURCES.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)        1 2023-05-22 08:43:24.000000 ito_diffusions-1.4.0/ito_diffusions.egg-info/dependency_links.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)       31 2023-05-22 08:43:24.000000 ito_diffusions-1.4.0/ito_diffusions.egg-info/requires.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)       15 2023-05-22 08:43:24.000000 ito_diffusions-1.4.0/ito_diffusions.egg-info/top_level.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)       38 2023-05-22 08:43:24.367065 ito_diffusions-1.4.0/setup.cfg
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1001)      563 2023-05-22 08:42:08.000000 ito_diffusions-1.4.0/setup.py
```

### Comparing `ito_diffusions-1.3.0/LICENSE.txt` & `ito_diffusions-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ito_diffusions-1.3.0/PKG-INFO` & `ito_diffusions-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: ito_diffusions
-Version: 1.3.0
+Version: 1.4.0
 Summary: Library for stochastic process simulation
 Home-page: https://github.com/sauxpa/ito_diffusions
 Author: Patrick Saux
 Author-email: patrick.jr.saux@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### ito_diffusions
 Libraries for stochastic processes simulation and visualization including:
 * Ito diffusion : Brownian motion, Geometric Brownian motion, Vasicek, CIR...
-* Jump processes : Ito diffusion driven by a Levy process i.e with a jump component with a given intensity and jump size distribution
-* Multidimensional processes, stochastic volatility diffusions (SABR...)
-* Fractional Brownian motion, Karhunen-Loeve expansion, fractional diffusions
-* Self-Avoiding Walks (SAW), Schramm-Loewner Evolution (SLE)
+* Jump processes : Ito diffusion driven by a Levy process i.e with a jump component with a given intensity and jump size distribution;
+* Multidimensional processes, stochastic volatility diffusions (SABR...);
+* Fractional Brownian motion, Karhunen-Loeve expansion, fractional diffusions;
+* Times series models (AR, MA, ARMA, ARCH, GARCH, NAGARCH...);
+* Self-Avoiding Walks (SAW), Schramm-Loewner Evolution (SLE).
 
 **To install** : pip install ito-diffusions
 https://pypi.org/project/ito-diffusions/
 
 
 **To test** : python -m pytest
 
 For numerous examples : https://github.com/sauxpa/stochastic
 
 <img src="./brownian_sheaf.png"
      style="float: left; margin-right: 10px;" />
 
+<img src="./nagarch.png"
+     style="float: left; margin-right: 10px;" />
 
 <img src="./saw_square.png"
      style="float: left; margin-right: 10px;" />
 
 <img src="./sle_peaks.png"
      style="float: left; margin-right: 10px;" />
```

### Comparing `ito_diffusions-1.3.0/README.md` & `ito_diffusions-1.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 ### ito_diffusions
 Libraries for stochastic processes simulation and visualization including:
 * Ito diffusion : Brownian motion, Geometric Brownian motion, Vasicek, CIR...
-* Jump processes : Ito diffusion driven by a Levy process i.e with a jump component with a given intensity and jump size distribution
-* Multidimensional processes, stochastic volatility diffusions (SABR...)
-* Fractional Brownian motion, Karhunen-Loeve expansion, fractional diffusions
-* Self-Avoiding Walks (SAW), Schramm-Loewner Evolution (SLE)
+* Jump processes : Ito diffusion driven by a Levy process i.e with a jump component with a given intensity and jump size distribution;
+* Multidimensional processes, stochastic volatility diffusions (SABR...);
+* Fractional Brownian motion, Karhunen-Loeve expansion, fractional diffusions;
+* Times series models (AR, MA, ARMA, ARCH, GARCH, NAGARCH...);
+* Self-Avoiding Walks (SAW), Schramm-Loewner Evolution (SLE).
 
 **To install** : pip install ito-diffusions
 https://pypi.org/project/ito-diffusions/
 
 
 **To test** : python -m pytest
 
 For numerous examples : https://github.com/sauxpa/stochastic
 
 <img src="./brownian_sheaf.png"
      style="float: left; margin-right: 10px;" />
 
+<img src="./nagarch.png"
+     style="float: left; margin-right: 10px;" />
 
 <img src="./saw_square.png"
      style="float: left; margin-right: 10px;" />
 
 <img src="./sle_peaks.png"
      style="float: left; margin-right: 10px;" />
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/ito_diffusion.py` & `ito_diffusions-1.4.0/ito_diffusions/ito_diffusion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+# Author: Patrick Saux <patrick.saux@inria.fr>
+
 import numpy as np
 import abc
 from collections import defaultdict
 from .noise import Fractional_Gaussian_Noise
+from typing import List, Union
 
 
 class Ito_diffusion(abc.ABC):
     """Generic class for Ito diffusion
     dX_t = b(t,X_t)dt + sigma(t,X_t)*dW_t
     with a potential boundary condition at barrier.
     Supports standard gaussian noise and fractional gaussian noise
     Typical example : barrier=0, barrier_condition='absorb'
     (only this one is supported for now)
     """
 
     def __init__(
         self,
-        x0: float = 0.0,
+        x0: Union[float, List] = 0.0,
         T: float = 1.0,
         scheme_steps: int = 100,
         barrier: None = None,
         barrier_condition: None = None,
         noise_params: defaultdict = defaultdict(float),
         jump_params: defaultdict = defaultdict(float),
         rng: np.random._generator.Generator = np.random.default_rng(),
@@ -54,22 +57,29 @@
         else:
             self._noise = None
 
         # For tqdm
         self._verbose = verbose
 
     @property
-    def x0(self) -> float:
+    def x0(self) -> Union[float, List]:
         return self._x0
 
     @x0.setter
-    def x0(self, new_x0: float) -> None:
+    def x0(self, new_x0: Union[float, List]) -> None:
         self._x0 = new_x0
 
     @property
+    def len_x0(self) -> int:
+        if hasattr(self.x0, "__len__"):
+            return len(self.x0)
+        else:
+            return 1
+
+    @property
     def T(self) -> float:
         return self._T
 
     @T.setter
     def T(self, new_T) -> None:
         self._T = new_T
 
@@ -197,25 +207,25 @@
         return self.T / self.scheme_steps
 
     @property
     def scheme_step_sqrt(self) -> float:
         return np.sqrt(self.scheme_step)
 
     @property
-    def time_steps(self) -> np.ndarray:
+    def time_steps(self) -> List:
         return np.linspace(0, self.T, self.scheme_steps + 1)
 
     def barrier_crossed(self, x, y, barrier) -> bool:
         """barrier is crossed if x and y are on each side of the barrier"""
         return (x <= barrier and y >= barrier) or (x >= barrier and y <= barrier)
 
     @abc.abstractmethod
-    def drift(self, t, x):
+    def drift(self, t: float, x: Union[float, List]):
         pass
 
     @abc.abstractmethod
-    def vol(self, t, x):
+    def vol(self, t: float, x: Union[float, List]):
         pass
 
     @abc.abstractmethod
     def simulate(self):
         pass
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/ito_diffusion_1d.py` & `ito_diffusions-1.4.0/ito_diffusions/ito_diffusion_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+# Author: Patrick Saux <patrick.saux@inria.fr>
+
 import numpy as np
-from numpy import random as rd
 import pandas as pd
 import abc
 from functools import lru_cache
 from collections import defaultdict
 from scipy.stats import uniform
 from typing import Callable, Union
 from tqdm import tqdm
@@ -116,24 +117,24 @@
         self._vol_double = float(vol)
 
     @property
     def drift_double(self) -> float:
         return self._drift_double
 
     @drift_double.setter
-    def drift_double(self, new_drift) -> None:
-        self._drift_double = new_drift
+    def drift_double(self, new_drift: float) -> None:
+        self._drift_double = float(new_drift)
 
     @property
     def vol_double(self) -> float:
         return self._vol_double
 
     @vol_double.setter
-    def vol_double(self, new_vol) -> None:
-        self._vol_double = new_vol
+    def vol_double(self, new_vol: float) -> None:
+        self._vol_double = float(new_vol)
 
     def drift(self, t, x) -> float:
         return self.drift_double
 
     def vol(self, t, x) -> float:
         return self.vol_double
 
@@ -173,24 +174,24 @@
         self._vol_double = float(vol)
 
     @property
     def drift_double(self) -> float:
         return self._drift_double
 
     @drift_double.setter
-    def drift_double(self, new_drift) -> None:
-        self._drift_double = new_drift
+    def drift_double(self, new_drift: float) -> None:
+        self._drift_double = float(new_drift)
 
     @property
     def vol_double(self) -> float:
         return self._vol_double
 
     @vol_double.setter
-    def vol_double(self, new_vol) -> None:
-        self._vol_double = new_vol
+    def vol_double(self, new_vol: float) -> None:
+        self._vol_double = float(new_vol)
 
     def drift(self, t, x) -> float:
         return self.drift_double * x
 
     def vol(self, t, x) -> float:
         return self.vol_double * x
 
@@ -248,16 +249,16 @@
         self._d = new_d
 
     @property
     def vol_double(self) -> float:
         return self._vol_double
 
     @vol_double.setter
-    def vol_double(self, new_vol) -> None:
-        self._vol_double = new_vol
+    def vol_double(self, new_vol: float) -> None:
+        self._vol_double = float(new_vol)
 
     def drift(self, t, x) -> float:
         return 0.5 * (self.d - 1) / x
 
     def vol(self, t, x) -> float:
         return self.vol_double * x
 
@@ -391,27 +392,27 @@
             barrier=barrier,
             barrier_condition=barrier_condition,
             noise_params=noise_params,
             jump_params=jump_params,
             verbose=verbose,
             **kwargs,
         )
-        self._drift_double = drift
+        self._drift_double = float(drift)
         self._sigma = sigma
         self._shift = shift
         self._mixing = mixing
         self._L = L
 
     @property
     def drift_double(self) -> float:
         return self._drift_double
 
     @drift_double.setter
-    def drift_double(self, new_drift) -> None:
-        self._drift_double = new_drift
+    def drift_double(self, new_drift: float) -> None:
+        self._drift_double = float(new_drift)
 
     @property
     def sigma(self) -> float:
         return self._sigma
 
     @sigma.setter
     def sigma(self, new_sigma) -> None:
@@ -505,16 +506,16 @@
         self._long_term = new_long_term
 
     @property
     def vol_double(self) -> float:
         return self._vol_double
 
     @vol_double.setter
-    def vol_double(self, new_vol) -> None:
-        self._vol_double = new_vol
+    def vol_double(self, new_vol: float) -> None:
+        self._vol_double = float(new_vol)
 
     def drift(self, t, x) -> float:
         return self.mean_reversion * (self.long_term - x)
 
     def vol(self, t, x) -> float:
         return self.vol_double
 
@@ -572,16 +573,16 @@
         self._long_term = new_long_term
 
     @property
     def vol_double(self) -> float:
         return self._vol_double
 
     @vol_double.setter
-    def vol_double(self, new_vol) -> None:
-        self._vol_double = new_vol
+    def vol_double(self, new_vol: float) -> None:
+        self._vol_double = float(new_vol)
 
     @property
     def feller_condition(self) -> bool:
         """Returns whether mean_reversion * long_term > 0.5*vol^2"""
         return self.mean_reversion * self.long_term > 0.5 * self.vol_double**2
 
     def drift(self, t, x) -> float:
@@ -676,24 +677,24 @@
         self._vol_double = float(vol)
 
     @property
     def drift_double(self) -> float:
         return self._drift_double
 
     @drift_double.setter
-    def drift_double(self, new_drift) -> None:
-        self._drift_double = new_drift
+    def drift_double(self, new_drift: float) -> None:
+        self._drift_double = float(new_drift)
 
     @property
     def vol_double(self) -> float:
         return self._vol_double
 
     @vol_double.setter
-    def vol_double(self, new_vol) -> None:
-        self._vol_double = new_vol
+    def vol_double(self, new_vol: float) -> None:
+        self._vol_double = float(new_vol)
 
     def drift(self, t, x) -> float:
         return self.drift_double
 
     def vol(self, t, x) -> float:
         return self.vol_double * x
 
@@ -897,16 +898,16 @@
         self._alpha = new_alpha
 
     @property
     def vol_double(self) -> float:
         return self._vol_double
 
     @vol_double.setter
-    def vol_double(self, new_vol) -> None:
-        self._vol_double = new_vol
+    def vol_double(self, new_vol: float) -> None:
+        self._vol_double = float(new_vol)
 
     def _h(self, t) -> float:
         if t == self.T:
             return 0
         else:
             return self.alpha / (self.T - t)
 
@@ -1103,24 +1104,24 @@
         self.jump_params["jump_size_distr"] = new_jump_size_distr
 
     @property
     def drift_double(self) -> float:
         return self._drift_double
 
     @drift_double.setter
-    def drift_double(self, new_drift) -> None:
-        self._drift_double = new_drift
+    def drift_double(self, new_drift: float) -> None:
+        self._drift_double = float(new_drift)
 
     @property
     def vol_double(self) -> float:
         return self._vol_double
 
     @vol_double.setter
-    def vol_double(self, new_vol) -> None:
-        self._vol_double = new_vol
+    def vol_double(self, new_vol: float) -> None:
+        self._vol_double = float(new_vol)
 
     def drift(self, t, x) -> float:
         return self.drift_double
 
     def vol(self, t, x) -> float:
         return self.vol_double
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/ito_diffusion_multi_d.py` & `ito_diffusions-1.4.0/ito_diffusions/ito_diffusion_multi_d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# Author: Patrick Saux <patrick.saux@inria.fr>
+
 import numpy as np
 from numpy import random as rd
 import pandas as pd
 from tqdm import tqdm
 from collections import defaultdict
 from .ito_diffusion import Ito_diffusion
+from typing import List
 
 
 class Ito_diffusion_multi_d(Ito_diffusion):
     """Generic class for multidimensional Ito diffusion
     x0, drift and vol can be supplied as list/np.array...
     they will be casted to np.array
     x0 : initial vector, the dimension d of which is used to infer the
@@ -18,21 +21,21 @@
     Potential boundary condition at barrier=(x1,...,xd).
     Example syntax : barrier=(0, None) means the boundary condition is on the
     first coordinate only, at 0.
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.zeros(1),
+        x0: List = np.zeros(1),
         T: float = 1.0,
         scheme_steps: int = 100,
         n_factors: int = 1,
         keys: None = None,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         jump_params: defaultdict = defaultdict(int),
         verbose: bool = False,
         **kwargs,
     ) -> None:
 
         x0 = np.array(x0)
         super().__init__(
@@ -108,22 +111,22 @@
     """Instantiate Ito_diffusion to simulate a drifted Brownian motion
     dX_t = drift*dt + vol*dW_t
     where drift and vol are real vector and matrix respectively
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.zeros(1),
+        x0: List = np.zeros(1),
         T: float = 1.0,
         scheme_steps: int = 100,
-        drift: np.ndarray = np.zeros(1),
-        vol: np.ndarray = np.eye(1),
+        drift: List = np.zeros(1),
+        vol: List = np.eye(1),
         keys: None = None,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         verbose: bool = False,
         **kwargs,
     ) -> None:
         self._drift_vector = np.array(drift)
         # vol is actually a covariance matrix here
         self._vol_matrix = np.array(vol)
         n_factors = self._vol_matrix.shape[1]
@@ -136,52 +139,52 @@
             barrier=barrier,
             barrier_condition=barrier_condition,
             verbose=verbose,
             **kwargs,
         )
 
     @property
-    def drift_vector(self) -> np.ndarray:
+    def drift_vector(self) -> List:
         return self._drift_vector
 
     @drift_vector.setter
-    def drift_vector(self, new_drift: np.ndarray) -> None:
+    def drift_vector(self, new_drift: List) -> None:
         self._drift_vector = np.array(new_drift)
 
     @property
-    def vol_matrix(self) -> np.ndarray:
+    def vol_matrix(self) -> List:
         return self._vol_matrix
 
     @vol_matrix.setter
-    def vol_matrix(self, new_vol: np.ndarray) -> None:
+    def vol_matrix(self, new_vol: List) -> None:
         self._vol_matrix = np.array(new_vol)
 
-    def drift(self, t, x) -> np.ndarray:
+    def drift(self, t, x) -> List:
         return self.drift_vector
 
-    def vol(self, t, x) -> np.ndarray:
+    def vol(self, t, x) -> List:
         return self.vol_matrix
 
 
 class GBM_multi_d(Ito_diffusion_multi_d):
     """Instantiate Ito_diffusion to simulate a geometric Brownian motion
     dX_t = drift*X_t*dt + vol*X_t*dW_t
     where drift and vol are real vector and matrix respectively
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.ones(1),
+        x0: List = np.ones(1),
         T: float = 1.0,
         scheme_steps: int = 100,
-        drift: np.ndarray = np.zeros(1),
-        vol: np.ndarray = np.eye(1),
+        drift: List = np.zeros(1),
+        vol: List = np.eye(1),
         keys: None = None,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         verbose: bool = False,
         **kwargs,
     ) -> None:
         self._drift_vector = np.array(drift)
         # vol is actually a covariance matrix here
         self._vol_matrix = np.array(vol)
         n_factors = self._vol_matrix.shape[1]
@@ -194,54 +197,54 @@
             barrier=barrier,
             barrier_condition=barrier_condition,
             verbose=verbose,
             **kwargs,
         )
 
     @property
-    def drift_vector(self) -> np.ndarray:
+    def drift_vector(self) -> List:
         return self._drift_vector
 
     @drift_vector.setter
-    def drift_vector(self, new_drift: np.ndarray) -> np.ndarray:
+    def drift_vector(self, new_drift: List) -> List:
         self._drift_vector = np.array(new_drift)
 
     @property
-    def vol_matrix(self) -> np.ndarray:
+    def vol_matrix(self) -> List:
         return self._vol_matrix
 
     @vol_matrix.setter
-    def vol_matrix(self, new_vol: np.ndarray) -> None:
+    def vol_matrix(self, new_vol: List) -> None:
         self._vol_matrix = np.array(new_vol)
 
-    def drift(self, t, x: np.ndarray) -> np.ndarray:
+    def drift(self, t, x: List) -> List:
         return np.multiply(x, self.drift_vector)
 
-    def vol(self, t, x: np.ndarray) -> np.ndarray:
+    def vol(self, t, x: List) -> List:
         return np.multiply(x, self.vol_matrix.T).T
 
 
 class Vasicek_multi_d(Ito_diffusion_multi_d):
     """Instantiate Ito_diffusion to simulate a mean-reverting mutlivariate
     correlated Vasicek diffusion:
     dX_t = mean_reversion*(long_term-X_t)*dt + vol*dW_t
     where mean_reversion, long_term and vol are real numbers.
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.ones(1),
+        x0: List = np.ones(1),
         T: float = 1.0,
         scheme_steps: int = 100,
-        mean_reversion: np.ndarray = np.zeros(1),
-        long_term: np.ndarray = np.zeros(1),
-        vol: np.ndarray = np.eye(1),
+        mean_reversion: List = np.zeros(1),
+        long_term: List = np.zeros(1),
+        vol: List = np.eye(1),
         keys: None = None,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         verbose: bool = False,
         **kwargs,
     ) -> None:
 
         self._mean_reversion = np.array(mean_reversion)
         self._long_term = np.array(long_term)
         # vol is actually a covariance matrix here
@@ -256,62 +259,62 @@
             barrier=barrier,
             barrier_condition=barrier_condition,
             verbose=verbose,
             **kwargs,
         )
 
     @property
-    def mean_reversion(self) -> np.ndarray:
+    def mean_reversion(self) -> List:
         return self._mean_reversion
 
     @mean_reversion.setter
-    def mean_reversion(self, new_mean_reversion: np.ndarray) -> None:
+    def mean_reversion(self, new_mean_reversion: List) -> None:
         self._mean_reversion = new_mean_reversion
 
     @property
-    def long_term(self) -> np.ndarray:
+    def long_term(self) -> List:
         return self._long_term
 
     @long_term.setter
-    def long_term(self, new_long_term: np.ndarray) -> None:
+    def long_term(self, new_long_term: List) -> None:
         self._long_term = new_long_term
 
     @property
-    def vol_matrix(self) -> np.ndarray:
+    def vol_matrix(self) -> List:
         return self._vol_matrix
 
     @vol_matrix.setter
-    def vol_matrix(self, new_vol: np.ndarray) -> None:
+    def vol_matrix(self, new_vol: List) -> None:
         self._vol_matrix = np.array(new_vol)
 
-    def drift(self, t, x: np.ndarray) -> np.ndarray:
+    def drift(self, t, x: List) -> List:
         return np.multiply(self.long_term - x, self.mean_reversion)
 
-    def vol(self, t, x: np.ndarray) -> np.ndarray:
+    def vol(self, t, x: List) -> List:
         return self.vol_matrix
 
 
 class BlackKarasinski_multi_d(Vasicek_multi_d):
     """Instantiate Ito_diffusion to simulate a mean-reverting mutlivariate
     correlated Black-Karasinski diffusion:
     dlog(X_t) = mean_reversion*(long_term-log(X_t))*dt + vol*dW_t
     where mean_reversion, long_term and vol are real numbers.
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.ones(1),
+        x0: List = np.ones(1),
         T: float = 1.0,
         scheme_steps: int = 100,
-        mean_reversion: np.ndarray = np.zeros(1),
-        long_term: np.ndarray = np.ones(1),
-        vol: np.ndarray = np.eye(1),
+        mean_reversion: List = np.zeros(1),
+        long_term: List = np.ones(1),
+        vol: List = np.eye(1),
         keys: None = None,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         verbose: bool = False,
         **kwargs,
     ) -> None:
 
         super().__init__(
             x0=np.log(x0),
             T=T,
@@ -347,23 +350,23 @@
     ds_t = vov*s_t*dB_t
     d<W,B>_t = rho*dt
     where beta, vov, rho are real numbers
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.array([1.0, 1.0]),
+        x0: List = np.array([1.0, 1.0]),
         T: float = 1.0,
         scheme_steps: int = 100,
         keys: None = None,
         beta: float = 1.0,
         vov: float = 1.0,
         rho: float = 0.0,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         verbose: bool = False,
         **kwargs,
     ) -> None:
         self._beta = float(beta)
         self._vov = float(vov)
         self._rho = float(rho)
         n_factors = 2
@@ -403,18 +406,18 @@
     def vov(self, new_vov: float) -> None:
         self._vov = new_vov
 
     @property
     def rho_dual(self) -> float:
         return np.sqrt(1 - self.rho**2)
 
-    def drift(self, t, x) -> np.ndarray:
+    def drift(self, t, x) -> List:
         return np.zeros_like(x)
 
-    def vol(self, t, x: np.ndarray) -> np.ndarray:
+    def vol(self, t, x: List) -> List:
         """Project dB onto dW and an orhtogonal white noise dZ
         dB_t = rho*dW_t + sqrt(1-rho^2)*dZ_t
         """
         return np.array(
             [
                 [x[1] * (x[0]) ** self.beta, 0],
                 [self.vov * x[1] * self.rho, self.vov * x[1] * self.rho_dual],
@@ -429,25 +432,25 @@
     d<W,B>_t = rho*dt
     C(x) = exp(-c*log((y+shift)/K_max)^2)
     where shift, K_max, c, vov, rho are real numbers
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.array([1.0, 1.0]),
+        x0: List = np.array([1.0, 1.0]),
         T: float = 1.0,
         scheme_steps: int = 100,
         keys: None = None,
         shift: float = 0.0,
         K_max: float = 1.0,
         c: float = 1.0,
         vov: float = 1.0,
         rho: float = 0.0,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         verbose: bool = False,
         **kwargs,
     ) -> None:
         self._shift = float(shift)
         self._K_max = float(K_max)
         self._c = float(c)
         self._vov = float(vov)
@@ -505,18 +508,18 @@
     def vov(self, new_vov: float) -> None:
         self._vov = new_vov
 
     @property
     def rho_dual(self) -> float:
         return np.sqrt(1 - self.rho**2)
 
-    def drift(self, t, x: np.ndarray) -> np.ndarray:
+    def drift(self, t, x: List) -> List:
         return np.zeros_like(x)
 
-    def vol(self, t, x: np.ndarray) -> np.ndarray:
+    def vol(self, t, x: List) -> List:
         """Project dB onto dW and an orhtogonal white noise dZ
         dB_t = rho*dW_t + sqrt(1-rho^2)*dZ_t
         """
         return np.array(
             [
                 [
                     x[1]
@@ -537,25 +540,25 @@
     xs = x + shift
     mode = alpha*((beta-1)/(beta+1))^(1-beta)
     where shift, mode, beta, vov, rho are real numbers
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.array([1.0, 1.0]),
+        x0: List = np.array([1.0, 1.0]),
         T: float = 1.0,
         scheme_steps: int = 100,
         keys: None = None,
         shift: float = 0.0,
         mode: float = 1.0,
         beta: float = 1.0,
         vov: float = 1.0,
         rho: float = 0.0,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         verbose: bool = False,
         **kwargs,
     ) -> None:
         self._shift = float(shift)
         self._mode = float(mode)
         self._beta = float(beta)
         self._vov = float(vov)
@@ -613,22 +616,22 @@
     def vov(self, new_vov: float) -> None:
         self._vov = new_vov
 
     @property
     def rho_dual(self) -> float:
         return np.sqrt(1 - self.rho**2)
 
-    def drift(self, t, x: np.ndarray) -> np.ndarray:
+    def drift(self, t, x: List) -> List:
         return np.zeros_like(x)
 
     @property
     def alpha(self):
         return self.mode / (((self.beta - 1) / (self.beta + 1)) ** (1 - self.beta))
 
-    def vol(self, t, x: np.ndarray) -> np.ndarray:
+    def vol(self, t, x: List) -> List:
         """Project dB onto dW and an orhtogonal white noise dZ
         dB_t = rho*dW_t + sqrt(1-rho^2)*dZ_t
         """
         return np.array(
             [
                 [
                     x[1]
@@ -651,24 +654,24 @@
     d<W,B>_t = rho*dt
     C(x) = tanh((x+shift)/l)
     where shift, l, vov, rho are real numbers
     """
 
     def __init__(
         self,
-        x0: np.ndarray = np.array([1.0, 1.0]),
+        x0: List = np.array([1.0, 1.0]),
         T: float = 1.0,
         scheme_steps: int = 100,
         keys: None = None,
         shift: float = 0.0,
         l: float = 1.0,
         vov: float = 1.0,
         rho: float = 0.0,
-        barrier: np.ndarray = np.full(1, None),
-        barrier_condition: np.ndarray = np.full(1, None),
+        barrier: List = np.full(1, None),
+        barrier_condition: List = np.full(1, None),
         verbose: bool = False,
         **kwargs,
     ) -> None:
         self._shift = float(shift)
         self._l = float(l)
         self._vov = float(vov)
         self._rho = float(rho)
@@ -686,15 +689,15 @@
         )
 
     @property
     def shift(self) -> float:
         return self._shift
 
     @shift.setter
-    def shift(self, new_shift: np.ndarray) -> None:
+    def shift(self, new_shift: List) -> None:
         self._shift = float(new_shift)
 
     @property
     def l(self) -> float:  # noqa
         return self._l
 
     @l.setter
@@ -717,18 +720,18 @@
     def vov(self, new_vov: float) -> None:
         self._vov = new_vov
 
     @property
     def rho_dual(self) -> float:
         return np.sqrt(1 - self.rho**2)
 
-    def drift(self, t, x: np.ndarray) -> np.ndarray:
+    def drift(self, t, x: List) -> List:
         return np.zeros_like(x)
 
-    def vol(self, t, x: np.ndarray) -> np.ndarray:
+    def vol(self, t, x: List) -> List:
         """Project dB onto dW and an orhtogonal white noise dZ
         dB_t = rho*dW_t + sqrt(1-rho^2)*dZ_t
         """
         return np.array(
             [
                 [x[1] * np.tanh((x[0] + self.shift) / self.l), 0],
                 [self.vov * x[1] * self.rho, self.vov * x[1] * self.rho_dual],
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/ito_diffusion_sheaf.py` & `ito_diffusions-1.4.0/ito_diffusions/ito_diffusion_sheaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# Author: Patrick Saux <patrick.saux@inria.fr>
+
 from .ito_diffusion import Ito_diffusion
 from .ito_diffusion_1d import (
     BM,
     GBM,
     Vasicek,
     CIR,
     pseudo_GBM,
     Pinned_diffusion,
     Alpha_pinned_BM,
     F_pinned_BM,
 )
 
 import numpy as np
-from numpy import random as rd
 import pandas as pd
 
 # Diffusion sheaf
 # This is an attempt to create a sheaf of diffusion paths. Loosely speaking,
 # from a given realization of a diffusion, the aim is to create a sequence of
 # paths that share the same statistical properties as the original path while
 # being "continous deformations" of it. That can be achieved by using "similar"
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/noise.py` & `ito_diffusions-1.4.0/ito_diffusions/noise.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-#!/usr/bin/env python
-# coding: utf-8
+# Author: Patrick Saux <patrick.jr.saux@gmail.com>
 
 import numpy as np
-from numpy import random as rd
 from scipy.special import gamma, beta
 import mpmath as mp
 from functools import lru_cache
 
 #  Fractional Gaussian noise
 #
 # Covariance function of fractional Brownian motion :
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/pdmp.py` & `ito_diffusions-1.4.0/ito_diffusions/pdmp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Author: Patrick Saux <patrick.jr.saux@gmail.com>
+
 import numpy as np
 import abc
 from collections import defaultdict
 from typing import List
 
 
 class PDMP(abc.ABC):
@@ -131,15 +133,15 @@
         return self.jump_params["jump_mode_func"]
 
     @property
     def scheme_step(self) -> float:
         return (self.T - self.t0) / self.scheme_steps
 
     @property
-    def time_steps(self) -> np.ndarray:
+    def time_steps(self) -> List:
         return np.linspace(self.t0, self.T, self.scheme_steps + 1)
 
     def barrier_crossed(self, x, y, barrier) -> bool:
         """barrier is crossed if x and y are on each side of the barrier"""
         return (
             x < barrier - self._barrier_tol and y >= barrier - self._barrier_tol
         ) or (x > barrier + self._barrier_tol and y <= barrier + self._barrier_tol)
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/pdmp_1d.py` & `ito_diffusions-1.4.0/ito_diffusions/pdmp_1d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Author: Patrick Saux <patrick.jr.saux@gmail.com>
+
 import numpy as np
 import pandas as pd
 from collections import defaultdict
 from typing import List
 from tqdm import tqdm
 from .pdmp import PDMP
 
@@ -49,15 +51,17 @@
                 previous_step = last_step
                 last_step += self.drift(t, last_step, last_mode) * self.scheme_step
                 intensity = self.natural_jump_intensity_func(
                     t, previous_step, last_mode
                 )
                 if self.rng.poisson(intensity * self.scheme_step) > 0:
                     last_mode = int(
-                        self.natural_jump_mode_func(t, previous_step, last_mode).rvs(random_state=self.rng)
+                        self.natural_jump_mode_func(t, previous_step, last_mode).rvs(
+                            random_state=self.rng
+                        )
                     )
                     natural_jump[i + 1] = True
 
                 for barrier_idx, barrier in enumerate(self.barriers):
                     if self.barrier_crossed(previous_step, last_step, barrier):
                         last_mode = int(
                             self.barrier_jump_mode_func[barrier_idx](
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/saw.py` & `ito_diffusions-1.4.0/ito_diffusions/saw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Author: Patrick Saux <patrick.jr.saux@gmail.com>
+
 import numpy as np
 import pandas as pd
 from scipy.spatial.distance import cdist
 from functools import lru_cache
 from tqdm import tqdm
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions/sle.py` & `ito_diffusions-1.4.0/ito_diffusions/sle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Author: Patrick Saux <patrick.jr.saux@gmail.com>
+
 import numpy as np
 import pandas as pd
 from functools import lru_cache
 from tqdm import tqdm
 
 
 class FastChordalSLEHalfPlane:
```

### Comparing `ito_diffusions-1.3.0/ito_diffusions.egg-info/PKG-INFO` & `ito_diffusions-1.4.0/ito_diffusions.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: ito-diffusions
-Version: 1.3.0
+Version: 1.4.0
 Summary: Library for stochastic process simulation
 Home-page: https://github.com/sauxpa/ito_diffusions
 Author: Patrick Saux
 Author-email: patrick.jr.saux@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### ito_diffusions
 Libraries for stochastic processes simulation and visualization including:
 * Ito diffusion : Brownian motion, Geometric Brownian motion, Vasicek, CIR...
-* Jump processes : Ito diffusion driven by a Levy process i.e with a jump component with a given intensity and jump size distribution
-* Multidimensional processes, stochastic volatility diffusions (SABR...)
-* Fractional Brownian motion, Karhunen-Loeve expansion, fractional diffusions
-* Self-Avoiding Walks (SAW), Schramm-Loewner Evolution (SLE)
+* Jump processes : Ito diffusion driven by a Levy process i.e with a jump component with a given intensity and jump size distribution;
+* Multidimensional processes, stochastic volatility diffusions (SABR...);
+* Fractional Brownian motion, Karhunen-Loeve expansion, fractional diffusions;
+* Times series models (AR, MA, ARMA, ARCH, GARCH, NAGARCH...);
+* Self-Avoiding Walks (SAW), Schramm-Loewner Evolution (SLE).
 
 **To install** : pip install ito-diffusions
 https://pypi.org/project/ito-diffusions/
 
 
 **To test** : python -m pytest
 
 For numerous examples : https://github.com/sauxpa/stochastic
 
 <img src="./brownian_sheaf.png"
      style="float: left; margin-right: 10px;" />
 
+<img src="./nagarch.png"
+     style="float: left; margin-right: 10px;" />
 
 <img src="./saw_square.png"
      style="float: left; margin-right: 10px;" />
 
 <img src="./sle_peaks.png"
      style="float: left; margin-right: 10px;" />
```

### Comparing `ito_diffusions-1.3.0/setup.py` & `ito_diffusions-1.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ito_diffusions',
     packages=['ito_diffusions'],
-    version='1.3.0',
+    version='1.4.0',
     author="Patrick Saux",
     author_email="patrick.jr.saux@gmail.com",
     description="Library for stochastic process simulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sauxpa/ito_diffusions",
     install_requires=['numpy', 'scipy', 'pandas', 'mpmath', 'tqdm'],
```

