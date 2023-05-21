# Comparing `tmp/arfs-1.0.7.tar.gz` & `tmp/arfs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-1.0.7.tar", last modified: Thu Apr 27 11:33:29 2023, max compression
+gzip compressed data, was "arfs-1.1.0.tar", last modified: Sun May 21 19:19:53 2023, max compression
```

## Comparing `arfs-1.0.7.tar` & `arfs-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.390123 arfs-1.0.7/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.0.7/LICENSE.md
--rw-rw-rw-   0        0        0    11069 2023-04-27 11:33:29.392091 arfs-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.0.7/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1389 2023-04-27 11:33:29.401091 arfs-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.028442 arfs-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.147727 arfs-1.0.7/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-04-21 14:47:13.000000 arfs-1.0.7/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.0.7/src/arfs/association.py
--rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.030439 arfs-1.0.7/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.268991 arfs-1.0.7/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.0.7/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.0.7/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.362636 arfs-1.0.7/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    83997 2023-04-27 11:30:49.000000 arfs-1.0.7/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    12718 2023-04-27 11:30:47.000000 arfs-1.0.7/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2627 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15051 2023-01-06 14:55:49.000000 arfs-1.0.7/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    14764 2023-04-27 11:30:48.000000 arfs-1.0.7/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    22780 2023-01-09 09:22:51.000000 arfs-1.0.7/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    29117 2023-04-27 11:30:48.000000 arfs-1.0.7/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.0.7/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    22356 2023-01-06 15:03:38.000000 arfs-1.0.7/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.204252 arfs-1.0.7/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-04-27 11:33:28.000000 arfs-1.0.7/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-04-27 11:33:29.000000 arfs-1.0.7/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 11:33:28.000000 arfs-1.0.7/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.0.7/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      365 2023-04-27 11:33:28.000000 arfs-1.0.7/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 11:33:28.000000 arfs-1.0.7/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.381089 arfs-1.0.7/tests/
--rw-rw-rw-   0        0        0    10657 2023-01-09 09:22:50.000000 arfs-1.0.7/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19566 2023-01-09 09:22:50.000000 arfs-1.0.7/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:19:53.045740 arfs-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0    11069 2023-05-21 19:19:53.046741 arfs-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.1.0/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1389 2023-05-21 19:19:53.053742 arfs-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.602690 arfs-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.764751 arfs-1.1.0/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-05-21 19:17:41.000000 arfs-1.1.0/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.1.0/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.1.0/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.604700 arfs-1.1.0/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.894743 arfs-1.1.0/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.1.0/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.1.0/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-05-21 19:19:53.008742 arfs-1.1.0/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.1.0/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    90381 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.1.0/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    13420 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15449 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    14764 2023-04-27 11:30:48.000000 arfs-1.1.0/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21796 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.1.0/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    28685 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.1.0/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    24872 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.829741 arfs-1.1.0/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.1.0/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      365 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 19:19:53.036742 arfs-1.1.0/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-1.1.0/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-1.1.0/tests/test_featselect.py
```

### Comparing `arfs-1.0.7/LICENSE.md` & `arfs-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/PKG-INFO` & `arfs-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.0.7
+Version: 1.1.0
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.0.7/README.md` & `arfs-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/setup.cfg` & `arfs-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/association.py` & `arfs-1.1.0/src/arfs/association.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/benchmark.py` & `arfs-1.1.0/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-1.1.0/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/dataset/data/housing.zip` & `arfs-1.1.0/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/feature_selection/__init__.py` & `arfs-1.1.0/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/feature_selection/allrelevant.py` & `arfs-1.1.0/src/arfs/feature_selection/allrelevant.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,16 @@
 import numpy as np
 import pandas as pd
 import lightgbm as lgb
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import scipy as sp
 
-from tqdm import tqdm
+from typing import Tuple
+from tqdm.auto import tqdm
 from sklearn.utils import check_random_state, check_X_y
 from sklearn.base import BaseEstimator, is_regressor, is_classifier, clone
 
 from sklearn.utils.validation import check_is_fitted
 from sklearn.feature_selection._base import SelectorMixin
 from sklearn.model_selection import RepeatedKFold, train_test_split
 from sklearn.inspection import permutation_importance
@@ -69,25 +70,70 @@
 
 from ..utils import (
     check_if_tree_based,
     is_lightgbm,
     is_catboost,
     create_dtype_dict,
     get_pandas_cat_codes,
+    validate_sample_weight,
 )
 
 ########################################################################################
 #
 # Main Classes and Methods
 # Provide a fit, transform and fit_transform method
 #
 ########################################################################################
 # !/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+NO_FEATURE_SELECTED_WARNINGS = "No feature selected - No data to plot"
+ARFS_COLOR_LIST = [
+    "#000000",
+    "#7F3C8D",
+    "#11A579",
+    "#3969AC",
+    "#F2B701",
+    "#E73F74",
+    "#80BA5A",
+    "#E68310",
+    "#008695",
+    "#CF1C90",
+    "#F97B72",
+]
+BLUE = "#2590fa"
+YELLOW = "#f0be00"
+RED = "#b51204"
+BCKGRD_COLOR = "#f5f5f5"
+PLT_PARAMS = {
+    "axes.prop_cycle": plt.cycler(color=ARFS_COLOR_LIST),
+    "axes.facecolor": BCKGRD_COLOR,
+    "patch.edgecolor": BCKGRD_COLOR,
+    "figure.facecolor": BCKGRD_COLOR,
+    "axes.edgecolor": BCKGRD_COLOR,
+    "savefig.edgecolor": BCKGRD_COLOR,
+    "savefig.facecolor": BCKGRD_COLOR,
+    "grid.color": "#d2d2d2",
+    "lines.linewidth": 1.5,
+}
+PLOT_KWARGS = dict(
+    kind="box",
+    boxprops=dict(linestyle="-", linewidth=1.5, color="gray", facecolor="gray"),
+    flierprops=dict(linestyle="-", linewidth=1.5, color="gray"),
+    medianprops=dict(linestyle="-", linewidth=1.5, color="#000000"),
+    whiskerprops=dict(linestyle="-", linewidth=1.5, color="gray"),
+    capprops=dict(linestyle="-", linewidth=1.5, color="gray"),
+    showfliers=False,
+    grid=True,
+    rot=0,
+    vert=False,
+    patch_artist=True,
+    fontsize=9,
+)
+
 
 class Leshy(SelectorMixin, BaseEstimator):
     """This is an improved version of BorutaPy which itself is an
     improved Python implementation of the Boruta R package.
     Boruta is an all relevant feature selection method, while most other are
     minimal optimal; this means it tries to find all features carrying
     information usable for prediction, rather than finding a possibly compact
@@ -275,45 +321,92 @@
         self.imp_real_hist = np.empty((0, X.shape[1]), float)
         self._fit(X, y, sample_weight=sample_weight)
         self.selected_features_ = self.feature_names_in_[self.support_]
         self.not_selected_features_ = self.feature_names_in_[~self.support_]
 
         return self
 
-    def _get_support_mask(self):
-        check_is_fitted(self)
-
-        return self.support_
-
     def transform(self, X):
         if not isinstance(X, pd.DataFrame):
             raise TypeError("X is not a dataframe")
         return X[self.selected_features_]
 
-    def _more_tags(self):
-        return {"allow_nan": True, "requires_y": True}
-
-    @staticmethod
-    def _validate_pandas_input(arg):
-        """Validate if pandas or numpy arrays are provided
+    @mpl.rc_context(PLT_PARAMS)
+    def plot_importance(self, n_feat_per_inch=5):
+        """Boxplot of the variable importance, ordered by magnitude
+        The max shadow variable importance illustrated by the dashed line.
+        Requires to apply the fit method first.
 
         Parameters
         ----------
-        arg : pd.DataFrame or np.array
-            the object to validate
+        n_feat_per_inch : int, default=5
+            number of features to plot per inch (for scaling the figure)
 
-        Raises
-        ------
-        TypeError
-            error if pandas or numpy arrays are not provided
+        Returns
+        -------
+        fig : plt.figure
+            the matplotlib figure object containing the boxplot
         """
-        try:
-            return arg.values
-        except AttributeError:
-            raise TypeError("input needs to be a numpy array or pandas data frame.")
+
+        if self.imp_real_hist is None:
+            raise ValueError("Use the fit method first to compute the var.imp")
+
+        vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
+        vimp_df = vimp_df.reindex(
+            vimp_df.mean().sort_values(ascending=True).index, axis=1
+        )
+
+        if vimp_df.dropna().empty:
+            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
+            return None
+        else:
+            fig, ax = plt.subplots(figsize=(16, vimp_df.shape[1] / n_feat_per_inch))
+            bp = vimp_df.plot(**PLOT_KWARGS, ax=ax)
+
+            n_strong = sum(self.support_)
+            n_weak = np.sum(self.support_weak_)
+            n_discarded = np.sum(~(self.support_ | self.support_weak_))
+            box_face_col = (
+                [BLUE] * n_strong + [YELLOW] * n_weak + ["gray"] * n_discarded
+            )
+            for c in range(len(box_face_col)):
+                bp.findobj(mpl.patches.Patch)[len(self.support_) - c - 1].set_facecolor(
+                    box_face_col[c]
+                )
+                bp.findobj(mpl.patches.Patch)[len(self.support_) - c - 1].set_color(
+                    box_face_col[c]
+                )
+
+            xrange = vimp_df.max(skipna=True).max(skipna=True) - vimp_df.min(
+                skipna=True
+            ).min(skipna=True)
+            bp.set_xlim(left=vimp_df.min(skipna=True).min(skipna=True) - 0.10 * xrange)
+
+            custom_lines = [
+                Line2D([0], [0], color=BLUE, lw=5),
+                Line2D([0], [0], color=YELLOW, lw=5),
+                Line2D([0], [0], color="gray", lw=5),
+                Line2D([0], [0], linestyle="--", color=RED, lw=2),
+            ]
+            bp.legend(
+                custom_lines,
+                ["confirmed", "tentative", "rejected", "sha. max"],
+                loc="lower right",
+            )
+            ax.axvline(x=self.sha_max, linestyle="--", color=RED)
+            ax.set_title("Leshy importance and selected predictors")
+            return fig
+
+    def _get_support_mask(self):
+        check_is_fitted(self)
+
+        return self.support_
+
+    def _more_tags(self):
+        return {"allow_nan": True, "requires_y": True}
 
     def _fit(self, X_raw, y, sample_weight=None):
         """Private method. See the methods overview in the documentation
         for explanation of the process
 
         Parameters
         ----------
@@ -325,38 +418,29 @@
             Individual weights for each sample
 
         Returns
         -------
         self : object
             Nothing but attributes
         """
-        # self.is_cat = is_catboost(self.estimator)
 
         start_time = time.time()
         # the basic cat features encoding
         # is performed when getting importances
         # because the columns are dynamically created/rejected
         X = X_raw
 
-        X = np.nan_to_num(X)
-        y = np.nan_to_num(y)
+        # only sklearn requires to fillna data
+        # modern GBM implementations can handle this
+        #X = X.fillna(0)
+        y = pd.Series(y).fillna(0) if not isinstance(y, pd.Series) else y.fillna(0)
 
         # check input params
         self._check_params(X, y)
-
-        if not isinstance(X, np.ndarray):
-            X = self._validate_pandas_input(X)
-
-        if not isinstance(y, np.ndarray):
-            y = self._validate_pandas_input(y)
-
-        if sample_weight is not None:
-            if not isinstance(sample_weight, np.ndarray):
-                sample_weight = self._validate_pandas_input(sample_weight)
-
+        sample_weight = validate_sample_weight(sample_weight)
         self.random_state = check_random_state(self.random_state)
 
         # setup variables for Boruta
         n_sample, n_feat = X.shape
         _iter = 1
         # holds the decision about each feature:
         # 0  - default state = tentative in original code
@@ -370,290 +454,60 @@
         imp_history = np.zeros(n_feat, dtype=float)
         sha_max_history = []
 
         # set n_estimators
         if self.n_estimators != "auto":
             self.estimator.set_params(n_estimators=self.n_estimators)
 
-        # main feature selection loop
-        pbar = tqdm(total=self.max_iter, desc="Leshy iteration")
-        while np.any(dec_reg == 0) and _iter < self.max_iter:
-            # find optimal number of trees and depth
-            if self.n_estimators == "auto":
-                # number of features that aren't rejected
-                not_rejected = np.where(dec_reg >= 0)[0].shape[0]
-                n_tree = self._get_tree_num(not_rejected)
-                self.estimator.set_params(n_estimators=n_tree)
-
-            # make sure we start with a new tree in each iteration
-            # Catboost doesn't allow to change random seed after fitting
-            if self.is_cat is False:
-                if self.is_lgb:
-                    self.estimator.set_params(
-                        random_state=self.random_state.randint(0, 10000)
-                    )
-                else:
-                    self.estimator.set_params(random_state=self.random_state)
-
-            # add shadow attributes, shuffle them and train estimator, get imps
-            cur_imp = self._add_shadows_get_imps(X, y, sample_weight, dec_reg)
-
-            # get the threshold of shadow importances we will use for rejection
-            imp_sha_max = np.percentile(cur_imp[1], self.perc)
-
-            # record importance history
-            sha_max_history.append(imp_sha_max)
-            imp_history = np.vstack((imp_history, cur_imp[0]))
-
-            # register which feature is more imp than the max of shadows
-            hit_reg = self._assign_hits(hit_reg, cur_imp, imp_sha_max)
-
-            # based on hit_reg we check if a feature is doing better than
-            # expected by chance
-            dec_reg = self._do_tests(dec_reg, hit_reg, _iter)
-
-            # print out confirmed features
-            # if self.verbose > 0 and _iter < self.max_iter:
-            #     self._print_results(dec_reg, _iter, 0)
-            if _iter < self.max_iter:
-                _iter += 1
-                pbar.update(1)
-        pbar.close()
-        # we automatically apply R package's rough fix for tentative ones
-        confirmed = np.where(dec_reg == 1)[0]
-        tentative = np.where(dec_reg == 0)[0]
-        # ignore the first row of zeros
-        tentative_median = np.median(imp_history[1:, tentative], axis=0)
-        # which tentative to keep
-        tentative_confirmed = np.where(tentative_median > np.median(sha_max_history))[0]
-        tentative = tentative[tentative_confirmed]
-
-        # basic result variables
-        self.n_features_ = confirmed.shape[0]
-        self.support_ = np.zeros(n_feat, dtype=bool)
-        self.support_weak_ = np.zeros(n_feat, dtype=bool)
-        self.support_[confirmed] = 1
-        self.support_weak_ = np.zeros(n_feat, dtype=bool)
-        self.support_weak_[tentative] = 1
-        if self.keep_weak:
-            self.support_[tentative] = 1
+        dec_reg, sha_max_history, imp_history, imp_sha_max = self.select_features(
+            X=X, y=y, sample_weight=sample_weight
+        )
+        confirmed, tentative = _get_confirmed_and_tentative(dec_reg)
+        tentative = _select_tentative(tentative, imp_history, sha_max_history)
+        self._calculate_support(confirmed, tentative, n_feat)
 
         # for plotting
         self.imp_real_hist = imp_history
         self.sha_max = imp_sha_max
 
