# Comparing `tmp/cefeste-1.1.3.tar.gz` & `tmp/cefeste-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.1.3.tar", last modified: Thu May 11 12:59:37 2023, max compression
+gzip compressed data, was "cefeste-1.1.4.tar", last modified: Mon May 22 13:17:43 2023, max compression
```

## Comparing `cefeste-1.1.3.tar` & `cefeste-1.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.603643 cefeste-1.1.3/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.3/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2076 2023-05-11 12:59:37.603643 cefeste-1.1.3/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1560 2023-05-10 10:23:33.000000 cefeste-1.1.3/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-05-11 12:55:44.000000 cefeste-1.1.3/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-11 12:59:37.603643 cefeste-1.1.3/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      999 2023-05-11 12:55:44.000000 cefeste-1.1.3/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.555639 cefeste-1.1.3/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.591642 cefeste-1.1.3/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.595642 cefeste-1.1.3/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15368 2023-05-10 10:23:33.000000 cefeste-1.1.3/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25817 2023-05-10 10:23:33.000000 cefeste-1.1.3/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.603643 cefeste-1.1.3/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.603643 cefeste-1.1.3/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.3/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.595642 cefeste-1.1.3/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2076 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 13:17:43.649895 cefeste-1.1.4/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.4/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2821 2023-05-22 13:17:43.649895 cefeste-1.1.4/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2023-05-22 13:14:02.000000 cefeste-1.1.4/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      754 2023-05-22 13:17:30.000000 cefeste-1.1.4/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-22 13:17:43.649895 cefeste-1.1.4/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      999 2023-05-22 13:06:46.000000 cefeste-1.1.4/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 13:17:43.629893 cefeste-1.1.4/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 13:17:43.641894 cefeste-1.1.4/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.4/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.4/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 13:17:43.645894 cefeste-1.1.4/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15386 2023-05-22 13:02:11.000000 cefeste-1.1.4/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25817 2023-05-10 10:23:33.000000 cefeste-1.1.4/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 13:17:43.649895 cefeste-1.1.4/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.4/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.4/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.4/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.4/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 13:17:43.649895 cefeste-1.1.4/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2629 2023-05-22 13:06:15.000000 cefeste-1.1.4/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.4/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 13:17:43.641894 cefeste-1.1.4/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2821 2023-05-22 13:17:43.000000 cefeste-1.1.4/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-22 13:17:43.000000 cefeste-1.1.4/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-22 13:17:43.000000 cefeste-1.1.4/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-22 13:17:43.000000 cefeste-1.1.4/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-22 13:17:43.000000 cefeste-1.1.4/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.1.3/LICENCE` & `cefeste-1.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.3/PKG-INFO` & `cefeste-1.1.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-Metadata-Version: 2.1
-Name: cefeste
-Version: 1.1.3
-Summary: Feature Selection and Elimination
-Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
-Author: DAT/Mattia Centurelli
-Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
-Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9, <4
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# **C**redito **E**miliano -  **Fe**ature **S**election, **T**ransformation and **E**limination (CE - FeSTE)
-
-This repo contains the 'FeSTE' python package which helps in the features management from the pre-filtering to the pre-processing and feature elimination.
-
-# Installation
-
-To install it:
-
-1) **Optional**: create a new Python virtual environment (through bash terminal run: "py -m venv your_env_name" and then "source your_env_name/Scripts/activate )
-2) Install the package:
-    - User Mode: 
-```pip install ce-feste```
-
-
-# Structure
-
-The .py package is stored in src and contains 3 sub-modules:
-- **selection**: contains the feature preliminary selection functions
-- **transform**: contains the feature pre-processing functions
-- **elimination**: contains the feature elimination functions
-
-# Filters
-
-## Selection
-
-- Univariate filters:
-    - No constant features
-    - Number of distinct value too low
-    - Number of missing values too high
-    - Too concentrate in the most frequent value
-    - Unstable between sets
-- Multivariate filters:
-    - Spearman Correlation for numerical features
-    - Cramer's V for categorical features
-    - R2 for mixed features
-    - VIF
-- Explanatory filters:
-    - Feature AUROC for classification 
-    - Feature Correlation with target for regression
-    
-## Elimination
-- Shap Recursive Feature Elimination with HyperParam Optimization
-
-# Trasformation
-
-- Only 2 classes added to select and rename columns in datasets. Useful for generating the production pipeline
+# **C**redito **E**miliano -  **Fe**ature **S**election, **T**ransformation and **E**limination (CE - FeSTE)
+
+This repo contains the 'FeSTE' python package which helps in the features management from the pre-filtering to the pre-processing and feature elimination.
+
+# Installation
+
+To install it:
+
+1) **Optional**: create a new Python virtual environment (through bash terminal run: "py -m venv your_env_name" and then "source your_env_name/Scripts/activate )
+2) Install the package:
+    - User Mode: 
+```pip install cefeste```
+
+
+# Structure
+
+The .py package is stored in src and contains 3 sub-modules:
+- **selection**: contains the feature preliminary selection functions
+- **transform**: contains the feature pre-processing functions
+- **elimination**: contains the feature elimination functions
+
+# Filters
+
+## Selection
+
+The main class of this module is FeatureSelection. It applies several filters that can be grouped in the following:
+
+- Univariate filters:
+    - No constant features
+    - Number of distinct value too low
+    - Number of missing values too high
+    - Too concentrate in the most frequent value
+    - Unstable between sets
+- Multivariate filters:
+    - Spearman Correlation for numerical features
+    - Cramer's V for categorical features
+    - R2 for mixed features
+    - VIF
+- Explanatory filters:
+    - Feature AUROC for classification 
+    - Feature Correlation with target for regression
+    
+## Trasformation
+
+It is more a technical module which contains 3 classes useful for generating the production pipeline:
+
+- ColumnExtractor: to extract columns from a pd.DataFrame
+- ColumnRenamer: to rename columns and to transform a np.ndarray to a pd.DataFrame
+- Categorizer: to trasform the dtype of pd.DataFrame columns from 'object' to 'category'
+
+## Elimination
+
+The main class of this module is FeatureElimination which is useful for selecting the most useful feature to keep in the model and optimize the hyperparams in the meanwhile.
+
+It is a recursive method that at each iteration can:
+
+- Perform the hyperparameters optimization using user-defined model, grid, gridsearch method, evaluation measure
+- Calculate the feature shap importance value
+- Identify the last importance feature(/s) and Delete them for the next iteration
+
```

### Comparing `cefeste-1.1.3/pyproject.toml` & `cefeste-1.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="DAT - Mattia Centurelli", email="mcenturelli@credem.it" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-
+dependencies=[
+    "typed-ast==1.5.4",
+    "numpy==1.22.4",
+    "pandas==1.4.2",
+    "scikit-learn==1.1.1",
+    "scipy==1.8.1",
+    "statsmodels==0.13.2",
+    "PyYAML==6.0",
+    "shap==0.38.1",
+    "ipython",
+]
 [project.urls]
 "Homepage" = "https://dev.azure.com/credem-data/DAT/_git/ce-feste"
