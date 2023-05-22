# Comparing `tmp/dynbps-0.0.6.tar.gz` & `tmp/dynbps-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynbps-0.0.6.tar", last modified: Wed May 17 22:43:25 2023, max compression
+gzip compressed data, was "dist/dynbps-0.0.7.tar", last modified: Mon May 22 19:23:59 2023, max compression
```

## Comparing `dynbps-0.0.6.tar` & `dynbps-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 22:43:25.543419 dynbps-0.0.6/
--rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.6/LICENSE
--rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.6/MANIFEST.in
--rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-17 22:43:25.542475 dynbps-0.0.6/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      284 2023-05-17 22:26:24.000000 dynbps-0.0.6/README.md
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 22:43:25.533932 dynbps-0.0.6/dynbps/
--rw-r--r--   0 josephrilling   (501) staff       (20)     9023 2023-05-17 22:43:19.000000 dynbps-0.0.6/dynbps/BPS.py
--rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-17 22:43:19.000000 dynbps-0.0.6/dynbps/__init__.py
--rw-r--r--   0 josephrilling   (501) staff       (20)      763 2023-05-17 22:43:19.000000 dynbps-0.0.6/dynbps/_modidx.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 22:43:25.540431 dynbps-0.0.6/dynbps/datasets/
--rw-r--r--   0 josephrilling   (501) staff       (20)    41999 2023-05-17 22:21:27.000000 dynbps-0.0.6/dynbps/datasets/data.xlsx
--rw-r--r--   0 josephrilling   (501) staff       (20)      747 2023-05-17 22:43:19.000000 dynbps-0.0.6/dynbps/loadData.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 22:43:25.539606 dynbps-0.0.6/dynbps.egg-info/
--rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-17 22:43:25.000000 dynbps-0.0.6/dynbps.egg-info/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      358 2023-05-17 22:43:25.000000 dynbps-0.0.6/dynbps.egg-info/SOURCES.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-17 22:43:25.000000 dynbps-0.0.6/dynbps.egg-info/dependency_links.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-17 22:43:25.000000 dynbps-0.0.6/dynbps.egg-info/entry_points.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.6/dynbps.egg-info/not-zip-safe
--rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-17 22:43:25.000000 dynbps-0.0.6/dynbps.egg-info/requires.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-17 22:43:25.000000 dynbps-0.0.6/dynbps.egg-info/top_level.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-17 22:43:19.000000 dynbps-0.0.6/settings.ini
--rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-17 22:43:25.544001 dynbps-0.0.6/setup.cfg
--rw-rw-r--   0 josephrilling   (501) staff       (20)     2640 2023-05-17 22:24:08.000000 dynbps-0.0.6/setup.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 19:23:59.562447 dynbps-0.0.7/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.7/LICENSE
+-rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.7/MANIFEST.in
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-22 19:23:59.561791 dynbps-0.0.7/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      284 2023-05-22 19:10:12.000000 dynbps-0.0.7/README.md
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 19:23:59.551951 dynbps-0.0.7/dynbps/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     8905 2023-05-22 19:23:47.000000 dynbps-0.0.7/dynbps/BPS.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-22 19:23:47.000000 dynbps-0.0.7/dynbps/__init__.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)      763 2023-05-22 19:23:47.000000 dynbps-0.0.7/dynbps/_modidx.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 19:23:59.559712 dynbps-0.0.7/dynbps/datasets/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    41999 2023-05-17 22:21:27.000000 dynbps-0.0.7/dynbps/datasets/data.xlsx
+-rw-r--r--   0 josephrilling   (501) staff       (20)      747 2023-05-22 19:23:47.000000 dynbps-0.0.7/dynbps/loadData.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 19:23:59.558803 dynbps-0.0.7/dynbps.egg-info/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      358 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/SOURCES.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/dependency_links.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/entry_points.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.7/dynbps.egg-info/not-zip-safe
+-rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/requires.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/top_level.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-22 19:23:47.000000 dynbps-0.0.7/settings.ini
+-rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-22 19:23:59.562617 dynbps-0.0.7/setup.cfg
+-rw-rw-r--   0 josephrilling   (501) staff       (20)     2640 2023-05-17 22:24:08.000000 dynbps-0.0.7/setup.py
```

### Comparing `dynbps-0.0.6/LICENSE` & `dynbps-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.6/PKG-INFO` & `dynbps-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.6/dynbps/BPS.py` & `dynbps-0.0.7/dynbps/BPS.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         def std_var(x):
             return (x + np.transpose(x))/2
 
         def chol(A):
             '''returns upper triangle of matrix'''
             return cholesky(A, lower = False)
 
