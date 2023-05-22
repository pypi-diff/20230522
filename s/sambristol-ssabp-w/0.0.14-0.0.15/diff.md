# Comparing `tmp/sambristol_ssabp_w-0.0.14.tar.gz` & `tmp/sambristol_ssabp_w-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mv19141/Documents/python_packages/sambristol_ssabp_w/dist/tmp70lghjnn/sambristol_ssabp_w-0.0.14.tar", last modified: Sat Oct  8 13:12:15 2022, max compression
+gzip compressed data, was "sambristol_ssabp_w-0.0.15.tar", last modified: Mon May 22 10:31:53 2023, max compression
```

## Comparing `sambristol_ssabp_w-0.0.14.tar` & `sambristol_ssabp_w-0.0.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)    35149 2020-12-15 12:54:24.000000 sambristol_ssabp_w-0.0.14/LICENSE
--rw-rw-r--   0 mv19141   (1001) mv19141   (1001)      707 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/PKG-INFO
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      163 2021-02-03 11:27:56.000000 sambristol_ssabp_w-0.0.14/README.rst
-drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      479 2022-10-08 13:11:27.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/__init__.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     8668 2021-08-23 15:00:49.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/correlationintegrands.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     3223 2021-02-03 12:13:03.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/effectivepotential.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)    16303 2021-02-04 10:08:35.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/mayerint.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     3386 2021-03-14 20:00:37.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/meshode.py
--rwxr-xr-x   0 mv19141   (1001) mv19141   (1001)     9185 2022-10-08 11:53:55.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/trimerbc.py
--rwxr-xr-x   0 mv19141   (1001) mv19141   (1001)    10050 2021-03-14 19:52:44.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wbessel.py
--rw-rw-r--   0 mv19141   (1001) mv19141   (1001)     7052 2022-09-28 08:15:56.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wdiffpot.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     5504 2021-08-24 12:54:57.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/whardsphere.py
--rw-rw-r--   0 mv19141   (1001) mv19141   (1001)     4535 2022-10-08 11:55:31.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wlowDt.py
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)     7034 2022-09-27 14:00:00.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wperturb.py
--rw-rw-r--   0 mv19141   (1001) mv19141   (1001)    12503 2021-08-25 07:58:50.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wxi.py
-drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      707 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/PKG-INFO
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      625 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/SOURCES.txt
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)        1 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/dependency_links.txt
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)       36 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/requires.txt
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)       19 2022-10-08 13:12:15.000000 sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/top_level.txt
--rw-rw-r--   0 mv19141   (1001) mv19141   (1001)       38 2022-10-08 13:12:15.642828 sambristol_ssabp_w-0.0.14/setup.cfg
--rw-r--r--   0 mv19141   (1001) mv19141   (1001)      844 2022-10-08 13:11:37.000000 sambristol_ssabp_w-0.0.14/setup.py
+drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2023-05-22 10:31:53.856972 sambristol_ssabp_w-0.0.15/
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)    35149 2020-12-15 12:54:24.000000 sambristol_ssabp_w-0.0.15/LICENSE
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)      707 2023-05-22 10:31:53.856972 sambristol_ssabp_w-0.0.15/PKG-INFO
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      163 2021-02-03 11:27:56.000000 sambristol_ssabp_w-0.0.15/README.rst
+drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2023-05-22 10:31:53.856972 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      479 2022-10-08 13:16:58.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/__init__.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     8668 2021-08-23 15:00:49.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/correlationintegrands.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     3223 2021-02-03 12:13:03.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/effectivepotential.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)    16303 2021-02-04 10:08:35.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/mayerint.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     3386 2021-03-14 20:00:37.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/meshode.py
+-rwxr-xr-x   0 mv19141   (1001) mv19141   (1001)     9185 2022-10-08 11:53:55.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/trimerbc.py
+-rwxr-xr-x   0 mv19141   (1001) mv19141   (1001)    10050 2021-03-14 19:52:44.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wbessel.py
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)     7052 2022-09-28 08:15:56.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wdiffpot.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     5504 2021-08-24 12:54:57.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/whardsphere.py
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)     4540 2022-10-08 13:18:14.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wlowDt.py
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)     7034 2022-09-27 14:00:00.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wperturb.py
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)    12503 2021-08-25 07:58:50.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wxi.py
+drwxrwxr-x   0 mv19141   (1001) mv19141   (1001)        0 2023-05-22 10:31:53.856972 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w.egg-info/
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      707 2023-05-22 10:31:53.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w.egg-info/PKG-INFO
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      625 2023-05-22 10:31:53.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w.egg-info/SOURCES.txt
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)        1 2023-05-22 10:31:53.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w.egg-info/dependency_links.txt
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)       36 2023-05-22 10:31:53.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w.egg-info/requires.txt
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)       19 2023-05-22 10:31:53.000000 sambristol_ssabp_w-0.0.15/sambristol_ssabp_w.egg-info/top_level.txt
+-rw-rw-r--   0 mv19141   (1001) mv19141   (1001)       38 2023-05-22 10:31:53.856972 sambristol_ssabp_w-0.0.15/setup.cfg
+-rw-r--r--   0 mv19141   (1001) mv19141   (1001)      844 2023-05-22 10:31:26.000000 sambristol_ssabp_w-0.0.15/setup.py
```

### Comparing `sambristol_ssabp_w-0.0.14/LICENSE` & `sambristol_ssabp_w-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/PKG-INFO` & `sambristol_ssabp_w-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sambristol_ssabp_w
-Version: 0.0.14
+Version: 0.0.15
 Summary: package to compute ODE's and statmech relevant to active brownian particle steady states
 Home-page: https://github.com/samueljmcameron/sambristol_ssabp_w
 Author: Sam Cameron
 Author-email: samuel.j.m.cameron@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/correlationintegrands.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/correlationintegrands.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/effectivepotential.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/effectivepotential.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/mayerint.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/mayerint.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/meshode.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/meshode.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/trimerbc.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/trimerbc.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wbessel.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wbessel.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wdiffpot.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wdiffpot.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/whardsphere.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/whardsphere.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wlowDt.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wlowDt.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import scipy.special as special
 
 
 from .effectivepotential import twobody_value, twobody_derivative
 from .effectivepotential import threebody_value, threebody_derivative_u
 
 