```

### Comparing `cefeste-1.1.3/setup.py` & `cefeste-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.1.3",
+    version="1.1.4",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT/Mattia Centurelli",
     author_email="mcenturelli@credem.it",
     url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `cefeste-1.1.3/src/cefeste/__init__.py` & `cefeste-1.1.4/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.3/src/cefeste/elimination/__init__.py` & `cefeste-1.1.4/src/cefeste/elimination/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             grid (dict): hyperparameters grid.
             feat_to_check (list, optional): Feature to analyze. If None all are used. Defaults to None.
             sample_col (str, optional): Name of the columns that indicates the samples (train, test). Defaults to None.
             sample_train_value (str, optional): Value of the sample column that indicates the train set. Defaults to None.
             algo_type (str, optional): "classification", "multiclass", "regression", describes the problem type.
                 "classification" has to be used only for binary classification. Defaults to "classification".
             cv_funct: function or class for the Cross Validation. Defaults to RandomizedSearchCV
-            cv_scoring: scoring argument of the cv_functs. Defaults to "auto" selects "roc_auc" fo classification, "r2" for regression 
+            cv_scoring: scoring argument of the cv_functs. Defaults to "auto" selects "roc_auc" fo classification, "r2" for regression
                 and "balanced accuracy" for multiclass.
             n_iter (int, optional): number of iteration, i.e. set of hyperparams tested in Cross Validation. Defaults to 20.
             manage_groups (bool, optional): determines if there is a feature whose groups have to be kept joined in CV. Defaults to False.
             groups (pd.Series, optional): feature whose groups have to be kept joined in CV. Defaults to None.
             cv_type : function or class for defining the CV sets. Defaults to StratifiedKFold(5, random_state=42, shuffle=True).
             use_ohe (bool, optional): determines whether to use One Hot Encoding on categorical features or not. Defaults to False.
             step_size (int or float, optional): determines how many features to remove at each step.
@@ -212,41 +212,41 @@
             dim_cat_threshold=self.dim_cat_threshold,
         )
 
         self.report = shap_report
 
         return self.report
 
-    def shap_plot(self):
-        """Plot the report."""
+    def plot_report(self):
+        """Plot the report train and validation score."""
         if self.report is not None:
             self.report.plot(
                 x="n_feat", y=["train_score", "valid_score"], xlim=(max(self.report.n_feat), min(self.report.n_feat))
             )
         else:
             raise ValueError("Missing report, run .make_report() first")
 
     def extract_features(self, selection_rule="decrease_perf", number_feat_rep=None, gap=0.1, alpha=0.5):
         """Extract survived features after SHAP RFE.
 
         Args:
             selection_rule (str, optional): "decrease_perf", "best_valid", "num_feat", "robust_tradeoff" describes the rule for which the features after shap are chosen. Defaults to 'decrease_perf'.
             number_feat_rep (int, optional): valid only for the selection_rule "num_feat", determines the number of features to be extracted according to the report. Defaults to None.
             gap(float, optional): valid only for the selection_rule "decrease_perf", identifies the maximum gap over which the decrease in performance is not acceptable.
-            alpha(float, optional): valid only fot the selection_rule "robust_tradeoff", determines which term is preferred betweeen robustness and average performances in the formula 
+            alpha(float, optional): valid only fot the selection_rule "robust_tradeoff", determines which term is preferred betweeen robustness and average performances in the formula
             α * Average_Perf - (1-α) * Gap_Robust
         Returns:
             list: list of features extracted after SHAP RFE according to the selection_rule.
         """
         self.selection_rule = selection_rule
         self.number_feat_rep = number_feat_rep
         self.gap = gap
         self.alpha = alpha
         # Check the target var and set the algo type
-        if selection_rule not in ["decrease_perf", "best_valid", "num_feat","robust_tradeoff"]:
+        if selection_rule not in ["decrease_perf", "best_valid", "num_feat", "robust_tradeoff"]:
             raise ValueError(
                 f"{selection_rule} is not a valid selection_rule. It should be one of the following:\n ['decrease_perf', 'best_valid', 'num_feat', 'robust_tradeoff']"
             )
 
         if self.report is not None:
             if selection_rule == "decrease_perf":
                 # Define n_feat: the first time the validation score decreases of more than 10%
@@ -274,28 +274,31 @@
 
             elif selection_rule == "best_valid":
                 # Define n_feat: best validation score iteration
                 n_min_feat = self.report.loc[
                     self.report["valid_score"] == self.report["valid_score"].max(), "n_feat"
                 ].min()
                 self.final_feat = list(self.report.loc[self.report["n_feat"] == n_min_feat, "feat_used"])[0]
-            
+
             elif selection_rule == "robust_tradeoff":
                 # Define n_feat: best score of the formula α * Average_Perf - (1-α) * Gap_Robust
                 adding_report = (
-                    self.report[["n_feat","train_score","valid_score"]]
-                    .assign(average_scoring=lambda x: (x.train_score + x.valid_score)/2)
+                    self.report[["n_feat", "train_score", "valid_score"]]
+                    .assign(avg_scoring=lambda x: (x.train_score + x.valid_score) / 2)
                     .assign(gap_ratio=lambda x: abs(x.train_score - x.valid_score))
-                    .assign(average_scoring=lambda x: (x.average_scoring - x.average_scoring.mean())/x.average_scoring.std())
-                    .assign(gap_ratio=lambda x: (x.gap_ratio - x.gap_ratio.mean())/x.gap_ratio.std())
-                    .assign(tradeoff_robust_average_scoring=lambda x: (alpha * x.average_scoring - (1 - alpha) * x.gap_ratio))
+                    .assign(avg_scoring=lambda x: (x.avg_scoring - x.avg_scoring.mean()) / x.avg_scoring.std())
+                    .assign(gap_ratio=lambda x: (x.gap_ratio - x.gap_ratio.mean()) / x.gap_ratio.std())
+                    .assign(tradeoff_robust_avg_scoring=lambda x: (alpha * x.avg_scoring - (1 - alpha) * x.gap_ratio))
                 )
-                n_min_feat = adding_report.loc[adding_report.tradeoff_robust_average_scoring == adding_report.tradeoff_robust_average_scoring.max(),"n_feat"].min()
+                n_min_feat = adding_report.loc[
+                    lambda x: x.tradeoff_robust_avg_scoring == x.tradeoff_robust_avg_scoring.max(),
+                    "n_feat",
+                ].min()
                 self.final_feat = list(self.report.loc[self.report["n_feat"] == n_min_feat, "feat_used"])[0]
-                
+
             else:
                 # Define n_feat: the user choose the features to use according to number of features to be used
                 if number_feat_rep is not None:
                     try:
                         self.final_feat = list(self.report.loc[self.report["n_feat"] == number_feat_rep, "feat_used"])[
                             0
                         ]
```