-        if isinstance(X_raw, np.ndarray):
-            X_raw = pd.DataFrame(X_raw)
-
-        # absolute ranking
-        vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
-        self.ranking_absolutes_ = list(
-            vimp_df.mean().sort_values(ascending=False).index
-        )
-
-        # ranking, confirmed variables are rank 1
-        self.ranking_ = np.ones(n_feat, dtype=int)
-        # tentative variables are rank 2
-        self.ranking_[tentative] = 2
-        # selected = confirmed and tentative
-        selected = np.hstack((confirmed, tentative))
-        # all rejected features are sorted by importance history
-        not_selected = np.setdiff1d(np.arange(n_feat), selected)
-        # large importance values should rank higher = lower ranks -> *(-1)
-        imp_history_rejected = imp_history[1:, not_selected] * -1
-
-        # update rank for not_selected features
-        if not_selected.shape[0] > 0:
-            # calculate ranks in each iteration, then median of ranks across feats
-            iter_ranks = self._nanrankdata(imp_history_rejected, axis=1)
-            rank_medians = np.nanmedian(iter_ranks, axis=0)
-            ranks = self._nanrankdata(rank_medians, axis=0)
-
-            # set smallest rank to 3 if there are tentative feats
-            if tentative.shape[0] > 0:
-                ranks = ranks - np.min(ranks) + 3
-            else:
-                # and 2 otherwise
-                ranks = ranks - np.min(ranks) + 2
-            self.ranking_[not_selected] = ranks
-        else:
-            # all are selected, thus we set feature supports to True
-            self.support_ = np.ones(n_feat, dtype=bool)
-
-        # notify user
-        if self.verbose > 0:
-            self._print_results(dec_reg, _iter, 1)
-        self.running_time = time.time() - start_time
-        hours, rem = divmod(self.running_time, 3600)
-        minutes, seconds = divmod(rem, 60)
-        print(
-            "All relevant predictors selected in {:0>2}:{:0>2}:{:05.2f}".format(
-                int(hours), int(minutes), seconds
-            )
+        # absolute and relative ranking
+        self._calculate_absolute_ranking()
+        self._calculate_relative_ranking(
+            n_feat=n_feat,
+            tentative=tentative,
+            confirmed=confirmed,
+            imp_history=imp_history,
         )
+        self._print_result(dec_reg, _iter, start_time)
         return self
 
-    def plot_importance(self, n_feat_per_inch=5):
-        """Boxplot of the variable importance, ordered by magnitude
-        The max shadow variable importance illustrated by the dashed line.
-        Requires to apply the fit method first.
-
-        Parameters
-        ----------
-        n_feat_per_inch : int, default=5
-            number of features to plot per inch (for scaling the figure)
-
-        Returns
-        -------
-        fig : plt.figure
-            the matplotlib figure object containing the boxplot
-        """
-        # plt.style.use('fivethirtyeight')
-        my_colors_list = [
-            "#000000",
-            "#7F3C8D",
-            "#11A579",
-            "#3969AC",
-            "#F2B701",
-            "#E73F74",
-            "#80BA5A",
-            "#E68310",
-            "#008695",
-            "#CF1C90",
-            "#F97B72",
-        ]
-        bckgnd_color = "#f5f5f5"
-        params = {
-            "axes.prop_cycle": plt.cycler(color=my_colors_list),
-            "axes.facecolor": bckgnd_color,
-            "patch.edgecolor": bckgnd_color,
-            "figure.facecolor": bckgnd_color,
-            "axes.edgecolor": bckgnd_color,
-            "savefig.edgecolor": bckgnd_color,
-            "savefig.facecolor": bckgnd_color,
-            "grid.color": "#d2d2d2",
-            "lines.linewidth": 1.5,
-        }  # plt.cycler(color=my_colors_list)
-        mpl.rcParams.update(params)
-
-        if self.imp_real_hist is None:
-            raise ValueError("Use the fit method first to compute the var.imp")
-
-        color = {
-            "boxes": "gray",
-            "whiskers": "gray",
-            "medians": "#000000",
-            "caps": "gray",
-        }
-        vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
-        vimp_df = vimp_df.reindex(
-            vimp_df.mean().sort_values(ascending=True).index, axis=1
-        )
-
-        if vimp_df.dropna().empty:
-            warnings.warn("No feature selected - No data to plot")
-            return None
-        else:
-            bp = vimp_df.boxplot(
-                color=color,
-                boxprops=dict(linestyle="-", linewidth=1.5),
-                flierprops=dict(linestyle="-", linewidth=1.5),
-                medianprops=dict(linestyle="-", linewidth=1.5, color="#000000"),
-                whiskerprops=dict(linestyle="-", linewidth=1.5),
-                capprops=dict(linestyle="-", linewidth=1.5),
-                showfliers=False,
-                grid=True,
-                rot=0,
-                vert=False,
-                patch_artist=True,
-                figsize=(16, vimp_df.shape[1] / n_feat_per_inch),
-                fontsize=9,
-            )
-            blue_color = "#2590fa"
-            yellow_color = "#f0be00"
-
-            n_strong = sum(self.support_)
-            n_weak = np.sum(self.support_weak_)
-            n_discarded = np.sum(~(self.support_ | self.support_weak_))
-            box_face_col = (
-                [blue_color] * n_strong
-                + [yellow_color] * n_weak
-                + ["gray"] * n_discarded
-            )
-            for c in range(len(box_face_col)):
-                bp.findobj(mpl.patches.Patch)[len(self.support_) - c - 1].set_facecolor(
-                    box_face_col[c]
-                )
-                bp.findobj(mpl.patches.Patch)[len(self.support_) - c - 1].set_color(
-                    box_face_col[c]
-                )
-
-            xrange = vimp_df.max(skipna=True).max(skipna=True) - vimp_df.min(
-                skipna=True
-            ).min(skipna=True)
-            bp.set_xlim(left=vimp_df.min(skipna=True).min(skipna=True) - 0.10 * xrange)
-
-            custom_lines = [
-                Line2D([0], [0], color=blue_color, lw=5),
-                Line2D([0], [0], color=yellow_color, lw=5),
-                Line2D([0], [0], color="gray", lw=5),
-                Line2D([0], [0], linestyle="--", color="gray", lw=2),
-            ]
-            bp.legend(
-                custom_lines,
-                ["confirmed", "tentative", "rejected", "sha. max"],
-                loc="lower right",
-            )
-            plt.axvline(x=self.sha_max, linestyle="--", color="gray")
-            fig = bp.get_figure()
-            plt.title("Leshy importance and selected predictors")
-            # fig.set_size_inches((10, 1.5 * np.rint(max(vimp_df.shape) / 10)))
-            # plt.tight_layout()
-            # plt.show()
-            return fig
-
     def _get_tree_num(self, n_feat):
         """private method, get a good estimated for the number of trees
            given the number of features
 
         Parameters
         ----------
         n_feat : int
             The number of features
 
         Returns
         -------
         n_estimators : int
             the number of trees
         """
-        depth = self.estimator.get_params()["max_depth"]
+        depth = self.estimator.get_params()["max_depth"] if not self.is_cat else self.estimator.get_param("max_depth")
         if depth is None:
             depth = 10
         # how many times a feature should be considered on average
         f_repr = 100
         # n_feat * 2 because the training matrix is extended with n shadow features
         multi = (n_feat * 2) / (np.sqrt(n_feat * 2) * depth)
         n_estimators = int(multi * f_repr)
         return n_estimators
 
-    def _get_shuffle(self, seq):
-        """private method, shuffle a sequence
-
-        Parameters
-        ----------
-        seq : np.array
-            the sequence to shuffle
-        Returns
-        -------
-        seq : np.array
-            the shufled sequence
-        """
-        self.random_state.shuffle(seq)
-        return seq
-
     def _add_shadows_get_imps(self, X, y, sample_weight, dec_reg):
         """Add a shuffled copy of the columns (shadows) and get the feature
         importance of the augmented data set
 
         Parameters
         ----------
         X: pd.DataFrame of shape [n_samples, n_features]
@@ -669,34 +523,37 @@
          imp_real: array
             feature importance of the real predictors
          imp_sha: array
             feature importance of the shadow predictors
         """
         # find features that are tentative still
         x_cur_ind = np.where(dec_reg >= 0)[0]
-        x_cur = np.copy(X[:, x_cur_ind])
+        x_cur = X.iloc[:, x_cur_ind].copy()
         x_cur_w = x_cur.shape[1]
         # deep copy the matrix for the shadow matrix
-        x_sha = np.copy(x_cur)
+        x_sha = x_cur.copy()
         # make sure there's at least 5 columns in the shadow matrix for
         while x_sha.shape[1] < 5:
-            x_sha = np.hstack((x_sha, x_sha))
+            x_sha = pd.concat([x_sha, x_sha], axis=1)
         # shuffle xSha
-        x_sha = np.apply_along_axis(self._get_shuffle, 0, x_sha)
+        x_sha = x_sha.apply(self.random_state.permutation, axis=0)
+        x_sha.columns = [f"Shadow_{i}" for i in range(x_sha.shape[1])]
         # get importance of the merged matrix
         if self.importance == "shap":
             imp = _get_shap_imp(
-                self.estimator, np.hstack((x_cur, x_sha)), y, sample_weight
+                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
             )
         elif self.importance == "pimp":
             imp = _get_perm_imp(
-                self.estimator, np.hstack((x_cur, x_sha)), y, sample_weight
+                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
             )
         else:
-            imp = _get_imp(self.estimator, np.hstack((x_cur, x_sha)), y, sample_weight)
+            imp = _get_imp(
+                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
+            )
 
         # separate importances of real and shadow features
         imp_sha = imp[x_cur_w:]
         imp_real = np.zeros(X.shape[1])
         imp_real[:] = np.nan
         imp_real[x_cur_ind] = imp[:x_cur_w]
 
@@ -911,14 +768,355 @@
             else:
                 vimp = "native"
             output = (
                 "\n\nLeshy finished running using " + vimp + " var. imp.\n\n" + result
             )
         print(output)
 
+    def _update_estimator(self):
+        """
+        Update the estimator with a new random state, if applicable.
+
+        If the dataset is not categorical, the estimator's `random_state` parameter is updated
+        with a new random state generated by the `random_state` attribute of the Leshy object.
+        If the estimator is a LightGBM model, the random state value is generated between 0 and 10000.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
+        if self.is_cat is False:
+            if self.is_lgb:
+                self.estimator.set_params(
+                    random_state=self.random_state.randint(0, 10000)
+                )
+            else:
+                self.estimator.set_params(random_state=self.random_state)
+
+    def _update_tree_num(self, dec_reg):
+        """Update the number of trees in the estimator based on the number of selected features.
+
+        Parameters
+        ----------
+        dec_reg : array-like of shape (n_features,)
+            The decision rule for each feature, where negative values indicate that the feature should be rejected
+            and non-negative values indicate that the feature should be selected.
+
+        Returns
+        -------
+        None
+
+        Notes
+        -----
+        This function updates the `n_estimators` parameter of the estimator if it is set to "auto". The number of trees is
+        determined based on the number of selected features. Specifically, the number of trees is set to the value returned
+        by the `_get_tree_num` method, which takes as input the number of selected features that are not rejected.
+
+        If `n_estimators` is not set to "auto", this function does nothing.
+        """
+        if self.n_estimators == "auto":
+            # number of features that aren't rejected
+            not_rejected = np.where(dec_reg >= 0)[0].shape[0]
+            n_tree = self._get_tree_num(not_rejected)
+            self.estimator.set_params(n_estimators=n_tree)
+
+    def _run_iteration(
+        self, X, y, sample_weight, dec_reg, sha_max_history, imp_history, hit_reg, _iter
+    ):
+        """
+        Run an iteration of the Gradient Boosting algorithm.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input samples.
+
+        y : array-like of shape (n_samples,)
+            The target values.
+
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights. If None, then samples are equally weighted.
+
+        dec_reg : array-like of shape (n_samples,)
+            Decision function of the estimator.
+
+        sha_max_history : list of floats
+            List of the maximum shadow importance value at each iteration.
+
+        imp_history : array-like of shape (n_iterations, n_features)
+            Matrix of feature importances at each iteration.
+
+        hit_reg : array-like of shape (n_samples,)
+            Array of hit counts for each sample.
+
+        _iter : int
+            The current iteration number.
+
+        Returns
+        -------
+        dec_reg : array-like of shape (n_samples,)
+            Updated decision function of the estimator.
+
+        sha_max_history : list of floats
+            List of the maximum shadow importance value at each iteration.
+
+        imp_history : array-like of shape (n_iterations, n_features)
+            Matrix of feature importances at each iteration.
+
+        hit_reg : array-like of shape (n_samples,)
+            Array of hit counts for each sample.
+
+        imp_sha_max : float
+            The maximum shadow importance value for this iteration.
+        """
+        cur_imp = self._add_shadows_get_imps(X, y, sample_weight, dec_reg)
+        imp_sha_max = np.percentile(cur_imp[1], self.perc)
+        sha_max_history.append(imp_sha_max)
+        imp_history = np.vstack((imp_history, cur_imp[0]))
+        hit_reg = self._assign_hits(hit_reg, cur_imp, imp_sha_max)
+        dec_reg = self._do_tests(dec_reg, hit_reg, _iter)
+        return dec_reg, sha_max_history, imp_history, hit_reg, imp_sha_max
+
+    def select_features(self, X, y, sample_weight=None):
+        """
+        Select features using the Leshy algorithm.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input data.
+        y : array-like of shape (n_samples,)
+            The target values.
+        sample_weight : array-like of shape (n_samples,), default=None
+            Individual weights for each sample.
+
+        Returns
+        -------
+        dec_reg : ndarray of shape (n_features,)
+            The decision rule. 1 means the feature is selected, 0 means the feature is not selected.
+        sha_max_history : list
+            List of the maximum shadow importances per iteration.
+        imp_history : ndarray of shape (n_iterations, n_features)
+            Array containing the feature importances per iteration.
+        imp_sha_max : float
+            Maximum shadow importance value.
+        """
+        pbar = tqdm(total=self.max_iter, desc="Leshy iteration")
+        dec_reg = np.zeros(X.shape[1])
+        hit_reg = np.zeros(X.shape[1])
+        sha_max_history = []
+        imp_history = np.empty((0, X.shape[1]))
+
+        for _iter in range(1, self.max_iter):
+            if not np.any(dec_reg == 0):
+                break
+            self._update_tree_num(dec_reg)
+            self._update_estimator()
+            (
+                dec_reg,
+                sha_max_history,
+                imp_history,
+                hit_reg,
+                imp_sha_max,
+            ) = self._run_iteration(
+                X,
+                y,
+                sample_weight,
+                dec_reg,
+                sha_max_history,
+                imp_history,
+                hit_reg,
+                _iter,
+            )
+            _iter += 1
+            pbar.update(1)
+
+        pbar.close()
+        return dec_reg, sha_max_history, imp_history, imp_sha_max
+
+    def _calculate_support(self, confirmed, tentative, n_feat):
+        """Calculates the feature support arrays for the BorutaPy feature selection algorithm.
+
+        Parameters
+        ----------
+        confirmed : array-like of shape (n_features,)
+            Indices of confirmed features.
+
+        tentative : array-like of shape (n_features,)
+            Indices of tentative features.
+
+        n_feat : int
+            Number of features in the dataset.
+
+        Returns
+        -------
+        None
+            The function only sets the following class attributes:
+
+            n_features_ : int
+                Number of confirmed features.
+
+            support_ : ndarray of bool, shape (n_features,)
+                Boolean array representing the confirmed features.
+
+            support_weak_ : ndarray of bool, shape (n_features,)
+                Boolean array representing the tentative features.
+
+        Notes
+        -----
+        - The function modifies the following class attributes:
+            * self.n_features_
+            * self.support_
+            * self.support_weak_
+        - If self.keep_weak is True, the support_weak_ is also added to the support_.
+        """
+        # basic result variables
+        self.n_features_ = confirmed.shape[0]
+        self.support_ = np.zeros(n_feat, dtype=bool)
+        self.support_weak_ = np.zeros(n_feat, dtype=bool)
+        self.support_[confirmed] = 1
+        self.support_weak_ = np.zeros(n_feat, dtype=bool)
+        self.support_weak_[tentative] = 1
+        if self.keep_weak:
+            self.support_[tentative] = 1
+
+    def _calculate_absolute_ranking(self):
+        """
+        Calculates the absolute ranking of the features based on their mean importance.
+
+        Returns:
+        -------
+        None
+            The function updates the `ranking_absolutes_` attribute of the instance with the absolute ranking.
+        """
+        vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
+        self.ranking_absolutes_ = list(
+            vimp_df.mean().sort_values(ascending=False).index
+        )
+
+    def _calculate_relative_ranking(self, n_feat, tentative, confirmed, imp_history):
+        """
+        Calculates the relative ranking of features based on their importance history.
+
+        Parameters
+        ----------
+        n_feat : int
+            The total number of features.
+        tentative : ndarray of shape (n_tentative_features,)
+            An array containing the indices of tentative features.
+        confirmed : ndarray of shape (n_confirmed_features,)
+            An array containing the indices of confirmed features.
+        imp_history : ndarray of shape (n_iterations + 1, n_features)
+            An array containing the feature importances for each iteration.
+
+        Returns
+        -------
+        None
+
+        """
+        # ranking, confirmed variables are rank 1
+        self.ranking_ = np.ones(n_feat, dtype=int)
+        # tentative variables are rank 2
+        self.ranking_[tentative] = 2
+        selected = np.hstack((confirmed, tentative))
+        # all rejected features are sorted by importance history
+        not_selected = np.setdiff1d(np.arange(n_feat), selected)
+        # large importance values should rank higher = lower ranks -> *(-1)
+        imp_history_rejected = imp_history[1:, not_selected] * -1
+
+        # update rank for not_selected features
+        if not_selected.shape[0] > 0:
+            # calculate ranks in each iteration, then median of ranks across feats
+            iter_ranks = self._nanrankdata(imp_history_rejected, axis=1)
+            rank_medians = np.nanmedian(iter_ranks, axis=0)
+            ranks = self._nanrankdata(rank_medians, axis=0)
+
+            # set smallest rank to 3 if there are tentative feats
+            if tentative.shape[0] > 0:
+                ranks = ranks - np.min(ranks) + 3
+            else:
+                # and 2 otherwise
+                ranks = ranks - np.min(ranks) + 2
+            self.ranking_[not_selected] = ranks
+        else:
+            # all are selected, thus we set feature supports to True
+            self.support_ = np.ones(n_feat, dtype=bool)
+
+    def _print_result(self, dec_reg, _iter, start_time):
+        """
+        Calculate the feature support arrays.
+
+        Parameters
+        ----------
+        confirmed : array-like of shape (n_confirmed,)
+            Indices of confirmed features.
+        tentative : array-like of shape (n_tentative,)
+            Indices of tentative features.
+        n_feat : int
+            Total number of features.
+
+        Returns
+        -------
+        None
+            The function populates the following class attributes:
+            - n_features_ : int
+                Number of selected features.
+            - support_ : ndarray of shape (n_feat,)
+                Boolean array indicating the selected features.
+            - support_weak_ : ndarray of shape (n_feat,)
+                Boolean array indicating the tentatively selected features.
+        """
+        if self.verbose > 0:
+            self._print_results(dec_reg, _iter, 1)
+        self.running_time = time.time() - start_time
+        hours, rem = divmod(self.running_time, 3600)
+        minutes, seconds = divmod(rem, 60)
+        print(
+            "All relevant predictors selected in {:0>2}:{:0>2}:{:05.2f}".format(
+                int(hours), int(minutes), seconds
+            )
+        )
+
+
+def _get_confirmed_and_tentative(dec_reg):
+    """Extracts the confirmed and tentative features from dec_reg."""
+    confirmed = np.where(dec_reg == 1)[0]
+    tentative = np.where(dec_reg == 0)[0]
+    return confirmed, tentative
+
+
+def _select_tentative(tentative, imp_history, sha_max_history):
+    """
+    Select tentative features based on median importance values.
+
+    Parameters
+    ----------
+    tentative: array-like of shape (n_tentative,)
+        Array of indices representing tentative features.
+    imp_history: array-like of shape (n_iterations + 1, n_features)
+        Importance values for each feature in each iteration.
+    sha_max_history: array-like of shape (n_iterations + 1,)
+        The history of the highest stability scores.
+
+    Returns
+    -------
+    tentative: array-like of shape (n_tentative_confirmed,)
+        The confirmed tentative features based on their median importance values.
+    """
+    # ignore the first row of zeros
+    tentative_median = np.median(imp_history[1:, tentative], axis=0)
+    # which tentative to keep
+    tentative_confirmed = np.where(tentative_median > np.median(sha_max_history))[0]
+    tentative = tentative[tentative_confirmed]
+    return tentative
+
 
 def _split_fit_estimator(estimator, X, y, sample_weight=None, cat_feature=None):
     """Private function, split the train, test and fit the model
 
     Parameters
     ----------
     estimator : estimator object implementing 'fit' and 'predict'
@@ -939,15 +1137,14 @@
      X_tt : array [n_samples, n_features]
         the test split, predictors
      y_tt : array [n_samples]
         the test split, target
     """
     if cat_feature is None:
         # detect, store and encode categorical predictors
-        X = pd.DataFrame(X)
         X, _, cat_idx = get_pandas_cat_codes(X)
     else:
         cat_idx = cat_feature
 
     if sample_weight is not None:
         w = sample_weight
         if is_regressor(estimator):
@@ -961,17 +1158,14 @@
     else:
         if is_regressor(estimator):
             X_tr, X_tt, y_tr, y_tt = train_test_split(X, y, random_state=42)
         else:
             X_tr, X_tt, y_tr, y_tt = train_test_split(X, y, stratify=y, random_state=42)
         w_tr, w_tt = None, None
 
-    X_tr = pd.DataFrame(X_tr)
-    X_tt = pd.DataFrame(X_tt)
-
     if check_if_tree_based(estimator):
         try:
             # handle cat features if supported by the fit method
             if is_catboost(estimator) or (
                 "cat_feature" in estimator.fit.__code__.co_varnames
             ):
                 model = estimator.fit(
@@ -988,71 +1182,71 @@
     else:
         raise ValueError("Not a tree based model")
 
     return model, X_tt, y_tt, w_tt
 
 
 def _get_shap_imp(estimator, X, y, sample_weight=None, cat_feature=None):
-    """Private function, Get the SHAP feature importance
+    """Get the SHAP feature importance
 
     Parameters
     ----------
-    estimator: sklearn estimator
+    estimator : estimator object
+        An estimator object implementing `fit` and `predict` methods.
     X : pd.DataFrame of shape [n_samples, n_features]
-        predictor matrix
-    y : pd.series of shape [n_samples]
-        target
+        Predictor matrix.
+    y : pd.Series of shape [n_samples]
+        Target variable.
     sample_weight : array-like, shape = [n_samples], default=None
-        Individual weights for each sample
-    cat_feature : list of int or None
-        the list of integers, cols loc, of the categorical predictors. Avoids to detect and encode
+        Individual weights for each sample.
+    cat_feature : list of int or None, default=None
+        The list of integers, columns loc, of the categorical predictors. Avoids detecting and encoding
         each iteration if the exact same columns are passed to the selection methods.
+
     Returns
     -------
     shap_imp : array
-        the SHAP importance array
+        The SHAP importance array.
     """
-
-    # be sure to use an non-fitted estimator
+    # Clone the estimator to avoid modifying the original one
     estimator = clone(estimator)
 
+    # Split the data into train and test sets and fit the model
     model, X_tt, y_tt, w_tt = _split_fit_estimator(
         estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
     )
 
-    # Faster and safer to use the builtin lightGBM method
-    # Note the xgboost and catboost have builtin shap as well
-    # but it requires to use DMatrix or Pool respectively
-    # for other tree-based models, no builtin SHAP
+    # Compute the SHAP values
     if is_lightgbm(estimator):
+        # For LightGBM models use the built-in SHAP method
         shap_matrix = model.predict(X_tt, pred_contrib=True)
-        # the dim changed in lightGBM 3
-        # X_SHAP_values array-like of shape = [n_samples, n_features + 1] for regression and binay classification and
-        # shape = [n_samples, (n_features + 1) * n_classes] or list with n_classes length of such objects
+
+        # The shape of the shap_matrix depends on whether the estimator is a classifier or a regressor
         if is_classifier(estimator) and (len(np.unique(y_tt)) > 2):
-            # remove every (n_features+1)th element, python indexes from zero
+            # For multi-class classifiers, reshape the shap_matrix
             n_features = X_tt.shape[1]
             shap_matrix = np.delete(
                 shap_matrix,
                 list(range(n_features, shap_matrix.shape[1], n_features + 1)),
                 axis=1,
             )
             shap_imp = np.mean(np.abs(shap_matrix), axis=0)
         else:
             shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
     else:
-        # build the explainer
+        # For other tree-based models, use the shap.TreeExplainer method to compute SHAP values
         explainer = shap.TreeExplainer(
             model, feature_perturbation="tree_path_dependent"
         )
         shap_values = explainer.shap_values(X_tt)
-        # flatten to 2D if classification and lightgbm
+
+        # For multi-class classifiers, reshape the shap_values
         if is_classifier(estimator):
             if isinstance(shap_values, list):
-                # for lightgbm clf sklearn api, shap returns list of arrays
+                # For LightGBM classifier in sklearn API, SHAP returns a list of arrays
                 # https://github.com/slundberg/shap/issues/526
                 class_inds = range(len(shap_values))
                 shap_imp = np.zeros(shap_values[0].shape[1])
                 for i, ind in enumerate(class_inds):
                     shap_imp += np.abs(shap_values[ind]).mean(0)
                 shap_imp /= len(shap_values)
             else:
@@ -1126,22 +1320,19 @@
     imp : array
         the permutation importance array
     """
     # be sure to use an non-fitted estimator
     estimator = clone(estimator)
 
     try:
-        # handle categoricals
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-
         if cat_feature is None:
             X, _, cat_idx = get_pandas_cat_codes(X)
         else:
             cat_idx = cat_feature
+        
 
         # handle catboost and cat features
         if is_catboost(estimator) or (
             "cat_feature" in estimator.fit.__code__.co_varnames
         ):
             X = pd.DataFrame(X)
             estimator.fit(X, y, sample_weight=sample_weight, cat_features=cat_idx)
@@ -1175,18 +1366,17 @@
     information usable for prediction, rather than finding a possibly compact
     subset of features on which some estimator has a minimal error.
     Why bother with all relevant feature selection?
     When you try to understand the phenomenon that made your data, you should
     care about all factors that contribute to it, not just the bluntest signs
     of it in context of your methodology (minimal optimal set of features
     by definition depends on your estimator choice).
-
     Parameters
     ----------
-    est : sklear estimator
+    estimator : sklear estimator
         the model to train, lightGBM recommended, see the reduce lightgbm method
     cutoff : float
         the value by which the max of shadow imp is divided, to compare to real importance
     iters : int (>0)
         The number of iterations to average for the feature importance (on the same split),
         to reduce the variance
     max_rounds : int (>0)
@@ -1195,16 +1385,14 @@
     delta : float (0 < delta <= 1)
         Stopping criteria for whether another round is started
     silent : bool
         Set to True if don't want to see the BoostARoota output printed.
     importance : str, default='shap'
         the kind of feature importance to use. Possible values: 'shap' (Shapley values),
         'pimp' (permutation importance) and 'native' (Gini/impurity)
-
-
     Attributes
     ----------
     selected_features_ : list of str
         the list of columns to keep
     ranking_ : array of shape [n_features]
         The feature ranking, such that ``ranking_[i]`` corresponds to the
         ranking position of the i-th feature. Selected (i.e., estimated
@@ -1214,42 +1402,39 @@
         The absolute feature ranking as ordered by selection process. It does not guarantee
         that this order is correct for all models. For a model agnostic ranking, see the
         the attribute ``ranking``
     sha_cutoff_df : dataframe
         feature importance of the real+shadow predictors over iterations
     mean_shadow : float
         the threshold below which the predictors are rejected
-
-
     Examples
     --------
     >>> X = df[filtered_features].copy()
     >>> y = df['target'].copy()
     >>> w = df['weight'].copy()
     >>>
     >>> model = LGBMRegressor(n_jobs=-1, n_estimators=100, objective='rmse',
     >>>                       random_state=42, verbose=0)
     >>> feat_selector = BoostAGroota(est=model, cutoff=1, iters=10, max_rounds=10, delta=0.1, importance='shap')
     >>> feat_selector.fit(X, y, sample_weight=None)
     >>> print(feat_selector.selected_features_)
     >>> feat_selector.plot_importance(n_feat_per_inch=5)
-
     """
 
     def __init__(
         self,
-        est=None,
+        estimator=None,
         cutoff=4,
         iters=10,
         max_rounds=500,
         delta=0.1,
         silent=True,
         importance="shap",
     ):
-        self.est = est
+        self.estimator = estimator
         self.cutoff = cutoff
         self.iters = iters
         self.max_rounds = max_rounds
         self.delta = delta
         self.silent = silent
         self.importance = importance
         self.sha_cutoff_df = None
@@ -1287,74 +1472,68 @@
             "BoostARoota(est={est}, \n"
             "                cutoff={cutoff},\n"
             "                iters={iters},\n"
             "                max_rounds={mr},\n"
             "                delta={delta},\n"
             "                silent={silent}, \n"
             '                importance="{importance}")'.format(
-                est=self.est,
+                estimator=self.estimator,
                 cutoff=self.cutoff,
                 iters=self.iters,
                 mr=self.max_rounds,
                 delta=self.delta,
                 silent=self.silent,
                 importance=self.importance,
             )
         )
         return s
 
     def fit(self, X, y, sample_weight=None):
         """Fit the BoostAGroota transformer with the provided estimator.
-
         Parameters
         ----------
         X : pd.DataFrame
             the predictors matrix
         y : pd.Series
             the target
         sample_weight : pd.series
             sample_weight, if any
-
         """
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
         else:
             raise TypeError("X is not a dataframe")
 
         if sample_weight is not None:
             sample_weight = _check_sample_weight(sample_weight, X)
 
         # crit, keep_vars, df_vimp, mean_shadow
