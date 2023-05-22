# Comparing `tmp/sambristol_ssabp_w-0.0.12.tar.gz` & `tmp/sambristol_ssabp_w-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mv19141/Documents/python_packages/sambristol_ssabp_w/dist/tmpb54ewbdw/sambristol_ssabp_w-0.0.12.tar", last modified: Wed Aug 25 10:15:41 2021, max compression
+gzip compressed data, was "/home/mv19141/Documents/python_packages/sambristol_ssabp_w/dist/tmp70lghjnn/sambristol_ssabp_w-0.0.14.tar", last modified: Sat Oct  8 13:12:15 2022, max compression
```

## Comparing `sambristol_ssabp_w-0.0.12.tar` & `sambristol_ssabp_w-0.0.14.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2021-08-25 10:15:41.835945 sambristol_ssabp_w-0.0.12/
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)    35149 2020-12-15 12:54:24.000000 sambristol_ssabp_w-0.0.12/LICENSE
--rw-rw-r--   0 mv19141   (1001) mv19141   (1001)      744 2021-08-25 10:15:41.835945 sambristol_ssabp_w-0.0.12/PKG-INFO
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      163 2021-02-03 11:27:56.000000 sambristol_ssabp_w-0.0.12/README.rst
-drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2021-08-25 10:15:41.835945 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      391 2021-08-24 13:54:10.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/__init__.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     8668 2021-08-23 15:00:49.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/correlationintegrands.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     3223 2021-02-03 12:13:03.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/effectivepotential.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)    16303 2021-02-04 10:08:35.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/mayerint.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     3386 2021-03-14 20:00:37.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/meshode.py
--rwxr-xr-x   0 mv19141   (1001) mv19141   (1001)     6336 2021-02-11 11:07:41.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/trimerbc.py
--rwxr-xr-x   0 mv19141   (1001) mv19141   (1001)    10050 2021-03-14 19:52:44.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/wbessel.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     5504 2021-08-24 12:54:57.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/whardsphere.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     7072 2021-08-23 09:39:48.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/wperturb.py
--rw-rw-r--   0 mv19141   (1001) mv19141   (1001)    12503 2021-08-25 07:58:50.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/wxi.py
-drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2021-08-25 10:15:41.835945 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w.egg-info/
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      744 2021-08-25 10:15:41.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w.egg-info/PKG-INFO
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      565 2021-08-25 10:15:41.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w.egg-info/SOURCES.txt
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)        1 2021-08-25 10:15:41.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w.egg-info/dependency_links.txt
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)       36 2021-08-25 10:15:41.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w.egg-info/requires.txt
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)       19 2021-08-25 10:15:41.000000 sambristol_ssabp_w-0.0.12/sambristol_ssabp_w.egg-info/top_level.txt
--rw-rw-r--   0 mv19141   (1001) mv19141   (1001)       38 2021-08-25 10:15:41.835945 sambristol_ssabp_w-0.0.12/setup.cfg
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      844 2021-08-25 10:14:21.000000 sambristol_ssabp_w-0.0.12/setup.py
+drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)    35149 2020-12-15 12:54:24.000000 sambristol_ssabp_w-0.0.14/LICENSE
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)      707 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/PKG-INFO
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      163 2021-02-03 11:27:56.000000 sambristol_ssabp_w-0.0.14/README.rst
+drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      479 2022-10-08 13:11:27.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/__init__.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     8668 2021-08-23 15:00:49.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/correlationintegrands.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     3223 2021-02-03 12:13:03.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/effectivepotential.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)    16303 2021-02-04 10:08:35.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/mayerint.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     3386 2021-03-14 20:00:37.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/meshode.py
+-rwxr-xr-x   0 mv19141   (1001) mv19141   (1001)     9185 2022-10-08 11:53:55.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/trimerbc.py
+-rwxr-xr-x   0 mv19141   (1001) mv19141   (1001)    10050 2021-03-14 19:52:44.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wbessel.py
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)     7052 2022-09-28 08:15:56.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wdiffpot.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     5504 2021-08-24 12:54:57.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/whardsphere.py
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)     4535 2022-10-08 11:55:31.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wlowDt.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     7034 2022-09-27 14:00:00.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wperturb.py
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)    12503 2021-08-25 07:58:50.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wxi.py
+drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      707 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/PKG-INFO
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      625 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/SOURCES.txt
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)        1 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/dependency_links.txt
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)       36 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/requires.txt
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)       19 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/top_level.txt
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)       38 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/setup.cfg
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      844 2022-10-08 13:11:37.000000 sambristol_ssabp_w-0.0.14/setup.py
```

### Comparing `sambristol_ssabp_w-0.0.12/LICENSE` & `sambristol_ssabp_w-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/correlationintegrands.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/correlationintegrands.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/effectivepotential.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/effectivepotential.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/mayerint.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/mayerint.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/meshode.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/meshode.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/trimerbc.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/trimerbc.py`

 * *Files 23% similar despite different names*

```diff
@@ -79,14 +79,146 @@
         Derivative value of shiftedLJ potential
         """
 
         
         return -24*self.epsilon*(2*r**(-13)-r**(-7))
 
 
+    def V_doublederivative(self,r):
+
+        """
+        Compute second derivative value of shiftedLJ potential at r.
+
+        Parameters
+        ----------
+        r : float or np.array
+            distance between particles.
+
+        Returns
+        -------
+        Derivative value of shiftedLJ potential
+        """
+        
+
+        return 24*self.epsilon*(26/r**16-7/r**8)
+
+
+class expPot():
+
+    """
+    Simple class which allows for different potential. Note that length
+    is measured in units of 'a'. The explicit form of the
+    potential is
+
+    V(r) = epsilon*exp(-1/(1-(r/a)**2))
+
+
+    Attributes
+    ----------
+    epsilon : float (optional)
+        value of the potential strength. Default is 1.
+
+    Methods
+    -------
+
+    __init__(self,epsilon=1)
+        Initialise attributes.
+
+    V_value(self,r)
+        Compute value of potential at r (could be array or scalar).
+
+    V_derivative(self,r)
+        Compute derivative of potential at r (could be array or
+        scalar).
+
+    """
+
+    def __init__(self,epsilon=500):
+
+        """
+        Initialise potential strength epsilon.
+
+        Parameters
+        ----------
+        epsilon : float (optional)
+            value of the potential strength. Default is 1.
+        """
+        
+        
+        self.epsilon = epsilon
+
+        return
+
+    def V_value(self,r):
+        """
+        Compute value of expPot potential at r.
+
+        Parameters
+        ----------
+        r : float or np.array
+            distance between particles.
+
+        Returns
+        -------
+        Value of expPot potential
+        """
+        r = np.asarray(r)
+        mask = (r < 1.0)
+        x = np.empty_like(r)
+        x[mask] = self.epsilon*np.exp(-1/(1-r[mask]**2))
+        x[~mask] = 0.0
+        
+        return x
+    
+    def V_derivative(self,r):
+        """
+        Compute derivative value of expPot potential at r.
+
+        Parameters
+        ----------
+        r : float or np.array
+            distance between particles.
+
+        Returns
+        -------
+        Derivative value of expPot potential
+        """
+        r = np.asarray(r)
+        mask = (r < 1.0)
+        x = np.empty_like(r)
+        x[mask] = -2*self.epsilon*r[mask]*np.exp(-1/(1-r[mask]**2))/(1-r[mask]**2)**2
+        x[~mask] = 0.0
+        
+        return x
+
+
+    def V_doublederivative(self,r):
+        """
+        Compute second derivative value of expPot potential at r.
+
+        Parameters
+        ----------
+        r : float or np.array
+            distance between particles.
+
+        Returns
+        -------
+        Derivative value of expPot potential
+        """
+        
+        r = np.asarray(r)
+        mask = (r < 1.0)
+        x = np.empty_like(r)
+        x[mask] = -2*self.epsilon*(1-3*r[mask]**2)*np.exp(-1/(1-r[mask]**2))/(1-r[mask]**2)**4
+        x[~mask] = 0.0
+        
+        return x
+
+    
+    
 import numpy as np
 import scipy.optimize as optimize
 
 class TrimerBC(shiftedLJ):
 
     """
     Class to compute the zero-force distance r0 for a trimer of active
