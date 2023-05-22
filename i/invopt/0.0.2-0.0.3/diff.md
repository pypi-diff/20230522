# Comparing `tmp/invopt-0.0.2.tar.gz` & `tmp/invopt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invopt-0.0.2.tar", last modified: Fri May 12 10:50:40 2023, max compression
+gzip compressed data, was "invopt-0.0.3.tar", last modified: Mon May 22 13:13:58 2023, max compression
```

## Comparing `invopt-0.0.2.tar` & `invopt-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.340857 invopt-0.0.2/
--rw-rw-rw-   0        0        0     1099 2023-05-01 20:52:18.000000 invopt-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2991 2023-05-12 10:50:40.340857 invopt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2401 2023-05-11 19:19:40.000000 invopt-0.0.2/README.md
--rw-rw-rw-   0        0        0      712 2023-05-12 10:50:14.000000 invopt-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 10:50:40.340857 invopt-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.300486 invopt-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.312416 invopt-0.0.2/src/invopt/
--rw-rw-rw-   0        0        0      371 2023-05-02 08:10:57.000000 invopt-0.0.2/src/invopt/__init__.py
--rw-rw-rw-   0        0        0    53363 2023-05-12 10:48:05.000000 invopt-0.0.2/src/invopt/main.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.336879 invopt-0.0.2/src/invopt.egg-info/
--rw-rw-rw-   0        0        0     2991 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.338871 invopt-0.0.2/tests/
--rw-rw-rw-   0        0        0     1682 2023-05-12 10:16:00.000000 invopt-0.0.2/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.093986 invopt-0.0.3/
+-rw-rw-rw-   0        0        0     1099 2023-05-01 20:52:18.000000 invopt-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3928 2023-05-22 13:13:58.093986 invopt-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3338 2023-05-16 12:23:45.000000 invopt-0.0.3/README.md
+-rw-rw-rw-   0        0        0      712 2023-05-22 13:10:07.000000 invopt-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 13:13:58.093986 invopt-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.031453 invopt-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.062713 invopt-0.0.3/src/invopt/
+-rw-rw-rw-   0        0        0      371 2023-05-02 08:10:57.000000 invopt-0.0.3/src/invopt/__init__.py
+-rw-rw-rw-   0        0        0    54267 2023-05-18 11:10:46.000000 invopt-0.0.3/src/invopt/main.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.093986 invopt-0.0.3/src/invopt.egg-info/
+-rw-rw-rw-   0        0        0     3928 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.093986 invopt-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1682 2023-05-12 10:16:00.000000 invopt-0.0.3/tests/test_examples.py
```

### Comparing `invopt-0.0.2/LICENSE.txt` & `invopt-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `invopt-0.0.2/PKG-INFO` & `invopt-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: invopt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Inverse Optimization with Python
 Author-email: Pedro Zattoni Scroccaro <pedroszattoni@gmail.com>
 Project-URL: Homepage, https://github.com/pedroszattoni/invopt
 Project-URL: Bug Tracker, https://github.com/pedroszattoni/inverse-optimization/issues
 Keywords: inverse-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# InvOpt: Inverse Optimization in Python
 
-InvOpt is a Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in the exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, our goal is to model the cost function being optimized by the expert, using examples of exogenous signals and corresponding expert response actions. More concretely, given a dataset $\mathcal{D} = \{(\hat{s}_i, \hat{x}_i)\}_{i=1}^N$ of exogenous signals $\hat{s}_i$ and the respective expert's response $\hat{x}_i$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that the **Forward Optimization Problem (FOP)** with feature mapping $\phi$
-$$
-x_i \in \arg\min_{x \in \mathbb{X}(\hat{s}_i)} \ \theta^\top \phi(\hat{s}_i,x) 
-$$reproduces (or in some sense approximates) the expert's action $\hat{x}_i$. For a more detailed description of the IO problem and its modelling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/0000.00000) and the references therein. 
+# InvOpt: Inverse Optimization with Python
+
+InvOpt is a Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in the exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, our goal is to model the cost function being optimized by the expert, using examples of exogenous signals and corresponding expert response actions. More concretely, given a dataset $\mathcal{D} = \\{(\hat{s}_ i, \hat{x}_ i)\\}_ {i=1}^N$ of exogenous signals $\hat{s}_ i$ and the respective expert's response $\hat{x}_ i$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that the **Forward Optimization Problem (FOP)** with feature mapping $\phi$
+$$x_i \in \arg\min_ {x \in \mathbb{X}(\hat{s}_ i)} \ \theta^\top \phi(\hat{s}_ i,x)$$ reproduces (or in some sense approximates) the expert's action $\hat{x}_ i$. For a more detailed description of the IO problem and its modelling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/2305.07730) and the references therein. 
 
 ## Installation
 
 ```bash
 pip install invopt
 ```
 InvOpt depends on NumPy. Moreover, some of its functions also depend on gurobipy or cvxpy. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
 
-## Usage & examples
+## Usage and examples
+
+The following functions are available in the InvOpt package to solving IO problems:
 
-The folder [examples](https://github.com/pedroszattoni/invopt/tree/main/examples) contains descriptions of the functions available in the InvOpt package, as well as multiple examples.
+- [`discrete_model_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
+- [`discrete_model`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model): for FOPs with dicrete decision spaces (e.g., binary).
+- [`MIP_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
+- [`MIP_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
+- [`FOM`](https://github.com/pedroszattoni/invopt/tree/main/examples/FOM): for general FOPs. Solves IO problem approximately using first-order methods.
 
 ## Contributing
 
 Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains a number of ideas to possibly improve the InvOpt package.
 
 ## Citing
 If you use InvOpt for research, please cite our accompanying paper:
 
 ```bibtex
 @article{zattoniscroccaro2023learning,
-  title={Learning in Inverse Optimization: Incenter Cost, Augmented Suboptimality Loss, and Algorithm},
+  title={Learning in Inverse Optimization: Incenter Cost, Augmented Suboptimality Loss, and Algorithms},
   author={Zattoni Scroccaro, Pedro and Atasoy, Bilge and Mohajerin Esfahani, Peyman},
-  journal={arXiv preprint arXiv:0000.00000},
+  journal={https://arxiv.org/abs/2305.07730},
   year={2023}
 }
 ```
```

### Comparing `invopt-0.0.2/pyproject.toml` & `invopt-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invopt"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Pedro Zattoni Scroccaro", email="pedroszattoni@gmail.com" },
 ]
 description = "Inverse Optimization with Python"
 readme = "README.md"
 keywords = ["inverse-optimization"]
 requires-python = ">=3.7"