### Comparing `cefeste-1.1.3/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.1.4/src/cefeste/elimination/shap_rfe.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.3/src/cefeste/selection/__init__.py` & `cefeste-1.1.4/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.3/src/cefeste/selection/explanatory.py` & `cefeste-1.1.4/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.3/src/cefeste/selection/multivariate.py` & `cefeste-1.1.4/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.3/src/cefeste/selection/univariate.py` & `cefeste-1.1.4/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.3/src/cefeste/utils.py` & `cefeste-1.1.4/src/cefeste/utils.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.3/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.3
+Version: 1.1.4
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,28 +20,30 @@
 # Installation
 
 To install it:
 
 1) **Optional**: create a new Python virtual environment (through bash terminal run: "py -m venv your_env_name" and then "source your_env_name/Scripts/activate )
 2) Install the package:
     - User Mode: 
-```pip install ce-feste```
+```pip install cefeste```
 
 
 # Structure
 
 The .py package is stored in src and contains 3 sub-modules:
 - **selection**: contains the feature preliminary selection functions
 - **transform**: contains the feature pre-processing functions
 - **elimination**: contains the feature elimination functions
 
 # Filters
 
 ## Selection
 
+The main class of this module is FeatureSelection. It applies several filters that can be grouped in the following:
+
 - Univariate filters:
     - No constant features
     - Number of distinct value too low
     - Number of missing values too high
     - Too concentrate in the most frequent value
     - Unstable between sets
 - Multivariate filters:
@@ -49,13 +51,25 @@
     - Cramer's V for categorical features
     - R2 for mixed features
     - VIF
 - Explanatory filters:
     - Feature AUROC for classification 
     - Feature Correlation with target for regression
     
+## Trasformation
+
+It is more a technical module which contains 3 classes useful for generating the production pipeline:
+
+- ColumnExtractor: to extract columns from a pd.DataFrame
+- ColumnRenamer: to rename columns and to transform a np.ndarray to a pd.DataFrame
+- Categorizer: to trasform the dtype of pd.DataFrame columns from 'object' to 'category'
+
 ## Elimination
-- Shap Recursive Feature Elimination with HyperParam Optimization
 
-# Trasformation
+The main class of this module is FeatureElimination which is useful for selecting the most useful feature to keep in the model and optimize the hyperparams in the meanwhile.
+
+It is a recursive method that at each iteration can:
+
+- Perform the hyperparameters optimization using user-defined model, grid, gridsearch method, evaluation measure
+- Calculate the feature shap importance value
+- Identify the last importance feature(/s) and Delete them for the next iteration
 
-- Only 2 classes added to select and rename columns in datasets. Useful for generating the production pipeline
```

### Comparing `cefeste-1.1.3/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.1.4/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