```

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/wbessel.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wbessel.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/whardsphere.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/whardsphere.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/wperturb.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wperturb.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         self.__c0 = -1./(self.denom*np.sqrt(self.Pi/2.))/special.kvp(1,np.sqrt(self.Pi/2.)*self.r0,1)
 
 
         self.__w_lower = self.__below_r0()
 
         return
 
-    def __fun(self,r,y,p):
+    def __fun(self,r,y):
 
         """
         RHS of y' = f(r,y) for ODE to be solved, with y[0] = w, y[1] = w'.
 
         Parameters
         ----------
 
@@ -152,17 +152,16 @@
 
 
     def __below_r0(self,rf = 0.7):
 
         y0 = self.__y0()
         t_span = (self.r0,rf)
         # since self.__fun takes a dummy argument, I'll set it to 1
-        dum_arg = 1
 
-        res = solve_ivp(self.__fun,t_span,y0,args=(dum_arg,),
+        res = solve_ivp(self.__fun,t_span,y0,
                         vectorized=True,dense_output=True)
 
         return res.sol
     
     def __w_minus_both(self,r):
```

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w/wxi.py` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wxi.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w.egg-info/PKG-INFO` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: sambristol-ssabp-w
-Version: 0.0.12
+Version: 0.0.14
 Summary: package to compute ODE's and statmech relevant to active brownian particle steady states
 Home-page: https://github.com/samueljmcameron/sambristol_ssabp_w
 Author: Sam Cameron
 Author-email: samuel.j.m.cameron@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # sambristolwfunctions
 
 Computes different ODEs which are related to the probability distribution
 of active brownian particles interacting with a WCA potential. 
 
-
-
```

### Comparing `sambristol_ssabp_w-0.0.12/sambristol_ssabp_w.egg-info/SOURCES.txt` & `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 sambristol_ssabp_w/__init__.py
 sambristol_ssabp_w/correlationintegrands.py
 sambristol_ssabp_w/effectivepotential.py
 sambristol_ssabp_w/mayerint.py
 sambristol_ssabp_w/meshode.py
 sambristol_ssabp_w/trimerbc.py
 sambristol_ssabp_w/wbessel.py
+sambristol_ssabp_w/wdiffpot.py
 sambristol_ssabp_w/whardsphere.py
+sambristol_ssabp_w/wlowDt.py
 sambristol_ssabp_w/wperturb.py
 sambristol_ssabp_w/wxi.py
 sambristol_ssabp_w.egg-info/PKG-INFO
 sambristol_ssabp_w.egg-info/SOURCES.txt
 sambristol_ssabp_w.egg-info/dependency_links.txt
 sambristol_ssabp_w.egg-info/requires.txt
 sambristol_ssabp_w.egg-info/top_level.txt
```

### Comparing `sambristol_ssabp_w-0.0.12/setup.py` & `sambristol_ssabp_w-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sambristol_ssabp_w",
-    version="0.0.12",
+    version="0.0.14",
     author="Sam Cameron",
     author_email="samuel.j.m.cameron@gmail.com",
     description="package to compute ODE's and statmech "
     "relevant to active brownian particle steady states",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/samueljmcameron/sambristol_ssabp_w",
```