-        y =self.y[0:-1]
-        a_j =self.a_j[0:-1,]
-        A_j =self.A_j[0:-1,]
+        y =self.y
+        a_j =self.a_j
+        A_j =self.A_j
         n_j =self.n_j 
         delta =self.delta 
         m_0 = self.m_0
         C_0 =self.C_0
         n_0 =self.n_0 
         s_0 =self.s_0 
         burn_in = self.burn_in
@@ -148,38 +148,36 @@
 
         self.theta_post_samples = theta_t[:, (burn_in*p_x):]
         self.X_post_samples = X_t[:, (burn_in * p_x):]
         self.a_k_samples = a_k[burn_in:, :]
         self.R_k_samples = R_k[(p * burn_in):, :]
         self.v_k_samples = v_k[burn_in:, :]
         self.a_k = self.a_k_samples.mean(axis=0)
-    def predict(self):
+    def predict(self,a_new, A_new, n_new):
         def std_var(x):
             return (x + np.transpose(x))/2
 
         def chol(A):
             '''returns upper triangle of matrix'''
             return cholesky(A, lower = False)
-        a = self.a_j[-1,:]
-        A = self.A_j[-1,:]
-        n = self.n_j[-1,0]
+        a = a_new
+        A = A_new
+        n = n_new
         delta = self.delta
         mcmc_iter = self.mcmc_iter
         p = self.p
         E_BPS = np.zeros(shape = [mcmc_iter, 1]) # posterior BPS mean
         V_BPS = np.zeros(shape = [mcmc_iter, 1]) # posterior BPS variance
         error = np.zeros(shape = [mcmc_iter, 1])
         mlike = np.zeros(shape = [mcmc_iter, 1])
         for i in range(self.mcmc_iter):
         # sample x(t + 1)
             lambda_ = np.sqrt(0.5 * delta[1] * n/np.random.gamma(shape = delta[1] * n/2)) 
             x_t = np.append(np.array([1]), a + lambda_ * np.matmul(np.random.normal(size = [1, self.p_x]), chol(std_var(np.diag(A)))))
             E_BPS[i] = np.matmul(x_t, self.a_k_samples[i, :])
             V_BPS[i] = np.matmul(x_t, np.matmul(self.R_k_samples[(p*i):(p*(i + 1)), :], x_t.reshape([x_t.shape[0], 1]))) + self.v_k_samples[i, :]
-            error[i] = self.y[-1] - E_BPS[i]
             #mlike[i, t] = np.exp(np.log(ss.gamma(0.5 * (nu[t] + 1))) - np.log(ss.gamma(0.5 * nu[t])) - 0.5 * np.log(np.pi * nu[t] * V_BPS[i, t]) - (0.5 * (nu[t] + 1)) * np.log(1 + 1/(nu[t] * V_BPS[i, t]) * (yI[t + 1] - E_BPS[i, t]))**2)
         self.prediction = E_BPS.mean()
         self.variance = V_BPS.mean()
-        self.error = error.mean()
-        result = [self.prediction, self.variance, self.error]
+        result = [self.prediction, self.variance]
         return(result)
```

### Comparing `dynbps-0.0.6/dynbps/_modidx.py` & `dynbps-0.0.7/dynbps/_modidx.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.6/dynbps/datasets/data.xlsx` & `dynbps-0.0.7/dynbps/datasets/data.xlsx`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.6/dynbps/loadData.py` & `dynbps-0.0.7/dynbps/loadData.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.6/dynbps.egg-info/PKG-INFO` & `dynbps-0.0.7/dynbps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.6/settings.ini` & `dynbps-0.0.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dynbps
 lib_name = dynbps
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dynbps
 nbs_path = nbs
 recursive = True
```

### Comparing `dynbps-0.0.6/setup.py` & `dynbps-0.0.7/setup.py`

 * *Files identical despite different names*