-        _, self.selected_features_, self.sha_cutoff_df, self.mean_shadow = _BoostARoota(
+        _, self.selected_features_, self.sha_cutoff_df, self.mean_shadow = _boostaroota(
             X,
             y,
             # metric=self.metric,
-            est=self.est,
+            estimator=self.estimator,
             cutoff=self.cutoff,
             iters=self.iters,
             max_rounds=self.max_rounds,
             delta=self.delta,
             silent=self.silent,
             weight=sample_weight,
             imp=self.importance,
         )
         self.selected_features_ = self.selected_features_.values
         self.support_ = np.asarray(
-            [
-                True if c in self.selected_features_ else False
-                for c in self.feature_names_in_
-            ]
+            [c in self.selected_features_ for c in self.feature_names_in_]
         )
-
-        b_df = self.sha_cutoff_df
-        real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
         self.ranking_absolutes_ = list(
-            real_df.mean().sort_values(ascending=False).index
+            self.sha_cutoff_df.iloc[:, : int(self.sha_cutoff_df.shape[1] / 2)]
+            .mean()
+            .sort_values(ascending=False)
+            .index
         )
-
         self.ranking_ = np.where(self.support_, 2, 1)
         return self
 
     def _get_support_mask(self):
         check_is_fitted(self)
 
         return self.support_
@@ -1363,149 +1542,92 @@
         if not isinstance(X, pd.DataFrame):
             raise TypeError("X is not a dataframe")
         return X[self.selected_features_]
 
     def _more_tags(self):
         return {"allow_nan": True, "requires_y": True}
 
+    @mpl.rc_context(PLT_PARAMS)
     def plot_importance(self, n_feat_per_inch=5):
-        """Boxplot of the variable importance, ordered by magnitude
+        """
+        Boxplot of the variable importance, ordered by magnitude.
         The max shadow variable importance illustrated by the dashed line.
         Requires to apply the fit method first.
 
         Parameters
         ----------
         n_feat_per_inch : int, default=5
-            number of features to plot per inch (for scaling the figure)
+            Number of features to plot per inch (for scaling the figure).
 
         Returns
         -------
-        fig : plt.figure
-            the matplotlib figure object containing the boxplot
+        fig : plt.figure or None
+            The matplotlib figure object containing the boxplot, or None if there are no selected features.
         """
-        # plt.style.use('fivethirtyeight')
-        my_colors_list = [
-            "#000000",
-            "#7F3C8D",
-            "#11A579",
-            "#3969AC",
-            "#F2B701",
-            "#E73F74",
-            "#80BA5A",
-            "#E68310",
-            "#008695",
-            "#CF1C90",
-            "#F97B72",
-        ]
-        bckgnd_color = "#f5f5f5"
-        params = {
-            "axes.prop_cycle": plt.cycler(color=my_colors_list),
-            "axes.facecolor": bckgnd_color,
-            "patch.edgecolor": bckgnd_color,
-            "figure.facecolor": bckgnd_color,
-            "axes.edgecolor": bckgnd_color,
-            "savefig.edgecolor": bckgnd_color,
-            "savefig.facecolor": bckgnd_color,
-            "grid.color": "#d2d2d2",
-            "lines.linewidth": 1.5,
-        }  # plt.cycler(color=my_colors_list)
-        mpl.rcParams.update(params)
-
         if self.mean_shadow is None:
             raise ValueError("Apply fit method first")
 
-        # b_df = self.sha_cutoff_df.T.copy()
-        # b_df.columns = b_df.iloc[0]
-        # b_df = b_df.drop(b_df.index[0])
-        # b_df = b_df.drop(b_df.index[-1])
         b_df = self.sha_cutoff_df
         real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
-        blue_color = "#2590fa"
-        color = {
-            "boxes": "gray",
-            "whiskers": "gray",
-            "medians": "#000000",
-            "caps": "gray",
-        }
+
         real_df = real_df.reindex(
             real_df.mean().sort_values(ascending=True).index, axis=1
         )
 
         if real_df.dropna().empty:
-            warnings.warn("No feature selected - No data to plot")
+            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
             return None
-        else:
-            bp = real_df.plot.box(  # kind='box',
-                color=color,
-                boxprops=dict(
-                    linestyle="-", linewidth=1.5, color="gray", facecolor="gray"
-                ),
-                flierprops=dict(linestyle="-", linewidth=1.5),
-                medianprops=dict(linestyle="-", linewidth=1.5, color="#000000"),
-                whiskerprops=dict(linestyle="-", linewidth=1.5),
-                capprops=dict(linestyle="-", linewidth=1.5),
-                showfliers=False,
-                grid=True,
-                rot=0,
-                vert=False,
-                patch_artist=True,
-                figsize=(16, real_df.shape[1] / n_feat_per_inch),
-                fontsize=9,
-            )
-            # xrange = real_df.max(skipna=True).max(skipna=True)-real_df.min(skipna=True).min(skipna=True)
-            bp.set_xlim(left=real_df.min(skipna=True).min(skipna=True) - 0.025)
 
-            for c in range(len(self.selected_features_)):
-                bp.findobj(mpl.patches.Patch)[real_df.shape[1] - c - 1].set_facecolor(
-                    blue_color
-                )
-                bp.findobj(mpl.patches.Patch)[real_df.shape[1] - c - 1].set_color(
-                    blue_color
-                )
+        fig, ax = plt.subplots(figsize=(16, real_df.shape[1] / n_feat_per_inch))
+        bp = real_df.plot(**PLOT_KWARGS, ax=ax)
+        bp.set_xlim(left=real_df.min(skipna=True).min(skipna=True) - 0.025)
+
+        for c in range(len(self.selected_features_)):
+            patch = bp.findobj(mpl.patches.Patch)[real_df.shape[1] - c - 1]
+            patch.set_facecolor(BLUE)
+            patch.set_color(BLUE)
+
+        custom_lines = [
+            Line2D([0], [0], color=BLUE, lw=5),
+            Line2D([0], [0], color="gray", lw=5),
+            Line2D([0], [0], linestyle="--", color=RED, lw=2),
+        ]
+        bp.legend(
+            custom_lines, ["confirmed", "rejected", "sha. max"], loc="lower right"
+        )
 
-            custom_lines = [
-                Line2D([0], [0], color=blue_color, lw=5),
-                Line2D([0], [0], color="gray", lw=5),
-                Line2D([0], [0], linestyle="--", color="gray", lw=2),
-            ]
-            bp.legend(
-                custom_lines, ["confirmed", "rejected", "sha. max"], loc="lower right"
-            )
-            plt.axvline(x=self.mean_shadow, linestyle="--", color="gray")
+        ax.axvline(x=self.mean_shadow, linestyle="--", color=RED)
+        ax.set_title("BoostAGroota importance of selected predictors")
 
-            fig = bp.get_figure()
-            plt.title("BoostAGroota importance of selected predictors")
-            # plt.tight_layout()
-            # plt.show()
-            return fig
+        return fig
 
 
 ############################################
 # Helper Functions to do the Heavy Lifting
 ############################################
 
 
 def _create_shadow(X_train):
-    """Private function, Take all X variables, creating copies and randomly shuffling them
+    """Create shadow features by making copies of all X variables and randomly shuffling them.
 
     Parameters
     ----------
     X_train : pd.DataFrame
-        the dataframe to create shadow features on
+        The dataframe to create shadow features on.
 
     Returns
     -------
-    new_x : pd.DataFrame
-        dataframe 2x width and the names of the shadows for removing later
+    pd.DataFrame
+        A dataframe that is twice the width of X_train and contains the shadow features, along with a list of the shadow feature names.
     """
     X_shadow = X_train.copy()
     for c in X_shadow.columns:
         np.random.shuffle(X_shadow[c].values)
-    # rename the shadow
-    shadow_names = ["ShadowVar" + str(i + 1) for i in range(X_train.shape[1])]
+    # Rename the shadow variables
+    shadow_names = [f"ShadowVar{i+1}" for i in range(X_train.shape[1])]
     X_shadow.columns = shadow_names
     # Combine to make one new dataframe
     new_x = pd.concat([X_train, X_shadow], axis=1)
     return new_x, shadow_names
 
 
 ########################################################################################
@@ -1513,15 +1635,15 @@
 # the _ in front of the function name, they're internal functions)
 ########################################################################################
 
 
 def _reduce_vars_sklearn(
     X,
     y,
-    est,
+    estimator,
     this_round,
     cutoff,
     n_iterations,
     delta,
     silent,
     weight,
     imp_kind,
@@ -1531,15 +1653,15 @@
 
     Parameters
     ----------
     x : pd.DataFrame
         the dataframe to create shadow features on
     y : pd.Series
         the target
-    est : sklear estimator
+    estimator : sklearn estimator
         the model to train, lightGBM recommended
     this_round : int
         The number of times the core BoostARoota algorithm will run.
         Each round eliminates more and more features
     cutoff : float
         the value by which the max of shadow imp is divided, to compare to real importance
     n_iterations : int
@@ -1566,58 +1688,45 @@
         feature importance of the real predictors over iter
     df : pd.DataFrame
         feature importance of the real+shadow predictors over iter
     mean_shadow : float
         the feature importance threshold, to reject or not the predictors
 
     Raises
-    ------_reduce_vars_sklearn
+    ------
     ValueError
-        error if the feature importance type is not"""
+        error if the feature importance type is not
+    """
     # Set up the parameters for running the model in XGBoost - split is on multi log loss
-
     for i in range(1, n_iterations + 1):
         # Create the shadow variables and run the model to obtain importances
         new_x, shadow_names = _create_shadow(X)
-        if imp_kind == "shap":
-            imp = _get_shap_imp(
-                est, new_x, y, sample_weight=weight, cat_feature=cat_feature
-            )
-        elif imp_kind == "pimp":
-            imp = _get_perm_imp(
-                est, new_x, y, sample_weight=weight, cat_feature=cat_feature
-            )
-        elif imp_kind == "native":
-            imp = _get_imp(est, new_x, y, sample_weight=weight, cat_feature=cat_feature)
-        else:
-            raise ValueError(
-                "'imp' should be either 'native', 'shap' or 'pimp', "
-                "'native' is not recommended"
-            )
+        imp_func = {"shap": _get_shap_imp, "pimp": _get_perm_imp, "native": _get_imp}
+        importance = imp_func[imp_kind](
+            estimator, new_x, y, sample_weight=weight, cat_feature=cat_feature
+        )
 
+        # Create a dataframe to store the feature importances
         if i == 1:
             df = pd.DataFrame({"feature": new_x.columns})
             df2 = df.copy()
-            pass
+
+        # Store the feature importances in df2
         try:
-            importance = imp  # est.feature_importances_
-            df2["fscore" + str(i)] = importance
+            # Normalize the feature importances
+            df2["fscore" + str(i)] = importance / importance.sum()
         except ValueError:
-            print(
-                "this clf doesn't have the feature_importances_ method.  "
-                "Only Sklearn tree based methods allowed"
-            )
-
-        # importance = sorted(importance.items(), key=operator.itemgetter(1))
+            print("Only Sklearn tree based methods allowed")
 
-        # df2 = pd.DataFrame(importance, columns=['feature', 'fscore'+str(i)])
-        df2["fscore" + str(i)] = df2["fscore" + str(i)] / df2["fscore" + str(i)].sum()
+        # Merge the current feature importances with the existing ones in df
         df = pd.merge(
             df, df2, on="feature", how="outer", suffixes=("_x" + str(i), "_y" + str(i))
         )
+
+        # Print the iteration number if not silent
         if not silent:
             print("Round: ", this_round, " iteration: ", i)
 
     df["Mean"] = df.select_dtypes(include=[np.number]).mean(axis=1, skipna=True)
     # Split them back out
     real_vars = df.loc[~df["feature"].isin(shadow_names)]
     shadow_vars = df.loc[df["feature"].isin(shadow_names)]
@@ -1628,36 +1737,34 @@
         .max(skipna=True)
         .mean(skipna=True)
         / cutoff
     )
     real_vars = real_vars[(real_vars.Mean >= mean_shadow)]
 
     # Check for the stopping criteria
-    # Basically looking to make sure we are removing at least 10% of the variables, or we should stop
-    if len(X.columns) == 0 | len(real_vars["feature"]) == 0:
-        criteria = True
-    elif (len(real_vars["feature"]) / len(X.columns)) > (1 - delta):
-        criteria = True
-    else:
-        criteria = False
+    # Compute the fraction of features selected in this round
+    selected_frac = len(real_vars) / len(X.columns)
+
+    # Check if we should stop feature selection
+    # make sure we are removing at least delta % of the variables
+    criteria = len(X.columns) == 0 or selected_frac == 0 or selected_frac > 1 - delta
 
     return criteria, real_vars["feature"], df, mean_shadow
 
 
-# Main function exposed to run the algorithm
-def _BoostARoota(X, y, est, cutoff, iters, max_rounds, delta, silent, weight, imp):
+def _boostaroota(
+    X, y, estimator, cutoff, iters, max_rounds, delta, silent, weight, imp
+):
     """Private function, reduce the number of predictors using a sklearn estimator
-
     Parameters
-
     x : pd.DataFrame
         the dataframe to create shadow features on
     y : pd.Series
         the target
-    est : sklear estimator
+    estimator : sklear estimator
         the model to train, lightGBM recommended, see the reduce lightgbm method
     cutoff : float
         the value by which the max of shadow imp is divided, to compare to real importance
     iters : int (>0)
         The number of iterations to average for the feature importances (on the same split),
         to reduce the variance
     max_rounds : int (>0)
@@ -1666,83 +1773,73 @@
     delta : float (0 < delta <= 1)
         Stopping criteria for whether another round is started
     silent : bool
         Set to True if don't want to see the BoostARoota output printed.
         Will still show any errors or warnings that may occur
     weight : pd.series
         sample_weight, if any
-
     Returns
     -------
     crit : bool
         if the criteria has been reached or not
     keep_vars : pd.dataframe
         feature importance of the real predictors over iter
     df_vimp : pd.DataFrame
         feature importance of the real+shadow predictors over iter
     mean_shadow : float
         the feature importance threshold, to reject or not the predictors
     """
-    t_boostaroota = time.time()
+    start_time = time.time()
     new_x = X.copy()
 
     # extract the categorical names for the first time, store it for next iterations
     # In the below while loop this list will be update only once some of the predictors
     # are removed. This way the encoding is done only every predictors update and not
     # every iteration. The code will then be much faster since the encoding is done only once.
     new_x, obj_feat, cat_idx = get_pandas_cat_codes(X)
 
     # Run through loop until "crit" changes
     i = 0
-    pbar = tqdm(total=max_rounds, desc="BoostaGRoota round")
     imp_dic = {}
-    while True:
-        # Inside this loop we reduce the dataset on each iteration exiting with keep_vars
-        i += 1
-        crit, keep_vars, df_vimp, mean_shadow = _reduce_vars_sklearn(
-            new_x,
-            y,
-            est=est,
-            this_round=i,
-            cutoff=cutoff,
-            n_iterations=iters,
-            delta=delta,
-            silent=silent,
-            weight=weight,
-            imp_kind=imp,
-            cat_feature=cat_idx,
-        )
+    with tqdm(total=max_rounds, desc="BoostaGRoota round") as pbar:
+        while True:
+            # Inside this loop we reduce the dataset on each iteration exiting with keep_vars
+            i += 1
+            crit, keep_vars, df_vimp, mean_shadow = _reduce_vars_sklearn(
+                new_x,
+                y,
+                estimator=estimator,
+                this_round=i,
+                cutoff=cutoff,
+                n_iterations=iters,
+                delta=delta,
+                silent=silent,
+                weight=weight,
+                imp_kind=imp,
+                cat_feature=cat_idx,
+            )
+
+            b_df = df_vimp.T.iloc[1:-1].astype(float)
+            b_df.columns = df_vimp.T.iloc[0].values
+            imp_dic.update(b_df.to_dict())
 
-        b_df = df_vimp.T.copy()
-        b_df.columns = b_df.iloc[0]
-        b_df = b_df.drop(b_df.index[0])
-        b_df = b_df.drop(b_df.index[-1])
-        b_df = b_df.convert_dtypes()
-        for c in b_df.columns:
-            imp_dic[c] = b_df[c].values
+            if crit or i >= max_rounds or len(keep_vars) == 0:
+                break
+            else:
+                new_x = new_x[keep_vars].copy()
+                _, _, cat_idx = get_pandas_cat_codes(new_x)
 
-        if crit | (i >= max_rounds) | (len(keep_vars) == 0):
-            break  # exit and use keep_vars as final variables
-        else:
-            new_x = new_x[keep_vars].copy()
-            _, _, cat_idx = get_pandas_cat_codes(new_x)
+                pbar.update(1)
 
-            pbar.update(1)
-    pbar.close()
-    elapsed = time.time() - t_boostaroota
-    elapsed = elapsed / 60
+    elapsed = (time.time() - start_time) / 60
     if not silent:
-        print("BoostARoota ran successfully! Algorithm went through ", i, " rounds.")
-        print(
-            "\nThe feature selection BoostARoota running time is {0:8.2f} min".format(
-                elapsed
-            )
-        )
+        print(f"BoostARoota ran successfully! Algorithm went through {i} rounds.")
+        print(f"The feature selection BoostARoota running time is {elapsed:8.2f} min")
 
-    df_vimp = pd.DataFrame(imp_dic)
+    df_vimp = pd.DataFrame.from_dict(imp_dic)
 
     return crit, keep_vars, df_vimp, mean_shadow
 
 
 ###################################
 #
 # GrootCV
@@ -1752,39 +1849,35 @@
 
 class GrootCV(SelectorMixin, BaseEstimator):
     """A shuffled copy of the predictors matrix is added (shadows) to the original set of predictors.
     The lightGBM is fitted using repeated cross-validation, the feature importance
     is extracted each time and averaged to smooth out the noise.
     If the feature importance is larger than the average shadow feature importance then the predictors
     are rejected, the others are kept.
-
-
     - Cross-validated feature importance to smooth out the noise, based on lightGBM only
       (which is, most of the time, the fastest and more accurate Boosting).
     - the feature importance is derived using SHAP importance
     - Taking the max of median of the shadow var. imp over folds otherwise not enough conservative and
       it improves the convergence (needs less evaluation to find a threshold)
     - Not based on a given percentage of cols needed to be deleted
     - Plot method for var. imp
-
     Parameters
     ----------
     objective: str
         the lightGBM objective
     cutoff: float
         the value by which the max of shadow imp is divided, to compare to real importance
     n_folds: int, default=5
         the number of folds for the cross-val
     n_iter: int, default=5
         the number of times the cross-validation is repeated
     silent: bool, default=False
         print out details or not
     rf: bool, default=False
         the lightGBM implementation of the random forest
-
     Attributes
     ----------
     selected_features_: list of str
         the list of columns to keep
     ranking_ : array of shape [n_features]
         The feature ranking, such that ``ranking_[i]`` corresponds to the
         ranking position of the i-th feature. Selected (i.e., estimated
@@ -1794,25 +1887,23 @@
         The absolute feature ranking as ordered by selection process. It does not guarantee
         that this order is correct for all models. For a model agnostic ranking, see the
         the attribute ``ranking``
     cv_df: dataframe
         the statistics of the feature importance over the different repeats of the X-val
     sha_cutoff: float
         the threshold below which the predictors are rejected
-
     Examples
     -------
     >>> X = df[filtered_features].copy()
     >>> y = df['target'].copy()
     >>> w = df['weight'].copy()
     >>>
     >>> feat_selector = arfsgroot.GrootCV(objective='rmse', cutoff = 1, n_folds=5, n_iter=5)
     >>> feat_selector.fit(X, y, sample_weight=None)
     >>> feat_selector.plot_importance(n_feat_per_inch=5)
-
     """
 
     def __init__(
         self, objective=None, cutoff=1, n_folds=5, n_iter=5, silent=True, rf=False
     ):
         self.objective = objective
         self.cutoff = cutoff
@@ -1822,52 +1913,45 @@
         self.rf = rf
         self.cv_df = None
         self.sha_cutoff = None
         self.ranking_absolutes_ = None
         self.ranking_ = None
 
         # Throw errors if the inputted parameters don't meet the necessary criteria
-        if cutoff <= 0:
-            raise ValueError(
-                "cutoff should be greater than 0. You entered" + str(cutoff)
-            )
-        if n_iter <= 0:
-            raise ValueError(
-                "n_iter should be greater than 0. You entered" + str(n_iter)
-            )
-        if n_folds <= 0:
-            raise ValueError(
-                "n_folds should be greater than 0. You entered" + str(n_folds)
-            )
+        # Ensure parameters meet necessary criteria
+        if cutoff <= 0 or n_iter <= 0 or n_folds <= 0:
+            raise ValueError("cutoff, n_iter, and n_folds should be greater than 0.")
 
     def fit(self, X, y, sample_weight=None):
         """Fit the GrootCV transformer with the provided estimator.
 
         Parameters
         ----------
         X : pd.DataFrame
             the predictors matrix
         y : pd.Series
             the target
-        sample_weight : pd.series
-            sample_weight, if any
+        sample_weight : pd.Series, optional
+            sample weights, if any
 
+        Returns
+        -------
+        self : GrootCV
+            fitted estimator
         """
 
-        if isinstance(X, pd.DataFrame):
-            self.feature_names_in_ = X.columns.to_numpy()
-        else:
-            raise TypeError("X is not a dataframe")
+        if not isinstance(X, pd.DataFrame):
+            raise TypeError("X is not a pandas DataFrame")
 
-        if isinstance(y, pd.Series) is not True:
-            y = pd.Series(y)
+        self.feature_names_in_ = X.columns.to_numpy()
+        y = pd.Series(y) if not isinstance(y, pd.Series) else y
 
         if sample_weight is not None:
-            sample_weight = _check_sample_weight(sample_weight, X)
             sample_weight = pd.Series(sample_weight)
+            sample_weight = _check_sample_weight(sample_weight, X)
 
         # internal encoding (ordinal encoding)
         X, obj_feat, cat_idx = get_pandas_cat_codes(X)
 
         self.selected_features_, self.cv_df, self.sha_cutoff = _reduce_vars_lgb_cv(
             X,
             y,
@@ -1875,34 +1959,30 @@
             cutoff=self.cutoff,
             n_folds=self.n_folds,
             n_iter=self.n_iter,
             silent=self.silent,
             weight=sample_weight,
             rf=self.rf,
         )
+
         self.selected_features_ = self.selected_features_.values
         self.support_ = np.asarray(
-            [
-                True if c in self.selected_features_ else False
-                for c in self.feature_names_in_
-            ]
+            [c in self.selected_features_ for c in self.feature_names_in_]
         )
+        self.ranking_ = np.where(self.support_, 2, 1)
 
         b_df = self.cv_df.T.copy()
         b_df.columns = b_df.iloc[0]
         b_df = b_df.drop(b_df.index[0])
         b_df = b_df.drop(b_df.index[-1])
         b_df = b_df.convert_dtypes()
         real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
         self.ranking_absolutes_ = list(
             real_df.mean().sort_values(ascending=False).index
         )
-
-        self.ranking_ = np.where(self.support_, 2, 1)
-
         return self
 
     def _get_support_mask(self):
         check_is_fitted(self)
 
         return self.support_
 
@@ -1910,143 +1990,89 @@
         if not isinstance(X, pd.DataFrame):
             raise TypeError("X is not a dataframe")
         return X[self.selected_features_]
 
     def _more_tags(self):
         return {"allow_nan": True, "requires_y": True}
 
+    @mpl.rc_context(PLT_PARAMS)
     def plot_importance(self, n_feat_per_inch=5):
         """Boxplot of the variable importance, ordered by magnitude
         The max shadow variable importance illustrated by the dashed line.
         Requires to apply the fit method first.
-
         Parameters
         ----------
         n_feat_per_inch : int, default=5
             number of features to plot per inch (for scaling the figure)
-
         Returns
         -------
         fig : plt.figure
             the matplotlib figure object containing the boxplot
         """
 
-        # plt.style.use('fivethirtyeight')
-        my_colors_list = [
-            "#000000",
-            "#7F3C8D",
-            "#11A579",
-            "#3969AC",
-            "#F2B701",
-            "#E73F74",
-            "#80BA5A",
-            "#E68310",
-            "#008695",
-            "#CF1C90",
-            "#F97B72",
-        ]
-        bckgnd_color = "#f5f5f5"
-        params = {
-            "axes.prop_cycle": plt.cycler(color=my_colors_list),
-            "axes.facecolor": bckgnd_color,
-            "patch.edgecolor": bckgnd_color,
-            "figure.facecolor": bckgnd_color,
-            "axes.edgecolor": bckgnd_color,
-            "savefig.edgecolor": bckgnd_color,
-            "savefig.facecolor": bckgnd_color,
-            "grid.color": "#d2d2d2",
-            "lines.linewidth": 1.5,
-        }  # plt.cycler(color=my_colors_list)
-        mpl.rcParams.update(params)
-
         if self.sha_cutoff is None:
             raise ValueError("Apply fit method first")
 
         b_df = self.cv_df.T.copy()
         b_df.columns = b_df.iloc[0]
         b_df = b_df.drop(b_df.index[0])
         b_df = b_df.drop(b_df.index[-1])
         b_df = b_df.convert_dtypes()
         real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
         sha_df = b_df.iloc[:, int(b_df.shape[1] / 2) :].copy()
 
-        color = {
-            "boxes": "gray",
-            "whiskers": "gray",
-            "medians": "#000000",
-            "caps": "gray",
-        }
         real_df = real_df.reindex(
             real_df.select_dtypes(include=[np.number])
             .mean()
             .sort_values(ascending=True)
             .index,
             axis=1,
         )
 
         if real_df.dropna().empty:
-            warnings.warn("No feature selected - No data to plot")
+            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
             return None
         else:
-            bp = real_df.plot(
-                kind="box",
-                color=color,
-                boxprops=dict(linestyle="-", linewidth=1.5),
-                flierprops=dict(linestyle="-", linewidth=1.5),
-                medianprops=dict(linestyle="-", linewidth=1.5, color="#000000"),
-                whiskerprops=dict(linestyle="-", linewidth=1.5),
-                capprops=dict(linestyle="-", linewidth=1.5),
-                showfliers=False,
-                grid=True,
-                rot=0,
-                vert=False,
-                patch_artist=True,
-                figsize=(16, real_df.shape[1] / n_feat_per_inch),
-                fontsize=9,
-            )
+            fig, ax = plt.subplots(figsize=(16, real_df.shape[1] / n_feat_per_inch))
+            bp = real_df.plot(**PLOT_KWARGS, ax=ax)
             col_idx = np.argwhere(real_df.columns.isin(self.selected_features_)).ravel()
-            blue_color = "#2590fa"
 
             for c in range(real_df.shape[1]):
                 bp.findobj(mpl.patches.Patch)[c].set_facecolor("gray")
                 bp.findobj(mpl.patches.Patch)[c].set_color("gray")
 
             for c in col_idx:
-                bp.findobj(mpl.patches.Patch)[c].set_facecolor(blue_color)
-                bp.findobj(mpl.patches.Patch)[c].set_color(blue_color)
+                bp.findobj(mpl.patches.Patch)[c].set_facecolor(BLUE)
+                bp.findobj(mpl.patches.Patch)[c].set_color(BLUE)
 
-            plt.axvline(x=self.sha_cutoff, linestyle="--", color="gray")
-            # xrange = real_df.max(skipna=True).max(skipna=True)-real_df.min(skipna=True).min(skipna=True)
+            ax.axvline(x=self.sha_cutoff, linestyle="--", color=RED)
             bp.set_xlim(left=real_df.min(skipna=True).min(skipna=True) - 0.025)
             custom_lines = [
-                Line2D([0], [0], color=blue_color, lw=5),
+                Line2D([0], [0], color=BLUE, lw=5),
                 Line2D([0], [0], color="gray", lw=5),
-                Line2D([0], [0], linestyle="--", color="gray", lw=2),
+                Line2D([0], [0], linestyle="--", color=RED, lw=2),
             ]
             bp.legend(
                 custom_lines, ["confirmed", "rejected", "threshold"], loc="lower right"
             )
-            plt.title("Groot CV importance and selected predictors")
-            fig = bp.get_figure()
-            # plt.tight_layout()
-            # plt.show()
+            ax.set_title("Groot CV importance and selected predictors")
+
             return fig
 
 
 ########################################################################################
 #
-# BoostARoota. In principle, you cannot/don't need to access those methods (reason of
+# GrootCV. In principle, you cannot/don't need to access those methods (reason of
 # the _ in front of the function name, they're internal functions)
 #
 ########################################################################################
 
 
 def _reduce_vars_lgb_cv(X, y, objective, n_folds, cutoff, n_iter, silent, weight, rf):
     """Private function, reduce the number of predictors using a lightgbm (python API)
-
     Parameters
     ----------
     x : pd.DataFrame
         the dataframe to create shadow features on
     y : pd.Series
         the target
     objective : str
@@ -2058,55 +2084,123 @@
     silent : bool
         Set to True if don't want to see the BoostARoota output printed.
         Will still show any errors or warnings that may occur
     weight : pd.series
         sample_weight, if any
     rf : bool, default=False
         the lightGBM implementation of the random forest
-
     returns
     -------
      real_vars['feature'] : pd.dataframe
         feature importance of the real predictors over iter
      df : pd.DataFrame
         feature importance of the real+shadow predictors over iter
      cutoff_shadow : float
         the feature importance threshold, to reject or not the predictors
     """
 
-    # Set up the parameters for running the model in LGBM - split is on multi log loss
+    param = _set_lgb_parameters(X=X, y=y, objective=objective, rf=rf, silent=silent)
 
-    n_feat = X.shape[1]
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+    category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
+    cat_idx = [X.columns.get_loc(col) for col in category_cols]
 
-    if objective == "softmax":
-        param = {
-            "objective": objective,
-            "num_class": len(np.unique(y)),
-        }
-    else:
-        param = {"objective": objective}
+    rkf = RepeatedKFold(n_splits=n_folds, n_repeats=n_iter, random_state=2652124)
+    iter = 0
+    for tridx, validx in tqdm(
+        rkf.split(X, y), total=rkf.get_n_splits(), desc="Repeated k-fold"
+    ):
+        X_train, X_val, y_train, y_val, weight_tr, weight_val = _split_data(
+            X, y, tridx, validx, weight
+        )
 
-    param.update({"verbosity": -1})
+        # Create the shadow variables and run the model to obtain importances
+        new_x_tr, shadow_names = _create_shadow(X_train)
+        new_x_val, _ = _create_shadow(X_val)
 
-    # best feature fraction according to "Elements of statistical learning"
-    if objective in ["softmax", "binary"]:
-        feat_frac = np.sqrt(n_feat) / n_feat
-    else:
-        feat_frac = n_feat / (3 * n_feat)
+        bst, shap_matrix, bst.best_iteration = _train_lgb_model(
+            new_x_tr,
+            y_train,
+            weight_tr,
+            new_x_val,
+            y_val,
+            weight_val,
+            category_cols=category_cols,
+            early_stopping_rounds=20,
+            **param,
+        )
+
+        importance = _compute_importance(new_x_tr, shap_matrix, param, objective)
+        if iter == 0:
+            df = pd.DataFrame({"feature": new_x_tr.columns})
+        df = _merge_importance_df(
+            df=df,
+            importance=importance,
+            iter=iter,
+            n_folds=n_folds,
+            column_names=new_x_tr.columns,
+            silent=silent,
+        )
+        iter += 1
+
+    df["Med"] = df.select_dtypes(include=[np.number]).mean(axis=1)
+    # Split them back out
+    real_vars = df[~df["feature"].isin(shadow_names)]
+    shadow_vars = df[df["feature"].isin(shadow_names)]
+
+    # Get median value from the shadows, comparing predictor by predictor. Not the same criteria
+    # max().max() like in Boruta but max of the median to mitigate.
+    # Otherwise too conservative (reject too often)
+    cutoff_shadow = shadow_vars.select_dtypes(include=[np.number]).max().mean() / cutoff
+    real_vars = real_vars[(real_vars.Med.values >= cutoff_shadow)]
+
+    return real_vars["feature"], df, cutoff_shadow
+
+
+def _set_lgb_parameters(X, y, objective, rf=False, silent=True):
+    """Set parameters for a LightGBM model based on the input features and the objective.
+
+    Parameters
+    ----------
+    X : numpy array or pandas DataFrame
+        The feature matrix of the training data.
+    y : numpy array or pandas Series
+        The target variable of the training data.
+    objective : str
+        The objective function to optimize during training.
+    rf : bool, default False
+        Whether to use random forest boosting.
+    silent : bool, default True
+        Whether to print messages during parameter setting.
 
+    Returns
+    -------
+    dict
+        The dictionary of LightGBM parameters.
+
+    """
+    n_feat = X.shape[1]
+    param = {"objective": objective}
+    param.update({"verbosity": -1})
+    if objective == "softmax":
+        param["num_class"] = len(np.unique(y))
     if rf:
+        feat_frac = (
+            np.sqrt(n_feat) / n_feat
+            if objective in ["softmax", "binary"]
+            else n_feat / (3 * n_feat)
+        )
         param.update(
             {
                 "boosting_type": "rf",
                 "bagging_fraction": "0.7",
                 "feature_fraction": feat_frac,
                 "bagging_freq": "1",
             }
         )
-
     clf_losses = [
         "binary",
         "softmax",
         "multi_logloss",
         "multiclassova",
         "multiclass",
         "multiclass_ova",
@@ -2116,117 +2210,193 @@
     ]
     if objective in clf_losses:
         y = y.astype(int)
         y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
         n_classes = y_freq_table.size
         if n_classes > 2 and objective != "softmax":
             param["objective"] = "softmax"
-            param["num_class"] = (len(np.unique(y)),)
+            param["num_class"] = len(np.unique(y))
             if not silent:
                 print("Multi-class task, setting objective to softmax")
-
         main_class = y_freq_table[0]
         if not silent:
             print("GrootCV: classification with unbalance classes")
-
         if main_class > 0.8:
             param.update({"is_unbalance": True})
-
     param.update({"num_threads": 0})
+    return param
 
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-    category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
-    cat_idx = [X.columns.get_loc(col) for col in category_cols]
 
-    rkf = RepeatedKFold(n_splits=n_folds, n_repeats=n_iter, random_state=2652124)
-    i = 0
-    for tridx, validx in tqdm(
-        rkf.split(X, y), total=rkf.get_n_splits(), desc="Repeated k-fold"
-    ):
-        if weight is not None:
-            X_train, y_train, weight_tr = (
-                X.iloc[tridx, :],
-                y.iloc[tridx],
-                weight.iloc[tridx],
-            )
-            X_val, y_val, weight_val = (
-                X.iloc[validx, :],
-                y.iloc[validx],
-                weight.iloc[validx],
-            )
-        else:
-            X_train, y_train = X.iloc[tridx, :], y.iloc[tridx]
-            X_val, y_val = X.iloc[validx, :], y.iloc[validx]
-            weight_tr = None
-            weight_val = None
+def _split_data(X, y, tridx, validx, weight=None):
+    """
+    Split data into train and validation sets based on provided indices.
 
-        # Create the shadow variables and run the model to obtain importances
-        new_x_tr, shadow_names = _create_shadow(X_train)
-        new_x_val, _ = _create_shadow(X_val)
+    Parameters
+    ----------
+    X : pandas.DataFrame
+        Features.
+    y : pandas.Series
+        Target variable.
+    tridx : list
+        Indices to be used for training.
+    validx : list
+        Indices to be used for validation.
+    weight : pandas.Series, optional
+        Weights for each sample, by default None.
 
-        d_train = lgb.Dataset(
-            new_x_tr, label=y_train, weight=weight_tr, categorical_feature=category_cols
-        )
-        d_valid = lgb.Dataset(
-            new_x_val, label=y_val, weight=weight_val, categorical_feature=category_cols
+    Returns
+    -------
+    tuple of pandas.DataFrame and pandas.Series
+        X_train, X_val, y_train, y_val, weight_tr, weight_val
+    """
+    if weight is not None:
+        X_train, y_train, weight_tr = (
+            X.iloc[tridx, :],
+            y.iloc[tridx],
+            weight.iloc[tridx],
+        )
+        X_val, y_val, weight_val = (
+            X.iloc[validx, :],
+            y.iloc[validx],
+            weight.iloc[validx],
         )
-        watchlist = [d_train, d_valid]
+    else:
+        X_train, y_train = X.iloc[tridx, :], y.iloc[tridx]
+        X_val, y_val = X.iloc[validx, :], y.iloc[validx]
+        weight_tr = None
+        weight_val = None
+    return X_train, X_val, y_train, y_val, weight_tr, weight_val
+
+
+def _train_lgb_model(
+    X_train,
+    y_train,
+    weight_train,
+    X_val,
+    y_val,
+    weight_val,
+    category_cols=None,
+    early_stopping_rounds=20,
+    **params,
+):
+    """
+    Train a LightGBM model with the given training data and hyperparameters and return the trained model and its SHAP values.
 
-        bst = lgb.train(
-            param,
-            train_set=d_train,
-            num_boost_round=10000,
-            valid_sets=watchlist,
-            # early_stopping_rounds=20,
-            # verbose_eval=0,
-            categorical_feature=category_cols,
-            callbacks=[early_stopping(20, False, False)],
-        )
-        if i == 0:
-            df = pd.DataFrame({"feature": new_x_tr.columns})
-            pass
+    Parameters
+    ----------
+    X_train : array-like of shape (n_samples, n_features)
+        The input training data.
+    y_train : array-like of shape (n_samples,)
+        The target training data.
+    weight_train : array-like of shape (n_samples,)
+        The sample weights for training data.
+    X_val : array-like of shape (n_val_samples, n_features)
+        The input validation data.
+    y_val : array-like of shape (n_val_samples,)
+        The target validation data.
+    weight_val : array-like of shape (n_val_samples,)
+        The sample weights for validation data.
+    category_cols : array-like or None, optional (default=None)
+        The indices of categorical columns. If None, no categorical columns will be considered.
+    early_stopping_rounds : int, optional (default=20)
+        Activates early stopping. Validation metric needs to improve at least once in every early_stopping_rounds
+        round(s) to continue training.
+    **params : dict
+        Other parameters passed to the LightGBM model.
 
-        shap_matrix = bst.predict(new_x_tr, pred_contrib=True)
+    Returns
+    -------
+    tuple of (Booster, numpy.ndarray, int)
+        The trained LightGBM model, its SHAP values for X_train, and the best iteration reached during training.
+    """
 
-        # the dim changed in lightGBM >= 3.0.0
-        if objective == "softmax":
-            # X_SHAP_values (array-like of shape = [n_samples, n_features + 1]
-            # or shape = [n_samples, (n_features + 1) * n_classes])
-            # index starts from 0
-            n_feat = new_x_tr.shape[1]
-            shap_matrix = np.delete(
-                shap_matrix,
-                list(range(n_feat, (n_feat + 1) * n_classes, n_feat + 1)),
-                axis=1,
-            )
-            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
-        else:
-            # for binary, only one class is returned, for regression a single column added as well
-            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+    d_train = lgb.Dataset(
+        X_train, label=y_train, weight=weight_train, categorical_feature=category_cols
+    )
+    d_valid = lgb.Dataset(
+        X_val, label=y_val, weight=weight_val, categorical_feature=category_cols
+    )
+    watchlist = [d_train, d_valid]
 
-        importance = dict(
-            zip(new_x_tr.columns, shap_imp)
-        )  # bst.feature_importance() ))
-        importance = sorted(importance.items(), key=operator.itemgetter(1))
-        df2 = pd.DataFrame(importance, columns=["feature", "fscore" + str(i)])
-        df2["fscore" + str(i)] = df2["fscore" + str(i)] / df2["fscore" + str(i)].sum()
-        df = pd.merge(df, df2, on="feature", how="outer")
-        nit = divmod(i, n_folds)[0]
-        nf = divmod(i, n_folds)[1]
-        if not silent:
-            if nf == 0:
-                print("Groot iteration: ", nit, " with " + str(n_folds) + " folds")
+    bst = lgb.train(
+        params,
+        train_set=d_train,
+        num_boost_round=10000,
+        valid_sets=watchlist,
+        categorical_feature=category_cols,
+        callbacks=[early_stopping(early_stopping_rounds, False, False)],
+    )
 
-        i += 1
+    shap_matrix = bst.predict(X_train, pred_contrib=True)
+    return bst, shap_matrix, bst.best_iteration
 
-    df["Med"] = df.select_dtypes(include=[np.number]).mean(axis=1)
-    # Split them back out
-    real_vars = df[~df["feature"].isin(shadow_names)]
-    shadow_vars = df[df["feature"].isin(shadow_names)]
 
-    # Get median value from the shadows, comparing predictor by predictor. Not the same criteria
-    # max().max() like in Boruta but max of the median to mitigate.
-    # Otherwise too conservative (reject too often)
-    cutoff_shadow = shadow_vars.select_dtypes(include=[np.number]).max().mean() / cutoff
-    real_vars = real_vars[(real_vars.Med.values >= cutoff_shadow)]
+def _compute_importance(new_x_tr, shap_matrix, param, objective):
+    """
+    Compute feature importance scores using SHAP values.
 
-    return real_vars["feature"], df, cutoff_shadow
+    Parameters:
+    -----------
+    new_x_tr : numpy.ndarray
+        The training dataset after being processed.
+    shap_matrix : numpy.ndarray
+        The matrix containing SHAP values computed by a LightGBM model.
+    param : dict
+        A dictionary containing the parameters for a LightGBM model.
+    objective : str
+        The objective function of the LightGBM model.
+
+    Returns:
+    --------
+    list
+        A list of tuples containing feature names and their corresponding importance scores.
+    """
+    if objective == "softmax":
+        n_feat = new_x_tr.shape[1]
+        shap_matrix = np.delete(
+            shap_matrix,
+            list(range(n_feat, (n_feat + 1) * param["num_class"], n_feat + 1)),
+            axis=1,
+        )
+        shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+    else:
+        shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+    importance = dict(zip(new_x_tr.columns, shap_imp))
+    return sorted(importance.items(), key=operator.itemgetter(1))
+
+
+def _merge_importance_df(df, importance, iter, n_folds, column_names, silent=True):
+    """
+    Merge the feature importance dataframe `df` with the importance
+    information for the current iteration of a cross-validation loop.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        The current feature importance dataframe.
+    importance : dict
+        A dictionary with the feature importance information for
+        the current iteration.
+    i : int
+        The index of the current iteration.
+    n_folds : int
+        The number of folds used in the cross-validation loop.
+    silent : bool, optional
+        If True, suppress output.
+
+    Returns
+    -------
+    pandas.DataFrame
+        The updated feature importance dataframe.
+    """
+
+    df2 = pd.DataFrame(importance, columns=["feature", "fscore" + str(iter)])
+    df2["fscore" + str(iter)] = (
+        df2["fscore" + str(iter)] / df2["fscore" + str(iter)].sum()
+    )
+    df = pd.merge(df, df2, on="feature", how="outer")
+    nit = divmod(iter, n_folds)[0]
+    nf = divmod(iter, n_folds)[1]
+    if not silent:
+        if nf == 0:
+            print("Groot iteration: ", nit, " with " + str(n_folds) + " folds")
+    return df
```

### Comparing `arfs-1.0.7/src/arfs/feature_selection/base.py` & `arfs-1.1.0/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/feature_selection/mrmr.py` & `arfs-1.1.0/src/arfs/feature_selection/mrmr.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 import functools
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_is_fitted
-from tqdm import tqdm
+from tqdm.auto import tqdm
 from sklearn.feature_selection._base import SelectorMixin
 from ..association import (
     f_stat_classification_parallel,
     f_stat_regression_parallel,
     association_series,
 )
 
@@ -168,104 +168,51 @@
         target = y.copy()
         if self.task == "classification":
             target = target.astype("category")
 
         self.relevance_args = {"X": X, "y": target, "sample_weight": sample_weight}
         self.redundancy_args = {"X": X, "sample_weight": sample_weight}
 
-        relevance = self.relevance_func(**self.relevance_args)
-        features = relevance[~relevance.isna()].index.to_list()
-        relevance = relevance.loc[features]
-        redundancy = pd.DataFrame(FLOOR, index=features, columns=features)
-        self.n_features_to_select = min(self.n_features_to_select, len(features))
+        self.relevance = self.relevance_func(**self.relevance_args)
+        self.features = self.relevance[~self.relevance.isna()].index.to_list()
+        self.relevance = self.relevance.loc[self.features]
+        self.redundancy = pd.DataFrame(
+            FLOOR, index=self.features, columns=self.features
+        )
+        self.n_features_to_select = min(self.n_features_to_select, len(self.features))
 
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
 
-        self.n_features_in_ = len(features)
+        self.n_features_in_ = len(self.features)
 
-        selected_features = []
-        not_selected_features = features.copy()
+        self.selected_features = []
+        self.not_selected_features = self.features.copy()
         self.ranking_ = pd.Series(
             dtype="float64"
         )  # pd.DataFrame(columns=['var_name', 'mrmr', 'relevancy', 'redundancy'])
         self.redundancy_ = pd.Series(dtype="float64")
-        for i in tqdm(range(self.n_features_to_select), disable=not self.show_progress):
-            score_numerator = relevance.loc[not_selected_features]
-
-            if i > 0:
-                last_selected_feature = selected_features[-1]
-
-                if self.only_same_domain:
-                    not_selected_features_sub = [
-                        c
-                        for c in not_selected_features
-                        if c.split("_")[0] == last_selected_feature.split("_")[0]
-                    ]
-                else:
-                    not_selected_features_sub = not_selected_features
-
-                if not_selected_features_sub:
-                    redundancy.loc[not_selected_features_sub, last_selected_feature] = (
-                        self.redundancy_func(
-                            target=last_selected_feature,
-                            features=not_selected_features_sub,
-                            **self.redundancy_args,
-                        )
-                        .fillna(FLOOR)
-                        .abs()
-                        .clip(FLOOR)
-                    )
-                    score_denominator = (
-                        redundancy.loc[not_selected_features, selected_features]
-                        .apply(self.denominator_func, axis=1)
-                        .replace(1.0, float("Inf"))
-                    )
-
-            else:
-                score_denominator = pd.Series(1, index=features)
+        self.run_feature_selection()
 
-            score = score_numerator / score_denominator
-            score = score.sort_values(ascending=False)
-            best_feature = score.index[score.argmax()]
-            self.ranking_ = pd.concat(
-                [
-                    self.ranking_,
-                    pd.Series({best_feature: score.loc[best_feature]}, dtype="float64"),
-                ]
-            )
-            self.redundancy_ = pd.concat(
-                [
-                    self.redundancy_,
-                    pd.Series(
-                        {best_feature: score_denominator.loc[best_feature]},
-                        dtype="float64",
-                    ),
-                ]
-            )
-            # the first selected feature has a default denominator (redundancy) = 1 to avoid dividing by zero
-            # I set it back to zero
-            self.redundancy_ = self.redundancy_.replace(1.0, 0.0)
-            selected_features.append(best_feature)
-            not_selected_features.remove(best_feature)
-        self.relevance_ = relevance
+        # store the output in the sklearn flavour
+        self.relevance_ = self.relevance
         self.ranking_ = pd.concat(
             [self.ranking_, self.relevance_, self.redundancy_], axis=1
         )
         self.ranking_.columns = ["mrmr", "relevance", "redundancy"]
         self.ranking_ = self.ranking_.iloc[: self.n_features_to_select, :]
-        # set back the mrmr score to inf for the first selected feature
-        # (redundancy with NULL is 0 and dividing by zero is INF)
+
+        # Set back the mrmr score to Inf for the first selected feature to avoid dividing by zero
         self.ranking_.iloc[0, 0] = float("Inf")
-        self.selected_features_ = selected_features
+
+        self.selected_features_ = self.selected_features
         self.support_ = np.asarray(
-            [x in selected_features for x in self.feature_names_in_]
+            [x in self.selected_features for x in self.feature_names_in_]
         )
-        self.not_selected_features_ = not_selected_features
-
+        self.not_selected_features_ = self.not_selected_features
         return self
 
     def transform(self, X):
         """
         Transform the data, returns a transformed version of `X`.
 
         Parameters
@@ -312,7 +259,85 @@
     def _get_support_mask(self):
         check_is_fitted(self)
 
         return self.support_
 
     def _more_tags(self):
         return {"allow_nan": True}
+
+    def select_next_feature(
+        self, not_selected_features, selected_features, relevance, redundancy
+    ):
+        score_numerator = relevance.loc[not_selected_features]
+
+        if len(selected_features) > 0:
+            last_selected_feature = selected_features[-1]
+
+            if self.only_same_domain:
+                not_selected_features_sub = [
+                    c
+                    for c in not_selected_features
+                    if c.split("_")[0] == last_selected_feature.split("_")[0]
+                ]
+            else:
+                not_selected_features_sub = not_selected_features
+
+            if not_selected_features_sub:
+                redundancy.loc[not_selected_features_sub, last_selected_feature] = (
+                    self.redundancy_func(
+                        target=last_selected_feature,
+                        features=not_selected_features_sub,
+                        **self.redundancy_args,
+                    )
+                    .fillna(FLOOR)
+                    .abs()
+                    .clip(FLOOR)
+                )
+                score_denominator = (
+                    redundancy.loc[not_selected_features, selected_features]
+                    .apply(self.denominator_func, axis=1)
+                    .replace(1.0, float("Inf"))
+                )
+
+            else:
+                score_denominator = pd.Series(1, index=self.features)
+
+        else:
+            score_denominator = pd.Series(1, index=self.features)
+
+        score = score_numerator / score_denominator
+        score = score.sort_values(ascending=False)
+        best_feature = score.index[score.argmax()]
+
+        return best_feature, score, score_denominator
+
+    def update_ranks(self, best_feature, score, score_denominator):
+        self.ranking_ = pd.concat(
+            [
+                self.ranking_,
+                pd.Series({best_feature: score.loc[best_feature]}, dtype="float64"),
+            ]
+        )
+        self.redundancy_ = pd.concat(
+            [
+                self.redundancy_,
+                pd.Series(
+                    {best_feature: score_denominator.loc[best_feature]},
+                    dtype="float64",
+                ),
+            ]
+        )
+        # the first selected feature has a default denominator (redundancy) = 1 to avoid dividing by zero
+        # I set it back to zero
+        self.redundancy_ = self.redundancy_.replace(1.0, 0.0)
+        self.selected_features.append(best_feature)
+        self.not_selected_features.remove(best_feature)
+
+    def run_feature_selection(self):
+        for i in tqdm(range(self.n_features_to_select), disable=not self.show_progress):
+            best_feature, score, score_denominator = self.select_next_feature(
+                self.not_selected_features,
+                self.selected_features,
+                self.relevance,
+                self.redundancy,
+            )
+            self.update_ranks(best_feature, score, score_denominator)
```

### Comparing `arfs-1.0.7/src/arfs/feature_selection/summary.py` & `arfs-1.1.0/src/arfs/feature_selection/summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     s : array-like of shape (n_features,)
         the boolean array for defining the style
 
 
     """
     is_X = s == 0
     return [
-        "background-color: #d65f5f" if v else "background-color: #33a654" for v in is_X
+        "background-color: #ba0202" if v else "background-color: #0c8a30" for v in is_X
     ]
 
 
 def make_fs_summary(selector_pipe):
     """make_fs_summary makes a summary dataframe highlighting at which step a
     given predictor has been rejected (if any).
 
@@ -49,27 +49,25 @@
     >>> groot_pipeline.fit_transform(
         X=df[predictors],
         y=df[target],
         lowimp__sample_weight=df[weight],
         grootcv__sample_weight=df[weight])
     >>> fs_summary_df = make_fs_summary(groot_pipeline)
     """
-
     tag_df = pd.DataFrame({"predictor": selector_pipe[0].feature_names_in_})
-    for selector_name in selector_pipe.named_steps.keys():
-        if hasattr(selector_pipe.named_steps[selector_name], "support_"):
-            feature_in = selector_pipe.named_steps[selector_name].feature_names_in_
-            to_drop = list(
-                set(selector_pipe.named_steps[selector_name].feature_names_in_)
-                - set(selector_pipe.named_steps[selector_name].get_feature_names_out())
-            )
+    for selector_name, selector in selector_pipe.named_steps.items():
+        if hasattr(selector, "support_"):
+            feature_in = selector.feature_names_in_
+            to_drop = list(set(feature_in) - set(selector.get_feature_names_out()))
             tag_df[selector_name] = np.where(
                 tag_df["predictor"].isin(to_drop), 0, 1
             ) * np.where(tag_df["predictor"].isin(feature_in), 1, np.nan)
+        else:
+            tag_df[selector_name] = np.nan
 
-    col_to_apply_style = tag_df.columns[1:]
-    tag_df = (
-        tag_df.style.apply(highlight_discarded, subset=col_to_apply_style)
-        .applymap(lambda x: "" if x == x else "background-color: #ffa500")
+    style = (
+        tag_df.style.apply(highlight_discarded, subset=tag_df.columns[1:])
+        .applymap(lambda x: "" if x == x else "background-color: #f57505")
         .format(precision=0)
     )
-    return tag_df
+
+    return style
```

### Comparing `arfs-1.0.7/src/arfs/feature_selection/unsupervised.py` & `arfs-1.1.0/src/arfs/feature_selection/unsupervised.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,14 +138,32 @@
             threshold=threshold,
             statistic_fn=_pandas_count_unique_values,
             greater_than_threshold=True,
         )
 
 
 def _pandas_count_unique_values_cat_features(X):
+    """
+    Counts the number of unique values in categorical features of a pandas DataFrame.
+
+    Parameters
+    ----------
+    X : pandas DataFrame
+        The input data.
+
+    Returns
+    -------
+    pandas Series
+        The number of unique values in each categorical feature.
+
+    Raises
+    ------
+    TypeError
+        If the input data is not a pandas DataFrame.
+    """
     if not isinstance(X, pd.DataFrame):
         raise TypeError("X should be a pandas DataFrame")
     count_series = pd.Series(data=0, index=X.columns)
     dtype_dic = create_dtype_dict(X, dic_keys="dtypes")
     for c in dtype_dic["cat"]:
         count_series[c] = X[c].nunique()
     return count_series
```

### Comparing `arfs-1.0.7/src/arfs/feature_selection/variable_importance.py` & `arfs-1.1.0/src/arfs/feature_selection/variable_importance.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/gbm.py` & `arfs-1.1.0/src/arfs/gbm.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,54 +22,35 @@
 import joblib
 from datetime import date
 import warnings
 import gc
 import os
 from pathlib import Path
 
-qual_colors_list = [
+QUAL_COLORS = [
     (0.188235, 0.635294, 0.854902),
     (0.898039, 0.682353, 0.219608),
     (0.988235, 0.309804, 0.188235),
     (0.427451, 0.564706, 0.309804),
 ]
+BCKGRND_COLOR = "#f5f5f5"
 
-
-def set_my_plt_style(height=3, width=5, linewidth=2):
-    """This set the style of matplotlib to fivethirtyeight with some modifications (colours, axes)
-
-    Parameters
-    ----------
-    height : float, default = 3
-        fig height in inches (yeah they're still struggling with the metric system) (default ``3``)
-    width : float, default = 5
-        fig width in inches (yeah they're still struggling with the metric system) (default ``5``)
-    linewidth : float
-         (default ``2``)
-
-    """
-    plt.style.use("fivethirtyeight")
-    my_colors_list = qual_colors_list  # Bold_10.hex_colors
-    # myorder = [2, 3, 4, 1, 0, 6, 5, 8, 9, 7]
-    # my_colors_list = [my_colors_list[i] for i in myorder]
-    bckgnd_color = "#f5f5f5"
-    params = {
-        "figure.figsize": (width, height),
-        "axes.prop_cycle": plt.cycler(color=my_colors_list),
-        "axes.facecolor": bckgnd_color,
-        "patch.edgecolor": bckgnd_color,
-        "figure.facecolor": bckgnd_color,
-        "axes.edgecolor": bckgnd_color,
-        "savefig.edgecolor": bckgnd_color,
-        "savefig.facecolor": bckgnd_color,
-        "grid.color": "#d2d2d2",
-        "lines.linewidth": linewidth,
-        "grid.alpha": 0.5,
-    }  # plt.cycler(color=my_colors_list)
-    mpl.rcParams.update(params)
+MPL_PARAMS = {
+    "figure.figsize": (5, 3),
+    "axes.prop_cycle": plt.cycler(color=QUAL_COLORS),
+    "axes.facecolor": BCKGRND_COLOR,
+    "patch.edgecolor": BCKGRND_COLOR,
+    "figure.facecolor": BCKGRND_COLOR,
+    "axes.edgecolor": BCKGRND_COLOR,
+    "savefig.edgecolor": BCKGRND_COLOR,
+    "savefig.facecolor": BCKGRND_COLOR,
+    "grid.color": "#d2d2d2",
+    "lines.linewidth": 2,
+    "grid.alpha": 0.5,
+}
 
 
 class GradientBoosting:
     """Performs the training of a base lightGBM/CatBoost using early stopping. It works for any of the
     supported loss function (lightGBM/CatBoost), so for regression and classification you can use an instance of
     this class. For the early stopping process, 20% of the data set is used and a fix seed is used for
     reproducibility.
@@ -428,15 +409,14 @@
         init_score=init_score,
         groups=groups,
         stratified=stratified,
         test_size=0.2,
     )
 
     col_list = list(X.columns)
-    # cat_idx = [col_list.index(c) for c in cat_feat if c in x]
     d_train = lgb.Dataset(
         X_train, label=y_train, categorical_feature=cat_feat, free_raw_data=False
     )
     d_valid = lgb.Dataset(
         X_val,
         label=y_val,
         categorical_feature=cat_feat,
@@ -489,17 +469,14 @@
 
     if callable(params["objective"]):
         fobj_call = params["objective"]
         params.pop("objective")
     else:
         fobj_call = None
 
-    # if 'categorical_feature' in params.keys():
-    #     params.pop('categorical_feature')
-
     watchlist = [d_train, d_valid]
     evals_result = {}
     params["verbosity"] = -1
 
     n_trees = params["num_boost_round"] if "num_boost_round" in params else 10_000
     # remove key if exists to avoid LGB userwarnings
     params.pop("num_boost_round", None)
@@ -515,22 +492,22 @@
             early_stopping(10, verbose=False),
             log_evaluation(verbose_eval),
             record_evaluation(eval_result=evals_result),
         ],
     )
 
     if learning_curve:
-        set_my_plt_style()
-        fig, ax = plt.subplots()
-        ax = lgb.plot_metric(evals_result, ax=ax)
-        up_lim = model.best_iteration + 50
-        ax.axvline(
-            x=model.best_iteration, color="grey", linestyle="--", label="best_iter"
-        )
-        ax.set_xlim([0, up_lim])
+        with mpl.rc_context(MPL_PARAMS):
+            fig, ax = plt.subplots()
+            ax = lgb.plot_metric(evals_result, ax=ax)
+            up_lim = model.best_iteration + 50
+            ax.axvline(
+                x=model.best_iteration, color="grey", linestyle="--", label="best_iter"
+            )
+            ax.set_xlim([0, up_lim])
 
         del d_train
         del d_valid
         gc.enable()
         gc.collect()
         if return_valid_features:
             return model, X_val, fig
```

### Comparing `arfs-1.0.7/src/arfs/parallel.py` & `arfs-1.1.0/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/preprocessing.py` & `arfs-1.1.0/src/arfs/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - The ``dtype_column_selector`` for standardizing selection of columns based on their dtypes
 - The ``TreeDiscretizer`` for discretizing continuous columns and auto-group levels of categorical columns
 
 """
 
 # Settings and libraries
 from __future__ import print_function
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 # pandas
 import pandas as pd
 
 # numpy
 import numpy as np
 
@@ -171,15 +171,14 @@
         X_out : pd.DataFrame (n_samples, n_features)
             Transformed input.
         """
         X_trans = X.copy()
         X_trans[self.categorical_features_] = super(
             OrdinalEncoderPandas, self
         ).transform(X_trans[self.categorical_features_])
-        # X_trans.loc[:, self.feature_names_in_] = X_trans.loc[:, self.feature_names_in_].apply(pd.to_numeric, errors="ignore", axis=1)
 
         if self.return_pandas_categorical:
             X_trans[self.categorical_features_] = X_trans[
                 self.categorical_features_
             ].astype("category")
         return X_trans
 
@@ -522,64 +521,57 @@
         elif isinstance(self.bin_features, str) and (
             self.bin_features == "categorical"
         ):
             self.bin_features = list(X.select_dtypes(["category", "object"]).columns)
             self.cat_features = self.bin_features
 
         for col in self.bin_features:
-            if (self.cat_features is not None) and (col in self.cat_features):
+            is_categorical = (self.cat_features is not None) and (
+                col in self.cat_features
+            )
+            if is_categorical:
                 encoder = OrdinalEncoder(
                     handle_unknown="use_encoded_value", unknown_value=np.nan
                 )
                 # create a category for missing
-                # X[col] = X[col].astype("category").cat.add_categories("missing").fillna("missing")
                 X[col] = (
                     X[col]
                     .astype("category")
                     .cat.add_categories("missing_added")
                     .fillna("missing_added")
                 )
                 # encode
                 self.ordinal_encoder_dic[col] = encoder.fit(X[[col]])
                 X[col] = encoder.transform(X[[col]]).ravel()
+            else:
+                encoder = None
 
             gbm_param = self.boost_params.copy()
             tree = GradientBoosting(
-                cat_feat=None,
-                params=gbm_param,
-                show_learning_curve=False,
+                cat_feat=None, params=gbm_param, show_learning_curve=False
             )
-
             tree.fit(X[[col]], y, sample_weight=sample_weight)
 
             # store each fitted tree in a dictionary
             self.tree_dic[col] = tree
 
             # create the bins series
             # predict, group by original values
             # create monotonicly increasing bin for pd.cut
             X[f"{col}_g"] = tree.predict(X[[col]])
 
-            if (self.cat_features is not None) and (col in self.cat_features):
+            if is_categorical:
+                # retrieve original values
+                X[col] = encoder.inverse_transform(X[[col]]).ravel()
                 self.cat_bin_dict[col] = (
                     X[[f"{col}_g", col]]
                     .groupby(f"{col}_g")
-                    .aggregate(
-                        lambda x: " / ".join(
-                            map(
-                                str,
-                                encoder.inverse_transform(
-                                    np.expand_dims(X.loc[x.index, col].unique(), axis=1)
-                                ).ravel(),
-                            )
-                        )
-                    )
-                    .to_dict()[col]
+                    .apply(lambda x: " / ".join(map(str, x[col].unique())))
+                    .to_dict()
                 )
-
             else:
                 bin_array = (
                     X[[f"{col}_g", col]]
                     .groupby(f"{col}_g")
                     .aggregate(max)
                     .sort_values(col)
                     .values.ravel()
@@ -598,14 +590,15 @@
                 pred_values = tree.predict(np.expand_dims(non_nan_values, axis=1))
                 # store the value for knowing the bin into which the NaN should fall
                 self.tree_imputer[col] = non_nan_values.flat[
                     np.abs(pred_values - nan_pred_val).argmin()
                 ]
 
             del tree
+
         return self
 
     def transform(self, X):
         """Apply the discretizer on `X`.
         Parameters
         ----------
         X :
```

### Comparing `arfs-1.0.7/src/arfs/sampling.py` & `arfs-1.1.0/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/src/arfs/utils.py` & `arfs-1.1.0/src/arfs/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 
 from pkg_resources import resource_filename
 from matplotlib import pyplot as plt
 from sklearn.impute import SimpleImputer
-from sklearn.compose import ColumnTransformer
-from sklearn.pipeline import Pipeline
+from sklearn.compose import make_column_transformer
+from sklearn.pipeline import make_pipeline
 from sklearn.datasets import fetch_openml
 from sklearn.datasets import load_breast_cancer
 from sklearn.utils import Bunch
 import joblib
 
 qualitative_colors = [
     "#7F3C8D",
@@ -75,80 +75,185 @@
         "savefig.facecolor": bckgnd_color,
         "grid.color": "#9e9e9e",
         "lines.linewidth": linewidth,
     }  # plt.cycler(color=my_colors_list)
     mpl.rcParams.update(params)
 
 
-def create_dtype_dict(df: pd.DataFrame, dic_keys: str = "col_names"):
-    """create a custom dictionary of data type for adding suffixes
-    to column names in the plotting utility for association matrix
+def create_dtype_dict(df: pd.DataFrame, dic_keys: str = "col_names") -> dict:
+    """Create a custom dictionary of data type for adding suffixes
+    to column names in the plotting utility for association matrix.
 
     Parameters
     ----------
-    df :
-        the dataframe used for computing the association matrix
-    dic_keys :
+    df : pandas.DataFrame
+        The dataframe used for computing the association matrix.
+    dic_keys : str
         Either "col_names" or "dtypes" for returning either a dictionary
         with column names or dtypes as keys.
+
+    Returns
+    -------
+    dict
+        A dictionary with either column names or dtypes as keys.
+
+    Raises
+    ------
+    ValueError
+        If `dic_keys` is not either "col_names" or "dtypes".
     """
-    cat_cols = list(df.select_dtypes(include=["object", "category", "bool"]))
-    time_cols = list(df.select_dtypes(include=["datetime", "timedelta", "datetimetz"]))
-    num_cols = list(df.select_dtypes(include=[np.number]))
-    remaining_cols = list(
-        set(df.columns) - set(cat_cols).union(set(num_cols)).union(time_cols)
+    if not isinstance(df, pd.DataFrame):
+        raise TypeError("df should be a pandas DataFrame")
+
+    cat_cols = df.select_dtypes(include=["object", "category", "bool"]).columns
+    time_cols = df.select_dtypes(
+        include=["datetime", "timedelta", "datetimetz"]
+    ).columns
+    num_cols = df.select_dtypes(include=np.number).columns
+    remaining_cols = (
+        df.columns.difference(cat_cols).difference(num_cols).difference(time_cols)
     )
 
     if dic_keys == "col_names":
-        cat_dic = {c: "cat" for c in cat_cols}
-        num_dic = {c: "num" for c in num_cols}
-        time_dic = {c: "time" for c in time_cols}
-        remainder_dic = {c: "unk" for c in remaining_cols}
-        return {**cat_dic, **num_dic, **time_dic, **remainder_dic}
-    elif dic_keys == "dtypes":
-        cat_dic = {"cat": cat_cols}
-        num_dic = {"num": num_cols}
-        time_dic = {"time": time_cols}
-        remainder_dic = {"unk": remaining_cols}
-        return {**cat_dic, **num_dic, **time_dic, **remainder_dic}
-    else:
-        raise ValueError("'dic_keys' should be either 'col_names' or 'dtypes'")
+        cat_dict = dict.fromkeys(cat_cols, "cat")
+        num_dict = dict.fromkeys(num_cols, "num")
+        time_dict = dict.fromkeys(time_cols, "time")
+        remaining_dict = dict.fromkeys(remaining_cols, "unk")
+        return {**cat_dict, **num_dict, **time_dict, **remaining_dict}
+
+    if dic_keys == "dtypes":
+        return {
+            "cat": cat_cols.tolist(),
+            "num": num_cols.tolist(),
+            "time": time_cols.tolist(),
+            "unk": remaining_cols.tolist(),
+        }
+
+    raise ValueError("dic_keys should be either 'col_names' or 'dtypes'")
 
 
 def get_pandas_cat_codes(X):
+    """
+    Converts categorical and time features in a pandas DataFrame into numerical codes.
+
+    Parameters
+    ----------
+    X : pandas DataFrame
+        The input DataFrame containing categorical and/or time features.
+
+    Returns
+    -------
+    X : pandas DataFrame
+        The modified input DataFrame with categorical and time features replaced by numerical codes.
+    obj_feat : list or None
+        List of column names that were converted to numerical codes. Returns None if no categorical or time features found.
+    cat_idx : list or None
+        List of column indices for the columns in obj_feat. Returns None if no categorical or time features found.
+    """
     dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
     obj_feat = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
 
     if obj_feat:
-        cat = X[obj_feat].stack().astype("str").astype("category").cat.codes.unstack()
-        X = pd.concat([X[X.columns.difference(obj_feat)], cat], axis=1)
+        for obj_column in obj_feat:
+            column = X[obj_column].astype("str").astype("category")
+            # performs label encoding
+            _, inverse = np.unique(column, return_inverse=True)
+            X[obj_column] = inverse
         cat_idx = [X.columns.get_loc(col) for col in obj_feat]
     else:
         obj_feat = None
         cat_idx = None
 
     return X, obj_feat, cat_idx
 
 
+def validate_sample_weight(sample_weight):
+    """Ensures sample_weight parameter is a numpy array."""
+    if isinstance(sample_weight, pd.Series):
+        return sample_weight.values
+    elif isinstance(sample_weight, np.ndarray):
+        return sample_weight
+    elif sample_weight is None:
+        return None
+    else:
+        raise ValueError("sample_weight must be an array-like object or None.")
+
+
+def validate_sample_weight(sample_weight):
+    """
+    Validate the sample_weight parameter.
+
+    Parameters
+    ----------
+    sample_weight : array-like or None
+        Input sample weights.
+
+    Returns
+    -------
+    np.ndarray or None
+        If sample_weight is a Pandas Series, its values are returned as a
+        numpy array. If sample_weight is already a numpy array, it is
+        returned unmodified. If sample_weight is None, None is returned.
+
+    Raises
+    ------
+    ValueError
+        If sample_weight is not an array-like object or None.
+    """
+    if isinstance(sample_weight, pd.Series):
+        return sample_weight.values
+    elif isinstance(sample_weight, np.ndarray):
+        return sample_weight
+    elif sample_weight is None:
+        return None
+    else:
+        raise ValueError("sample_weight must be an array-like object or None.")
+
+
+def validate_pandas_input(arg):
+    """Validate if pandas or numpy arrays are provided
+    Parameters
+    ----------
+    arg : pd.DataFrame or np.array
+        the object to validate
+    Raises
+    ------
+    TypeError
+        error if pandas or numpy arrays are not provided
+    """
+    try:
+        return arg.values
+    except AttributeError:
+        raise TypeError("input needs to be a numpy array or pandas data frame.")
+
+
 def check_if_tree_based(model):
     """check if estimator is tree based
 
     Parameters
     ----------
     model : object
         the estimator to check
 
     Returns
     -------
     condition : boolean
         if tree based or not
     """
-    tree_based_models = ["lightgbm", "xgboost", "catboost", "_forest", "boosting"]
-    condition = any(i in str(type(model)).lower() for i in tree_based_models)
-    return condition
+    tree_based_models = [
+        "lightgbm",
+        "lgbm",
+        "xgboost",
+        "xgb",
+        "catboost",
+        "forest",
+        "boosting",
+        "tree",
+    ]
+    return any(m in model.__class__.__name__.lower() for m in tree_based_models)
 
 
 def is_lightgbm(estimator):
     """check if estimator is lightgbm
 
     Parameters
     ----------
@@ -156,15 +261,15 @@
         the estimator to check
 
     Returns
     -------
     condition : boolean
         if lgbm based or not
     """
-    is_lgb = "lightgbm" in str(type(estimator))
+    is_lgb = "lgbm" in estimator.__class__.__name__.lower()
     return is_lgb
 
 
 def is_catboost(estimator):
     """check if estimator is catboost
 
     Parameters
@@ -173,15 +278,15 @@
         the estimator to check
 
     Returns
     -------
     condition : boolean
         if catboost based or not
     """
-    is_cat = "catboost" in str(type(estimator))
+    is_cat = "catboost" in estimator.__class__.__name__.lower()
     return is_cat
 
 
 def is_xgboost(estimator):
     """check if estimator is xgboost
 
     Parameters
@@ -190,15 +295,15 @@
         the estimator to check
 
     Returns
     -------
     condition : boolean
         if xgboost based or not
     """
-    is_xgb = "xgboost" in str(type(estimator))
+    is_xgb = "xgb" in estimator.__class__.__name__.lower()
     return is_xgb
 
 
 def LightForestRegressor(n_feat, n_estimators=10):
     """lightGBM implementation of the Random Forest regressor with the
     ideal number of features, according to Elements of statistical learning
 
@@ -252,33 +357,34 @@
         colsample_bytree=feat_frac,
         boosting_type="rf",
         subsample_freq=1,
     )
 
 
 def is_list_of_str(str_list):
-    """Check if ``str_list`` is not a list of strings
+    """Check if ``str_list`` is a list of strings.
 
     Parameters
     ----------
-    str_list : list of str
-        the list we want to check for
+    str_list : list or None
+        The list to check.
 
     Returns
     -------
     bool
-        True if list of strings, else False
+        True if the list is a list of strings, False otherwise.
     """
-    if str_list is not None:
-        if not (
-            isinstance(str_list, list) and all(isinstance(s, str) for s in str_list)
-        ):
-            return False
-        else:
-            return True
+    if (
+        str_list is not None
+        and isinstance(str_list, list)
+        and all(isinstance(s, str) for s in str_list)
+    ):
+        return True
+    else:
+        return False
 
 
 def is_list_of_bool(bool_list):
     """Check if ``bool_list`` is not a list of Booleans
 
     Parameters
     ----------
@@ -286,21 +392,22 @@
         the list we want to check for
 
     Returns
     -------
     bool
         True if list of Booleans, else False
     """
-    if bool_list is not None:
-        if not (
-            isinstance(bool_list, list) and all(isinstance(s, bool) for s in bool_list)
-        ):
-            return False
-        else:
-            return True
+    if (
+        bool_list is not None
+        and isinstance(bool_list, list)
+        and all(isinstance(s, bool) for s in bool_list)
+    ):
+        return True
+    else:
+        return False
 
 
 def is_list_of_int(int_list):
     """Check if ``int_list`` is not a list of integers
 
     Parameters
     ----------
@@ -308,21 +415,22 @@
         the list we want to check for
 
     Returns
     -------
     bool
         True if list of integers, else False
     """
-    if int_list is not None:
-        if not (
-            isinstance(int_list, list) and all(isinstance(s, int) for s in int_list)
-        ):
-            return False
-        else:
-            return True
+    if (
+        int_list is not None
+        and isinstance(int_list, list)
+        and all(isinstance(s, int) for s in int_list)
+    ):
+        return True
+    else:
+        return False
 
 
 def _get_titanic_data():
     """Load Titanic data and add dummies (random predictors, numeric and categorical) and
     a genuine one, for benchmarking purpose. Classification (binary)
 
     Returns
@@ -336,56 +444,57 @@
     X, y = fetch_openml("titanic", version=1, as_frame=True, return_X_y=True)
     rng = np.random.RandomState(seed=42)
     nice_guys = ["Rick", "Bender", "Cartman", "Morty", "Fry", "Vador", "Thanos"]
     X["random_cat"] = np.random.choice(nice_guys, X.shape[0])
     X["random_num"] = rng.randn(X.shape[0])
     X["family_size"] = X["parch"] + X["sibsp"]
     X.drop(["parch", "sibsp"], axis=1, inplace=True)
-    X["is_alone"] = 1
-    X.loc[X["family_size"] > 1, "is_alone"] = 0
+    X["is_alone"] = np.where(X["family_size"] > 1, 0, 1)
     X["title"] = (
         X["name"].str.split(", ", expand=True)[1].str.split(".", expand=True)[0]
     )
-    X.loc[X.title == "Miss", "title"] = "Mrs"
+    X.loc[X["title"] == "Miss", "title"] = "Mrs"
     title_counts = X["title"].value_counts()
     rare_titles = title_counts[title_counts < 10].index
     X.loc[X["title"].isin(rare_titles), "title"] = "rare"
-    # X['title'] = X.title.apply(lambda x: 'rare' if rare_titles[x] else x)
-
     categorical_columns = [
         "pclass",
         "sex",
         "embarked",
         "random_cat",
         "is_alone",
         "title",
     ]
     numerical_columns = ["age", "family_size", "fare", "random_num"]
     X = X[categorical_columns + numerical_columns]
-    # Impute
-    categorical_pipe = Pipeline(
-        [("imputer", SimpleImputer(strategy="constant", fill_value="missing"))]
+
+    # Preprocessing
+    categorical_pipe = make_pipeline(
+        SimpleImputer(strategy="constant", fill_value="missing")
     )
-    numerical_pipe = Pipeline([("imputer", SimpleImputer(strategy="mean"))])
-    preprocessing = ColumnTransformer(
-        [
-            ("cat", categorical_pipe, categorical_columns),
-            ("num", numerical_pipe, numerical_columns),
-        ]
+    numerical_pipe = make_pipeline(SimpleImputer(strategy="mean"))
+    preprocessor = make_column_transformer(
+        (categorical_pipe, categorical_columns),
+        (numerical_pipe, numerical_columns),
     )
-    X_trans = preprocessing.fit_transform(X)
-    X = pd.DataFrame(X_trans, columns=X.columns)
-    # encode
-    # X, cat_var_df, inv_mapper = cat_var(X)
+    X = preprocessor.fit_transform(X)
+
+    # Encode categorical variables
+    X = pd.DataFrame(X, columns=categorical_columns + numerical_columns)
     X[categorical_columns] = X[categorical_columns].astype(str)
     X[numerical_columns] = X[numerical_columns].astype(float)
-    # sample weight is just a dummy random vector for testing purpose
+
+    # Create sample weights
     sample_weight = np.random.uniform(0, 1, len(y))
+
     return Bunch(
-        data=X, target=y, sample_weight=sample_weight, categorical=categorical_columns
+        data=X,
+        target=y,
+        sample_weight=sample_weight,
+        categorical=categorical_columns,
     )
 
 
 def _get_cancer_data():
     """Load breast cancer data and add dummies (random predictors) and a genuine one, for benchmarking purpose
     Classification (binary)
 
@@ -471,61 +580,48 @@
 
 def plot_y_vs_X(X, y, ncols=2, figsize=(10, 10)):
     """Plot target vs relevant and non-relevant predictors
 
     Parameters
     ----------
     X : pd.DataFrame
-        the pd DF of the predictors
+        The DataFrame of the predictors.
     y : np.array
-        the target
+        The target.
     ncols : int, optional
-        the number of columns in the facet plot, by default 2
+        The number of columns in the facet plot. Default is 2.
     figsize : tuple, optional
-        the figure size, by default (10, 10)
+        The figure size. Default is (10, 10).
 
     Returns
     -------
     plt.figure
-        the univariate plots y vs pred_i
+        The univariate plots y vs pred_i.
     """
+    n_cols_to_plot = X.shape[1]
+    n_rows = int(np.ceil(n_cols_to_plot / ncols))
 
-    X = pd.DataFrame(X)
-    ncols_to_plot = X.shape[1]
-    n_rows = int(np.ceil(ncols_to_plot / ncols))
-
-    # Create figure and axes (this time it's 9, arranged 3 by 3)
+    # Create figure and axes
     f, axs = plt.subplots(nrows=n_rows, ncols=ncols, figsize=figsize)
 
-    # delete non-used axes
-    n_charts = ncols_to_plot
-    n_subplots = n_rows * ncols
-    cols_to_enum = X.columns
-
-    # Make the axes accessible with single indexing
-    if n_charts > 1:
-        axs = axs.flatten()
-
-    for i, col in enumerate(cols_to_enum):
-        # select the axis where the map will go
-        if n_charts > 1:
-            ax = axs[i]
-        else:
-            ax = axs
-
-        ax.scatter(X[col], y, alpha=0.1)
-        ax.set_title(col)
-
-    if n_subplots > n_charts > 1:
-        for i in range(n_charts, n_subplots):
-            ax = axs[i]
-            ax.set_axis_off()
+    for i, col in enumerate(X.columns):
+        row = i // ncols
+        col = i % ncols
+        axs[row, col].scatter(X[col], y, alpha=0.1)
+        axs[row, col].set_title(col)
+
+    # Hide unused subplots
+    for i in range(n_cols_to_plot, n_rows * ncols):
+        row = i // ncols
+        col = i % ncols
+        axs[row, col].set_axis_off()
 
-    # Display the figure
+    # Adjust spacing between subplots
     plt.tight_layout()
+
     return f
 
 
 def load_data(name="Titanic"):
     """Load some toy data set to test the All Relevant Feature Selection methods.
     Dummies (random) predictors are added and ARFS should be able to filter them out.
     The Titanic predictors are encoded (needed for scikit estimators).
@@ -563,171 +659,169 @@
         return _load_housing(as_frame=False)
     else:
         raise ValueError(
             "`name should be in ['Titanic', 'Boston', 'cancer', 'housing']`"
         )
 
 
-def _generated_corr_dataset_regr(size=1000):
-    """Generate artificial dataset for regression tasks. Some columns are
-    correlated, have no variance, large cardinality, numerical and categorical.
+def _make_corr_dataset_regression(size=1000):
+    """Generate an artificial dataset for regression tasks with columns that
+    are correlated, have no variance, large cardinality, numerical and categorical.
 
     Parameters
     ----------
     size : int, optional
         number of rows to generate, by default 1000
 
     Returns
     -------
     pd.DataFrame, pd.Series, pd.Series
         the predictors matrix, the target and the weights
     """
-    # weights
+    # generate weights
     w = np.random.beta(a=1, b=0.5, size=size)
-    # fixing the seed and the target
+
+    # set seed for reproducibility
     np.random.seed(42)
+
+    # generate target variable
     sigma = 0.2
     y = np.random.normal(1, sigma, size)
-    z = y - np.random.normal(1, sigma / 5, size) + np.random.normal(1, sigma / 5, size)
-    X = np.zeros((size, 13))
 
-    # 5 relevant features, with positive and negative correlation to the target
-    X[:, 0] = z
-    X[:, 1] = y * np.abs(np.random.normal(0, sigma * 2, size)) + np.random.normal(
-        0, sigma / 10, size
-    )
-    X[:, 2] = -y + np.random.normal(0, sigma, size)
-    X[:, 3] = y**2 + np.random.normal(0, sigma, size)
-    X[:, 4] = np.sqrt(y) + np.random.gamma(1, 0.2, size)
-
-    # 5 irrelevant features
-    X[:, 5] = np.random.normal(0, 1, size)
-    X[:, 6] = np.random.poisson(1, size)
-    X[:, 7] = np.random.binomial(1, 0.3, size)
-    X[:, 8] = np.random.normal(0, 1, size)
-    X[:, 9] = np.random.poisson(1, size)
-    # zero variance
-    X[:, 10] = np.ones(size)
-    # high cardinality
-    half_size = int(size / 2)
-    X[:, 11] = np.concatenate(
-        [
-            np.arange(start=0, stop=half_size, step=1),
-            np.arange(start=0, stop=size - half_size, step=1),
-        ]
+    # generate correlated features
+    z = y - np.random.normal(1, sigma / 5, size) + np.random.normal(1, sigma / 5, size)
+    X = pd.DataFrame(
+        {
+            "var0": z,
+            "var1": y * np.abs(np.random.normal(0, sigma * 2, size))
+            + np.random.normal(0, sigma / 10, size),
+            "var2": -y + np.random.normal(0, sigma, size),
+            "var3": y**2 + np.random.normal(0, sigma, size),
+            "var4": np.sqrt(y) + np.random.gamma(1, 0.2, size),
+            "var5": np.random.normal(0, 1, size),
+            "var6": np.random.poisson(1, size),
+            "var7": np.random.binomial(1, 0.3, size),
+            "var8": np.random.normal(0, 1, size),
+            "var9": np.random.poisson(1, size),
+            "var10": np.ones(size),
+            "var11": np.concatenate(
+                [
+                    np.arange(start=0, stop=int(size / 2), step=1),
+                    np.arange(start=0, stop=int(size / 2), step=1),
+                ]
+            ),
+            "var12": y**3 + np.abs(np.random.normal(0, 1, size)),
+        }
     )
-    # a lot of missing values
+
+    # introduce missing values
     idx_nan = np.random.choice(size, int(round(size / 2)), replace=False)
-    X[:, 12] = y**3 + np.abs(np.random.normal(0, 1, size))
-    X[idx_nan, 12] = np.nan
+    X.loc[idx_nan, "var12"] = np.nan
 
-    # make  it a pandas DF
-    column_names = ["var" + str(i) for i in range(13)]
-    column_names[11] = "dummy_cat"
-    X = pd.DataFrame(X)
-    X.columns = column_names
-    X["dummy_cat"] = X["dummy_cat"].astype("category")
-    # low cardinality
-    nice_guys = [
-        "Rick",
-        "Bender",
-        "Cartman",
-        "Morty",
-        "Fry",
-        "Vador",
-        "Thanos",
-        "Bejita",
-        "Cell",
-        "Tinkywinky",
-        "Lecter",
-        "Alien",
-        "Terminator",
-        "Drago",
-        "Dracula",
-        "Krueger",
-        "Geoffrey",
-        "Goldfinder",
-        "Blackbeard",
-        "Excel",
-        "SAS",
-        "Bias",
-        "Variance",
-        "Scrum",
-        "Human",
-        "Garry",
-        "Coldplay",
-        "Imaginedragons",
-        "Platist",
-        "Creationist",
-        "Gruber",
-        "KeyserSoze",
-        "Luthor",
-        "Klaue",
-        "Bane",
-        "MarkZ",
-    ]
-    X["nice_guys"] = np.random.choice(nice_guys, X.shape[0])
+    # set column names and types
+    X.columns = ["var" + str(i) for i in range(13)]
+    X["var11"] = X["var11"].astype("category")
+    X["nice_guys"] = np.random.choice(
+        [
+            "Rick",
+            "Bender",
+            "Cartman",
+            "Morty",
+            "Fry",
+            "Vador",
+            "Thanos",
+            "Bejita",
+            "Cell",
+            "Tinkywinky",
+            "Lecter",
+            "Alien",
+            "Terminator",
+            "Drago",
+            "Dracula",
+            "Krueger",
+            "Geoffrey",
+            "Goldfinder",
+            "Blackbeard",
+            "Excel",
+            "SAS",
+            "Bias",
+            "Variance",
+            "Scrum",
+            "Human",
+            "Garry",
+            "Coldplay",
+            "Imaginedragons",
+            "Platist",
+            "Creationist",
+            "Gruber",
+            "KeyserSoze",
+            "Luthor",
+            "Klaue",
+            "Bane",
+            "MarkZ",
+        ],
+        size,
+    )
 
     return X, y, w
 
 
-def _generated_corr_dataset_classification(size=1000):
-    """Generate artificial dataset for classification tasks. Some columns are
-    correlated, have no variance, large cardinality, numerical and categorical.
+def _make_corr_dataset_classification(size=1000):
+    """
+    Generate an artificial dataset for classification tasks. Some columns are correlated,
+    have no variance, large cardinality, numerical and categorical.
 
-    Parameters
-    ----------
-    size : int, optional
-        number of rows to generate, by default 1000
+    Parameters:
+        size (int): The number of rows to generate. Default is 1000.
 
-    Returns
-    -------
-    pd.DataFrame, pd.Series, pd.Series
-        the predictors matrix, the target and the weights
+    Returns:
+        tuple: A tuple containing the predictors matrix, the target, and the weights.
     """
-    # weights
+    # Generate weights
     w = np.random.beta(a=1, b=0.5, size=size)
-    # fixing the seed and the target
+
+    # Fix the seed and generate the target
     np.random.seed(42)
     y = np.random.binomial(1, 0.5, size)
+
+    # Generate the predictors matrix
     X = np.zeros((size, 13))
 
     z = y - np.random.binomial(1, 0.1, size) + np.random.binomial(1, 0.1, size)
     z[z == -1] = 0
     z[z == 2] = 1
 
-    # 5 relevant features, with positive and negative correlation to the target
+    # Generate 5 relevant features, with positive and negative correlation to the target
     X[:, 0] = z
     X[:, 1] = y * np.abs(np.random.normal(0, 1, size)) + np.random.normal(0, 0.1, size)
     X[:, 2] = -y + np.random.normal(0, 1, size)
     X[:, 3] = y**2 + np.random.normal(0, 1, size)
     X[:, 4] = np.sqrt(y) + np.random.binomial(2, 0.1, size)
 
-    # 5 irrelevant features
-    X[:, 5] = np.random.normal(0, 1, size)
-    X[:, 6] = np.random.poisson(1, size)
-    X[:, 7] = np.random.binomial(1, 0.3, size)
-    X[:, 8] = np.random.normal(0, 1, size)
-    X[:, 9] = np.random.poisson(1, size)
-    # zero variance
+    # Generate 5 irrelevant features
+    X[:, 5:10] = np.random.normal(0, 1, size=(size, 5))
+
+    # Generate a column with zero variance
     X[:, 10] = np.ones(size)
-    # high cardinality
+
+    # Generate a column with high cardinality
     X[:, 11] = np.arange(start=0, stop=size, step=1)
-    # a lot of missing values
+
+    # Generate a column with a lot of missing values
     idx_nan = np.random.choice(size, int(round(size / 2)), replace=False)
     X[:, 12] = y**3 + np.abs(np.random.normal(0, 1, size))
     X[idx_nan, 12] = np.nan
 
-    # make  it a pandas DF
+    # Make the predictors matrix a pandas DataFrame
     column_names = ["var" + str(i) for i in range(13)]
     column_names[11] = "dummy"
-    X = pd.DataFrame(X)
-    X.columns = column_names
+    X = pd.DataFrame(X, columns=column_names)
     X["dummy"] = X["dummy"].astype("category")
 
+    # Add a column of random values from a list
     nice_guys = [
         "Rick",
         "Bender",
         "Cartman",
         "Morty",
         "Fry",
         "Vador",
@@ -758,10 +852,7 @@
         "Gruber",
         "KeyserSoze",
         "Luthor",
         "Klaue",
         "Bane",
         "MarkZ",
     ]
-    X["nice_guys"] = np.random.choice(nice_guys, X.shape[0])
-
-    return X, y, w
```

### Comparing `arfs-1.0.7/src/arfs.egg-info/PKG-INFO` & `arfs-1.1.0/src/arfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.0.7
+Version: 1.1.0
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.0.7/src/arfs.egg-info/SOURCES.txt` & `arfs-1.1.0/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-1.0.7/tests/test_allrelevant.py` & `arfs-1.1.0/tests/test_allrelevant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import numpy as np
 import lightgbm as lgb
 from arfs.feature_selection.allrelevant import Leshy, BoostAGroota, GrootCV
 from arfs.utils import (
-    generated_corr_dataset_regr,
-    generated_corr_dataset_classification,
+    _generated_corr_dataset_regr,
+    _generated_corr_dataset_classification,
 )
 from arfs.utils import LightForestClassifier, LightForestRegressor
 
 
 class TestLeshy:
     """
     Test suite for all-relevant FS boruta-like method: Leshy
@@ -22,21 +22,21 @@
         # rfc = RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100)
         # bt = BorutaPy(rfc)
         # bt.fit(X.values, y)
         # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
 
         # lightGBM random forest implementation
         baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-        X, y, w = generated_corr_dataset_classification(size=100)
+        X, y, w = _generated_corr_dataset_classification(size=100)
         n_feat = X.shape[1]
         rfc = LightForestClassifier(n_feat)
         # RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100) # --> too slow
         arfs = Leshy(rfc, verbose=0, max_iter=10, random_state=42, importance="native")
         arfs.fit(X, y)
-        leshy_rfc_list = sorted(arfs.support_names_)
+        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
         assert bool(
             set(baseline_list) & set(leshy_rfc_list)
         ), "expect non-empty intersection"
 
     def test_borutaPy_vs_leshy_with_rfr_and_native_feature_importance(self):
@@ -47,21 +47,21 @@
         # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=100)
         # bt = BorutaPy(rfr)
         # bt.fit(X.values, y)
         # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
 
         # lightGBM random forest implementation
         baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-        X, y, w = generated_corr_dataset_regr(size=100)
+        X, y, w = _generated_corr_dataset_regr(size=100)
         n_feat = X.shape[1]
         rfr = LightForestRegressor(n_feat)
         # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=10)
         arfs = Leshy(rfr, verbose=0, max_iter=10, random_state=42, importance="native")
         arfs.fit(X, y)
-        leshy_rfc_list = sorted(arfs.support_names_)
+        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
         assert bool(
             set(baseline_list) & set(leshy_rfc_list)
         ), "expect non-empty intersection"
 
     def test_borutaPy_vs_leshy_with_rfc_and_shap_feature_importance(self):
@@ -72,20 +72,20 @@
         # rfc = RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100)
         # bt = BorutaPy(rfc)
         # bt.fit(X.values, y)
         # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
 
         # lightGBM random forest implementation
         baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-        X, y, w = generated_corr_dataset_classification(size=100)
+        X, y, w = _generated_corr_dataset_classification(size=100)
         n_feat = X.shape[1]
         model = LightForestClassifier(n_feat)
         arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
         arfs.fit(X, y)
-        leshy_rfc_list = sorted(arfs.support_names_)
+        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
         assert bool(
             set(baseline_list) & set(leshy_rfc_list)
         ), "expect non-empty intersection"
 
     def test_borutaPy_vs_leshy_with_rfr_and_shap_feature_importance(self):
@@ -96,47 +96,47 @@
         # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=100)
         # bt = BorutaPy(rfr)
         # bt.fit(X.values, y)
         # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
 
         # lightGBM random forest implementation
         baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-        X, y, w = generated_corr_dataset_regr(size=500)
+        X, y, w = _generated_corr_dataset_regr(size=500)
         n_feat = X.shape[1]
         model = LightForestRegressor(n_feat)
         arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
         arfs.fit(X, y)
-        leshy_rfc_list = sorted(arfs.support_names_)
+        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
         assert bool(
             set(baseline_list) & set(leshy_rfc_list)
         ), "expect non-empty intersection"
 
     def test_leshy_clf_with_lgb_and_shap_feature_importance_and_sample_weight(self):
         baseline_list = ["var0", "var1", "var2", "var3", "var4"]
 
-        X, y, w = generated_corr_dataset_classification(size=500)
+        X, y, w = _generated_corr_dataset_classification(size=500)
         model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
         arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
         arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.support_names_)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         assert bool(
             set(baseline_list) & set(leshy_list)
         ), "expect non-empty intersection"
 
     def test_leshy_regr_with_lgb_and_shap_feature_importance_and_sample_weight(self):
         baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
 
-        X, y, w = generated_corr_dataset_classification(size=500)
+        X, y, w = _generated_corr_dataset_classification(size=500)
         model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
         arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
         arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.support_names_)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         assert bool(
             set(baseline_list) & set(leshy_list)
         ), "expect non-empty intersection"
 
 
 class TestBoostAGroota:
@@ -145,123 +145,123 @@
     """
 
     def test_boostagroota_clf_with_lgb_and_shap_feature_importance_and_sample_weight(
         self,
     ):
         baseline_list = ["var0", "var1", "var2", "var3", "var4"]
 
-        X, y, w = generated_corr_dataset_classification(size=500)
+        X, y, w = _generated_corr_dataset_classification(size=500)
         model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
         arfs = BoostAGroota(
             est=model,
             cutoff=1,
             iters=3,
             max_rounds=3,
             delta=0.1,
             silent=False,
             importance="shap",
         )
         arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.support_names_)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         assert bool(
             set(baseline_list) & set(leshy_list)
         ), "expect non-empty intersection"
 
     def test_boostagroota_clf_with_lgb_and_pimp_feature_importance_and_sample_weight(
         self,
     ):
         baseline_list = ["var0", "var1", "var2", "var3", "var4"]
 
-        X, y, w = generated_corr_dataset_classification(size=500)
+        X, y, w = _generated_corr_dataset_classification(size=500)
         model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
         arfs = BoostAGroota(
             est=model,
             cutoff=1,
             iters=3,
             max_rounds=3,
             delta=0.1,
             silent=False,
             importance="pimp",
         )
         arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.support_names_)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         assert bool(
             set(baseline_list) & set(leshy_list)
         ), "expect non-empty intersection"
 
     def test_boostagroota_rgr_with_lgb_and_shap_feature_importance_and_sample_weight(
         self,
     ):
         baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
 
-        X, y, w = generated_corr_dataset_regr(size=500)
+        X, y, w = _generated_corr_dataset_regr(size=500)
         model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
         arfs = BoostAGroota(
             est=model,
             cutoff=1,
             iters=3,
             max_rounds=3,
             delta=0.1,
             silent=False,
             importance="shap",
         )
         arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.support_names_)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         assert bool(
             set(baseline_list) & set(leshy_list)
         ), "expect non-empty intersection"
 
     def test_boostagroota_regr_with_lgb_and_pimp_feature_importance_and_sample_weight(
         self,
     ):
         baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
 