```

### Comparing `invopt-0.0.2/src/invopt/main.py` & `invopt-0.0.3/src/invopt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,30 +277,33 @@
                               theta_hat=None,
                               feasibility=False,
                               verbose=False,
                               gurobi_params=None):
     """
     Inverse optimization for discrete models with consistent data.
 
-    Uses incenter (default) or feasibility strategy. See an example usage at
-    https://github.com/pedroszattoni/invopt/tree/main/examples
+    Uses incenter (default) or feasibility strategy. For more details, see
+    https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model_consistent
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
     phi : callable
         Feature function. Given a signal s and response x, returns a 1D
         ndarray feature vector. Syntax: phi(s, x).
     decision_space : {tuple('binary', n)}
         Tuple containing type and dimension of the decision space.
     X : {callable, None}, optional
         Constraint set. Given a signal s and response x, returns True if x is a
-        feasible response, and False otherwise. Syntax: X(s, x). If None, it
-        will be defined as "def X(s, x): return True". The default is None.
+        feasible response, and False otherwise. It does not need to check for
+        the type of the decision space contained in decision_space. For
+        example, if decision_space=('binary', n), X does not need to check if x
+        is a binary vector. Syntax: X(s, x). If None, it will be defined as
+        "def X(s, x): return True". The default is None.
     dist_func : {callable, None}, optional
         Distance function. Given two responses x1 and x2, returns the distance
         between them according to some distance metric. Not required when
         using the feasibility strategy. Syntax: dist_func(x1, x2). The default
         is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
@@ -456,30 +459,33 @@
                    theta_hat=None,
                    sub_loss=False,
                    verbose=False,
                    gurobi_params=None):
     """
     Inverse optimization for discrete models.
 