-class wHardSphere():
+class wLowDt():
 
     
     """
     Evaluate the w(r) function when D_t goes to 0 (is much smaller than D_r*sigma**2)
 
 
     Attributes
@@ -48,19 +48,19 @@
         """
         Initialise attributes.
 
         Parameters
         ----------
         potentialclass : potential
             class with potential that has attribute self.V_derivative(r) and
-            self.V_doublederiv(r)
+            self.V_doublederivative(r)
         """
 
         self.Vderiv = potentialclass.V_derivative
-        self.Vdoublederiv = potentialclass.V_doublederiv
+        self.Vdoublederiv = potentialclass.V_doublederivative
         self.cutoff = cutoff
         return
 
 
 
     def w(self,r):
         """
```

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wperturb.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wperturb.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w/wxi.py` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w/wxi.py`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/PKG-INFO` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sambristol-ssabp-w
-Version: 0.0.14
+Version: 0.0.15
 Summary: package to compute ODE's and statmech relevant to active brownian particle steady states
 Home-page: https://github.com/samueljmcameron/sambristol_ssabp_w
 Author: Sam Cameron
 Author-email: samuel.j.m.cameron@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `sambristol_ssabp_w-0.0.14/sambristol_ssabp_w.egg-info/SOURCES.txt` & `sambristol_ssabp_w-0.0.15/sambristol_ssabp_w.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sambristol_ssabp_w-0.0.14/setup.py` & `sambristol_ssabp_w-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sambristol_ssabp_w",
-    version="0.0.14",
+    version="0.0.15",
     author="Sam Cameron",
     author_email="samuel.j.m.cameron@gmail.com",
     description="package to compute ODE's and statmech "
     "relevant to active brownian particle steady states",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/samueljmcameron/sambristol_ssabp_w",
```