-        X, y, w = generated_corr_dataset_regr(size=500)
+        X, y, w = _generated_corr_dataset_regr(size=500)
         model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
         arfs = BoostAGroota(
             est=model,
             cutoff=1,
             iters=3,
             max_rounds=3,
             delta=0.1,
             silent=False,
             importance="pimp",
         )
         arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.support_names_)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         assert bool(
             set(baseline_list) & set(leshy_list)
         ), "expect non-empty intersection"
 
 
 class TestGrootCV:
     """
     Test suite for all-relevant FS boruta-like method: Leshy
     """
 
     def test_grootcv_classification_with_and_sample_weight(self):
         baseline_list = ["var0", "var1", "var2", "var3", "var4"]
 
-        X, y, w = generated_corr_dataset_classification(size=100)
+        X, y, w = _generated_corr_dataset_classification(size=100)
         arfs = GrootCV(objective="binary", cutoff=1, n_folds=3, n_iter=3, silent=False)
         arfs.fit(X, y, w)
-        grootcv_list = sorted(arfs.support_names_)
+        grootcv_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         assert bool(
             set(baseline_list) & set(grootcv_list)
         ), "expect non-empty intersection"
 
     def test_grootcv_regression_with_and_sample_weight(self):
         baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
 
-        X, y, w = generated_corr_dataset_regr(size=100)
+        X, y, w = _generated_corr_dataset_regr(size=100)
         arfs = GrootCV(objective="l2", cutoff=1, n_folds=3, n_iter=3, silent=False)
         arfs.fit(X, y, w)