-    See an example usage at
-    https://github.com/pedroszattoni/invopt/tree/main/examples
+    For more details, see
+    https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
     phi : callable
         Feature function. Given a signal s and response x, returns a 1D
         ndarray feature vector. Syntax: phi(s, x).
     decision_space : {tuple('binary', n)}
         Tuple containing type and dimension of the decision space.
     X : {callable, None}, optional
         Constraint set. Given a signal s and response x, returns True if x is a
-        feasible response, and False otherwise. Syntax: X(s, x). If None, it
-        will be defined as "def X(s, x): return True". The default is None.
+        feasible response, and False otherwise. It does not need to check for
+        the type of the decision space contained in decision_space. For
+        example, if decision_space=('binary', n), X does not need to check if x
+        is a binary vector. Syntax: X(s, x). If None, it will be defined as
+        "def X(s, x): return True". The default is None.
     dist_func : {callable, None}, optional
         Distance function. Given two responses x1 and x2, returns the distance
         between them according to some distance metric. Not required when
         sub_loss=True. Syntax: dist_func(x1, x2). The default is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
@@ -627,28 +633,32 @@
                reg_param=0,
                sub_loss=False,
                verbose=False,
                gurobi_params=None):
     """
     Inverse optimization for linear models with mixed-integer feasible sets.
 
-    See an example usage at
-    https://github.com/pedroszattoni/invopt/tree/main/examples
+    For more details, see
+    https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_linear
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
     decision_space : {tuple('binary', n)}
-        Tuple containing type and dimension of the decision space.
+        Tuple containing type and dimension of the decision space fo the
+        integer part of the decision vector.
     Z : {callable, None}, optional
         Constraint set of the integer part of the decision vector. Given a
         signal s = (A, B, c, w) and response x = (y, z), returns True if z
         (i.e., the integer part of x) is a feasible response, and False
-        otherwise. Syntax: Z(w, z). If None, it will be defined as
+        otherwise. It does not need to check for the type of the decision space
+        contained in decision_space. For example, if
+        decision_space=('binary', n), Z does not need to check if z
+        is a binary vector. Syntax: Z(w, z). If None, it will be defined as
         "def Z(w, x): return True". The default is None.
     phi1 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi1(w, z): return np.array([0])". The default is None.
     phi2 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
@@ -857,30 +867,219 @@
         Q_opt = np.array([[Q[i, j].X for i in range(m2)] for j in range(u1)])
         q_opt = np.array([q[i].X for i in range(u2)])
 
     theta_opt = np.concatenate((Q_opt.flatten('F'), q_opt))
     return theta_opt
 
 
+def MIP_quadratic(dataset, decision_space,
+                  Z=None,
+                  phi1=None,
+                  phi2=None,
+                  dist_func=None,
+                  Theta=None,
+                  regularizer='L2_squared',
+                  reg_param=0,
+                  sub_loss=False,
+                  verbose=False,
+                  solver='mosek'):
+    """
+    Inverse optimization for quadratic models with mixed-integer feasible sets.
+
+    For more details, see
+    https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_quadratic
+
+    Parameters
+    ----------
+    dataset : list of tuples
+        List of tuples (s, x), where s is the signal and x is the response.
+    decision_space : {tuple('binary', n)}
+        Tuple containing type and dimension of the decision space.
+    Z : {callable, None}, optional
+        Constraint set of the integer part of the decision vector. Given a
+        signal s = (A, B, c, w) and response x = (y, z), returns True if z
+        (i.e., the integer part of x) is a feasible response, and False
+        otherwise. It does not need to check for the type of the decision space
+        contained in decision_space. For example, if
+        decision_space=('binary', n), Z does not need to check if z
+        is a binary vector. Syntax: Z(w, z). If None, it will be defined as
+        "def Z(w, x): return True". The default is None.
+    phi1 : {callable, None}, optional
+        Feature function. Given w and response z, returns a 1D
+        ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
+        as "def phi1(w, z): return np.array([0])". The default is None.
+    phi2 : {callable, None}, optional
+        Feature function. Given w and response z, returns a 1D
+        ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
+        as "def phi2(w, z): return np.array([0])". The default is None.
+    dist_func : {callable, None}, optional
+        Distance function. Given two responses x1=(y1,z1) and x2=(y2,z2),
+        returns the distance of their integer parts according to some distance
+        metric. Not required when sub_loss=True. Syntax: dist_func(z1, z2).
+        The default is None.
+    Theta : {None, 'nonnegative'}, optional
+        Constraints on cost vector theta. The default is None.
+    regularizer : {'L2_squared', 'L1'}, optional
+        Type of regularization on cost vector theta. The default is
+        'L2_squared'.
+    reg_param : float, optional
+        Nonnegative regularization parameter. The default is 0.
+    sub_loss : bool, optional
+        If True, solve the problem using the Suboptimality loss. Namely,
+        searches over the facts of the unit L-infinity sphere for the cost
+        vector with the smallest loss. If Theta='nonnegative', only searches
+        over the nonnegative facet of the L-1 sphere. If False, solve the
+        problem using the Augmented Suboptimality loss. The default is False.
+    verbose : bool, optional
+        If True, print solver's output. The default is False.
+
+    Raises
+    ------
+    Exception
+        If unsupported Theta, regularizer, or decision_space. If Gurobi does
+        not find an optimal solution. If sub_loss=False and dist_func is None.
+
+    Returns
+    -------
+    theta_opt : 1D ndarray
+        An optimal cost vector according to the chosen strategy.
+
+    """
+    try:
+        import cvxpy as cp
+    except ImportError:
+        print("cvxpy is required for invopt's MIP_quadratic function.")
+
+    # Check if inputs are valid
+    check_Theta(Theta)
+    check_decision_space(decision_space)
+    check_regularizer(regularizer)
+    check_reg_parameter(reg_param)
+
+    # Warnings
+    warning_large_decision_space(decision_space)
+    warning_dist_func_reg_param_sub_loss(dist_func, reg_param, sub_loss)
+
+    N = len(dataset)
+
+    if Z is None:
+        def Z(s, z): return True
+
+    if phi1 is None:
+        def phi1(w, z): return np.array([0])
+    if phi2 is None:
+        def phi2(w, z): return np.array([0])
+
+    # Sample signal and response to get the the dimensions of the problem
+    s_test, x_test = dataset[0]
+    A_test, _, _, w_test = s_test
+    y_test, z_test = x_test
+    u1 = len(phi1(w_test, z_test))
+    u2 = len(phi2(w_test, z_test))
+    m1, m2 = A_test.shape
+
+    Qyy = cp.Variable((m2, m2), symmetric=True)
+    Q = cp.Variable((m2, u1))
+    q = cp.Variable((u2, 1))
+    beta = cp.Variable(N)
+
+    constraints = []
+
+    sum_beta = (1/N)*cp.sum(beta)
+
+    if Theta == 'nonnegative':
+        constraints += [Q >= 0, q >= 0]
+
+    for i in range(N):
+        s_hat, x_hat = dataset[i]
+        y_hat, z_hat = x_hat
+        A, B, c, w_hat = s_hat
+        if decision_space[0] == 'binary':
+            n = decision_space[1]
+            for k in range(2**n):
+                z = dec_to_bin(k, n)
+                if Z(w_hat, z):
+                    alpha = cp.Variable((1, 1))
+                    lamb = cp.Variable((m1, 1))
+
+                    if sub_loss:
+                        dist = 0
+                    else:
+                        dist = dist_func(z_hat, z)
+
+                    theta_phi_hat = (y_hat.T @ Qyy @ y_hat
+                                     + y_hat.T @ Q @ phi1(w_hat, z_hat)
+                                     + q.T @ phi2(w_hat, z_hat))
+
+                    lambcBz = lamb.T @ (c - B @ z)
+
+                    qphi2 = q.T @ phi2(w_hat, z)
+
+                    constraints += [theta_phi_hat + alpha + lambcBz - qphi2
+                                    <= beta[i] - dist]
+
+                    off_diag = Q @ phi1(w_hat, z).reshape((u1, 1)) + A.T @ lamb
+                    constraints += [cp.bmat([[Qyy, off_diag],
+                                             [off_diag.T, 4*alpha]]) >> 0]
+                    constraints += [lamb >= 0]
+
+    if sub_loss:
+        constraints += [cp.trace(Qyy) == 1]
+        obj = cp.Minimize(sum_beta)
+    else:
+        if regularizer == 'L2_squared':
+            Qyy_sum = cp.sum_squares(Qyy)
+            Q_sum = cp.sum_squares(Q)
+            q_sum = cp.sum_squares(q)
+            reg_term = (reg_param/2)*(Qyy_sum + Q_sum + q_sum)
+        elif regularizer == 'L1':
+            tQyy = cp.Variable((m2, m2), symmetric=True)
+            tQ = cp.Variable((m2, u1))
+            tq = cp.Variable((u2, 1))
+            reg_term = reg_param*(cp.sum(tQyy) + cp.sum(tQ) + cp.sum(tq))
+            constraints += [Qyy <= tQyy, -Qyy <= tQyy]
+            constraints += [Q <= tQ, -Q <= tQ]
+            constraints += [q <= tq, -q <= tq]
+
+        obj = cp.Minimize(reg_term + sum_beta)
+
+    prob = cp.Problem(obj, constraints)
+    prob.solve(verbose=verbose)
+
+    if prob.status != 'optimal':
+        raise Exception('Optimal solution not found. CVXPY status code '
+                        f'= {prob.status}. Set the flag verbose=True for more '
+                        'details.')
+
+    Qyy_opt = Qyy.value
+    Q_opt = Q.value
+    q_opt = q.value
+
+    theta_opt = np.concatenate((Qyy_opt.flatten('F'),
+                                Q_opt.flatten('F'),
+                                q_opt.flatten('F')))
+    return theta_opt
+
+
 def FOM(dataset, phi, theta_0, FOP, step_size, T,
         Theta=None,
         step='standard',
         regularizer='L2_squared',
         reg_param=0,
         theta_hat=None,
         batch_type=1,
         averaged=0,
         callback=None,
         normalize_grad=False,
         verbose=False):
     """
     Optimize (Augmented) Suboptimality loss using first-order methods.
 