-        grootcv_list = sorted(arfs.support_names_)
+        grootcv_list = sorted(arfs.feature_names_in_[arfs.support_])
 
         assert bool(
             set(baseline_list) & set(grootcv_list)
         ), "expect non-empty intersection"
```

### Comparing `arfs-1.0.7/tests/test_featselect.py` & `arfs-1.1.0/tests/test_featselect.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
     Test suite for FeatureSelector, missing values
     """
 
     def test_identify_single_unique_classification(self):
         # not task dependent (same for clf and regr)
         X, y, w = _generated_corr_dataset_classification(size=10)
-        fs = UniqueValuesThreshold(threshold=1)
+        fs = UniqueValuesThreshold(threshold=2)
         fs.fit(X)
         message = "Expected: {0}, Actual: {1}".format(
             "var10", fs.not_selected_features_
         )
         assert fs.not_selected_features_ == ["var10"], message
 
 
@@ -51,18 +51,18 @@
     """
 
     def test_identify_high_cardinality_classification(self):
         # not task dependent (same for clf and regr)
         X, y, w = _generated_corr_dataset_classification(size=100)
         fs = CardinalityThreshold(threshold=5)
         fs.fit(X)
-        message = "Expected: {0}, Actual: {1}".format(
-            "emb_dummy", fs.not_selected_features_
-        )
-        assert fs.not_selected_features_ == ["emb_dummy"], message
+        expected = sorted(["dummy", "nice_guys"])
+        actual = sorted(list(fs.not_selected_features_))
+        message = "Expected: {0}, Actual: {1}".format(expected, actual)
+        assert actual == expected, message
 
 
 # class TestFeatSelectCollinearity:
 #     """
 #     test suite for FeatureSelector, high cardinality
 #     """
```