-    See an example usage at
-    https://github.com/pedroszattoni/invopt/tree/main/examples
+    For more details, see
+    https://github.com/pedroszattoni/invopt/tree/main/examples/FOM
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
     phi : callable
         Feature function. Given a signal s and response x, returns a 1D
@@ -933,29 +1132,29 @@
         iterations: (1/T)*sum_{t=1}^{T} theta_t. If averaged=2, uses a weighted
         average of iterations: (2/(T*(T+1)))*sum_{t=1}^{T} t*theta_t. In
         theory, for strongly convex problems, the weighted average works better
         (see Lacoste-Julien et al. "A simpler approach to obtaining an O(1/t)
         convergence rate for the projected stochastic subgradient method"). The
         default is 0.
     callback : {callable, None}, optional
-        If not None, called after each iteration of the algorithm. The default
+        If not None, callback(theta_t) is evaluated for t=0,...,T. The default
         is None.
     normalize_grad : bool, optional
         If True, subgradient vectors are normalized before each iteration of
         the algorithm. If step='standard', the L2 norm of the subgradient is
-        used. If step='standard', the L-infinity norm of the subgradient is
-        used. The default is False.
+        used. If step='exponentiated', the L-infinity norm of the subgradient
+        is used. The default is False.
     verbose : bool, optional
         If True, prints iteration counter. The default is False.
 
     Raises
     ------
     Exception
-        If unsupported Theta or regularizer. If step = 'exponentiated',
-        reg_param > 0, and regularizer is not 'L1'.
+        If unsupported Theta or regularizer. If step = 'exponentiated', and
+        the regularizer is not 'L1'.
 
     Returns
     -------
     theta_T : {1D ndarray, list}
         If callback=None, returns the final (averaged) vector found after T
         iterations of the algorithm. Otherwise, returns a list of size T+1
         with elements callback(theta_t) for t=0,...,T, where theta_t is the
@@ -963,18 +1162,17 @@
 
     """
     # Check if inputs are valid
     check_Theta(Theta)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
 
-    if step == 'exponentiated':
-        if (reg_param == 0) or (regularizer != 'L1'):
-            raise Exception('To use step = \'exponentiated\', reg_param > 0,'
-                            'and regularizer = \'L1\' are required.')
+    if (step == 'exponentiated') and (regularizer != 'L1'):
+        raise Exception('To use step = \'exponentiated\', '
+                        'regularizer = \'L1\' is required.')
 
     # Get the number of examples and dimension of the problem
     N = len(dataset)
     p = len(theta_0)
 
     if theta_hat is None:
         theta_hat = np.zeros(p)
@@ -1180,193 +1378,7 @@
             theta_t1 = theta_t1/(reg_param*norm_theta_t1)
 
     # Projection onto Theta
     if Theta == 'nonnegative':
         theta_t = np.clip(theta_t, 0, None)
 
     return theta_t1
-
-
-def MIP_quadratic(dataset, decision_space,
-                  Z=None,
-                  phi1=None,
-                  phi2=None,
-                  dist_func=None,
-                  Theta=None,
-                  regularizer='L2_squared',
-                  reg_param=0,
-                  sub_loss=False,
-                  verbose=False,
-                  solver='mosek'):
-    """
-    Inverse optimization for quadratic models with mixed-integer feasible sets.
-
-    See an example usage at
-    https://github.com/pedroszattoni/invopt/tree/main/examples
-
-    Parameters
-    ----------
-    dataset : list of tuples
-        List of tuples (s, x), where s is the signal and x is the response.
-    decision_space : {tuple('binary', n)}
-        Tuple containing type and dimension of the decision space.
-    Z : {callable, None}, optional
-        Constraint set of the integer part of the decision vector. Given a
-        signal s = (A, B, c, w) and response x = (y, z), returns True if z
-        (i.e., the integer part of x) is a feasible response, and False
-        otherwise. Syntax: Z(w, z). If None, it will be defined as
-        "def Z(w, x): return True". The default is None.
-    phi1 : {callable, None}, optional
-        Feature function. Given w and response z, returns a 1D
-        ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
-        as "def phi1(w, z): return np.array([0])". The default is None.
-    phi2 : {callable, None}, optional
-        Feature function. Given w and response z, returns a 1D
-        ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
-        as "def phi2(w, z): return np.array([0])". The default is None.
-    dist_func : {callable, None}, optional
-        Distance function. Given two responses x1=(y1,z1) and x2=(y2,z2),
-        returns the distance of their integer parts according to some distance
-        metric. Not required when sub_loss=True. Syntax: dist_func(z1, z2).
-        The default is None.
-    Theta : {None, 'nonnegative'}, optional
-        Constraints on cost vector theta. The default is None.
-    regularizer : {'L2_squared', 'L1'}, optional
-        Type of regularization on cost vector theta. The default is
-        'L2_squared'.
-    reg_param : float, optional
-        Nonnegative regularization parameter. The default is 0.
-    sub_loss : bool, optional
-        If True, solve the problem using the Suboptimality loss. Namely,
-        searches over the facts of the unit L-infinity sphere for the cost
-        vector with the smallest loss. If Theta='nonnegative', only searches
-        over the nonnegative facet of the L-1 sphere. If False, solve the
-        problem using the Augmented Suboptimality loss. The default is False.
-    verbose : bool, optional
-        If True, print solver's output. The default is False.
-
-    Raises
-    ------
-    Exception
-        If unsupported Theta, regularizer, or decision_space. If Gurobi does
-        not find an optimal solution. If sub_loss=False and dist_func is None.
-
-    Returns
-    -------
-    theta_opt : 1D ndarray
-        An optimal cost vector according to the chosen strategy.
-
-    """
-    try:
-        import cvxpy as cp
-    except ImportError:
-        print("cvxpy is required for invopt's MIP_quadratic function.")
-
-    # Check if inputs are valid
-    check_Theta(Theta)
-    check_decision_space(decision_space)
-    check_regularizer(regularizer)
-    check_reg_parameter(reg_param)
-
-    # Warnings
-    warning_large_decision_space(decision_space)
-    warning_dist_func_reg_param_sub_loss(dist_func, reg_param, sub_loss)
-
-    N = len(dataset)
-
-    if Z is None:
-        def Z(s, z): return True
-
-    if phi1 is None:
-        def phi1(w, z): return np.array([0])
-    if phi2 is None:
-        def phi2(w, z): return np.array([0])
-
-    # Sample signal and response to get the the dimensions of the problem
-    s_test, x_test = dataset[0]
-    A_test, _, _, w_test = s_test
-    y_test, z_test = x_test
-    u1 = len(phi1(w_test, z_test))
-    u2 = len(phi2(w_test, z_test))
-    m1, m2 = A_test.shape
-
-    Qyy = cp.Variable((m2, m2), symmetric=True)
-    Q = cp.Variable((m2, u1))
-    q = cp.Variable((u2, 1))
-    beta = cp.Variable(N)
-
-    constraints = []
-
-    sum_beta = (1/N)*cp.sum(beta)
-
-    if Theta == 'nonnegative':
-        constraints += [Q >= 0, q >= 0]
-
-    for i in range(N):
-        s_hat, x_hat = dataset[i]
-        y_hat, z_hat = x_hat
-        A, B, c, w_hat = s_hat
-        if decision_space[0] == 'binary':
-            n = decision_space[1]
-            for k in range(2**n):
-                z = dec_to_bin(k, n)
-                if Z(w_hat, z):
-                    alpha = cp.Variable((1, 1))
-                    lamb = cp.Variable((m1, 1))
-
-                    if sub_loss:
-                        dist = 0
-                    else:
-                        dist = dist_func(z_hat, z)
-
-                    theta_phi_hat = (y_hat.T @ Qyy @ y_hat
-                                     + y_hat.T @ Q @ phi1(w_hat, z_hat)
-                                     + q.T @ phi2(w_hat, z_hat))
-
-                    lambcBz = lamb.T @ (c - B @ z)
-
-                    qphi2 = q.T @ phi2(w_hat, z)
-
-                    constraints += [theta_phi_hat + alpha + lambcBz - qphi2
-                                    <= beta[i] - dist]
-
-                    off_diag = Q @ phi1(w_hat, z).reshape((u1, 1)) + A.T @ lamb
-                    constraints += [cp.bmat([[Qyy, off_diag],
-                                             [off_diag.T, 4*alpha]]) >> 0]
-                    constraints += [lamb >= 0]
-
-    if sub_loss:
-        constraints += [cp.trace(Qyy) == 1]
-        obj = cp.Minimize(sum_beta)
-    else:
-        if regularizer == 'L2_squared':
-            Qyy_sum = cp.sum_squares(Qyy)
-            Q_sum = cp.sum_squares(Q)
-            q_sum = cp.sum_squares(q)
-            reg_term = (reg_param/2)*(Qyy_sum + Q_sum + q_sum)
-        elif regularizer == 'L1':
-            tQyy = cp.Variable((m2, m2), symmetric=True)
-            tQ = cp.Variable((m2, u1))
-            tq = cp.Variable((u2, 1))
-            reg_term = reg_param*(cp.sum(tQyy) + cp.sum(tQ) + cp.sum(tq))
-            constraints += [Qyy <= tQyy, -Qyy <= tQyy]
-            constraints += [Q <= tQ, -Q <= tQ]
-            constraints += [q <= tq, -q <= tq]
-
-        obj = cp.Minimize(reg_term + sum_beta)
-
-    prob = cp.Problem(obj, constraints)
-    prob.solve(verbose=verbose)
-
-    if prob.status != 'optimal':
-        raise Exception('Optimal solution not found. CVXPY status code '
-                        f'= {prob.status}. Set the flag verbose=True for more '
-                        'details.')
-
-    Qyy_opt = Qyy.value
-    Q_opt = Q.value
-    q_opt = q.value
-
-    theta_opt = np.concatenate((Qyy_opt.flatten('F'),
-                                Q_opt.flatten('F'),
-                                q_opt.flatten('F')))
-    return theta_opt
```

### Comparing `invopt-0.0.2/src/invopt.egg-info/PKG-INFO` & `invopt-0.0.3/src/invopt.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: invopt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Inverse Optimization with Python
 Author-email: Pedro Zattoni Scroccaro <pedroszattoni@gmail.com>
 Project-URL: Homepage, https://github.com/pedroszattoni/invopt
 Project-URL: Bug Tracker, https://github.com/pedroszattoni/inverse-optimization/issues
 Keywords: inverse-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# InvOpt: Inverse Optimization in Python
 
-InvOpt is a Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in the exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, our goal is to model the cost function being optimized by the expert, using examples of exogenous signals and corresponding expert response actions. More concretely, given a dataset $\mathcal{D} = \{(\hat{s}_i, \hat{x}_i)\}_{i=1}^N$ of exogenous signals $\hat{s}_i$ and the respective expert's response $\hat{x}_i$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that the **Forward Optimization Problem (FOP)** with feature mapping $\phi$
-$$
-x_i \in \arg\min_{x \in \mathbb{X}(\hat{s}_i)} \ \theta^\top \phi(\hat{s}_i,x) 
-$$reproduces (or in some sense approximates) the expert's action $\hat{x}_i$. For a more detailed description of the IO problem and its modelling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/0000.00000) and the references therein. 
+# InvOpt: Inverse Optimization with Python
+
+InvOpt is a Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in the exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, our goal is to model the cost function being optimized by the expert, using examples of exogenous signals and corresponding expert response actions. More concretely, given a dataset $\mathcal{D} = \\{(\hat{s}_ i, \hat{x}_ i)\\}_ {i=1}^N$ of exogenous signals $\hat{s}_ i$ and the respective expert's response $\hat{x}_ i$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that the **Forward Optimization Problem (FOP)** with feature mapping $\phi$
+$$x_i \in \arg\min_ {x \in \mathbb{X}(\hat{s}_ i)} \ \theta^\top \phi(\hat{s}_ i,x)$$ reproduces (or in some sense approximates) the expert's action $\hat{x}_ i$. For a more detailed description of the IO problem and its modelling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/2305.07730) and the references therein. 
 
 ## Installation
 
 ```bash
 pip install invopt
 ```
 InvOpt depends on NumPy. Moreover, some of its functions also depend on gurobipy or cvxpy. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
 
-## Usage & examples
+## Usage and examples
+
+The following functions are available in the InvOpt package to solving IO problems:
 
-The folder [examples](https://github.com/pedroszattoni/invopt/tree/main/examples) contains descriptions of the functions available in the InvOpt package, as well as multiple examples.
+- [`discrete_model_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
+- [`discrete_model`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model): for FOPs with dicrete decision spaces (e.g., binary).
+- [`MIP_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
+- [`MIP_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
+- [`FOM`](https://github.com/pedroszattoni/invopt/tree/main/examples/FOM): for general FOPs. Solves IO problem approximately using first-order methods.
 
 ## Contributing
 
 Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains a number of ideas to possibly improve the InvOpt package.
 
 ## Citing
 If you use InvOpt for research, please cite our accompanying paper:
 
 ```bibtex
 @article{zattoniscroccaro2023learning,
-  title={Learning in Inverse Optimization: Incenter Cost, Augmented Suboptimality Loss, and Algorithm},
+  title={Learning in Inverse Optimization: Incenter Cost, Augmented Suboptimality Loss, and Algorithms},
   author={Zattoni Scroccaro, Pedro and Atasoy, Bilge and Mohajerin Esfahani, Peyman},
-  journal={arXiv preprint arXiv:0000.00000},
+  journal={https://arxiv.org/abs/2305.07730},
   year={2023}
 }
 ```
```

### Comparing `invopt-0.0.2/tests/test_examples.py` & `invopt-0.0.3/tests/test_examples.py`

 * *Files identical despite different names*

