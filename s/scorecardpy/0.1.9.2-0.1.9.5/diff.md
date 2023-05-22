# Comparing `tmp/scorecardpy-0.1.9.2.tar.gz` & `tmp/scorecardpy-0.1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scorecardpy-0.1.9.2.tar", last modified: Tue Apr 14 12:57:30 2020, max compression
+gzip compressed data, was "scorecardpy-0.1.9.5.tar", last modified: Mon May 22 14:52:15 2023, max compression
```

## Comparing `scorecardpy-0.1.9.2.tar` & `scorecardpy-0.1.9.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     1067 2018-04-24 03:25:44.000000 scorecardpy-0.1.9.2/LICENSE
--rwxrwxrwx   0 shichenxie   (501) staff       (20)      128 2018-04-24 03:52:54.000000 scorecardpy-0.1.9.2/MANIFEST.in
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     4422 2020-03-26 16:10:36.000000 scorecardpy-0.1.9.2/NEWS.md
--rw-r--r--   0 shichenxie   (501) staff       (20)     4919 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/PKG-INFO
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     3285 2020-02-24 13:15:32.000000 scorecardpy-0.1.9.2/README.md
-drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/scorecardpy/
--rwxrwxrwx   0 shichenxie   (501) staff       (20)      685 2020-01-15 15:05:55.000000 scorecardpy-0.1.9.2/scorecardpy/__init__.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     7096 2020-04-03 09:14:13.000000 scorecardpy-0.1.9.2/scorecardpy/condition_fun.py
-drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/scorecardpy/data/
--rw-r--r--   0 shichenxie   (501) staff       (20)   267041 2019-11-25 07:00:56.000000 scorecardpy-0.1.9.2/scorecardpy/data/germancredit.csv
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     3697 2018-07-20 02:45:30.000000 scorecardpy-0.1.9.2/scorecardpy/germancredit.py
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     6092 2018-05-22 08:16:36.000000 scorecardpy-0.1.9.2/scorecardpy/info_ent_indx_gini.py
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     4582 2019-09-10 14:47:10.000000 scorecardpy-0.1.9.2/scorecardpy/info_value.py
--rw-r--r--   0 shichenxie   (501) staff       (20)     4215 2018-12-18 08:12:56.000000 scorecardpy-0.1.9.2/scorecardpy/one_hot.py
--rwxrwxrwx   0 shichenxie   (501) staff       (20)    22105 2018-10-11 03:57:32.000000 scorecardpy-0.1.9.2/scorecardpy/perf.py
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     8573 2019-10-08 15:44:17.000000 scorecardpy-0.1.9.2/scorecardpy/scorecard.py
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     2360 2018-12-17 13:57:32.000000 scorecardpy-0.1.9.2/scorecardpy/split_df.py
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     5709 2019-09-10 15:02:37.000000 scorecardpy-0.1.9.2/scorecardpy/var_filter.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)    58467 2020-04-03 05:09:05.000000 scorecardpy-0.1.9.2/scorecardpy/woebin.py
-drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/scorecardpy.egg-info/
--rw-r--r--   0 shichenxie   (501) staff       (20)     4919 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/scorecardpy.egg-info/PKG-INFO
--rw-r--r--   0 shichenxie   (501) staff       (20)      535 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/scorecardpy.egg-info/SOURCES.txt
--rw-r--r--   0 shichenxie   (501) staff       (20)        1 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/scorecardpy.egg-info/dependency_links.txt
--rw-r--r--   0 shichenxie   (501) staff       (20)       53 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/scorecardpy.egg-info/requires.txt
--rw-r--r--   0 shichenxie   (501) staff       (20)       12 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/scorecardpy.egg-info/top_level.txt
--rw-r--r--   0 shichenxie   (501) staff       (20)       38 2020-04-14 12:57:30.000000 scorecardpy-0.1.9.2/setup.cfg
--rwxrwxrwx   0 shichenxie   (501) staff       (20)     2615 2019-11-10 12:13:39.000000 scorecardpy-0.1.9.2/setup.py
+drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-05-22 14:52:15.632632 scorecardpy-0.1.9.5/
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     1067 2018-04-24 03:25:44.000000 scorecardpy-0.1.9.5/LICENSE
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)      128 2018-04-24 03:52:54.000000 scorecardpy-0.1.9.5/MANIFEST.in
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     4638 2023-05-22 14:51:54.000000 scorecardpy-0.1.9.5/NEWS.md
+-rw-r--r--   0 shichenxie   (501) staff       (20)     4276 2023-05-22 14:52:15.632475 scorecardpy-0.1.9.5/PKG-INFO
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     3285 2020-02-24 13:15:32.000000 scorecardpy-0.1.9.5/README.md
+drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-05-22 14:52:15.629744 scorecardpy-0.1.9.5/scorecardpy/
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)      738 2023-05-22 14:51:13.000000 scorecardpy-0.1.9.5/scorecardpy/__init__.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     8078 2023-05-22 12:21:28.000000 scorecardpy-0.1.9.5/scorecardpy/condition_fun.py
+drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-05-22 14:52:15.631120 scorecardpy-0.1.9.5/scorecardpy/data/
+-rw-r--r--   0 shichenxie   (501) staff       (20)   268042 2020-11-30 13:17:38.000000 scorecardpy-0.1.9.5/scorecardpy/data/germancredit.csv
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     3697 2020-11-30 13:32:32.000000 scorecardpy-0.1.9.5/scorecardpy/germancredit.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     6092 2018-05-22 08:16:36.000000 scorecardpy-0.1.9.5/scorecardpy/info_ent_indx_gini.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     4582 2019-09-10 14:47:10.000000 scorecardpy-0.1.9.5/scorecardpy/info_value.py
+-rw-r--r--   0 shichenxie   (501) staff       (20)     4215 2018-12-18 08:12:56.000000 scorecardpy-0.1.9.5/scorecardpy/one_hot.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)    22105 2018-10-11 03:57:32.000000 scorecardpy-0.1.9.5/scorecardpy/perf.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)    12829 2023-05-22 14:47:43.000000 scorecardpy-0.1.9.5/scorecardpy/scorecard.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     2360 2020-10-11 10:21:02.000000 scorecardpy-0.1.9.5/scorecardpy/split_df.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     5709 2019-09-10 15:02:37.000000 scorecardpy-0.1.9.5/scorecardpy/var_filter.py
+-rw-r--r--   0 shichenxie   (501) staff       (20)     2274 2023-05-22 12:21:28.000000 scorecardpy-0.1.9.5/scorecardpy/vif.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)    59997 2023-05-22 12:21:28.000000 scorecardpy-0.1.9.5/scorecardpy/woebin.py
+drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-05-22 14:52:15.630976 scorecardpy-0.1.9.5/scorecardpy.egg-info/
+-rw-r--r--   0 shichenxie   (501) staff       (20)     4276 2023-05-22 14:52:15.000000 scorecardpy-0.1.9.5/scorecardpy.egg-info/PKG-INFO
+-rw-r--r--   0 shichenxie   (501) staff       (20)      554 2023-05-22 14:52:15.000000 scorecardpy-0.1.9.5/scorecardpy.egg-info/SOURCES.txt
+-rw-r--r--   0 shichenxie   (501) staff       (20)        1 2023-05-22 14:52:15.000000 scorecardpy-0.1.9.5/scorecardpy.egg-info/dependency_links.txt
+-rw-r--r--   0 shichenxie   (501) staff       (20)       70 2023-05-22 14:52:15.000000 scorecardpy-0.1.9.5/scorecardpy.egg-info/requires.txt
+-rw-r--r--   0 shichenxie   (501) staff       (20)       12 2023-05-22 14:52:15.000000 scorecardpy-0.1.9.5/scorecardpy.egg-info/top_level.txt
+-rw-r--r--   0 shichenxie   (501) staff       (20)       38 2023-05-22 14:52:15.632684 scorecardpy-0.1.9.5/setup.cfg
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     2775 2023-05-22 14:46:51.000000 scorecardpy-0.1.9.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scorecardpy-0.1.9.2/LICENSE` & `scorecardpy-0.1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.2/NEWS.md` & `scorecardpy-0.1.9.5/NEWS.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# scorecardpy 0.1.9.5
+* fixed a bug on woebin function caused by pandas update (by @CBravoR)
+* suppressed warnings in woebin function caused by groupby operations (by @CBravoR)
+* added new functions vif, scorecard2
+
 # scorecardpy 0.1.9.2
 * fixed a bug in woebin function caused by the new function explode in pandas >= 0.25
 * fixed a bug when intialzing binning
 * modified the method to create initial fine binning breaks.
 
 # scorecardpy 0.1.9
 * fixed a bug in scorecard_ply, supports card as a DataFrame
```

### Comparing `scorecardpy-0.1.9.2/PKG-INFO` & `scorecardpy-0.1.9.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,120 @@
 Metadata-Version: 2.1
 Name: scorecardpy
-Version: 0.1.9.2
+Version: 0.1.9.5
 Summary: Credit Risk Scorecard
 Home-page: http://github.com/shichenxie/scorecardpy
 Author: Shichen Xie
 Author-email: xie@shichen.name
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/shichenxie/scorecardpy/issues
 Project-URL: Source, https://github.com/shichenxie/scorecardpy/
-Description: # scorecardpy
-        
-        [![PyPI version](https://img.shields.io/pypi/pyversions/scorecardpy.svg)](https://pypi.python.org/pypi/scorecardpy)
-        [![PyPI release](https://img.shields.io/pypi/v/scorecardpy.svg)](https://pypi.python.org/pypi/scorecardpy)
-        [![Downloads](http://pepy.tech/badge/scorecardpy)](http://pepy.tech/project/scorecardpy)
-        [![Downloads](https://pepy.tech/badge/scorecardpy/month)](https://pepy.tech/project/scorecardpy/month)
-        
-        
-        This package is python version of R package [scorecard](https://github.com/ShichenXie/scorecard). 
-        Its goal is to make the development of traditional credit risk scorecard model easier and efficient by providing functions for some common tasks. 
-        - data partition (`split_df`)
-        - variable selection (`iv`, `var_filter`)
-        - weight of evidence (woe) binning (`woebin`, `woebin_plot`, `woebin_adj`, `woebin_ply`)
-        - scorecard scaling (`scorecard`, `scorecard_ply`)
-        - performance evaluation (`perf_eva`, `perf_psi`)
-        
-        ## Installation
-        
-        - Install the release version of `scorecardpy` from [PYPI](https://pypi.org/project/scorecardpy/) with:
-        ```
-        pip install scorecardpy
-        ```
-        
-        - Install the latest version of `scorecardpy` from [github](https://github.com/shichenxie/scorecardpy) with:
-        ```
-        pip install git+git://github.com/shichenxie/scorecardpy.git
-        ```
-        
-        ## Example
-        
-        This is a basic example which shows you how to develop a common credit risk scorecard:
-        
-        ``` python
-        # Traditional Credit Scoring Using Logistic Regression
-        import scorecardpy as sc
-        
-        # data prepare ------
-        # load germancredit data
-        dat = sc.germancredit()
-        
-        # filter variable via missing rate, iv, identical value rate
-        dt_s = sc.var_filter(dat, y="creditability")
-        
-        # breaking dt into train and test
-        train, test = sc.split_df(dt_s, 'creditability').values()
-        
-        # woe binning ------
-        bins = sc.woebin(dt_s, y="creditability")
-        # sc.woebin_plot(bins)
-        
-        # binning adjustment
-        # # adjust breaks interactively
-        # breaks_adj = sc.woebin_adj(dt_s, "creditability", bins) 
-        # # or specify breaks manually
-        breaks_adj = {
-            'age.in.years': [26, 35, 40],
-            'other.debtors.or.guarantors': ["none", "co-applicant%,%guarantor"]
-        }
-        bins_adj = sc.woebin(dt_s, y="creditability", breaks_list=breaks_adj)
-        
-        # converting train and test into woe values
-        train_woe = sc.woebin_ply(train, bins_adj)
-        test_woe = sc.woebin_ply(test, bins_adj)
-        
-        y_train = train_woe.loc[:,'creditability']
-        X_train = train_woe.loc[:,train_woe.columns != 'creditability']
-        y_test = test_woe.loc[:,'creditability']
-        X_test = test_woe.loc[:,train_woe.columns != 'creditability']
-        
-        # logistic regression ------
-        from sklearn.linear_model import LogisticRegression
-        lr = LogisticRegression(penalty='l1', C=0.9, solver='saga', n_jobs=-1)
-        lr.fit(X_train, y_train)
-        # lr.coef_
-        # lr.intercept_
-        
-        # predicted proability
-        train_pred = lr.predict_proba(X_train)[:,1]
-        test_pred = lr.predict_proba(X_test)[:,1]
-        
-        # performance ks & roc ------
-        train_perf = sc.perf_eva(y_train, train_pred, title = "train")
-        test_perf = sc.perf_eva(y_test, test_pred, title = "test")
-        
-        # score ------
-        card = sc.scorecard(bins_adj, lr, X_train.columns)
-        # credit score
-        train_score = sc.scorecard_ply(train, card, print_step=0)
-        test_score = sc.scorecard_ply(test, card, print_step=0)
-        
-        # psi
-        sc.perf_psi(
-          score = {'train':train_score, 'test':test_score},
-          label = {'train':y_train, 'test':y_test}
-        )
-        ```
-        
 Keywords: credit scorecard,woe binning,performace evaluation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# scorecardpy
+
+[![PyPI version](https://img.shields.io/pypi/pyversions/scorecardpy.svg)](https://pypi.python.org/pypi/scorecardpy)
+[![PyPI release](https://img.shields.io/pypi/v/scorecardpy.svg)](https://pypi.python.org/pypi/scorecardpy)
+[![Downloads](http://pepy.tech/badge/scorecardpy)](http://pepy.tech/project/scorecardpy)
+[![Downloads](https://pepy.tech/badge/scorecardpy/month)](https://pepy.tech/project/scorecardpy/month)
+
+
+This package is python version of R package [scorecard](https://github.com/ShichenXie/scorecard). 
+Its goal is to make the development of traditional credit risk scorecard model easier and efficient by providing functions for some common tasks. 
+- data partition (`split_df`)
+- variable selection (`iv`, `var_filter`)
+- weight of evidence (woe) binning (`woebin`, `woebin_plot`, `woebin_adj`, `woebin_ply`)
+- scorecard scaling (`scorecard`, `scorecard_ply`)
+- performance evaluation (`perf_eva`, `perf_psi`)
+
+## Installation
+
+- Install the release version of `scorecardpy` from [PYPI](https://pypi.org/project/scorecardpy/) with:
+```
+pip install scorecardpy
+```
+
+- Install the latest version of `scorecardpy` from [github](https://github.com/shichenxie/scorecardpy) with:
+```
+pip install git+git://github.com/shichenxie/scorecardpy.git
+```
+
+## Example
+
+This is a basic example which shows you how to develop a common credit risk scorecard:
+
+``` python
+# Traditional Credit Scoring Using Logistic Regression
+import scorecardpy as sc
+
+# data prepare ------
+# load germancredit data
+dat = sc.germancredit()
+
+# filter variable via missing rate, iv, identical value rate
+dt_s = sc.var_filter(dat, y="creditability")
+
+# breaking dt into train and test
+train, test = sc.split_df(dt_s, 'creditability').values()
+
+# woe binning ------
+bins = sc.woebin(dt_s, y="creditability")
+# sc.woebin_plot(bins)
+
+# binning adjustment
+# # adjust breaks interactively
+# breaks_adj = sc.woebin_adj(dt_s, "creditability", bins) 
+# # or specify breaks manually
+breaks_adj = {
+    'age.in.years': [26, 35, 40],
+    'other.debtors.or.guarantors': ["none", "co-applicant%,%guarantor"]
+}
+bins_adj = sc.woebin(dt_s, y="creditability", breaks_list=breaks_adj)
+
+# converting train and test into woe values
+train_woe = sc.woebin_ply(train, bins_adj)
+test_woe = sc.woebin_ply(test, bins_adj)
+
+y_train = train_woe.loc[:,'creditability']
+X_train = train_woe.loc[:,train_woe.columns != 'creditability']
+y_test = test_woe.loc[:,'creditability']
+X_test = test_woe.loc[:,train_woe.columns != 'creditability']
+
+# logistic regression ------
+from sklearn.linear_model import LogisticRegression
+lr = LogisticRegression(penalty='l1', C=0.9, solver='saga', n_jobs=-1)
+lr.fit(X_train, y_train)
+# lr.coef_
+# lr.intercept_
+
+# predicted proability
+train_pred = lr.predict_proba(X_train)[:,1]
+test_pred = lr.predict_proba(X_test)[:,1]
+
+# performance ks & roc ------
+train_perf = sc.perf_eva(y_train, train_pred, title = "train")
+test_perf = sc.perf_eva(y_test, test_pred, title = "test")
+
+# score ------
+card = sc.scorecard(bins_adj, lr, X_train.columns)
+# credit score
+train_score = sc.scorecard_ply(train, card, print_step=0)
+test_score = sc.scorecard_ply(test, card, print_step=0)
+
+# psi
+sc.perf_psi(
+  score = {'train':train_score, 'test':test_score},
+  label = {'train':y_train, 'test':y_test}
+)
+```
```

### Comparing `scorecardpy-0.1.9.2/README.md` & `scorecardpy-0.1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.2/scorecardpy/__init__.py` & `scorecardpy-0.1.9.5/scorecardpy/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from scorecardpy.germancredit import germancredit
 from scorecardpy.split_df import split_df
 from scorecardpy.info_value import iv
 # from .info_ent_indx_gini import (ig, ie)
 from scorecardpy.var_filter import var_filter
 from scorecardpy.woebin import (woebin, woebin_ply, woebin_plot, woebin_adj)
 from scorecardpy.perf import (perf_eva, perf_psi)
-from scorecardpy.scorecard import (scorecard, scorecard_ply)
+from scorecardpy.scorecard import (scorecard, scorecard_ply, scorecard2)
 from scorecardpy.one_hot import one_hot
+from scorecardpy.vif import vif
 
 
-__version__ = '0.1.9.2'
+__version__ = '0.1.9.5'
 
 __all__ = (
     germancredit,
     split_df, 
     iv,
     var_filter,
     woebin, woebin_ply, woebin_plot, woebin_adj,
     perf_eva, perf_psi,
     scorecard, scorecard_ply,
-    one_hot
+    one_hot,
+    vif
 )
```

### Comparing `scorecardpy-0.1.9.2/scorecardpy/condition_fun.py` & `scorecardpy-0.1.9.5/scorecardpy/condition_fun.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 # -*- coding: utf-8 -*-
 
 import pandas as pd
 import numpy as np
 import warnings
 import re
 from pandas.api.types import is_numeric_dtype
+import statsmodels.api as sm
+
+def lr(dt, y, x):
+  # dty
+  dty = dt.loc[:,y] 
+  # dtx
+  dtx = dt.loc[:,x] 
+  dtx = sm.add_constant(dtx)
+  # logistic regression
+  lrfit = sm.GLM(
+    dty.astype(float), 
+    dtx.astype(float), 
+    family=sm.families.Binomial()
+  ).fit()
+  return lrfit
 
 def str_to_list(x):
     if x is not None and isinstance(x, str):
         x = [x]
     return x
     
 # remove constant columns
@@ -52,21 +67,37 @@
 #' @import data.table
 #'
 def rep_blank_na(dat): # cant replace blank string in categorical value with nan
     # remove duplicated index
     if dat.index.duplicated().any():
         dat = dat.reset_index(drop = True)
         warnings.warn('There are duplicated index in dataset. The index has been reseted.')
-    
-    blank_cols = [i for i in list(dat) if dat[i].astype(str).str.findall(r'^\s*$').apply(lambda x:0 if len(x)==0 else 1).sum()>0]
+
+    # replace "" with NaN
+    blank_cols = [col for col in list(dat) if
+                  dat[col].astype(str).str.findall(r'^\s*$').apply(lambda x: 0 if len(x) == 0 else 1).sum() > 0]
     if len(blank_cols) > 0:
-        warnings.warn('There are blank strings in {} columns, which are replaced with NaN. \n (ColumnNames: {})'.format(len(blank_cols), ', '.join(blank_cols)))
-#        dat[dat == [' ','']] = np.nan
-#        dat2 = dat.apply(lambda x: x.str.strip()).replace(r'^\s*$', np.nan, regex=True)
-        dat.replace(r'^\s*$', np.nan, regex=True)
+        warnings.warn('There are blank strings in {} columns, which are replaced with NaN. \n (ColumnNames: {})'.format(
+            len(blank_cols), ', '.join(blank_cols)))
+        #        dat[dat == [' ','']] = np.nan
+        #        dat2 = dat.apply(lambda x: x.str.strip()).replace(r'^\s*$', np.nan, regex=True)
+        for col in blank_cols:
+            dat.loc[dat[col] == "", col] = np.nan
+
+    # replace inf with -999
+    cols_num = [col for col in list(dat) if col not in blank_cols]
+    if len(cols_num) > 0:
+        cols_inf = [col for col in cols_num if
+                        any(dat[col] == np.inf) | any(dat[col] == -np.inf)]
+        if len(cols_inf) > 0:
+            warnings.warn(
+                'There are infinite or NaN values in {} columns, which are replaced with -999.\n (ColumnNames: {})'.format(
+                    len(cols_inf), ', '.join(cols_inf)))
+            for col in cols_inf:
+                dat.loc[(dat[col] == np.inf) | (dat[col] == -np.inf), col] = -999
     
     return dat
 
 
 # check y
 #' @import data.table
 #'
@@ -74,16 +105,14 @@
     positive = str(positive)
     # ncol of dt
     if not isinstance(dat, pd.DataFrame):
         raise Exception("Incorrect inputs; dat should be a DataFrame.")
     elif dat.shape[1] <= 1:
         raise Exception("Incorrect inputs; dat should be a DataFrame with at least two columns.")
 
-
-    
     # y ------
     y = str_to_list(y)
     # length of y == 1
     if len(y) != 1:
         raise Exception("Incorrect inputs; the length of y should be one")
     
     y = y[0]
@@ -93,15 +122,14 @@
     
     # remove na in y
     if dat[y].isnull().any():
         warnings.warn("There are NaNs in \'{}\' column. The rows with NaN in \'{}\' were removed from dat.".format(y,y))
         dat = dat.dropna(subset=[y])
         # dat = dat[pd.notna(dat[y])]
     
-    
     # numeric y to int
     if is_numeric_dtype(dat[y]):
         dat.loc[:,y] = dat[y].apply(lambda x: x if pd.isnull(x) else int(x)) #dat[y].astype(int)
     # length of unique values in y
     unique_y = np.unique(dat[y].values)
     if len(unique_y) == 2:
         # if [v not in [0,1] for v in unique_y] == [True, True]:
```

### Comparing `scorecardpy-0.1.9.2/scorecardpy/data/germancredit.csv` & `scorecardpy-0.1.9.5/scorecardpy/data/germancredit.csv`

 * *Files 12% similar despite different names*

```diff
@@ -1,1001 +1,1001 @@
-status.of.existing.checking.account,duration.in.month,credit.history,purpose,credit.amount,savings.account.and.bonds,present.employment.since,installment.rate.in.percentage.of.disposable.income,personal.status.and.sex,other.debtors.or.guarantors,present.residence.since,property,age.in.years,other.installment.plans,housing,number.of.existing.credits.at.this.bank,job,number.of.people.being.liable.to.provide.maintenance.for,telephone,foreign.worker,creditability
-... < 0 DM,6,critical account/ other credits existing (not at this bank),radio/television,1169,unknown/ no savings account,... >= 7 years,4,male : divorced/separated,none,4,real estate,67,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,48,existing credits paid back duly till now,radio/television,5951,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,real estate,22,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),education,2096,... < 100 DM,4 <= ... < 7 years,2,male : divorced/separated,none,3,real estate,49,none,own,1,unskilled - resident,2,none,yes,good
-... < 0 DM,42,existing credits paid back duly till now,furniture/equipment,7882,... < 100 DM,4 <= ... < 7 years,2,male : divorced/separated,guarantor,4,building society savings agreement/ life insurance,45,none,for free,1,skilled employee / official,2,none,yes,good
-... < 0 DM,24,delay in paying off in the past,car (new),4870,... < 100 DM,1 <= ... < 4 years,3,male : divorced/separated,none,4,unknown / no property,53,none,for free,2,skilled employee / official,2,none,yes,bad
-no checking account,36,existing credits paid back duly till now,education,9055,unknown/ no savings account,1 <= ... < 4 years,2,male : divorced/separated,none,4,unknown / no property,35,none,for free,1,unskilled - resident,2,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,furniture/equipment,2835,500 <= ... < 1000 DM,... >= 7 years,3,male : divorced/separated,none,4,building society savings agreement/ life insurance,53,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,car (used),6948,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",35,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,3059,... >= 1000 DM,4 <= ... < 7 years,2,male : divorced/separated,none,4,real estate,61,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,30,critical account/ other credits existing (not at this bank),car (new),5234,... < 100 DM,unemployed,4,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),1295,... < 100 DM,... < 1 year,3,male : divorced/separated,none,1,"car or other, not in attribute Savings account/bonds",25,none,rent,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,48,existing credits paid back duly till now,business,4308,... < 100 DM,... < 1 year,3,male : divorced/separated,none,4,building society savings agreement/ life insurance,24,none,rent,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1567,... < 100 DM,1 <= ... < 4 years,1,male : divorced/separated,none,1,"car or other, not in attribute Savings account/bonds",22,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,critical account/ other credits existing (not at this bank),car (new),1199,... < 100 DM,... >= 7 years,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",60,none,own,2,unskilled - resident,1,none,yes,bad
-... < 0 DM,15,existing credits paid back duly till now,car (new),1403,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,radio/television,1282,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,1,unskilled - resident,1,none,yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2424,unknown/ no savings account,... >= 7 years,4,male : divorced/separated,none,4,building society savings agreement/ life insurance,53,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,30,no credits taken/ all credits paid back duly,business,8072,unknown/ no savings account,... < 1 year,2,male : divorced/separated,none,3,"car or other, not in attribute Savings account/bonds",25,bank,own,3,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (used),12579,... < 100 DM,... >= 7 years,4,male : divorced/separated,none,2,unknown / no property,44,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,24,existing credits paid back duly till now,radio/television,3430,500 <= ... < 1000 DM,... >= 7 years,3,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,9,critical account/ other credits existing (not at this bank),car (new),2134,... < 100 DM,1 <= ... < 4 years,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",48,none,own,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,6,existing credits paid back duly till now,radio/television,2647,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : divorced/separated,none,3,real estate,44,none,rent,1,skilled employee / official,2,none,yes,good
-... < 0 DM,10,critical account/ other credits existing (not at this bank),car (new),2241,... < 100 DM,... < 1 year,1,male : divorced/separated,none,3,real estate,48,none,rent,2,unskilled - resident,2,none,no,good
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (used),1804,100 <= ... < 500 DM,... < 1 year,3,male : divorced/separated,none,4,building society savings agreement/ life insurance,44,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,10,critical account/ other credits existing (not at this bank),furniture/equipment,2069,unknown/ no savings account,1 <= ... < 4 years,2,male : divorced/separated,none,1,"car or other, not in attribute Savings account/bonds",26,none,own,2,skilled employee / official,1,none,no,good
-... < 0 DM,6,existing credits paid back duly till now,furniture/equipment,1374,... < 100 DM,1 <= ... < 4 years,1,male : divorced/separated,none,2,real estate,36,bank,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-no checking account,6,no credits taken/ all credits paid back duly,radio/television,426,... < 100 DM,... >= 7 years,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",39,none,own,1,unskilled - resident,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,all credits at this bank paid back duly,radio/television,409,... >= 1000 DM,1 <= ... < 4 years,3,male : divorced/separated,none,3,real estate,42,none,rent,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,7,existing credits paid back duly till now,radio/television,2415,... < 100 DM,1 <= ... < 4 years,3,male : divorced/separated,guarantor,2,real estate,34,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,60,delay in paying off in the past,business,6836,... < 100 DM,... >= 7 years,3,male : divorced/separated,none,4,unknown / no property,63,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,18,existing credits paid back duly till now,business,1913,... >= 1000 DM,... < 1 year,3,male : divorced/separated,none,3,real estate,36,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,4020,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",27,stores,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,car (new),5866,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),business,1264,unknown/ no savings account,... >= 7 years,4,male : divorced/separated,none,4,unknown / no property,57,none,rent,1,unskilled - resident,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,furniture/equipment,1474,... < 100 DM,... < 1 year,4,male : divorced/separated,none,1,building society savings agreement/ life insurance,33,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,45,critical account/ other credits existing (not at this bank),radio/television,4746,... < 100 DM,... < 1 year,4,male : divorced/separated,none,2,building society savings agreement/ life insurance,25,none,own,2,unskilled - resident,1,none,yes,bad
-no checking account,48,critical account/ other credits existing (not at this bank),education,6110,... < 100 DM,1 <= ... < 4 years,1,male : divorced/separated,none,3,unknown / no property,31,bank,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,18,existing credits paid back duly till now,radio/television,2100,... < 100 DM,1 <= ... < 4 years,4,male : divorced/separated,co-applicant,2,real estate,37,stores,own,1,skilled employee / official,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,10,existing credits paid back duly till now,domestic appliances,1225,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",37,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,458,... < 100 DM,1 <= ... < 4 years,4,male : divorced/separated,none,3,real estate,24,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,30,existing credits paid back duly till now,radio/television,2333,500 <= ... < 1000 DM,... >= 7 years,4,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",30,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1158,500 <= ... < 1000 DM,1 <= ... < 4 years,3,male : divorced/separated,none,1,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,delay in paying off in the past,repairs,6204,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,4,real estate,44,none,own,1,unskilled - resident,2,"yes, registered under the customers name",yes,good
-... < 0 DM,30,critical account/ other credits existing (not at this bank),car (used),6187,100 <= ... < 500 DM,4 <= ... < 7 years,1,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",24,none,rent,2,skilled employee / official,1,none,yes,good
-... < 0 DM,48,critical account/ other credits existing (not at this bank),car (used),6143,... < 100 DM,... >= 7 years,4,male : divorced/separated,none,4,unknown / no property,58,stores,for free,2,unskilled - resident,1,none,yes,bad
-no checking account,11,critical account/ other credits existing (not at this bank),car (new),1393,... < 100 DM,... < 1 year,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",35,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-no checking account,36,existing credits paid back duly till now,radio/television,2299,500 <= ... < 1000 DM,... >= 7 years,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",39,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,6,existing credits paid back duly till now,car (used),1352,500 <= ... < 1000 DM,unemployed,1,male : divorced/separated,none,2,building society savings agreement/ life insurance,23,none,rent,1,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,good
-no checking account,11,critical account/ other credits existing (not at this bank),car (new),7228,... < 100 DM,1 <= ... < 4 years,1,male : divorced/separated,none,4,building society savings agreement/ life insurance,39,none,own,2,unskilled - resident,1,none,yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,2073,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : divorced/separated,co-applicant,2,real estate,28,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,24,delay in paying off in the past,furniture/equipment,2333,unknown/ no savings account,... < 1 year,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,29,bank,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,27,delay in paying off in the past,car (used),5965,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,1262,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,car (used),3378,unknown/ no savings account,1 <= ... < 4 years,2,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,31,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,36,delay in paying off in the past,car (new),2225,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,57,bank,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,6,all credits at this bank paid back duly,car (new),783,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,guarantor,2,real estate,26,stores,own,1,unskilled - resident,2,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,6468,unknown/ no savings account,unemployed,2,female : divorced/separated/married,none,1,unknown / no property,52,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,36,critical account/ other credits existing (not at this bank),radio/television,9566,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,stores,own,2,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,18,existing credits paid back duly till now,car (new),1961,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",23,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-... < 0 DM,36,critical account/ other credits existing (not at this bank),furniture/equipment,6229,... < 100 DM,... < 1 year,4,female : divorced/separated/married,co-applicant,4,unknown / no property,23,none,rent,2,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,9,existing credits paid back duly till now,business,1391,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,1,real estate,27,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,15,critical account/ other credits existing (not at this bank),radio/television,1537,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,guarantor,4,real estate,50,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,36,no credits taken/ all credits paid back duly,business,1953,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,61,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,business,14421,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,24,existing credits paid back duly till now,radio/television,3181,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,27,existing credits paid back duly till now,repairs,5190,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,48,none,own,4,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,2171,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",29,bank,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),1007,... >= 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,real estate,22,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,36,existing credits paid back duly till now,education,1819,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,unknown / no property,37,stores,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,36,existing credits paid back duly till now,radio/television,2394,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",25,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,36,existing credits paid back duly till now,car (used),8133,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,30,bank,own,1,skilled employee / official,1,none,yes,good
-no checking account,7,critical account/ other credits existing (not at this bank),radio/television,730,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,46,none,rent,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
-... < 0 DM,8,critical account/ other credits existing (not at this bank),others,1164,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,51,bank,for free,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,42,critical account/ other credits existing (not at this bank),business,5954,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,1,real estate,41,bank,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,education,1977,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,40,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,12,critical account/ other credits existing (not at this bank),car (used),1526,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,66,none,for free,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-... < 0 DM,42,existing credits paid back duly till now,radio/television,3965,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,11,delay in paying off in the past,radio/television,4771,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,51,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,54,no credits taken/ all credits paid back duly,car (used),9436,unknown/ no savings account,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,39,none,own,1,unskilled - resident,2,none,yes,good
-0 <= ... < 200 DM,30,existing credits paid back duly till now,furniture/equipment,3832,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,22,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,5943,unknown/ no savings account,... < 1 year,1,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",44,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,15,existing credits paid back duly till now,radio/television,1213,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,47,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,18,existing credits paid back duly till now,business,1568,100 <= ... < 500 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,24,none,rent,1,unskilled - resident,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,others,1755,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,guarantor,4,real estate,58,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-... < 0 DM,10,existing credits paid back duly till now,radio/television,2315,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,real estate,52,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),business,1412,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,2,real estate,29,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,1295,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,education,12612,100 <= ... < 500 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,unknown / no property,47,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
-... < 0 DM,18,existing credits paid back duly till now,car (new),2249,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-... < 0 DM,12,no credits taken/ all credits paid back duly,repairs,1108,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,real estate,28,none,own,2,skilled employee / official,1,none,yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,618,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,56,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,12,critical account/ other credits existing (not at this bank),car (used),1409,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,3,real estate,54,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,797,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,33,bank,own,1,unskilled - resident,2,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,24,critical account/ other credits existing (not at this bank),furniture/equipment,3617,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,co-applicant,4,unknown / no property,20,none,rent,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),1318,... >= 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,54,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,54,no credits taken/ all credits paid back duly,business,15945,... < 100 DM,... < 1 year,3,female : divorced/separated/married,none,4,unknown / no property,58,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),education,2012,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",61,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,business,2622,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,36,critical account/ other credits existing (not at this bank),radio/television,2337,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,36,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,20,delay in paying off in the past,car (used),7057,unknown/ no savings account,4 <= ... < 7 years,3,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,36,bank,rent,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,car (new),1469,100 <= ... < 500 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,41,none,rent,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,radio/television,2323,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",24,none,rent,1,skilled employee / official,1,none,yes,good
-no checking account,6,delay in paying off in the past,radio/television,932,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,real estate,24,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,9,critical account/ other credits existing (not at this bank),furniture/equipment,1919,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",35,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,car (used),2445,unknown/ no savings account,... < 1 year,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",26,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),others,11938,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,co-applicant,3,"car or other, not in attribute Savings account/bonds",39,none,own,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,bad
-no checking account,18,all credits at this bank paid back duly,car (new),6458,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,39,bank,own,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),6078,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,7721,unknown/ no savings account,... < 1 year,1,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,30,none,own,1,skilled employee / official,1,"yes, registered under the customers name",no,good
-0 <= ... < 200 DM,14,existing credits paid back duly till now,business,1410,500 <= ... < 1000 DM,... >= 7 years,1,female : divorced/separated/married,none,2,real estate,35,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,6,delay in paying off in the past,business,1449,100 <= ... < 500 DM,... >= 7 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,bank,own,2,skilled employee / official,2,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,15,existing credits paid back duly till now,education,392,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,23,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,car (new),6260,... < 100 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,3,real estate,28,none,rent,1,unskilled - resident,1,none,yes,good
-no checking account,36,critical account/ other credits existing (not at this bank),car (new),7855,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,25,stores,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,12,existing credits paid back duly till now,radio/television,1680,500 <= ... < 1000 DM,... >= 7 years,3,female : divorced/separated/married,none,1,real estate,35,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,48,critical account/ other credits existing (not at this bank),radio/television,3578,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,1,real estate,47,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,42,existing credits paid back duly till now,radio/television,7174,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,10,critical account/ other credits existing (not at this bank),furniture/equipment,2132,unknown/ no savings account,... < 1 year,2,female : divorced/separated/married,co-applicant,3,real estate,27,none,rent,2,skilled employee / official,1,none,no,good
-... < 0 DM,33,critical account/ other credits existing (not at this bank),furniture/equipment,4281,500 <= ... < 1000 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",23,none,own,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (new),2366,500 <= ... < 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",36,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,21,existing credits paid back duly till now,radio/television,1835,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,real estate,25,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),car (used),3868,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",41,none,rent,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,furniture/equipment,1768,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,real estate,24,none,rent,1,unskilled - resident,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,10,critical account/ other credits existing (not at this bank),car (new),781,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,63,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,furniture/equipment,1924,unknown/ no savings account,... < 1 year,4,female : divorced/separated/married,none,3,real estate,27,none,rent,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),2121,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,30,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,radio/television,701,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,40,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,repairs,639,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (used),1860,... < 100 DM,unemployed,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),3499,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,co-applicant,2,real estate,29,none,own,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,48,existing credits paid back duly till now,car (new),8487,unknown/ no savings account,4 <= ... < 7 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,36,delay in paying off in the past,education,6887,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,29,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,15,existing credits paid back duly till now,furniture/equipment,2708,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,27,bank,own,2,unskilled - resident,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,furniture/equipment,1984,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,unknown / no property,47,bank,for free,2,skilled employee / official,1,none,yes,good
-no checking account,60,existing credits paid back duly till now,radio/television,10144,100 <= ... < 500 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,4,real estate,21,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,1240,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,real estate,38,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,27,delay in paying off in the past,car (used),8613,... >= 1000 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,766,500 <= ... < 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,real estate,66,none,own,1,unskilled - resident,1,none,yes,bad
-0 <= ... < 200 DM,15,critical account/ other credits existing (not at this bank),radio/television,2728,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,guarantor,2,real estate,35,bank,own,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,radio/television,1881,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",44,none,rent,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,6,existing credits paid back duly till now,car (new),709,... >= 1000 DM,... < 1 year,2,female : divorced/separated/married,none,2,real estate,27,none,own,1,unemployed/ unskilled - non-resident,1,none,no,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,radio/television,4795,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,1,unknown / no property,30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,27,existing credits paid back duly till now,radio/television,3416,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,2462,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",22,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,21,critical account/ other credits existing (not at this bank),furniture/equipment,2288,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,23,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,48,all credits at this bank paid back duly,business,3566,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),860,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,none,4,unknown / no property,39,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),car (new),682,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",51,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,36,critical account/ other credits existing (not at this bank),furniture/equipment,5371,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,guarantor,2,building society savings agreement/ life insurance,28,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1582,... >= 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",46,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,6,existing credits paid back duly till now,radio/television,1346,100 <= ... < 500 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,42,bank,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,10,existing credits paid back duly till now,radio/television,1924,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,38,none,own,1,skilled employee / official,1,"yes, registered under the customers name",no,good
-... >= 200 DM / salary assignments for at least 1 year,36,existing credits paid back duly till now,radio/television,5848,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),car (used),7758,... >= 1000 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,29,none,rent,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,24,delay in paying off in the past,business,6967,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",36,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1282,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",20,none,rent,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,9,critical account/ other credits existing (not at this bank),repairs,1288,100 <= ... < 500 DM,... >= 7 years,3,female : divorced/separated/married,guarantor,4,real estate,48,none,own,2,skilled employee / official,2,none,no,good
-... < 0 DM,12,all credits at this bank paid back duly,retraining,339,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",45,bank,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),3512,100 <= ... < 500 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",38,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1898,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,real estate,34,none,own,2,unskilled - resident,2,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2872,100 <= ... < 500 DM,... >= 7 years,3,female : divorced/separated/married,none,4,real estate,36,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),car (new),1055,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,30,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,15,existing credits paid back duly till now,domestic appliances,1262,500 <= ... < 1000 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,36,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,10,existing credits paid back duly till now,car (new),7308,... < 100 DM,unemployed,2,female : divorced/separated/married,none,4,unknown / no property,70,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,36,existing credits paid back duly till now,car (new),909,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,36,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,6,existing credits paid back duly till now,furniture/equipment,2978,500 <= ... < 1000 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,1131,... < 100 DM,unemployed,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,11,existing credits paid back duly till now,furniture/equipment,1577,... >= 1000 DM,... < 1 year,4,female : divorced/separated/married,none,1,real estate,20,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,furniture/equipment,3972,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,25,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),business,1935,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,31,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,15,no credits taken/ all credits paid back duly,car (new),950,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",33,none,rent,2,skilled employee / official,2,none,yes,bad
-no checking account,12,existing credits paid back duly till now,furniture/equipment,763,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,real estate,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,delay in paying off in the past,furniture/equipment,2064,... < 100 DM,unemployed,3,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,34,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,8,existing credits paid back duly till now,radio/television,1414,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,2,real estate,33,none,own,1,skilled employee / official,1,none,no,good
-... < 0 DM,21,delay in paying off in the past,education,3414,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,26,none,own,2,skilled employee / official,1,none,yes,bad
-no checking account,30,all credits at this bank paid back duly,car (used),7485,unknown/ no savings account,unemployed,4,female : divorced/separated/married,none,1,real estate,53,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,2577,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,6,critical account/ other credits existing (not at this bank),radio/television,338,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",52,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,1963,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,none,rent,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-... < 0 DM,21,critical account/ other credits existing (not at this bank),car (new),571,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,65,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,36,delay in paying off in the past,business,9572,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,36,delay in paying off in the past,business,4455,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,30,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,21,all credits at this bank paid back duly,car (new),1647,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,40,none,own,2,unskilled - resident,2,none,yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),furniture/equipment,3777,... >= 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,real estate,50,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),car (new),884,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",36,bank,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
-no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1360,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,31,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,9,all credits at this bank paid back duly,car (used),5129,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,74,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,16,critical account/ other credits existing (not at this bank),car (new),1175,... < 100 DM,unemployed,2,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",68,none,for free,3,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,radio/television,674,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,20,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,18,no credits taken/ all credits paid back duly,furniture/equipment,3244,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",33,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,business,4591,... >= 1000 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,54,none,own,3,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,business,3844,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,unknown / no property,34,none,for free,1,unskilled - resident,2,none,yes,bad
-0 <= ... < 200 DM,27,existing credits paid back duly till now,business,3915,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",36,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
-no checking account,6,existing credits paid back duly till now,radio/television,2108,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,2,real estate,29,none,rent,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,45,existing credits paid back duly till now,radio/television,3031,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,4,building society savings agreement/ life insurance,21,none,rent,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,9,critical account/ other credits existing (not at this bank),education,1501,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1382,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,951,100 <= ... < 500 DM,... < 1 year,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",27,bank,rent,4,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (used),2760,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,36,bank,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,delay in paying off in the past,furniture/equipment,4297,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,3,unknown / no property,40,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,9,critical account/ other credits existing (not at this bank),education,936,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",52,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,car (new),1168,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,real estate,27,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,27,delay in paying off in the past,business,5117,... < 100 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",26,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,retraining,902,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,21,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),car (new),1495,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,1,real estate,38,none,own,2,unskilled - resident,2,none,yes,good
-... < 0 DM,30,critical account/ other credits existing (not at this bank),car (used),10623,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,38,none,for free,3,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,1935,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,43,none,own,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),domestic appliances,1424,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,business,6568,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",21,stores,own,1,unskilled - resident,1,none,yes,good
-no checking account,12,existing credits paid back duly till now,car (used),1413,... >= 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,55,none,own,1,skilled employee / official,1,none,no,good
-no checking account,9,critical account/ other credits existing (not at this bank),radio/television,3074,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,real estate,33,none,own,2,skilled employee / official,2,none,yes,good
-no checking account,36,existing credits paid back duly till now,radio/television,3835,unknown/ no savings account,... >= 7 years,2,female : divorced/separated/married,none,4,real estate,45,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-... < 0 DM,27,no credits taken/ all credits paid back duly,business,5293,... < 100 DM,unemployed,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,50,stores,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... >= 200 DM / salary assignments for at least 1 year,30,delay in paying off in the past,business,1908,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,66,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,36,critical account/ other credits existing (not at this bank),radio/television,3342,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",51,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,6,critical account/ other credits existing (not at this bank),retraining,932,unknown/ no savings account,4 <= ... < 7 years,1,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,39,none,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,18,no credits taken/ all credits paid back duly,business,3104,... < 100 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,31,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,36,existing credits paid back duly till now,radio/television,3913,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,23,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,3021,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,24,none,rent,1,unskilled - resident,1,none,yes,good
-no checking account,10,existing credits paid back duly till now,car (new),1364,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",64,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,625,... < 100 DM,... < 1 year,4,female : divorced/separated/married,guarantor,1,real estate,26,bank,own,1,unskilled - resident,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,education,1200,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,23,bank,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,707,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,30,bank,own,2,skilled employee / official,1,none,yes,good
-no checking account,24,delay in paying off in the past,business,2978,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,real estate,32,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,15,existing credits paid back duly till now,car (used),4657,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,36,no credits taken/ all credits paid back duly,repairs,2613,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,48,existing credits paid back duly till now,radio/television,10961,... >= 1000 DM,4 <= ... < 7 years,1,female : divorced/separated/married,co-applicant,2,unknown / no property,27,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,7865,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,53,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,9,existing credits paid back duly till now,radio/television,1478,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",22,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,3149,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,1,unknown / no property,22,bank,for free,1,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,36,existing credits paid back duly till now,radio/television,4210,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,9,existing credits paid back duly till now,car (new),2507,500 <= ... < 1000 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,51,none,for free,1,unskilled - resident,1,none,yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,2141,100 <= ... < 500 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,1,unknown / no property,35,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,radio/television,866,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,2,real estate,25,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,4,critical account/ other credits existing (not at this bank),radio/television,1544,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,1,real estate,42,none,own,3,unskilled - resident,2,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,radio/television,1823,... < 100 DM,unemployed,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,stores,own,1,management/ self-employed/ highly qualified employee/ officer,2,none,yes,bad
-0 <= ... < 200 DM,6,existing credits paid back duly till now,car (new),14555,unknown/ no savings account,unemployed,1,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,23,none,own,1,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,21,existing credits paid back duly till now,business,2767,100 <= ... < 500 DM,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",61,bank,rent,2,unskilled - resident,1,none,yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,1291,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,35,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,30,existing credits paid back duly till now,radio/television,2522,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,guarantor,3,building society savings agreement/ life insurance,39,none,own,1,skilled employee / official,2,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,car (new),915,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",29,bank,own,1,skilled employee / official,1,none,yes,bad
-no checking account,6,existing credits paid back duly till now,radio/television,1595,... < 100 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,51,none,own,1,skilled employee / official,2,none,yes,good
-... < 0 DM,48,no credits taken/ all credits paid back duly,car (used),4605,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,24,none,for free,2,skilled employee / official,2,none,yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),business,1185,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,real estate,27,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,12,all credits at this bank paid back duly,retraining,3447,500 <= ... < 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,real estate,35,none,own,1,unskilled - resident,2,none,yes,good
-no checking account,24,existing credits paid back duly till now,business,1258,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,1,real estate,25,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,717,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,52,none,own,3,skilled employee / official,1,none,yes,good
-no checking account,6,no credits taken/ all credits paid back duly,car (new),1204,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,unknown / no property,35,bank,rent,1,skilled employee / official,1,none,no,good
-... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,furniture/equipment,1925,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,26,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,radio/television,433,... < 100 DM,unemployed,3,female : divorced/separated/married,co-applicant,4,real estate,22,none,rent,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),666,... >= 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,4,real estate,39,none,own,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,furniture/equipment,2251,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",46,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,30,existing credits paid back duly till now,car (new),2150,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,2,unknown / no property,24,bank,own,1,skilled employee / official,1,none,yes,bad
-no checking account,24,delay in paying off in the past,furniture/equipment,4151,100 <= ... < 500 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,35,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,furniture/equipment,2030,unknown/ no savings account,4 <= ... < 7 years,2,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,60,delay in paying off in the past,radio/television,7418,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,none,1,real estate,27,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2684,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,35,none,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,12,all credits at this bank paid back duly,radio/television,2149,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,unknown / no property,29,none,for free,1,skilled employee / official,1,none,yes,bad
-no checking account,15,existing credits paid back duly till now,car (used),3812,100 <= ... < 500 DM,... < 1 year,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",23,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,11,critical account/ other credits existing (not at this bank),radio/television,1154,100 <= ... < 500 DM,unemployed,4,female : divorced/separated/married,none,4,real estate,57,none,own,3,unskilled - resident,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1657,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,27,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,radio/television,1603,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",55,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,18,critical account/ other credits existing (not at this bank),car (new),5302,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,36,none,for free,3,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),education,2748,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,57,bank,for free,3,unskilled - resident,1,none,yes,good
-no checking account,10,critical account/ other credits existing (not at this bank),car (new),1231,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,real estate,32,none,own,2,unskilled - resident,2,none,no,good
-0 <= ... < 200 DM,15,existing credits paid back duly till now,radio/television,802,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",37,none,own,1,skilled employee / official,2,none,yes,bad
-no checking account,36,critical account/ other credits existing (not at this bank),business,6304,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,36,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,1533,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",38,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,14,existing credits paid back duly till now,car (new),8978,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,45,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",no,bad
-no checking account,24,existing credits paid back duly till now,radio/television,999,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,car (new),2662,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,32,none,own,1,skilled employee / official,1,none,no,good
-no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,1402,500 <= ... < 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",37,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,48,all credits at this bank paid back duly,car (new),12169,unknown/ no savings account,unemployed,4,female : divorced/separated/married,co-applicant,4,unknown / no property,36,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,48,existing credits paid back duly till now,radio/television,3060,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,real estate,28,none,own,2,skilled employee / official,1,none,yes,bad
-... < 0 DM,30,existing credits paid back duly till now,repairs,11998,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,1,unknown / no property,34,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-no checking account,9,existing credits paid back duly till now,radio/television,2697,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,real estate,32,none,own,1,skilled employee / official,2,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,2404,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1262,unknown/ no savings account,... >= 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,49,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-no checking account,6,existing credits paid back duly till now,furniture/equipment,4611,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,32,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,24,existing credits paid back duly till now,radio/television,1901,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",29,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),car (used),3368,... >= 1000 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,23,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,furniture/equipment,1574,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,50,none,own,1,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,18,all credits at this bank paid back duly,radio/television,1445,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",49,bank,own,1,unskilled - resident,1,none,yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),furniture/equipment,1520,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,63,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),car (new),3878,100 <= ... < 500 DM,... < 1 year,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",37,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,47,existing credits paid back duly till now,car (new),10722,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,1,real estate,35,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-... < 0 DM,48,existing credits paid back duly till now,car (used),4788,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,2,none,yes,good
-0 <= ... < 200 DM,48,delay in paying off in the past,others,7582,100 <= ... < 500 DM,unemployed,2,female : divorced/separated/married,none,4,unknown / no property,31,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1092,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,4,real estate,49,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,delay in paying off in the past,radio/television,1024,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,4,real estate,48,stores,own,1,skilled employee / official,1,none,yes,bad
-no checking account,12,existing credits paid back duly till now,business,1076,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",no,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,car (used),9398,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,24,critical account/ other credits existing (not at this bank),car (used),6419,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,44,none,for free,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,42,critical account/ other credits existing (not at this bank),car (used),4796,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,56,none,for free,1,skilled employee / official,1,none,yes,good
-no checking account,48,critical account/ other credits existing (not at this bank),business,7629,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",46,bank,own,2,management/ self-employed/ highly qualified employee/ officer,2,none,yes,good
-0 <= ... < 200 DM,48,existing credits paid back duly till now,furniture/equipment,9960,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,12,existing credits paid back duly till now,car (used),4675,unknown/ no savings account,... < 1 year,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",20,none,rent,1,skilled employee / official,1,none,yes,good
-no checking account,10,existing credits paid back duly till now,car (new),1287,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,co-applicant,2,building society savings agreement/ life insurance,45,none,own,1,unskilled - resident,1,none,no,good
-no checking account,18,existing credits paid back duly till now,furniture/equipment,2515,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,4,real estate,43,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,21,critical account/ other credits existing (not at this bank),furniture/equipment,2745,... >= 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,6,existing credits paid back duly till now,car (new),672,... < 100 DM,unemployed,1,female : divorced/separated/married,none,4,real estate,54,none,own,1,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,36,no credits taken/ all credits paid back duly,radio/television,3804,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... >= 200 DM / salary assignments for at least 1 year,24,critical account/ other credits existing (not at this bank),car (new),1344,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,real estate,37,bank,own,2,unskilled - resident,2,none,yes,bad
-... < 0 DM,10,critical account/ other credits existing (not at this bank),car (new),1038,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,co-applicant,3,building society savings agreement/ life insurance,49,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,48,critical account/ other credits existing (not at this bank),car (new),10127,500 <= ... < 1000 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,unknown / no property,44,bank,for free,1,skilled employee / official,1,none,yes,bad
-no checking account,6,existing credits paid back duly till now,furniture/equipment,1543,... >= 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,33,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,30,existing credits paid back duly till now,car (used),4811,unknown/ no savings account,4 <= ... < 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,24,stores,rent,1,unskilled - resident,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,radio/television,727,100 <= ... < 500 DM,... < 1 year,4,female : divorced/separated/married,none,3,unknown / no property,33,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,8,existing credits paid back duly till now,furniture/equipment,1237,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,4,real estate,24,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,9,existing credits paid back duly till now,car (new),276,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,real estate,22,none,rent,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,48,existing credits paid back duly till now,others,5381,unknown/ no savings account,unemployed,3,female : divorced/separated/married,none,4,unknown / no property,40,bank,for free,1,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,furniture/equipment,5511,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",25,stores,own,1,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,furniture/equipment,3749,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),685,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",25,bank,own,1,unskilled - resident,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,4,existing credits paid back duly till now,car (new),1494,unknown/ no savings account,... < 1 year,1,female : divorced/separated/married,none,2,real estate,29,none,own,1,unskilled - resident,2,none,no,good
-... < 0 DM,36,all credits at this bank paid back duly,furniture/equipment,2746,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",31,bank,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,708,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,guarantor,3,building society savings agreement/ life insurance,38,none,own,1,unskilled - resident,2,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,furniture/equipment,4351,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,48,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),education,701,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,15,delay in paying off in the past,furniture/equipment,3643,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,27,none,own,2,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,30,critical account/ other credits existing (not at this bank),car (new),4249,... < 100 DM,unemployed,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,radio/television,1938,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,32,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,car (used),2910,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,1,unknown / no property,34,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,2659,... >= 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),car (new),1028,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,real estate,36,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,8,critical account/ other credits existing (not at this bank),car (new),3398,... < 100 DM,4 <= ... < 7 years,1,female : divorced/separated/married,none,4,real estate,39,none,own,2,unskilled - resident,1,none,no,good
-no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,5801,unknown/ no savings account,... >= 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,49,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,car (new),1525,... >= 1000 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,36,existing credits paid back duly till now,radio/television,4473,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,1068,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,2,none,yes,good
-... < 0 DM,24,critical account/ other credits existing (not at this bank),car (used),6615,... < 100 DM,unemployed,2,female : divorced/separated/married,none,4,unknown / no property,75,none,for free,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),education,1864,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,30,none,own,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,60,existing credits paid back duly till now,car (new),7408,100 <= ... < 500 DM,... < 1 year,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,24,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
-no checking account,48,critical account/ other credits existing (not at this bank),car (used),11590,100 <= ... < 500 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",24,bank,rent,2,unskilled - resident,1,none,yes,bad
-... < 0 DM,24,no credits taken/ all credits paid back duly,furniture/equipment,4110,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,23,bank,rent,2,skilled employee / official,2,none,yes,bad
-... < 0 DM,6,critical account/ other credits existing (not at this bank),furniture/equipment,3384,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,real estate,44,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,13,existing credits paid back duly till now,radio/television,2101,... < 100 DM,... < 1 year,2,female : divorced/separated/married,guarantor,4,building society savings agreement/ life insurance,23,none,own,1,unskilled - resident,1,none,yes,good
-... < 0 DM,15,existing credits paid back duly till now,domestic appliances,1275,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",24,none,rent,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,4169,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,28,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,10,existing credits paid back duly till now,furniture/equipment,1521,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),education,5743,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,4,unknown / no property,24,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,21,existing credits paid back duly till now,furniture/equipment,3599,... < 100 DM,4 <= ... < 7 years,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",26,none,rent,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,radio/television,3213,500 <= ... < 1000 DM,... < 1 year,1,female : divorced/separated/married,none,3,real estate,25,none,rent,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,business,4439,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,co-applicant,1,real estate,33,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,10,existing credits paid back duly till now,car (new),3949,... < 100 DM,... < 1 year,1,female : divorced/separated/married,guarantor,1,building society savings agreement/ life insurance,37,none,own,1,unskilled - resident,2,none,yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1459,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",43,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,13,critical account/ other credits existing (not at this bank),radio/television,882,... < 100 DM,... < 1 year,4,female : divorced/separated/married,guarantor,4,real estate,23,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,3758,500 <= ... < 1000 DM,unemployed,1,female : divorced/separated/married,none,4,unknown / no property,23,none,rent,1,unemployed/ unskilled - non-resident,1,none,yes,good
-no checking account,6,delay in paying off in the past,business,1743,100 <= ... < 500 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,real estate,34,none,own,2,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,9,critical account/ other credits existing (not at this bank),education,1136,... >= 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,3,unknown / no property,32,none,for free,2,skilled employee / official,2,none,yes,bad
-no checking account,9,existing credits paid back duly till now,domestic appliances,1236,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,4,real estate,23,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,furniture/equipment,959,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",29,none,own,1,skilled employee / official,1,none,no,bad
-no checking account,18,critical account/ other credits existing (not at this bank),car (used),3229,unknown/ no savings account,unemployed,2,female : divorced/separated/married,none,4,unknown / no property,38,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,no credits taken/ all credits paid back duly,radio/television,6199,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,28,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,10,existing credits paid back duly till now,education,727,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,46,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),1246,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,2,real estate,23,stores,own,1,unskilled - resident,1,none,yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,2331,unknown/ no savings account,... >= 7 years,1,female : divorced/separated/married,co-applicant,4,real estate,49,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,36,delay in paying off in the past,radio/television,4463,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,12,existing credits paid back duly till now,radio/television,776,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,28,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,30,existing credits paid back duly till now,furniture/equipment,2406,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,real estate,23,none,rent,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,18,existing credits paid back duly till now,education,1239,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,61,none,for free,1,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,radio/television,3399,unknown/ no savings account,... >= 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",37,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,delay in paying off in the past,car (new),2247,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",36,stores,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,6,existing credits paid back duly till now,furniture/equipment,1766,... < 100 DM,1 <= ... < 4 years,1,male : single,none,2,building society savings agreement/ life insurance,21,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,2473,... < 100 DM,unemployed,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",25,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,bad
-no checking account,12,existing credits paid back duly till now,business,1542,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",36,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),car (used),3850,... < 100 DM,4 <= ... < 7 years,3,male : single,none,1,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,3650,... < 100 DM,... < 1 year,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",22,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,3446,... < 100 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,2,none,yes,bad
-0 <= ... < 200 DM,18,existing credits paid back duly till now,furniture/equipment,3001,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,real estate,40,none,rent,1,skilled employee / official,1,none,yes,good
-no checking account,36,existing credits paid back duly till now,car (new),3079,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,real estate,36,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,6070,... < 100 DM,... >= 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",33,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,10,critical account/ other credits existing (not at this bank),furniture/equipment,2146,... < 100 DM,... < 1 year,1,male : single,none,3,real estate,23,none,rent,2,skilled employee / official,1,none,yes,good
-no checking account,60,critical account/ other credits existing (not at this bank),car (new),13756,unknown/ no savings account,... >= 7 years,2,male : single,none,4,unknown / no property,63,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,60,all credits at this bank paid back duly,others,14782,100 <= ... < 500 DM,... >= 7 years,3,male : single,none,4,unknown / no property,60,bank,for free,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,48,all credits at this bank paid back duly,business,7685,... < 100 DM,4 <= ... < 7 years,2,male : single,guarantor,4,"car or other, not in attribute Savings account/bonds",37,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,18,delay in paying off in the past,radio/television,2320,... < 100 DM,unemployed,2,male : single,none,3,real estate,34,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,7,delay in paying off in the past,radio/television,846,unknown/ no savings account,... >= 7 years,3,male : single,none,4,unknown / no property,36,none,for free,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,car (new),14318,... < 100 DM,... >= 7 years,4,male : single,none,2,unknown / no property,57,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,6,critical account/ other credits existing (not at this bank),car (new),362,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",52,none,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,20,existing credits paid back duly till now,furniture/equipment,2212,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",39,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,car (used),12976,... < 100 DM,unemployed,3,male : single,none,4,unknown / no property,38,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,22,existing credits paid back duly till now,car (new),1283,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,building society savings agreement/ life insurance,25,none,rent,1,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,car (new),1330,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,26,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,30,delay in paying off in the past,business,4272,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,26,none,own,2,unskilled - resident,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,2238,... < 100 DM,1 <= ... < 4 years,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",25,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,radio/television,1126,unknown/ no savings account,... < 1 year,4,male : single,none,2,real estate,21,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,7374,... < 100 DM,unemployed,4,male : single,none,4,building society savings agreement/ life insurance,40,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,15,critical account/ other credits existing (not at this bank),business,2326,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,bank,own,1,skilled employee / official,1,none,yes,good
-no checking account,9,existing credits paid back duly till now,business,1449,... < 100 DM,4 <= ... < 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,car (new),1820,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,983,... >= 1000 DM,... < 1 year,1,male : single,none,4,real estate,19,none,rent,1,unskilled - resident,1,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,car (new),3249,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,unknown / no property,39,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-... < 0 DM,6,critical account/ other credits existing (not at this bank),radio/television,1957,... < 100 DM,4 <= ... < 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,9,critical account/ other credits existing (not at this bank),furniture/equipment,2406,... < 100 DM,unemployed,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",31,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-0 <= ... < 200 DM,39,delay in paying off in the past,education,11760,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,3,unknown / no property,32,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,2578,... < 100 DM,unemployed,3,male : single,none,4,unknown / no property,55,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-... < 0 DM,36,critical account/ other credits existing (not at this bank),furniture/equipment,2348,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,building society savings agreement/ life insurance,46,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),1223,... < 100 DM,... >= 7 years,1,male : single,none,1,real estate,46,none,rent,2,skilled employee / official,1,none,yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,1516,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,1,real estate,43,none,own,2,unskilled - resident,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,radio/television,1473,... < 100 DM,... < 1 year,3,male : single,none,4,real estate,39,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),business,1887,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,real estate,28,bank,own,2,skilled employee / official,1,none,yes,good
-no checking account,24,delay in paying off in the past,business,8648,... < 100 DM,... < 1 year,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",27,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,14,delay in paying off in the past,car (new),802,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,2,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,18,delay in paying off in the past,car (new),2899,unknown/ no savings account,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",43,none,own,1,skilled employee / official,2,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,2039,... < 100 DM,... < 1 year,1,male : single,none,1,building society savings agreement/ life insurance,22,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),car (used),2197,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",43,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,15,existing credits paid back duly till now,radio/television,1053,... < 100 DM,... < 1 year,4,male : single,none,2,real estate,27,none,own,1,skilled employee / official,1,none,no,good
-no checking account,24,existing credits paid back duly till now,radio/television,3235,500 <= ... < 1000 DM,... >= 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,critical account/ other credits existing (not at this bank),car (new),939,500 <= ... < 1000 DM,4 <= ... < 7 years,4,male : single,none,2,real estate,28,none,own,3,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,1967,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",20,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,33,critical account/ other credits existing (not at this bank),car (used),7253,... < 100 DM,4 <= ... < 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",35,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),business,2292,... < 100 DM,unemployed,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",42,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,10,existing credits paid back duly till now,car (new),1597,500 <= ... < 1000 DM,1 <= ... < 4 years,3,male : single,none,2,unknown / no property,40,none,rent,1,unskilled - resident,2,none,no,good
-... < 0 DM,24,existing credits paid back duly till now,car (new),1381,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,35,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,36,critical account/ other credits existing (not at this bank),car (used),5842,... < 100 DM,... >= 7 years,2,male : single,none,2,building society savings agreement/ life insurance,35,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,car (new),2579,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,33,none,own,1,unskilled - resident,2,none,yes,bad
-... < 0 DM,18,delay in paying off in the past,education,8471,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",23,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,21,existing credits paid back duly till now,car (new),2782,500 <= ... < 1000 DM,4 <= ... < 7 years,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,car (new),1042,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,33,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,15,existing credits paid back duly till now,car (new),3186,... >= 1000 DM,4 <= ... < 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",20,none,rent,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (used),2028,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (new),958,... < 100 DM,4 <= ... < 7 years,2,male : single,none,3,real estate,47,none,own,2,unskilled - resident,2,none,yes,good
-no checking account,21,delay in paying off in the past,furniture/equipment,1591,100 <= ... < 500 DM,4 <= ... < 7 years,4,male : single,none,3,real estate,34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,2762,unknown/ no savings account,... >= 7 years,1,male : single,none,2,building society savings agreement/ life insurance,25,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,18,existing credits paid back duly till now,car (used),2779,... < 100 DM,1 <= ... < 4 years,1,male : single,none,3,"car or other, not in attribute Savings account/bonds",21,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,28,critical account/ other credits existing (not at this bank),radio/television,2743,... < 100 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",29,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1149,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,46,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,9,existing credits paid back duly till now,furniture/equipment,1313,... < 100 DM,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",20,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,18,critical account/ other credits existing (not at this bank),repairs,1190,... < 100 DM,unemployed,2,male : single,none,4,unknown / no property,55,none,for free,3,unemployed/ unskilled - non-resident,2,none,yes,bad
-no checking account,5,existing credits paid back duly till now,business,3448,... < 100 DM,4 <= ... < 7 years,1,male : single,none,4,real estate,74,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,others,11328,... < 100 DM,1 <= ... < 4 years,2,male : single,co-applicant,3,"car or other, not in attribute Savings account/bonds",29,bank,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,6,critical account/ other credits existing (not at this bank),furniture/equipment,1872,... < 100 DM,unemployed,4,male : single,none,4,unknown / no property,36,none,for free,3,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),repairs,2058,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,33,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,9,existing credits paid back duly till now,furniture/equipment,2136,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,25,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1484,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,1,real estate,25,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,6,existing credits paid back duly till now,repairs,660,500 <= ... < 1000 DM,4 <= ... < 7 years,2,male : single,none,4,real estate,23,none,rent,1,unskilled - resident,1,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),car (new),1287,... >= 1000 DM,... >= 7 years,4,male : single,none,4,real estate,37,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,42,critical account/ other credits existing (not at this bank),repairs,3394,... < 100 DM,unemployed,4,male : single,co-applicant,4,"car or other, not in attribute Savings account/bonds",65,none,own,2,unemployed/ unskilled - non-resident,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,all credits at this bank paid back duly,business,609,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,26,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,bad
-no checking account,12,existing credits paid back duly till now,car (new),1884,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",39,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1620,... < 100 DM,1 <= ... < 4 years,2,male : single,co-applicant,3,building society savings agreement/ life insurance,30,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,20,delay in paying off in the past,others,2629,... < 100 DM,1 <= ... < 4 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",29,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,education,719,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",41,bank,own,1,unskilled - resident,2,none,yes,bad
-0 <= ... < 200 DM,48,critical account/ other credits existing (not at this bank),furniture/equipment,5096,... < 100 DM,1 <= ... < 4 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,9,critical account/ other credits existing (not at this bank),education,1244,unknown/ no savings account,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,41,none,rent,2,unskilled - resident,1,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,car (new),1842,... < 100 DM,... < 1 year,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,7,existing credits paid back duly till now,radio/television,2576,... < 100 DM,1 <= ... < 4 years,2,male : single,guarantor,2,real estate,35,none,own,1,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,furniture/equipment,1424,unknown/ no savings account,... >= 7 years,3,male : single,none,4,real estate,55,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,15,delay in paying off in the past,repairs,1512,... >= 1000 DM,1 <= ... < 4 years,3,male : single,none,3,building society savings agreement/ life insurance,61,stores,own,2,skilled employee / official,1,none,yes,bad
-no checking account,36,critical account/ other credits existing (not at this bank),car (used),11054,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,6,existing credits paid back duly till now,radio/television,518,... < 100 DM,1 <= ... < 4 years,3,male : single,none,1,real estate,29,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,12,no credits taken/ all credits paid back duly,furniture/equipment,2759,... < 100 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,34,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,car (used),2670,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",35,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,existing credits paid back duly till now,car (new),4817,... < 100 DM,4 <= ... < 7 years,2,male : single,co-applicant,3,building society savings agreement/ life insurance,31,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,24,existing credits paid back duly till now,car (used),2679,... < 100 DM,... < 1 year,4,male : single,none,1,unknown / no property,29,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,11,critical account/ other credits existing (not at this bank),car (new),3905,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,36,none,rent,2,skilled employee / official,2,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,car (used),3386,... < 100 DM,... >= 7 years,3,male : single,none,4,unknown / no property,35,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,6,existing credits paid back duly till now,domestic appliances,343,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,27,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,radio/television,4594,... < 100 DM,... < 1 year,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,3620,... < 100 DM,1 <= ... < 4 years,1,male : single,guarantor,2,building society savings agreement/ life insurance,37,none,own,1,skilled employee / official,2,none,yes,good
-... < 0 DM,15,existing credits paid back duly till now,car (new),1721,... < 100 DM,... < 1 year,2,male : single,none,3,real estate,36,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,3017,... < 100 DM,... < 1 year,3,male : single,none,1,real estate,34,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,retraining,754,unknown/ no savings account,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,38,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,business,1950,... < 100 DM,4 <= ... < 7 years,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",34,stores,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,existing credits paid back duly till now,car (used),2924,... < 100 DM,1 <= ... < 4 years,3,male : single,guarantor,4,unknown / no property,63,bank,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,24,delay in paying off in the past,radio/television,1659,... < 100 DM,... < 1 year,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",29,none,rent,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-no checking account,48,delay in paying off in the past,radio/television,7238,unknown/ no savings account,... >= 7 years,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",32,bank,own,2,skilled employee / official,2,none,yes,good
-no checking account,33,delay in paying off in the past,business,2764,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,delay in paying off in the past,car (used),4679,... < 100 DM,4 <= ... < 7 years,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",35,none,own,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,3092,100 <= ... < 500 DM,... < 1 year,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",22,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,6,existing credits paid back duly till now,education,448,... < 100 DM,... < 1 year,4,male : single,none,4,building society savings agreement/ life insurance,23,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,9,existing credits paid back duly till now,car (new),654,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",28,none,own,1,unskilled - resident,1,none,yes,bad
-no checking account,6,existing credits paid back duly till now,retraining,1238,unknown/ no savings account,unemployed,4,male : single,none,4,building society savings agreement/ life insurance,36,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),radio/television,1245,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,18,no credits taken/ all credits paid back duly,furniture/equipment,3114,... < 100 DM,... < 1 year,1,male : single,none,4,building society savings agreement/ life insurance,26,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,39,existing credits paid back duly till now,car (used),2569,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,radio/television,5152,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",25,bank,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,business,1037,100 <= ... < 500 DM,4 <= ... < 7 years,3,male : single,none,4,real estate,39,none,own,1,unskilled - resident,1,none,yes,good
-... < 0 DM,15,critical account/ other credits existing (not at this bank),furniture/equipment,1478,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",44,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),radio/television,3573,... < 100 DM,1 <= ... < 4 years,1,male : single,none,1,real estate,23,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),1201,... < 100 DM,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,30,existing credits paid back duly till now,furniture/equipment,3622,... >= 1000 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,57,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,15,delay in paying off in the past,furniture/equipment,960,... >= 1000 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,30,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),car (new),1163,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,44,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,6,delay in paying off in the past,car (new),1209,... < 100 DM,unemployed,4,male : single,none,4,building society savings agreement/ life insurance,47,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,12,existing credits paid back duly till now,radio/television,3077,... < 100 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",52,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,car (new),3757,... < 100 DM,... >= 7 years,4,male : single,co-applicant,4,unknown / no property,62,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,10,existing credits paid back duly till now,car (new),1418,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,35,none,rent,1,unskilled - resident,1,none,no,good
-no checking account,6,existing credits paid back duly till now,car (new),3518,... < 100 DM,1 <= ... < 4 years,2,male : single,guarantor,3,building society savings agreement/ life insurance,26,none,rent,1,skilled employee / official,1,none,yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,1934,... < 100 DM,... >= 7 years,2,male : single,none,2,unknown / no property,26,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,27,no credits taken/ all credits paid back duly,business,8318,... < 100 DM,... >= 7 years,2,male : single,none,4,unknown / no property,42,none,for free,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1237,100 <= ... < 500 DM,1 <= ... < 4 years,1,male : single,none,1,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,368,unknown/ no savings account,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,38,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),2122,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,39,none,rent,2,unskilled - resident,2,none,no,good
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,2996,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",20,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,36,existing credits paid back duly till now,furniture/equipment,9034,100 <= ... < 500 DM,... < 1 year,4,male : single,co-applicant,1,unknown / no property,29,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),furniture/equipment,1585,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,40,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,radio/television,1301,... < 100 DM,... >= 7 years,4,male : single,guarantor,2,real estate,32,none,own,1,unskilled - resident,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,6,critical account/ other credits existing (not at this bank),car (new),1323,100 <= ... < 500 DM,... >= 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,24,existing credits paid back duly till now,car (new),3123,... < 100 DM,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,27,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,36,existing credits paid back duly till now,car (used),5493,... < 100 DM,... >= 7 years,2,male : single,none,4,unknown / no property,42,none,for free,1,skilled employee / official,2,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,9,existing credits paid back duly till now,radio/television,1126,100 <= ... < 500 DM,... >= 7 years,2,male : single,none,4,real estate,49,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),radio/television,1216,100 <= ... < 500 DM,... < 1 year,4,male : single,none,4,unknown / no property,38,bank,own,2,skilled employee / official,2,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,car (new),1207,... < 100 DM,... < 1 year,4,male : single,none,4,building society savings agreement/ life insurance,24,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,10,existing credits paid back duly till now,car (new),1309,unknown/ no savings account,1 <= ... < 4 years,4,male : single,guarantor,4,building society savings agreement/ life insurance,27,none,own,1,unskilled - resident,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,15,critical account/ other credits existing (not at this bank),car (used),2360,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",36,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,15,all credits at this bank paid back duly,car (new),6850,100 <= ... < 500 DM,unemployed,1,male : single,none,2,building society savings agreement/ life insurance,34,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,bad
-no checking account,24,existing credits paid back duly till now,radio/television,1413,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,28,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,39,existing credits paid back duly till now,car (used),8588,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",45,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,car (new),759,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,real estate,26,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,36,existing credits paid back duly till now,car (used),4686,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,unknown / no property,32,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,15,existing credits paid back duly till now,business,2687,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,building society savings agreement/ life insurance,26,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,delay in paying off in the past,radio/television,585,... < 100 DM,1 <= ... < 4 years,4,male : single,co-applicant,4,real estate,20,none,rent,2,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,car (new),2255,unknown/ no savings account,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,54,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),609,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,37,none,own,2,skilled employee / official,1,none,no,good
-... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),1361,... < 100 DM,... < 1 year,2,male : single,none,4,real estate,40,none,own,1,unskilled - resident,2,none,no,good
-no checking account,36,critical account/ other credits existing (not at this bank),furniture/equipment,7127,... < 100 DM,... < 1 year,2,male : single,none,4,building society savings agreement/ life insurance,23,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,6,existing credits paid back duly till now,car (new),1203,100 <= ... < 500 DM,... >= 7 years,3,male : single,none,2,building society savings agreement/ life insurance,43,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,6,critical account/ other credits existing (not at this bank),radio/television,700,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,36,none,for free,2,skilled employee / official,1,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),repairs,5507,... < 100 DM,... >= 7 years,3,male : single,none,4,unknown / no property,44,none,for free,2,skilled employee / official,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,radio/television,3190,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,24,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,48,no credits taken/ all credits paid back duly,furniture/equipment,7119,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,unknown / no property,53,none,for free,2,skilled employee / official,2,none,yes,bad
-no checking account,24,existing credits paid back duly till now,car (used),3488,100 <= ... < 500 DM,4 <= ... < 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",23,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,radio/television,1113,... < 100 DM,1 <= ... < 4 years,4,male : single,guarantor,4,real estate,26,none,own,1,unskilled - resident,2,none,yes,good
-0 <= ... < 200 DM,26,existing credits paid back duly till now,car (used),7966,... < 100 DM,... < 1 year,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),education,1532,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,4,critical account/ other credits existing (not at this bank),radio/television,1503,... < 100 DM,4 <= ... < 7 years,2,male : single,none,1,real estate,42,none,own,2,unskilled - resident,2,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,radio/television,2302,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",31,none,rent,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,6,existing credits paid back duly till now,car (new),662,... < 100 DM,... < 1 year,3,male : single,none,4,real estate,41,none,own,1,unskilled - resident,2,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,education,2273,... < 100 DM,4 <= ... < 7 years,3,male : single,none,1,"car or other, not in attribute Savings account/bonds",32,none,own,2,skilled employee / official,2,none,yes,good
-0 <= ... < 200 DM,15,existing credits paid back duly till now,car (new),2631,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,12,delay in paying off in the past,car (used),1503,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,41,none,rent,1,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,1311,100 <= ... < 500 DM,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,3105,unknown/ no savings account,... < 1 year,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,2,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,21,critical account/ other credits existing (not at this bank),education,2319,... < 100 DM,... < 1 year,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",33,none,rent,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,6,existing credits paid back duly till now,car (new),1374,unknown/ no savings account,unemployed,4,male : single,none,3,building society savings agreement/ life insurance,75,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,3612,... < 100 DM,... >= 7 years,3,male : single,none,4,building society savings agreement/ life insurance,37,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,48,existing credits paid back duly till now,car (new),7763,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,42,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,18,existing credits paid back duly till now,furniture/equipment,3049,... < 100 DM,... < 1 year,1,male : single,none,1,building society savings agreement/ life insurance,45,stores,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1534,... < 100 DM,... < 1 year,1,male : single,none,1,real estate,23,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,24,delay in paying off in the past,car (new),2032,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,60,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,30,existing credits paid back duly till now,furniture/equipment,6350,unknown/ no savings account,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,31,none,own,1,skilled employee / official,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,18,existing credits paid back duly till now,furniture/equipment,2864,... < 100 DM,1 <= ... < 4 years,2,male : single,none,1,real estate,34,none,own,1,unskilled - resident,2,none,yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),car (new),1255,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,61,none,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,24,delay in paying off in the past,car (new),1333,... < 100 DM,unemployed,4,male : single,none,2,real estate,43,none,for free,2,skilled employee / official,2,none,yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),car (new),2022,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",37,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,1552,... < 100 DM,4 <= ... < 7 years,3,male : single,none,1,"car or other, not in attribute Savings account/bonds",32,bank,own,1,skilled employee / official,2,none,yes,good
-... < 0 DM,12,all credits at this bank paid back duly,radio/television,626,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,24,bank,own,1,unskilled - resident,1,none,yes,bad
-no checking account,48,critical account/ other credits existing (not at this bank),car (used),8858,unknown/ no savings account,4 <= ... < 7 years,2,male : single,none,1,unknown / no property,35,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),repairs,996,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,real estate,23,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,6,all credits at this bank paid back duly,radio/television,1750,500 <= ... < 1000 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,45,bank,own,1,unskilled - resident,2,none,yes,good
-... < 0 DM,48,existing credits paid back duly till now,radio/television,6999,... < 100 DM,4 <= ... < 7 years,1,male : single,guarantor,1,real estate,34,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (new),1995,100 <= ... < 500 DM,... < 1 year,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",27,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,education,1199,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,building society savings agreement/ life insurance,67,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1331,... < 100 DM,... < 1 year,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",22,stores,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,18,no credits taken/ all credits paid back duly,car (new),2278,100 <= ... < 500 DM,... < 1 year,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,1,none,yes,bad
-no checking account,21,no credits taken/ all credits paid back duly,car (new),5003,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,4,building society savings agreement/ life insurance,29,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,3552,... < 100 DM,4 <= ... < 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,bank,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,1928,... < 100 DM,... < 1 year,2,male : single,none,2,real estate,31,none,own,2,unskilled - resident,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,car (used),2964,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,49,bank,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,24,all credits at this bank paid back duly,radio/television,1546,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,4,"car or other, not in attribute Savings account/bonds",24,bank,rent,1,unskilled - resident,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,6,delay in paying off in the past,radio/television,683,... < 100 DM,... < 1 year,2,male : single,none,1,building society savings agreement/ life insurance,29,bank,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,car (new),12389,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,4,unknown / no property,37,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,24,delay in paying off in the past,business,4712,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,37,bank,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,delay in paying off in the past,radio/television,1553,100 <= ... < 500 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,23,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,car (new),1372,... < 100 DM,4 <= ... < 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",36,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2578,... >= 1000 DM,... >= 7 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,48,existing credits paid back duly till now,radio/television,3979,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",41,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,48,existing credits paid back duly till now,radio/television,6758,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,3234,... < 100 DM,... < 1 year,4,male : single,none,4,real estate,23,none,rent,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-no checking account,30,critical account/ other credits existing (not at this bank),radio/television,5954,... < 100 DM,4 <= ... < 7 years,3,male : single,co-applicant,2,"car or other, not in attribute Savings account/bonds",38,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,car (used),5433,unknown/ no savings account,unemployed,2,male : single,none,4,building society savings agreement/ life insurance,26,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,15,existing credits paid back duly till now,business,806,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,building society savings agreement/ life insurance,22,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,1082,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,none,own,2,unskilled - resident,1,none,yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),furniture/equipment,2788,... < 100 DM,4 <= ... < 7 years,2,male : single,co-applicant,3,"car or other, not in attribute Savings account/bonds",24,bank,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,2930,... < 100 DM,4 <= ... < 7 years,2,male : single,none,1,real estate,27,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),education,1927,unknown/ no savings account,1 <= ... < 4 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,36,critical account/ other credits existing (not at this bank),car (new),2820,... < 100 DM,... < 1 year,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,bad
-no checking account,24,existing credits paid back duly till now,retraining,937,... < 100 DM,... < 1 year,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",27,none,own,2,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),car (new),1056,... < 100 DM,... >= 7 years,3,male : single,guarantor,3,real estate,30,bank,own,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (new),3124,... < 100 DM,... < 1 year,1,male : single,none,3,real estate,49,bank,own,2,unskilled - resident,2,none,yes,good
-no checking account,9,existing credits paid back duly till now,furniture/equipment,1388,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,26,none,rent,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,repairs,2384,... < 100 DM,... < 1 year,4,male : single,none,1,unknown / no property,33,none,rent,1,unskilled - resident,1,none,yes,bad
-no checking account,12,existing credits paid back duly till now,car (new),2133,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,52,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,2039,... < 100 DM,1 <= ... < 4 years,1,male : single,none,4,real estate,20,bank,rent,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,9,critical account/ other credits existing (not at this bank),car (new),2799,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,36,none,rent,2,skilled employee / official,2,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1289,... < 100 DM,1 <= ... < 4 years,4,male : single,guarantor,1,building society savings agreement/ life insurance,21,none,own,1,unskilled - resident,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,domestic appliances,1217,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,47,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,12,critical account/ other credits existing (not at this bank),furniture/equipment,2246,... < 100 DM,... >= 7 years,3,male : single,none,3,building society savings agreement/ life insurance,60,none,own,2,skilled employee / official,1,none,yes,bad
-... < 0 DM,12,critical account/ other credits existing (not at this bank),radio/television,385,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,real estate,58,none,own,4,unskilled - resident,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,delay in paying off in the past,car (new),1965,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",42,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,21,existing credits paid back duly till now,business,1572,... >= 1000 DM,... >= 7 years,4,male : single,none,4,real estate,36,bank,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),2718,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,building society savings agreement/ life insurance,20,none,rent,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,24,all credits at this bank paid back duly,others,1358,unknown/ no savings account,... >= 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",40,stores,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,6,all credits at this bank paid back duly,car (new),931,100 <= ... < 500 DM,... < 1 year,1,male : single,none,1,building society savings agreement/ life insurance,32,stores,own,1,unskilled - resident,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,car (new),1442,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",23,none,rent,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,24,no credits taken/ all credits paid back duly,business,4241,... < 100 DM,1 <= ... < 4 years,1,male : single,none,4,real estate,36,none,own,3,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-no checking account,18,critical account/ other credits existing (not at this bank),car (new),2775,... < 100 DM,4 <= ... < 7 years,2,male : single,none,2,building society savings agreement/ life insurance,31,bank,own,2,skilled employee / official,1,none,yes,bad
-no checking account,24,delay in paying off in the past,business,3863,... < 100 DM,1 <= ... < 4 years,1,male : single,none,2,unknown / no property,32,none,for free,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,7,existing credits paid back duly till now,radio/television,2329,... < 100 DM,... < 1 year,1,male : single,guarantor,1,real estate,45,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,furniture/equipment,918,... < 100 DM,1 <= ... < 4 years,4,male : single,none,1,building society savings agreement/ life insurance,30,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,24,all credits at this bank paid back duly,education,1837,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,unknown / no property,34,bank,for free,1,unskilled - resident,1,none,yes,bad
-no checking account,36,existing credits paid back duly till now,furniture/equipment,3349,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... >= 200 DM / salary assignments for at least 1 year,10,existing credits paid back duly till now,furniture/equipment,1275,... < 100 DM,... < 1 year,4,male : single,none,2,building society savings agreement/ life insurance,23,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,2828,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,22,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),business,4526,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,74,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,radio/television,2671,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : single,co-applicant,4,unknown / no property,50,none,for free,1,skilled employee / official,1,none,yes,bad
-no checking account,18,existing credits paid back duly till now,radio/television,2051,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,33,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,15,existing credits paid back duly till now,car (used),1300,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,45,bank,for free,1,skilled employee / official,2,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,domestic appliances,741,100 <= ... < 500 DM,unemployed,4,male : single,none,3,building society savings agreement/ life insurance,22,none,own,1,skilled employee / official,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,10,existing credits paid back duly till now,car (new),1240,100 <= ... < 500 DM,... >= 7 years,1,male : single,none,4,unknown / no property,48,none,for free,1,unskilled - resident,2,none,yes,bad
-... < 0 DM,21,existing credits paid back duly till now,radio/television,3357,... >= 1000 DM,... < 1 year,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",29,bank,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,24,all credits at this bank paid back duly,car (used),3632,... < 100 DM,1 <= ... < 4 years,1,male : single,guarantor,4,"car or other, not in attribute Savings account/bonds",22,bank,rent,1,skilled employee / official,1,none,no,good
-no checking account,18,delay in paying off in the past,furniture/equipment,1808,... < 100 DM,4 <= ... < 7 years,4,male : single,none,1,real estate,22,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,business,12204,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",48,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,60,delay in paying off in the past,radio/television,9157,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,2,unknown / no property,27,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),3676,... < 100 DM,1 <= ... < 4 years,1,male : single,none,3,real estate,37,none,rent,3,skilled employee / official,2,none,yes,good
-0 <= ... < 200 DM,30,existing credits paid back duly till now,furniture/equipment,3441,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : single,co-applicant,4,"car or other, not in attribute Savings account/bonds",21,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,12,existing credits paid back duly till now,car (new),640,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,49,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,21,critical account/ other credits existing (not at this bank),business,3652,... < 100 DM,4 <= ... < 7 years,2,male : single,none,3,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),car (new),1530,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,building society savings agreement/ life insurance,32,bank,own,2,skilled employee / official,1,none,yes,bad
-no checking account,48,existing credits paid back duly till now,business,3914,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,real estate,38,bank,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1858,... < 100 DM,... < 1 year,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",22,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,radio/television,2600,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,65,none,for free,2,skilled employee / official,1,none,yes,bad
-no checking account,15,existing credits paid back duly till now,radio/television,1979,unknown/ no savings account,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",35,none,own,1,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,6,existing credits paid back duly till now,furniture/equipment,2116,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,41,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,9,all credits at this bank paid back duly,car (new),1437,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,3,unknown / no property,29,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,42,critical account/ other credits existing (not at this bank),furniture/equipment,4042,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,36,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,9,existing credits paid back duly till now,education,3832,unknown/ no savings account,... >= 7 years,1,male : single,none,4,real estate,64,none,own,1,unskilled - resident,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,radio/television,3660,... < 100 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,18,all credits at this bank paid back duly,furniture/equipment,1553,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",44,bank,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,15,existing credits paid back duly till now,radio/television,1444,unknown/ no savings account,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,23,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,9,existing credits paid back duly till now,furniture/equipment,1980,... < 100 DM,... < 1 year,2,male : single,co-applicant,2,"car or other, not in attribute Savings account/bonds",19,none,rent,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),1355,... < 100 DM,... < 1 year,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",25,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
-no checking account,12,existing credits paid back duly till now,education,1393,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,47,bank,own,3,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,1376,500 <= ... < 1000 DM,4 <= ... < 7 years,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,60,delay in paying off in the past,radio/television,15653,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",21,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,1493,... < 100 DM,... < 1 year,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,2,none,yes,good
-... < 0 DM,42,delay in paying off in the past,radio/television,4370,... < 100 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,26,bank,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,bad
-... < 0 DM,18,existing credits paid back duly till now,education,750,... < 100 DM,unemployed,4,male : single,none,1,real estate,27,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,bad
-0 <= ... < 200 DM,15,existing credits paid back duly till now,repairs,1308,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",38,none,own,2,unskilled - resident,1,none,yes,good
-no checking account,15,existing credits paid back duly till now,education,4623,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,2,building society savings agreement/ life insurance,40,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,1851,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,2,"car or other, not in attribute Savings account/bonds",33,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,critical account/ other credits existing (not at this bank),radio/television,1880,... < 100 DM,4 <= ... < 7 years,4,male : single,none,1,building society savings agreement/ life insurance,32,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,36,delay in paying off in the past,business,7980,unknown/ no savings account,... < 1 year,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,30,no credits taken/ all credits paid back duly,furniture/equipment,4583,... < 100 DM,1 <= ... < 4 years,2,male : single,guarantor,2,real estate,32,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,12,existing credits paid back duly till now,car (new),1386,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,car (new),947,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,unknown / no property,38,bank,for free,1,skilled employee / official,2,none,yes,bad
-... < 0 DM,12,existing credits paid back duly till now,education,684,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,rent,1,unskilled - resident,2,none,yes,bad
-... < 0 DM,48,existing credits paid back duly till now,education,7476,... < 100 DM,4 <= ... < 7 years,4,male : single,none,1,unknown / no property,50,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,1922,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,37,none,own,1,unskilled - resident,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,car (new),2303,... < 100 DM,... >= 7 years,4,male : single,co-applicant,1,real estate,45,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,36,delay in paying off in the past,car (new),8086,100 <= ... < 500 DM,... >= 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",42,none,own,4,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),car (used),2346,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",35,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,14,existing credits paid back duly till now,car (new),3973,... < 100 DM,unemployed,1,male : single,none,4,unknown / no property,22,none,for free,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),888,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",41,bank,own,1,unskilled - resident,2,none,yes,bad
-no checking account,48,existing credits paid back duly till now,radio/television,10222,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",37,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,30,no credits taken/ all credits paid back duly,business,4221,... < 100 DM,1 <= ... < 4 years,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,6361,... < 100 DM,... >= 7 years,2,male : single,none,1,unknown / no property,41,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,radio/television,1297,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,real estate,23,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,car (new),900,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",23,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,21,existing credits paid back duly till now,furniture/equipment,2241,... < 100 DM,... >= 7 years,4,male : single,none,2,real estate,50,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,6,delay in paying off in the past,furniture/equipment,1050,... < 100 DM,unemployed,4,male : single,none,1,building society savings agreement/ life insurance,35,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,6,critical account/ other credits existing (not at this bank),education,1047,... < 100 DM,1 <= ... < 4 years,2,male : single,none,4,building society savings agreement/ life insurance,50,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),others,6314,... < 100 DM,unemployed,4,male : single,co-applicant,2,unknown / no property,27,bank,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,30,all credits at this bank paid back duly,furniture/equipment,3496,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",34,stores,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,48,all credits at this bank paid back duly,business,3609,... < 100 DM,1 <= ... < 4 years,1,male : single,none,1,real estate,27,stores,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),4843,... < 100 DM,... >= 7 years,3,male : single,co-applicant,4,building society savings agreement/ life insurance,43,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... >= 200 DM / salary assignments for at least 1 year,30,critical account/ other credits existing (not at this bank),radio/television,3017,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,47,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),business,4139,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,3,building society savings agreement/ life insurance,27,none,own,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
-no checking account,36,existing credits paid back duly till now,business,5742,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,60,existing credits paid back duly till now,car (new),10366,... < 100 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,42,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,6,critical account/ other credits existing (not at this bank),car (new),2080,500 <= ... < 1000 DM,1 <= ... < 4 years,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,21,delay in paying off in the past,business,2580,500 <= ... < 1000 DM,... < 1 year,4,male : single,none,2,real estate,41,bank,own,1,unskilled - resident,2,none,yes,bad
-no checking account,30,critical account/ other credits existing (not at this bank),radio/television,4530,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",26,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),furniture/equipment,5150,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,72,existing credits paid back duly till now,radio/television,5595,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,radio/television,2384,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,64,bank,rent,1,unskilled - resident,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,radio/television,1453,... < 100 DM,... < 1 year,3,male : single,none,1,real estate,26,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,6,existing credits paid back duly till now,education,1538,... < 100 DM,... < 1 year,1,male : single,none,2,unknown / no property,56,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,2279,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,37,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,15,delay in paying off in the past,radio/television,1478,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,33,bank,own,2,skilled employee / official,1,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,5103,... < 100 DM,... < 1 year,3,male : single,none,3,unknown / no property,47,none,for free,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,36,delay in paying off in the past,business,9857,100 <= ... < 500 DM,4 <= ... < 7 years,1,male : single,none,3,building society savings agreement/ life insurance,31,none,own,2,unskilled - resident,2,"yes, registered under the customers name",yes,good
-no checking account,60,existing credits paid back duly till now,car (new),6527,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,34,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,10,critical account/ other credits existing (not at this bank),radio/television,1347,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,2,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,36,delay in paying off in the past,car (new),2862,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,3,unknown / no property,30,none,for free,1,skilled employee / official,1,none,yes,good
-no checking account,9,existing credits paid back duly till now,radio/television,2753,100 <= ... < 500 DM,... >= 7 years,3,male : single,co-applicant,4,"car or other, not in attribute Savings account/bonds",35,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,car (new),3651,... >= 1000 DM,1 <= ... < 4 years,1,male : single,none,3,building society savings agreement/ life insurance,31,none,own,1,skilled employee / official,2,none,yes,good
-... < 0 DM,15,critical account/ other credits existing (not at this bank),furniture/equipment,975,... < 100 DM,1 <= ... < 4 years,2,male : single,none,3,building society savings agreement/ life insurance,25,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,15,existing credits paid back duly till now,repairs,2631,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,25,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,2896,100 <= ... < 500 DM,... < 1 year,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",29,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),4716,unknown/ no savings account,... < 1 year,1,male : single,none,3,real estate,44,none,own,2,unskilled - resident,2,none,yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,2284,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,6,existing credits paid back duly till now,car (used),1236,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,4,building society savings agreement/ life insurance,50,none,rent,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1103,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,3,real estate,29,none,own,2,skilled employee / official,1,none,no,good
-no checking account,12,critical account/ other credits existing (not at this bank),car (new),926,... < 100 DM,unemployed,1,male : single,none,2,building society savings agreement/ life insurance,38,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1800,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",24,none,own,2,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,15,existing credits paid back duly till now,education,1905,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,furniture/equipment,1123,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",29,none,rent,1,unskilled - resident,1,none,yes,bad
-... < 0 DM,48,critical account/ other credits existing (not at this bank),car (used),6331,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,46,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,radio/television,1377,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,2,unknown / no property,47,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,30,delay in paying off in the past,business,2503,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,2,building society savings agreement/ life insurance,41,stores,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,27,existing credits paid back duly till now,business,2528,... < 100 DM,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,32,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,15,existing credits paid back duly till now,car (new),5324,500 <= ... < 1000 DM,... >= 7 years,1,male : single,none,4,unknown / no property,35,none,for free,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,48,existing credits paid back duly till now,car (new),6560,100 <= ... < 500 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,24,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,12,no credits taken/ all credits paid back duly,furniture/equipment,2969,... < 100 DM,... < 1 year,4,male : single,none,3,building society savings agreement/ life insurance,25,none,rent,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,1206,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,25,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,2118,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,37,none,own,1,unskilled - resident,2,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,629,500 <= ... < 1000 DM,... >= 7 years,4,male : single,none,3,building society savings agreement/ life insurance,32,bank,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,6,all credits at this bank paid back duly,education,1198,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,35,none,for free,1,skilled employee / official,1,none,yes,bad
-no checking account,21,existing credits paid back duly till now,car (used),2476,unknown/ no savings account,... >= 7 years,4,male : single,none,4,real estate,46,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,9,critical account/ other credits existing (not at this bank),radio/television,1138,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,25,none,own,2,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,60,existing credits paid back duly till now,car (new),14027,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,unknown / no property,27,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,30,critical account/ other credits existing (not at this bank),car (used),7596,unknown/ no savings account,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",63,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,30,critical account/ other credits existing (not at this bank),radio/television,3077,unknown/ no savings account,... >= 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",40,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,18,existing credits paid back duly till now,radio/television,1505,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,unknown / no property,32,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,24,critical account/ other credits existing (not at this bank),radio/television,3148,unknown/ no savings account,1 <= ... < 4 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,20,no credits taken/ all credits paid back duly,car (used),6148,100 <= ... < 500 DM,... >= 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",31,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,9,no credits taken/ all credits paid back duly,radio/television,1337,... < 100 DM,... < 1 year,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,6,all credits at this bank paid back duly,education,433,... >= 1000 DM,... < 1 year,4,male : single,none,2,building society savings agreement/ life insurance,24,bank,rent,1,skilled employee / official,2,none,yes,bad
-... < 0 DM,12,existing credits paid back duly till now,car (new),1228,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,24,none,own,1,unskilled - resident,1,none,yes,bad
-0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,790,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,66,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,27,existing credits paid back duly till now,car (new),2570,... < 100 DM,1 <= ... < 4 years,3,male : single,none,3,real estate,21,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,6,critical account/ other credits existing (not at this bank),car (new),250,... >= 1000 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,41,bank,own,2,unskilled - resident,1,none,yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1316,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,47,none,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,radio/television,1882,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",25,bank,rent,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,48,all credits at this bank paid back duly,business,6416,... < 100 DM,... >= 7 years,4,male : single,none,3,unknown / no property,59,none,rent,1,skilled employee / official,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,24,critical account/ other credits existing (not at this bank),business,1275,... >= 1000 DM,1 <= ... < 4 years,2,male : single,none,4,real estate,36,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,delay in paying off in the past,radio/television,6403,... < 100 DM,... < 1 year,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,radio/television,1987,... < 100 DM,1 <= ... < 4 years,2,male : single,none,4,real estate,21,none,rent,1,unskilled - resident,2,none,yes,bad
-0 <= ... < 200 DM,8,existing credits paid back duly till now,radio/television,760,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,2,real estate,44,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,car (used),2603,... >= 1000 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,4,critical account/ other credits existing (not at this bank),car (new),3380,... < 100 DM,4 <= ... < 7 years,1,male : single,none,1,real estate,37,none,own,1,skilled employee / official,2,none,yes,good
-0 <= ... < 200 DM,36,all credits at this bank paid back duly,domestic appliances,3990,unknown/ no savings account,... < 1 year,3,male : single,none,2,unknown / no property,29,bank,own,1,unemployed/ unskilled - non-resident,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (used),11560,... < 100 DM,1 <= ... < 4 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",23,none,rent,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
-... < 0 DM,18,existing credits paid back duly till now,car (new),4380,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",35,none,own,1,unskilled - resident,2,"yes, registered under the customers name",yes,good
-no checking account,6,critical account/ other credits existing (not at this bank),car (new),6761,... < 100 DM,4 <= ... < 7 years,1,male : single,none,3,unknown / no property,45,none,own,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,30,no credits taken/ all credits paid back duly,business,4280,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",26,none,rent,2,unskilled - resident,1,none,yes,bad
-... < 0 DM,24,all credits at this bank paid back duly,car (new),2325,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",32,bank,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,10,all credits at this bank paid back duly,radio/television,1048,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,23,stores,own,1,unskilled - resident,1,none,yes,good
-no checking account,21,existing credits paid back duly till now,radio/television,3160,unknown/ no savings account,... >= 7 years,4,male : single,none,3,building society savings agreement/ life insurance,41,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,2483,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,22,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,39,critical account/ other credits existing (not at this bank),furniture/equipment,14179,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,building society savings agreement/ life insurance,30,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,13,critical account/ other credits existing (not at this bank),business,1797,... < 100 DM,... < 1 year,3,male : single,none,1,building society savings agreement/ life insurance,28,bank,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,15,existing credits paid back duly till now,car (new),2511,... < 100 DM,unemployed,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",23,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,car (new),1274,... < 100 DM,... < 1 year,3,male : single,none,1,real estate,37,none,own,1,unskilled - resident,1,none,yes,bad
-no checking account,21,existing credits paid back duly till now,car (used),5248,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,3,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,15,existing credits paid back duly till now,car (used),3029,... < 100 DM,4 <= ... < 7 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,6,existing credits paid back duly till now,furniture/equipment,428,... < 100 DM,... >= 7 years,2,male : single,none,1,building society savings agreement/ life insurance,49,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,existing credits paid back duly till now,car (new),976,... < 100 DM,... < 1 year,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",23,none,own,1,unskilled - resident,1,none,yes,bad
-0 <= ... < 200 DM,12,existing credits paid back duly till now,business,841,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,4,real estate,23,none,rent,1,unskilled - resident,1,none,yes,good
-no checking account,30,critical account/ other credits existing (not at this bank),radio/television,5771,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,12,delay in paying off in the past,repairs,1555,... >= 1000 DM,... >= 7 years,4,male : single,none,4,unknown / no property,55,none,for free,2,skilled employee / official,2,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,car (new),1285,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,unknown / no property,32,none,rent,1,skilled employee / official,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,6,critical account/ other credits existing (not at this bank),car (new),1299,... < 100 DM,1 <= ... < 4 years,1,male : single,none,1,real estate,74,none,own,3,unemployed/ unskilled - non-resident,2,none,no,good
-... >= 200 DM / salary assignments for at least 1 year,15,critical account/ other credits existing (not at this bank),radio/television,1271,unknown/ no savings account,1 <= ... < 4 years,3,male : single,none,4,unknown / no property,39,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,24,existing credits paid back duly till now,car (new),1393,... < 100 DM,1 <= ... < 4 years,2,male : single,guarantor,2,real estate,31,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),691,... < 100 DM,... >= 7 years,4,male : single,none,3,building society savings agreement/ life insurance,35,none,own,2,skilled employee / official,1,none,yes,bad
-no checking account,15,critical account/ other credits existing (not at this bank),car (new),5045,unknown/ no savings account,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",59,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,2124,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,24,none,rent,2,skilled employee / official,1,none,yes,bad
-... < 0 DM,12,existing credits paid back duly till now,radio/television,2214,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,building society savings agreement/ life insurance,24,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,21,critical account/ other credits existing (not at this bank),car (new),12680,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,30,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),car (new),2463,100 <= ... < 500 DM,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1155,... < 100 DM,... >= 7 years,3,male : single,guarantor,3,real estate,40,bank,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,30,existing credits paid back duly till now,furniture/equipment,3108,... < 100 DM,... < 1 year,2,male : single,none,4,building society savings agreement/ life insurance,31,none,own,1,unskilled - resident,1,none,yes,bad
-no checking account,10,existing credits paid back duly till now,car (used),2901,unknown/ no savings account,... < 1 year,1,male : single,none,4,real estate,31,none,rent,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),furniture/equipment,3617,... < 100 DM,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,1655,... < 100 DM,... >= 7 years,2,male : single,none,4,real estate,63,none,own,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,existing credits paid back duly till now,car (used),2812,unknown/ no savings account,... >= 7 years,2,male : single,none,4,real estate,26,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,36,critical account/ other credits existing (not at this bank),education,8065,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,unknown / no property,25,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,21,critical account/ other credits existing (not at this bank),car (used),3275,... < 100 DM,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",36,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2223,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,52,bank,own,2,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,critical account/ other credits existing (not at this bank),car (new),1480,500 <= ... < 1000 DM,unemployed,2,male : single,none,4,unknown / no property,66,bank,for free,3,unemployed/ unskilled - non-resident,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,car (new),1371,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,real estate,25,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,36,critical account/ other credits existing (not at this bank),car (new),3535,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",37,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,existing credits paid back duly till now,radio/television,3509,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,1,real estate,25,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,36,critical account/ other credits existing (not at this bank),car (used),5711,... >= 1000 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",38,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,repairs,3872,... < 100 DM,unemployed,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",67,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,39,critical account/ other credits existing (not at this bank),radio/television,4933,... < 100 DM,4 <= ... < 7 years,2,male : single,guarantor,2,real estate,25,none,own,2,skilled employee / official,1,none,yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),car (new),1940,... >= 1000 DM,... >= 7 years,4,male : single,none,4,real estate,60,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,no credits taken/ all credits paid back duly,retraining,1410,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,31,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),836,100 <= ... < 500 DM,... < 1 year,4,male : single,none,2,building society savings agreement/ life insurance,23,bank,own,1,unskilled - resident,1,none,yes,bad
-0 <= ... < 200 DM,20,existing credits paid back duly till now,car (used),6468,unknown/ no savings account,unemployed,1,male : single,none,4,real estate,60,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,18,existing credits paid back duly till now,business,1941,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,35,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
-no checking account,22,existing credits paid back duly till now,radio/television,2675,500 <= ... < 1000 DM,... >= 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,48,critical account/ other credits existing (not at this bank),car (used),2751,unknown/ no savings account,... >= 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",38,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,48,delay in paying off in the past,education,6224,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,50,none,for free,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,40,critical account/ other credits existing (not at this bank),education,5998,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,unknown / no property,27,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,21,existing credits paid back duly till now,business,1188,... < 100 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,39,none,own,1,skilled employee / official,2,none,yes,bad
-no checking account,24,existing credits paid back duly till now,car (used),6313,unknown/ no savings account,... >= 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",41,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-no checking account,6,critical account/ other credits existing (not at this bank),furniture/equipment,1221,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,2,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,furniture/equipment,2892,... < 100 DM,... >= 7 years,3,male : single,none,4,unknown / no property,51,none,for free,1,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,furniture/equipment,3062,500 <= ... < 1000 DM,... >= 7 years,4,male : single,none,3,unknown / no property,32,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,9,existing credits paid back duly till now,furniture/equipment,2301,100 <= ... < 500 DM,... < 1 year,2,male : single,none,4,building society savings agreement/ life insurance,22,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,car (used),7511,unknown/ no savings account,... >= 7 years,1,male : single,none,4,building society savings agreement/ life insurance,51,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
-no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,1258,... < 100 DM,... < 1 year,2,male : single,none,4,building society savings agreement/ life insurance,22,none,rent,2,unskilled - resident,1,none,yes,good
-no checking account,24,delay in paying off in the past,car (new),717,unknown/ no savings account,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",54,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,car (new),1549,unknown/ no savings account,... < 1 year,4,male : single,none,2,real estate,35,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),education,1597,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,54,none,for free,2,skilled employee / official,2,none,yes,good
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),radio/television,1795,... < 100 DM,... >= 7 years,3,male : single,guarantor,4,real estate,48,bank,rent,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
-... < 0 DM,20,critical account/ other credits existing (not at this bank),furniture/equipment,4272,... < 100 DM,... >= 7 years,1,male : single,none,4,building society savings agreement/ life insurance,24,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,976,unknown/ no savings account,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",35,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),7472,unknown/ no savings account,unemployed,1,male : single,none,2,real estate,24,none,rent,1,unemployed/ unskilled - non-resident,1,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,car (new),9271,... < 100 DM,4 <= ... < 7 years,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,590,... < 100 DM,... < 1 year,3,male : single,none,3,real estate,26,none,own,1,unskilled - resident,1,none,no,good
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,930,unknown/ no savings account,... >= 7 years,4,male : single,none,4,real estate,65,none,own,4,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,42,all credits at this bank paid back duly,car (used),9283,... < 100 DM,unemployed,1,male : single,none,2,unknown / no property,55,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,15,no credits taken/ all credits paid back duly,car (new),1778,... < 100 DM,... < 1 year,2,male : single,none,1,real estate,26,none,rent,2,unemployed/ unskilled - non-resident,1,none,yes,bad
-0 <= ... < 200 DM,8,existing credits paid back duly till now,business,907,... < 100 DM,... < 1 year,3,male : single,none,2,real estate,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,484,... < 100 DM,4 <= ... < 7 years,3,male : single,guarantor,3,real estate,28,bank,own,1,unskilled - resident,1,none,yes,good
-... < 0 DM,36,critical account/ other credits existing (not at this bank),car (used),9629,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",24,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,48,existing credits paid back duly till now,domestic appliances,3051,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",54,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,48,existing credits paid back duly till now,car (new),3931,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,unknown / no property,46,none,for free,1,skilled employee / official,2,none,yes,bad
-0 <= ... < 200 DM,36,delay in paying off in the past,car (new),7432,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,54,none,rent,1,skilled employee / official,1,none,yes,good
-no checking account,6,existing credits paid back duly till now,domestic appliances,1338,500 <= ... < 1000 DM,1 <= ... < 4 years,1,male : single,none,4,real estate,62,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1554,... < 100 DM,4 <= ... < 7 years,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",24,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,36,existing credits paid back duly till now,others,15857,... < 100 DM,unemployed,2,male : single,co-applicant,3,"car or other, not in attribute Savings account/bonds",43,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,radio/television,1345,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,26,bank,own,1,skilled employee / official,1,none,yes,bad
-no checking account,12,existing credits paid back duly till now,car (new),1101,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,27,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,radio/television,3016,... < 100 DM,1 <= ... < 4 years,3,male : single,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,2712,... < 100 DM,... >= 7 years,2,male : single,none,2,building society savings agreement/ life insurance,41,bank,own,1,skilled employee / official,2,none,yes,bad
-... < 0 DM,8,critical account/ other credits existing (not at this bank),car (new),731,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,47,none,own,2,unskilled - resident,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),furniture/equipment,3780,... < 100 DM,... < 1 year,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",35,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,21,critical account/ other credits existing (not at this bank),car (new),1602,... < 100 DM,... >= 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,critical account/ other credits existing (not at this bank),car (new),3966,... < 100 DM,... >= 7 years,1,male : single,none,4,real estate,33,bank,rent,3,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,18,no credits taken/ all credits paid back duly,business,4165,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",36,stores,own,2,skilled employee / official,2,none,yes,bad
-... < 0 DM,36,existing credits paid back duly till now,car (used),8335,unknown/ no savings account,... >= 7 years,3,male : single,none,4,unknown / no property,47,none,for free,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,48,delay in paying off in the past,business,6681,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,38,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,24,delay in paying off in the past,business,2375,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",44,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,18,existing credits paid back duly till now,car (new),1216,... < 100 DM,... < 1 year,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",23,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,45,no credits taken/ all credits paid back duly,business,11816,... < 100 DM,... >= 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",29,none,rent,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,5084,unknown/ no savings account,... >= 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,15,existing credits paid back duly till now,radio/television,2327,... < 100 DM,... < 1 year,2,male : single,none,3,real estate,25,none,own,1,unskilled - resident,1,none,yes,bad
-... < 0 DM,12,no credits taken/ all credits paid back duly,car (new),1082,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",48,bank,own,2,skilled employee / official,1,none,yes,bad
-no checking account,12,existing credits paid back duly till now,radio/television,886,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",21,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,4,existing credits paid back duly till now,furniture/equipment,601,... < 100 DM,... < 1 year,1,male : single,none,3,real estate,23,none,rent,1,unskilled - resident,2,none,yes,good
-... < 0 DM,24,critical account/ other credits existing (not at this bank),car (used),2957,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,63,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2611,... < 100 DM,... >= 7 years,4,male : single,co-applicant,3,real estate,46,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,5179,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,building society savings agreement/ life insurance,29,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,21,delay in paying off in the past,car (used),2993,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,28,stores,own,2,unskilled - resident,1,none,yes,good
-no checking account,18,existing credits paid back duly till now,repairs,1943,... < 100 DM,... < 1 year,4,male : single,none,4,real estate,23,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,24,all credits at this bank paid back duly,business,1559,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",50,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,18,existing credits paid back duly till now,furniture/equipment,3422,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,47,bank,own,3,skilled employee / official,2,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,21,existing credits paid back duly till now,furniture/equipment,3976,unknown/ no savings account,4 <= ... < 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",35,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,18,existing credits paid back duly till now,car (new),6761,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",68,none,rent,2,skilled employee / official,1,none,yes,bad
-no checking account,24,existing credits paid back duly till now,car (new),1249,... < 100 DM,... < 1 year,4,male : single,none,2,real estate,28,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,9,existing credits paid back duly till now,radio/television,1364,... < 100 DM,4 <= ... < 7 years,3,male : single,none,4,real estate,59,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,radio/television,709,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,57,stores,own,1,unskilled - resident,1,none,yes,bad
-... < 0 DM,20,critical account/ other credits existing (not at this bank),car (new),2235,... < 100 DM,1 <= ... < 4 years,4,male : single,guarantor,2,building society savings agreement/ life insurance,33,bank,rent,2,skilled employee / official,1,none,no,bad
-no checking account,24,critical account/ other credits existing (not at this bank),car (used),4042,unknown/ no savings account,4 <= ... < 7 years,3,male : single,none,4,building society savings agreement/ life insurance,43,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1471,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,35,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,18,all credits at this bank paid back duly,car (new),1442,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,unknown / no property,32,none,for free,2,unskilled - resident,2,none,yes,bad
-no checking account,36,delay in paying off in the past,car (new),10875,... < 100 DM,... >= 7 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",45,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,car (new),1474,100 <= ... < 500 DM,... < 1 year,4,male : single,none,3,real estate,33,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,10,existing credits paid back duly till now,retraining,894,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,40,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),furniture/equipment,3343,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,unknown / no property,28,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,15,existing credits paid back duly till now,car (new),3959,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,building society savings agreement/ life insurance,29,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,9,existing credits paid back duly till now,car (new),3577,100 <= ... < 500 DM,1 <= ... < 4 years,1,male : single,guarantor,2,real estate,26,none,rent,1,skilled employee / official,2,none,no,good
-no checking account,24,critical account/ other credits existing (not at this bank),car (used),5804,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,27,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,delay in paying off in the past,business,2169,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,24,existing credits paid back duly till now,radio/television,2439,... < 100 DM,... < 1 year,4,male : single,none,4,real estate,35,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,27,critical account/ other credits existing (not at this bank),furniture/equipment,4526,... >= 1000 DM,... < 1 year,4,male : single,none,2,real estate,32,stores,own,2,unskilled - resident,2,"yes, registered under the customers name",yes,good
-no checking account,10,existing credits paid back duly till now,furniture/equipment,2210,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,25,bank,rent,1,unskilled - resident,1,none,yes,bad
-no checking account,15,existing credits paid back duly till now,furniture/equipment,2221,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",20,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,radio/television,2389,... < 100 DM,... < 1 year,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",27,stores,own,1,skilled employee / official,1,none,yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,3331,... < 100 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,42,stores,own,1,skilled employee / official,1,none,yes,good
-no checking account,36,existing credits paid back duly till now,business,7409,unknown/ no savings account,... >= 7 years,3,male : single,none,2,building society savings agreement/ life insurance,37,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,652,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,24,none,rent,1,skilled employee / official,1,none,yes,good
-no checking account,36,delay in paying off in the past,furniture/equipment,7678,500 <= ... < 1000 DM,4 <= ... < 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,6,critical account/ other credits existing (not at this bank),car (new),1343,... < 100 DM,... >= 7 years,1,male : single,none,4,real estate,46,none,own,2,skilled employee / official,2,none,no,good
-... < 0 DM,24,critical account/ other credits existing (not at this bank),business,1382,100 <= ... < 500 DM,4 <= ... < 7 years,4,male : single,none,1,real estate,26,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,15,existing credits paid back duly till now,domestic appliances,874,unknown/ no savings account,... < 1 year,4,male : single,none,1,real estate,24,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,3590,... < 100 DM,1 <= ... < 4 years,2,male : single,co-applicant,2,building society savings agreement/ life insurance,29,none,own,1,unskilled - resident,2,none,yes,good
-0 <= ... < 200 DM,11,critical account/ other credits existing (not at this bank),car (new),1322,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,18,all credits at this bank paid back duly,radio/television,1940,... < 100 DM,... < 1 year,3,male : single,co-applicant,4,unknown / no property,36,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,36,existing credits paid back duly till now,radio/television,3595,... < 100 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,9,existing credits paid back duly till now,car (new),1422,... < 100 DM,... < 1 year,3,male : single,none,2,unknown / no property,27,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,30,critical account/ other credits existing (not at this bank),radio/television,6742,unknown/ no savings account,4 <= ... < 7 years,2,male : single,none,3,building society savings agreement/ life insurance,36,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,car (used),7814,... < 100 DM,4 <= ... < 7 years,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",38,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,car (used),9277,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,4,unknown / no property,48,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,30,critical account/ other credits existing (not at this bank),car (new),2181,unknown/ no savings account,... >= 7 years,4,male : single,none,4,real estate,36,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1098,... < 100 DM,unemployed,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",65,none,own,2,unemployed/ unskilled - non-resident,1,none,yes,good
-0 <= ... < 200 DM,24,existing credits paid back duly till now,furniture/equipment,4057,... < 100 DM,4 <= ... < 7 years,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",43,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,12,existing credits paid back duly till now,education,795,... < 100 DM,... < 1 year,4,male : single,none,4,building society savings agreement/ life insurance,53,none,own,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),business,2825,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,3,unknown / no property,34,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,48,existing credits paid back duly till now,business,15672,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",23,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,36,critical account/ other credits existing (not at this bank),car (new),6614,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,28,all credits at this bank paid back duly,car (used),7824,unknown/ no savings account,... < 1 year,3,male : single,guarantor,4,real estate,40,bank,rent,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,27,critical account/ other credits existing (not at this bank),business,2442,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",43,stores,own,4,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1829,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",46,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),2171,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,building society savings agreement/ life insurance,38,bank,own,2,unskilled - resident,1,none,no,good
-0 <= ... < 200 DM,36,critical account/ other credits existing (not at this bank),car (used),5800,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",34,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1169,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,3,building society savings agreement/ life insurance,29,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,36,delay in paying off in the past,car (used),8947,unknown/ no savings account,4 <= ... < 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,stores,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-... < 0 DM,21,existing credits paid back duly till now,radio/television,2606,... < 100 DM,... < 1 year,4,male : single,none,4,building society savings agreement/ life insurance,28,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,1592,... >= 1000 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,35,none,own,1,skilled employee / official,1,none,no,good
-no checking account,15,existing credits paid back duly till now,furniture/equipment,2186,unknown/ no savings account,4 <= ... < 7 years,1,male : single,none,4,real estate,33,bank,rent,1,unskilled - resident,1,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,4153,... < 100 DM,1 <= ... < 4 years,2,male : single,co-applicant,3,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,16,critical account/ other credits existing (not at this bank),car (new),2625,... < 100 DM,... >= 7 years,2,male : single,guarantor,4,building society savings agreement/ life insurance,43,bank,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,20,critical account/ other credits existing (not at this bank),car (new),3485,unknown/ no savings account,... < 1 year,2,male : single,none,4,real estate,44,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,36,critical account/ other credits existing (not at this bank),car (used),10477,unknown/ no savings account,... >= 7 years,2,male : single,none,4,unknown / no property,42,none,for free,2,skilled employee / official,1,none,yes,good
-no checking account,15,existing credits paid back duly till now,radio/television,1386,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,real estate,40,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,1278,... < 100 DM,... >= 7 years,4,male : single,none,1,real estate,36,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,radio/television,1107,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,20,none,rent,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-... < 0 DM,21,existing credits paid back duly till now,car (new),3763,unknown/ no savings account,4 <= ... < 7 years,2,male : single,co-applicant,2,real estate,24,none,own,1,unskilled - resident,1,none,no,good
-0 <= ... < 200 DM,36,existing credits paid back duly till now,education,3711,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,15,delay in paying off in the past,car (used),3594,... < 100 DM,... < 1 year,1,male : married/widowed,none,2,building society savings agreement/ life insurance,46,none,own,2,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,car (new),3195,unknown/ no savings account,1 <= ... < 4 years,1,male : married/widowed,none,2,real estate,33,none,own,1,unskilled - resident,1,none,yes,good
-no checking account,36,delay in paying off in the past,radio/television,4454,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,4,real estate,34,none,own,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),furniture/equipment,4736,... < 100 DM,... < 1 year,2,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",25,bank,own,1,unskilled - resident,1,none,yes,bad
-0 <= ... < 200 DM,30,existing credits paid back duly till now,radio/television,2991,unknown/ no savings account,... >= 7 years,2,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",25,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,11,existing credits paid back duly till now,business,2142,... >= 1000 DM,... >= 7 years,1,male : married/widowed,none,2,real estate,28,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,all credits at this bank paid back duly,business,3161,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,31,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,others,18424,... < 100 DM,1 <= ... < 4 years,1,male : married/widowed,none,2,building society savings agreement/ life insurance,32,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",no,bad
-no checking account,10,existing credits paid back duly till now,car (used),2848,100 <= ... < 500 DM,1 <= ... < 4 years,1,male : married/widowed,co-applicant,2,real estate,32,none,own,1,skilled employee / official,2,none,yes,good
-... < 0 DM,6,existing credits paid back duly till now,car (new),14896,... < 100 DM,... >= 7 years,1,male : married/widowed,none,4,unknown / no property,68,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,2359,100 <= ... < 500 DM,unemployed,1,male : married/widowed,none,1,building society savings agreement/ life insurance,33,none,own,1,skilled employee / official,1,none,yes,bad
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,3345,... < 100 DM,... >= 7 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,39,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-no checking account,18,critical account/ other credits existing (not at this bank),furniture/equipment,1817,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,unknown / no property,28,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,48,delay in paying off in the past,radio/television,12749,500 <= ... < 1000 DM,4 <= ... < 7 years,4,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",37,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,9,existing credits paid back duly till now,radio/television,1366,... < 100 DM,... < 1 year,3,male : married/widowed,none,4,building society savings agreement/ life insurance,22,none,rent,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),2002,... < 100 DM,4 <= ... < 7 years,3,male : married/widowed,none,4,building society savings agreement/ life insurance,30,none,rent,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,6872,... < 100 DM,... < 1 year,2,male : married/widowed,none,1,building society savings agreement/ life insurance,55,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,12,all credits at this bank paid back duly,car (new),697,... < 100 DM,... < 1 year,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",46,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,1049,... < 100 DM,... < 1 year,4,male : married/widowed,none,4,building society savings agreement/ life insurance,21,none,rent,1,skilled employee / official,1,none,yes,good
-... < 0 DM,48,existing credits paid back duly till now,car (used),10297,... < 100 DM,4 <= ... < 7 years,4,male : married/widowed,none,4,unknown / no property,39,stores,for free,3,skilled employee / official,2,"yes, registered under the customers name",yes,bad
-no checking account,30,existing credits paid back duly till now,radio/television,1867,unknown/ no savings account,... >= 7 years,4,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",58,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,12,delay in paying off in the past,car (new),1344,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,real estate,43,none,own,2,unskilled - resident,2,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,1747,... < 100 DM,... < 1 year,4,male : married/widowed,co-applicant,1,building society savings agreement/ life insurance,24,none,own,1,unskilled - resident,1,none,no,good
-0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,1670,... < 100 DM,... < 1 year,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",22,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-no checking account,9,critical account/ other credits existing (not at this bank),car (new),1224,... < 100 DM,1 <= ... < 4 years,3,male : married/widowed,none,1,real estate,30,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),radio/television,522,500 <= ... < 1000 DM,... >= 7 years,4,male : married/widowed,none,4,building society savings agreement/ life insurance,42,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
-... < 0 DM,12,existing credits paid back duly till now,radio/television,1498,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",23,bank,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,30,delay in paying off in the past,radio/television,1919,100 <= ... < 500 DM,... < 1 year,4,male : married/widowed,none,3,unknown / no property,30,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
-... >= 200 DM / salary assignments for at least 1 year,9,existing credits paid back duly till now,radio/television,745,... < 100 DM,1 <= ... < 4 years,3,male : married/widowed,none,2,real estate,28,none,own,1,unskilled - resident,1,none,yes,bad
-0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,2063,... < 100 DM,... < 1 year,4,male : married/widowed,none,3,"car or other, not in attribute Savings account/bonds",30,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,60,existing credits paid back duly till now,education,6288,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,4,unknown / no property,42,none,for free,1,skilled employee / official,1,none,yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),car (used),6842,unknown/ no savings account,1 <= ... < 4 years,2,male : married/widowed,none,4,building society savings agreement/ life insurance,46,none,own,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,car (new),3527,unknown/ no savings account,... < 1 year,2,male : married/widowed,none,3,building society savings agreement/ life insurance,45,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
-no checking account,10,existing credits paid back duly till now,car (new),1546,... < 100 DM,1 <= ... < 4 years,3,male : married/widowed,none,2,real estate,31,none,own,1,unskilled - resident,2,none,no,good
-no checking account,24,existing credits paid back duly till now,furniture/equipment,929,unknown/ no savings account,4 <= ... < 7 years,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",31,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,4,critical account/ other credits existing (not at this bank),car (new),1455,... < 100 DM,4 <= ... < 7 years,2,male : married/widowed,none,1,real estate,42,none,own,3,unskilled - resident,2,none,yes,good
-... < 0 DM,15,existing credits paid back duly till now,furniture/equipment,1845,... < 100 DM,... < 1 year,4,male : married/widowed,guarantor,1,building society savings agreement/ life insurance,46,none,rent,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,car (new),8358,500 <= ... < 1000 DM,... < 1 year,1,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",30,none,own,2,skilled employee / official,1,none,yes,good
-... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,3349,500 <= ... < 1000 DM,... < 1 year,4,male : married/widowed,none,4,unknown / no property,30,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
-no checking account,12,existing credits paid back duly till now,car (new),2859,unknown/ no savings account,unemployed,4,male : married/widowed,none,4,unknown / no property,38,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,18,existing credits paid back duly till now,furniture/equipment,1533,... < 100 DM,... < 1 year,4,male : married/widowed,co-applicant,1,building society savings agreement/ life insurance,43,none,own,1,unskilled - resident,2,none,yes,bad
-no checking account,24,existing credits paid back duly till now,radio/television,3621,100 <= ... < 500 DM,... >= 7 years,2,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",31,none,own,2,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),business,3590,... < 100 DM,unemployed,3,male : married/widowed,none,3,"car or other, not in attribute Savings account/bonds",40,none,own,3,unemployed/ unskilled - non-resident,2,"yes, registered under the customers name",yes,good
-... < 0 DM,36,delay in paying off in the past,business,2145,... < 100 DM,4 <= ... < 7 years,2,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,24,existing credits paid back duly till now,car (used),4113,500 <= ... < 1000 DM,... < 1 year,3,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,36,existing credits paid back duly till now,furniture/equipment,10974,... < 100 DM,unemployed,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... < 0 DM,12,existing credits paid back duly till now,car (new),1893,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,guarantor,4,building society savings agreement/ life insurance,29,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,24,critical account/ other credits existing (not at this bank),radio/television,1231,... >= 1000 DM,... >= 7 years,4,male : married/widowed,none,4,building society savings agreement/ life insurance,57,none,rent,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,30,critical account/ other credits existing (not at this bank),radio/television,3656,unknown/ no savings account,... >= 7 years,4,male : married/widowed,none,4,building society savings agreement/ life insurance,49,stores,own,2,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,9,critical account/ other credits existing (not at this bank),radio/television,1154,... < 100 DM,... >= 7 years,2,male : married/widowed,none,4,real estate,37,none,own,3,unskilled - resident,1,none,yes,good
-... < 0 DM,28,existing credits paid back duly till now,car (new),4006,... < 100 DM,1 <= ... < 4 years,3,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",45,none,own,1,unskilled - resident,1,none,yes,bad
-0 <= ... < 200 DM,24,existing credits paid back duly till now,furniture/equipment,3069,100 <= ... < 500 DM,... >= 7 years,4,male : married/widowed,none,4,unknown / no property,30,none,for free,1,skilled employee / official,1,none,yes,good
-no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1740,... < 100 DM,... >= 7 years,2,male : married/widowed,none,2,real estate,30,none,rent,2,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,21,delay in paying off in the past,car (new),2353,... < 100 DM,1 <= ... < 4 years,1,male : married/widowed,none,4,building society savings agreement/ life insurance,47,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,15,existing credits paid back duly till now,car (new),3556,unknown/ no savings account,1 <= ... < 4 years,3,male : married/widowed,none,2,unknown / no property,29,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,radio/television,2397,500 <= ... < 1000 DM,... >= 7 years,3,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",35,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,6,existing credits paid back duly till now,repairs,454,... < 100 DM,... < 1 year,3,male : married/widowed,none,1,building society savings agreement/ life insurance,22,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,30,existing credits paid back duly till now,radio/television,1715,unknown/ no savings account,1 <= ... < 4 years,4,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,27,critical account/ other credits existing (not at this bank),radio/television,2520,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,23,none,own,2,unskilled - resident,1,none,yes,bad
-no checking account,15,existing credits paid back duly till now,radio/television,3568,... < 100 DM,... >= 7 years,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",54,bank,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,42,existing credits paid back duly till now,radio/television,7166,unknown/ no savings account,4 <= ... < 7 years,2,male : married/widowed,none,4,building society savings agreement/ life insurance,29,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... < 0 DM,11,critical account/ other credits existing (not at this bank),car (new),3939,... < 100 DM,1 <= ... < 4 years,1,male : married/widowed,none,2,real estate,40,none,own,2,unskilled - resident,2,none,yes,good
-0 <= ... < 200 DM,15,existing credits paid back duly till now,repairs,1514,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : married/widowed,guarantor,2,real estate,22,none,own,1,skilled employee / official,1,none,yes,good
-no checking account,24,existing credits paid back duly till now,car (new),7393,... < 100 DM,1 <= ... < 4 years,1,male : married/widowed,none,4,building society savings agreement/ life insurance,43,none,own,1,unskilled - resident,2,none,yes,good
-... < 0 DM,24,all credits at this bank paid back duly,car (new),1193,... < 100 DM,unemployed,1,male : married/widowed,co-applicant,4,unknown / no property,29,none,rent,2,unemployed/ unskilled - non-resident,1,none,yes,bad
-... < 0 DM,60,existing credits paid back duly till now,business,7297,... < 100 DM,... >= 7 years,4,male : married/widowed,co-applicant,4,unknown / no property,36,none,rent,1,skilled employee / official,1,none,yes,bad
-no checking account,30,critical account/ other credits existing (not at this bank),radio/television,2831,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,radio/television,1258,500 <= ... < 1000 DM,1 <= ... < 4 years,3,male : married/widowed,none,3,"car or other, not in attribute Savings account/bonds",57,none,own,1,unskilled - resident,1,none,yes,good
-0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,753,... < 100 DM,1 <= ... < 4 years,2,male : married/widowed,guarantor,3,real estate,64,none,own,1,skilled employee / official,1,none,yes,good
-0 <= ... < 200 DM,18,delay in paying off in the past,business,2427,unknown/ no savings account,... >= 7 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,42,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,24,delay in paying off in the past,car (new),2538,... < 100 DM,... >= 7 years,4,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",47,none,own,2,unskilled - resident,2,none,yes,bad
-0 <= ... < 200 DM,15,all credits at this bank paid back duly,car (new),1264,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : married/widowed,none,2,building society savings agreement/ life insurance,25,none,rent,1,skilled employee / official,1,none,yes,bad
-0 <= ... < 200 DM,30,critical account/ other credits existing (not at this bank),furniture/equipment,8386,... < 100 DM,4 <= ... < 7 years,2,male : married/widowed,none,2,building society savings agreement/ life insurance,49,none,own,1,skilled employee / official,1,none,yes,bad
-no checking account,48,existing credits paid back duly till now,business,4844,... < 100 DM,unemployed,3,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",33,bank,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
-... >= 200 DM / salary assignments for at least 1 year,21,existing credits paid back duly till now,car (new),2923,100 <= ... < 500 DM,1 <= ... < 4 years,1,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",28,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-... < 0 DM,36,existing credits paid back duly till now,car (used),8229,... < 100 DM,1 <= ... < 4 years,2,male : married/widowed,none,2,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,2,none,yes,bad
-no checking account,24,critical account/ other credits existing (not at this bank),furniture/equipment,2028,... < 100 DM,4 <= ... < 7 years,2,male : married/widowed,none,2,building society savings agreement/ life insurance,30,none,own,2,unskilled - resident,1,none,yes,good
-... < 0 DM,15,critical account/ other credits existing (not at this bank),furniture/equipment,1433,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,3,building society savings agreement/ life insurance,25,none,rent,2,skilled employee / official,1,none,yes,good
-... >= 200 DM / salary assignments for at least 1 year,42,no credits taken/ all credits paid back duly,business,6289,... < 100 DM,... < 1 year,2,male : married/widowed,none,1,building society savings agreement/ life insurance,33,none,own,2,skilled employee / official,1,none,yes,good
-no checking account,13,existing credits paid back duly till now,radio/television,1409,100 <= ... < 500 DM,unemployed,2,male : married/widowed,none,4,real estate,64,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,24,existing credits paid back duly till now,car (used),6579,... < 100 DM,unemployed,4,male : married/widowed,none,2,unknown / no property,29,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),radio/television,1743,... < 100 DM,... >= 7 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,48,none,own,2,unskilled - resident,1,none,yes,good
-no checking account,12,critical account/ other credits existing (not at this bank),education,3565,unknown/ no savings account,... < 1 year,2,male : married/widowed,none,1,building society savings agreement/ life insurance,37,none,own,2,unskilled - resident,2,none,yes,good
-no checking account,15,all credits at this bank paid back duly,radio/television,1569,100 <= ... < 500 DM,... >= 7 years,4,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",34,bank,own,1,unskilled - resident,2,none,yes,good
-... < 0 DM,18,existing credits paid back duly till now,radio/television,1936,unknown/ no savings account,4 <= ... < 7 years,2,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",23,none,rent,2,unskilled - resident,1,none,yes,good
-... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,3959,... < 100 DM,unemployed,4,male : married/widowed,none,3,building society savings agreement/ life insurance,30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,car (new),2390,unknown/ no savings account,... >= 7 years,4,male : married/widowed,none,3,"car or other, not in attribute Savings account/bonds",50,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,furniture/equipment,1736,... < 100 DM,4 <= ... < 7 years,3,male : married/widowed,none,4,real estate,31,none,own,1,unskilled - resident,1,none,yes,good
-... < 0 DM,30,existing credits paid back duly till now,car (used),3857,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,4,building society savings agreement/ life insurance,40,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
-no checking account,12,existing credits paid back duly till now,radio/television,804,... < 100 DM,... >= 7 years,4,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",38,none,own,1,skilled employee / official,1,none,yes,good
-... < 0 DM,45,existing credits paid back duly till now,radio/television,1845,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,4,unknown / no property,23,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
-0 <= ... < 200 DM,45,critical account/ other credits existing (not at this bank),car (used),4576,100 <= ... < 500 DM,unemployed,3,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",27,none,own,1,skilled employee / official,1,none,yes,good
+status_of_existing_checking_account,duration_in_month,credit_history,purpose,credit_amount,savings_account_and_bonds,present_employment_since,installment_rate_in_percentage_of_disposable_income,personal_status_and_sex,other_debtors_or_guarantors,present_residence_since,property,age_in_years,other_installment_plans,housing,number_of_existing_credits_at_this_bank,job,number_of_people_being_liable_to_provide_maintenance_for,telephone,foreign_worker,creditability
+... < 0 DM,6,critical account/ other credits existing (not at this bank),radio/television,1169,unknown/ no savings account,... >= 7 years,4,male : divorced/separated,none,4,real estate,67,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,48,existing credits paid back duly till now,radio/television,5951,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,real estate,22,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),education,2096,... < 100 DM,4 <= ... < 7 years,2,male : divorced/separated,none,3,real estate,49,none,own,1,unskilled - resident,2,none,yes,good
+... < 0 DM,42,existing credits paid back duly till now,furniture/equipment,7882,... < 100 DM,4 <= ... < 7 years,2,male : divorced/separated,guarantor,4,building society savings agreement/ life insurance,45,none,for free,1,skilled employee / official,2,none,yes,good
+... < 0 DM,24,delay in paying off in the past,car (new),4870,... < 100 DM,1 <= ... < 4 years,3,male : divorced/separated,none,4,unknown / no property,53,none,for free,2,skilled employee / official,2,none,yes,bad
+no checking account,36,existing credits paid back duly till now,education,9055,unknown/ no savings account,1 <= ... < 4 years,2,male : divorced/separated,none,4,unknown / no property,35,none,for free,1,unskilled - resident,2,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,furniture/equipment,2835,500 <= ... < 1000 DM,... >= 7 years,3,male : divorced/separated,none,4,building society savings agreement/ life insurance,53,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,car (used),6948,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",35,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,3059,... >= 1000 DM,4 <= ... < 7 years,2,male : divorced/separated,none,4,real estate,61,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,30,critical account/ other credits existing (not at this bank),car (new),5234,... < 100 DM,unemployed,4,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),1295,... < 100 DM,... < 1 year,3,male : divorced/separated,none,1,"car or other, not in attribute Savings account/bonds",25,none,rent,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,48,existing credits paid back duly till now,business,4308,... < 100 DM,... < 1 year,3,male : divorced/separated,none,4,building society savings agreement/ life insurance,24,none,rent,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1567,... < 100 DM,1 <= ... < 4 years,1,male : divorced/separated,none,1,"car or other, not in attribute Savings account/bonds",22,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,critical account/ other credits existing (not at this bank),car (new),1199,... < 100 DM,... >= 7 years,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",60,none,own,2,unskilled - resident,1,none,yes,bad
+... < 0 DM,15,existing credits paid back duly till now,car (new),1403,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,radio/television,1282,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,1,unskilled - resident,1,none,yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2424,unknown/ no savings account,... >= 7 years,4,male : divorced/separated,none,4,building society savings agreement/ life insurance,53,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,30,no credits taken/ all credits paid back duly,business,8072,unknown/ no savings account,... < 1 year,2,male : divorced/separated,none,3,"car or other, not in attribute Savings account/bonds",25,bank,own,3,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (used),12579,... < 100 DM,... >= 7 years,4,male : divorced/separated,none,2,unknown / no property,44,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,24,existing credits paid back duly till now,radio/television,3430,500 <= ... < 1000 DM,... >= 7 years,3,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,9,critical account/ other credits existing (not at this bank),car (new),2134,... < 100 DM,1 <= ... < 4 years,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",48,none,own,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,6,existing credits paid back duly till now,radio/television,2647,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : divorced/separated,none,3,real estate,44,none,rent,1,skilled employee / official,2,none,yes,good
+... < 0 DM,10,critical account/ other credits existing (not at this bank),car (new),2241,... < 100 DM,... < 1 year,1,male : divorced/separated,none,3,real estate,48,none,rent,2,unskilled - resident,2,none,no,good
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (used),1804,100 <= ... < 500 DM,... < 1 year,3,male : divorced/separated,none,4,building society savings agreement/ life insurance,44,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,10,critical account/ other credits existing (not at this bank),furniture/equipment,2069,unknown/ no savings account,1 <= ... < 4 years,2,male : divorced/separated,none,1,"car or other, not in attribute Savings account/bonds",26,none,own,2,skilled employee / official,1,none,no,good
+... < 0 DM,6,existing credits paid back duly till now,furniture/equipment,1374,... < 100 DM,1 <= ... < 4 years,1,male : divorced/separated,none,2,real estate,36,bank,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+no checking account,6,no credits taken/ all credits paid back duly,radio/television,426,... < 100 DM,... >= 7 years,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",39,none,own,1,unskilled - resident,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,all credits at this bank paid back duly,radio/television,409,... >= 1000 DM,1 <= ... < 4 years,3,male : divorced/separated,none,3,real estate,42,none,rent,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,7,existing credits paid back duly till now,radio/television,2415,... < 100 DM,1 <= ... < 4 years,3,male : divorced/separated,guarantor,2,real estate,34,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,60,delay in paying off in the past,business,6836,... < 100 DM,... >= 7 years,3,male : divorced/separated,none,4,unknown / no property,63,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,18,existing credits paid back duly till now,business,1913,... >= 1000 DM,... < 1 year,3,male : divorced/separated,none,3,real estate,36,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,4020,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",27,stores,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,car (new),5866,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),business,1264,unknown/ no savings account,... >= 7 years,4,male : divorced/separated,none,4,unknown / no property,57,none,rent,1,unskilled - resident,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,furniture/equipment,1474,... < 100 DM,... < 1 year,4,male : divorced/separated,none,1,building society savings agreement/ life insurance,33,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,45,critical account/ other credits existing (not at this bank),radio/television,4746,... < 100 DM,... < 1 year,4,male : divorced/separated,none,2,building society savings agreement/ life insurance,25,none,own,2,unskilled - resident,1,none,yes,bad
+no checking account,48,critical account/ other credits existing (not at this bank),education,6110,... < 100 DM,1 <= ... < 4 years,1,male : divorced/separated,none,3,unknown / no property,31,bank,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,18,existing credits paid back duly till now,radio/television,2100,... < 100 DM,1 <= ... < 4 years,4,male : divorced/separated,co-applicant,2,real estate,37,stores,own,1,skilled employee / official,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,10,existing credits paid back duly till now,domestic appliances,1225,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",37,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,458,... < 100 DM,1 <= ... < 4 years,4,male : divorced/separated,none,3,real estate,24,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,30,existing credits paid back duly till now,radio/television,2333,500 <= ... < 1000 DM,... >= 7 years,4,male : divorced/separated,none,2,"car or other, not in attribute Savings account/bonds",30,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1158,500 <= ... < 1000 DM,1 <= ... < 4 years,3,male : divorced/separated,none,1,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,delay in paying off in the past,repairs,6204,... < 100 DM,1 <= ... < 4 years,2,male : divorced/separated,none,4,real estate,44,none,own,1,unskilled - resident,2,"yes, registered under the customers name",yes,good
+... < 0 DM,30,critical account/ other credits existing (not at this bank),car (used),6187,100 <= ... < 500 DM,4 <= ... < 7 years,1,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",24,none,rent,2,skilled employee / official,1,none,yes,good
+... < 0 DM,48,critical account/ other credits existing (not at this bank),car (used),6143,... < 100 DM,... >= 7 years,4,male : divorced/separated,none,4,unknown / no property,58,stores,for free,2,unskilled - resident,1,none,yes,bad
+no checking account,11,critical account/ other credits existing (not at this bank),car (new),1393,... < 100 DM,... < 1 year,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",35,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+no checking account,36,existing credits paid back duly till now,radio/television,2299,500 <= ... < 1000 DM,... >= 7 years,4,male : divorced/separated,none,4,"car or other, not in attribute Savings account/bonds",39,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,6,existing credits paid back duly till now,car (used),1352,500 <= ... < 1000 DM,unemployed,1,male : divorced/separated,none,2,building society savings agreement/ life insurance,23,none,rent,1,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,good
+no checking account,11,critical account/ other credits existing (not at this bank),car (new),7228,... < 100 DM,1 <= ... < 4 years,1,male : divorced/separated,none,4,building society savings agreement/ life insurance,39,none,own,2,unskilled - resident,1,none,yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,2073,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : divorced/separated,co-applicant,2,real estate,28,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,24,delay in paying off in the past,furniture/equipment,2333,unknown/ no savings account,... < 1 year,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,29,bank,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,27,delay in paying off in the past,car (used),5965,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,1262,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,car (used),3378,unknown/ no savings account,1 <= ... < 4 years,2,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,31,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,36,delay in paying off in the past,car (new),2225,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,57,bank,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,6,all credits at this bank paid back duly,car (new),783,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,guarantor,2,real estate,26,stores,own,1,unskilled - resident,2,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,6468,unknown/ no savings account,unemployed,2,female : divorced/separated/married,none,1,unknown / no property,52,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,36,critical account/ other credits existing (not at this bank),radio/television,9566,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,stores,own,2,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,18,existing credits paid back duly till now,car (new),1961,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",23,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+... < 0 DM,36,critical account/ other credits existing (not at this bank),furniture/equipment,6229,... < 100 DM,... < 1 year,4,female : divorced/separated/married,co-applicant,4,unknown / no property,23,none,rent,2,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,9,existing credits paid back duly till now,business,1391,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,1,real estate,27,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,15,critical account/ other credits existing (not at this bank),radio/television,1537,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,guarantor,4,real estate,50,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,36,no credits taken/ all credits paid back duly,business,1953,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,61,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,business,14421,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,24,existing credits paid back duly till now,radio/television,3181,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,27,existing credits paid back duly till now,repairs,5190,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,48,none,own,4,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,2171,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",29,bank,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),1007,... >= 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,real estate,22,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,36,existing credits paid back duly till now,education,1819,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,unknown / no property,37,stores,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,36,existing credits paid back duly till now,radio/television,2394,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",25,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,36,existing credits paid back duly till now,car (used),8133,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,30,bank,own,1,skilled employee / official,1,none,yes,good
+no checking account,7,critical account/ other credits existing (not at this bank),radio/television,730,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,46,none,rent,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
+... < 0 DM,8,critical account/ other credits existing (not at this bank),others,1164,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,51,bank,for free,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,42,critical account/ other credits existing (not at this bank),business,5954,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,1,real estate,41,bank,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,education,1977,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,40,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,12,critical account/ other credits existing (not at this bank),car (used),1526,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,66,none,for free,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+... < 0 DM,42,existing credits paid back duly till now,radio/television,3965,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,11,delay in paying off in the past,radio/television,4771,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,51,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,54,no credits taken/ all credits paid back duly,car (used),9436,unknown/ no savings account,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,39,none,own,1,unskilled - resident,2,none,yes,good
+0 <= ... < 200 DM,30,existing credits paid back duly till now,furniture/equipment,3832,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,22,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,5943,unknown/ no savings account,... < 1 year,1,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",44,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,15,existing credits paid back duly till now,radio/television,1213,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,47,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,18,existing credits paid back duly till now,business,1568,100 <= ... < 500 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,24,none,rent,1,unskilled - resident,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,others,1755,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,guarantor,4,real estate,58,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+... < 0 DM,10,existing credits paid back duly till now,radio/television,2315,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,real estate,52,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),business,1412,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,2,real estate,29,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,1295,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,education,12612,100 <= ... < 500 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,unknown / no property,47,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
+... < 0 DM,18,existing credits paid back duly till now,car (new),2249,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+... < 0 DM,12,no credits taken/ all credits paid back duly,repairs,1108,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,real estate,28,none,own,2,skilled employee / official,1,none,yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,618,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,56,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,12,critical account/ other credits existing (not at this bank),car (used),1409,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,3,real estate,54,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,797,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,33,bank,own,1,unskilled - resident,2,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,24,critical account/ other credits existing (not at this bank),furniture/equipment,3617,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,co-applicant,4,unknown / no property,20,none,rent,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),1318,... >= 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,54,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,54,no credits taken/ all credits paid back duly,business,15945,... < 100 DM,... < 1 year,3,female : divorced/separated/married,none,4,unknown / no property,58,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),education,2012,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",61,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,business,2622,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,36,critical account/ other credits existing (not at this bank),radio/television,2337,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,36,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,20,delay in paying off in the past,car (used),7057,unknown/ no savings account,4 <= ... < 7 years,3,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,36,bank,rent,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,car (new),1469,100 <= ... < 500 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,41,none,rent,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,radio/television,2323,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",24,none,rent,1,skilled employee / official,1,none,yes,good
+no checking account,6,delay in paying off in the past,radio/television,932,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,real estate,24,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,9,critical account/ other credits existing (not at this bank),furniture/equipment,1919,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",35,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,car (used),2445,unknown/ no savings account,... < 1 year,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",26,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),others,11938,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,co-applicant,3,"car or other, not in attribute Savings account/bonds",39,none,own,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,bad
+no checking account,18,all credits at this bank paid back duly,car (new),6458,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,39,bank,own,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),6078,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,7721,unknown/ no savings account,... < 1 year,1,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,30,none,own,1,skilled employee / official,1,"yes, registered under the customers name",no,good
+0 <= ... < 200 DM,14,existing credits paid back duly till now,business,1410,500 <= ... < 1000 DM,... >= 7 years,1,female : divorced/separated/married,none,2,real estate,35,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,6,delay in paying off in the past,business,1449,100 <= ... < 500 DM,... >= 7 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,bank,own,2,skilled employee / official,2,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,15,existing credits paid back duly till now,education,392,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,23,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,car (new),6260,... < 100 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,3,real estate,28,none,rent,1,unskilled - resident,1,none,yes,good
+no checking account,36,critical account/ other credits existing (not at this bank),car (new),7855,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,25,stores,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,12,existing credits paid back duly till now,radio/television,1680,500 <= ... < 1000 DM,... >= 7 years,3,female : divorced/separated/married,none,1,real estate,35,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,48,critical account/ other credits existing (not at this bank),radio/television,3578,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,1,real estate,47,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,42,existing credits paid back duly till now,radio/television,7174,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,10,critical account/ other credits existing (not at this bank),furniture/equipment,2132,unknown/ no savings account,... < 1 year,2,female : divorced/separated/married,co-applicant,3,real estate,27,none,rent,2,skilled employee / official,1,none,no,good
+... < 0 DM,33,critical account/ other credits existing (not at this bank),furniture/equipment,4281,500 <= ... < 1000 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",23,none,own,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (new),2366,500 <= ... < 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",36,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,21,existing credits paid back duly till now,radio/television,1835,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,real estate,25,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),car (used),3868,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",41,none,rent,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,furniture/equipment,1768,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,real estate,24,none,rent,1,unskilled - resident,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,10,critical account/ other credits existing (not at this bank),car (new),781,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,63,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,furniture/equipment,1924,unknown/ no savings account,... < 1 year,4,female : divorced/separated/married,none,3,real estate,27,none,rent,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),2121,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,30,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,radio/television,701,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,40,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,repairs,639,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (used),1860,... < 100 DM,unemployed,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),3499,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,co-applicant,2,real estate,29,none,own,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,48,existing credits paid back duly till now,car (new),8487,unknown/ no savings account,4 <= ... < 7 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,36,delay in paying off in the past,education,6887,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,29,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,15,existing credits paid back duly till now,furniture/equipment,2708,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,27,bank,own,2,unskilled - resident,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,furniture/equipment,1984,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,unknown / no property,47,bank,for free,2,skilled employee / official,1,none,yes,good
+no checking account,60,existing credits paid back duly till now,radio/television,10144,100 <= ... < 500 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,4,real estate,21,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,1240,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,real estate,38,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,27,delay in paying off in the past,car (used),8613,... >= 1000 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,766,500 <= ... < 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,real estate,66,none,own,1,unskilled - resident,1,none,yes,bad
+0 <= ... < 200 DM,15,critical account/ other credits existing (not at this bank),radio/television,2728,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,guarantor,2,real estate,35,bank,own,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,radio/television,1881,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",44,none,rent,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,6,existing credits paid back duly till now,car (new),709,... >= 1000 DM,... < 1 year,2,female : divorced/separated/married,none,2,real estate,27,none,own,1,unemployed/ unskilled - non-resident,1,none,no,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,radio/television,4795,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,1,unknown / no property,30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,27,existing credits paid back duly till now,radio/television,3416,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,2462,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",22,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,21,critical account/ other credits existing (not at this bank),furniture/equipment,2288,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,23,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,48,all credits at this bank paid back duly,business,3566,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),860,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,none,4,unknown / no property,39,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),car (new),682,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",51,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,36,critical account/ other credits existing (not at this bank),furniture/equipment,5371,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,guarantor,2,building society savings agreement/ life insurance,28,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1582,... >= 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",46,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,6,existing credits paid back duly till now,radio/television,1346,100 <= ... < 500 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,42,bank,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,10,existing credits paid back duly till now,radio/television,1924,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,38,none,own,1,skilled employee / official,1,"yes, registered under the customers name",no,good
+... >= 200 DM / salary assignments for at least 1 year,36,existing credits paid back duly till now,radio/television,5848,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),car (used),7758,... >= 1000 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,29,none,rent,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,24,delay in paying off in the past,business,6967,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",36,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1282,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",20,none,rent,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,9,critical account/ other credits existing (not at this bank),repairs,1288,100 <= ... < 500 DM,... >= 7 years,3,female : divorced/separated/married,guarantor,4,real estate,48,none,own,2,skilled employee / official,2,none,no,good
+... < 0 DM,12,all credits at this bank paid back duly,retraining,339,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",45,bank,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),3512,100 <= ... < 500 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",38,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1898,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,real estate,34,none,own,2,unskilled - resident,2,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2872,100 <= ... < 500 DM,... >= 7 years,3,female : divorced/separated/married,none,4,real estate,36,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),car (new),1055,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,30,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,15,existing credits paid back duly till now,domestic appliances,1262,500 <= ... < 1000 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,36,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,10,existing credits paid back duly till now,car (new),7308,... < 100 DM,unemployed,2,female : divorced/separated/married,none,4,unknown / no property,70,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,36,existing credits paid back duly till now,car (new),909,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,36,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,6,existing credits paid back duly till now,furniture/equipment,2978,500 <= ... < 1000 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,1131,... < 100 DM,unemployed,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,11,existing credits paid back duly till now,furniture/equipment,1577,... >= 1000 DM,... < 1 year,4,female : divorced/separated/married,none,1,real estate,20,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,furniture/equipment,3972,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,25,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),business,1935,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,31,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,15,no credits taken/ all credits paid back duly,car (new),950,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",33,none,rent,2,skilled employee / official,2,none,yes,bad
+no checking account,12,existing credits paid back duly till now,furniture/equipment,763,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,real estate,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,delay in paying off in the past,furniture/equipment,2064,... < 100 DM,unemployed,3,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,34,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,8,existing credits paid back duly till now,radio/television,1414,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,2,real estate,33,none,own,1,skilled employee / official,1,none,no,good
+... < 0 DM,21,delay in paying off in the past,education,3414,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,26,none,own,2,skilled employee / official,1,none,yes,bad
+no checking account,30,all credits at this bank paid back duly,car (used),7485,unknown/ no savings account,unemployed,4,female : divorced/separated/married,none,1,real estate,53,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,2577,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,6,critical account/ other credits existing (not at this bank),radio/television,338,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",52,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,1963,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,none,rent,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+... < 0 DM,21,critical account/ other credits existing (not at this bank),car (new),571,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,65,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,36,delay in paying off in the past,business,9572,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,36,delay in paying off in the past,business,4455,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,30,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,21,all credits at this bank paid back duly,car (new),1647,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,40,none,own,2,unskilled - resident,2,none,yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),furniture/equipment,3777,... >= 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,real estate,50,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),car (new),884,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",36,bank,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
+no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1360,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,31,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,9,all credits at this bank paid back duly,car (used),5129,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,74,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,16,critical account/ other credits existing (not at this bank),car (new),1175,... < 100 DM,unemployed,2,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",68,none,for free,3,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,radio/television,674,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,20,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,18,no credits taken/ all credits paid back duly,furniture/equipment,3244,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",33,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,business,4591,... >= 1000 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,54,none,own,3,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,business,3844,100 <= ... < 500 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,unknown / no property,34,none,for free,1,unskilled - resident,2,none,yes,bad
+0 <= ... < 200 DM,27,existing credits paid back duly till now,business,3915,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",36,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
+no checking account,6,existing credits paid back duly till now,radio/television,2108,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,2,real estate,29,none,rent,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,45,existing credits paid back duly till now,radio/television,3031,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,4,building society savings agreement/ life insurance,21,none,rent,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,9,critical account/ other credits existing (not at this bank),education,1501,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1382,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,951,100 <= ... < 500 DM,... < 1 year,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",27,bank,rent,4,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (used),2760,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,36,bank,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,delay in paying off in the past,furniture/equipment,4297,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,3,unknown / no property,40,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,9,critical account/ other credits existing (not at this bank),education,936,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",52,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,car (new),1168,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,real estate,27,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,27,delay in paying off in the past,business,5117,... < 100 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",26,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,retraining,902,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,21,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),car (new),1495,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,1,real estate,38,none,own,2,unskilled - resident,2,none,yes,good
+... < 0 DM,30,critical account/ other credits existing (not at this bank),car (used),10623,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,38,none,for free,3,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,1935,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,43,none,own,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),domestic appliances,1424,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,business,6568,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",21,stores,own,1,unskilled - resident,1,none,yes,good
+no checking account,12,existing credits paid back duly till now,car (used),1413,... >= 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,55,none,own,1,skilled employee / official,1,none,no,good
+no checking account,9,critical account/ other credits existing (not at this bank),radio/television,3074,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,real estate,33,none,own,2,skilled employee / official,2,none,yes,good
+no checking account,36,existing credits paid back duly till now,radio/television,3835,unknown/ no savings account,... >= 7 years,2,female : divorced/separated/married,none,4,real estate,45,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+... < 0 DM,27,no credits taken/ all credits paid back duly,business,5293,... < 100 DM,unemployed,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,50,stores,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... >= 200 DM / salary assignments for at least 1 year,30,delay in paying off in the past,business,1908,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,66,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,36,critical account/ other credits existing (not at this bank),radio/television,3342,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",51,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,6,critical account/ other credits existing (not at this bank),retraining,932,unknown/ no savings account,4 <= ... < 7 years,1,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,39,none,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,18,no credits taken/ all credits paid back duly,business,3104,... < 100 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,1,building society savings agreement/ life insurance,31,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,36,existing credits paid back duly till now,radio/television,3913,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,23,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,3021,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,24,none,rent,1,unskilled - resident,1,none,yes,good
+no checking account,10,existing credits paid back duly till now,car (new),1364,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",64,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,625,... < 100 DM,... < 1 year,4,female : divorced/separated/married,guarantor,1,real estate,26,bank,own,1,unskilled - resident,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,education,1200,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,23,bank,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,707,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,30,bank,own,2,skilled employee / official,1,none,yes,good
+no checking account,24,delay in paying off in the past,business,2978,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,real estate,32,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,15,existing credits paid back duly till now,car (used),4657,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,36,no credits taken/ all credits paid back duly,repairs,2613,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,48,existing credits paid back duly till now,radio/television,10961,... >= 1000 DM,4 <= ... < 7 years,1,female : divorced/separated/married,co-applicant,2,unknown / no property,27,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,7865,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,53,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,9,existing credits paid back duly till now,radio/television,1478,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",22,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,3149,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,1,unknown / no property,22,bank,for free,1,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,36,existing credits paid back duly till now,radio/television,4210,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,9,existing credits paid back duly till now,car (new),2507,500 <= ... < 1000 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,51,none,for free,1,unskilled - resident,1,none,yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,2141,100 <= ... < 500 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,1,unknown / no property,35,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,radio/television,866,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,2,real estate,25,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,4,critical account/ other credits existing (not at this bank),radio/television,1544,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,1,real estate,42,none,own,3,unskilled - resident,2,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,radio/television,1823,... < 100 DM,unemployed,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",30,stores,own,1,management/ self-employed/ highly qualified employee/ officer,2,none,yes,bad
+0 <= ... < 200 DM,6,existing credits paid back duly till now,car (new),14555,unknown/ no savings account,unemployed,1,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,23,none,own,1,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,21,existing credits paid back duly till now,business,2767,100 <= ... < 500 DM,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",61,bank,rent,2,unskilled - resident,1,none,yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,1291,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,35,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,30,existing credits paid back duly till now,radio/television,2522,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,guarantor,3,building society savings agreement/ life insurance,39,none,own,1,skilled employee / official,2,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,car (new),915,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",29,bank,own,1,skilled employee / official,1,none,yes,bad
+no checking account,6,existing credits paid back duly till now,radio/television,1595,... < 100 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,51,none,own,1,skilled employee / official,2,none,yes,good
+... < 0 DM,48,no credits taken/ all credits paid back duly,car (used),4605,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,24,none,for free,2,skilled employee / official,2,none,yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),business,1185,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,2,real estate,27,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,12,all credits at this bank paid back duly,retraining,3447,500 <= ... < 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,real estate,35,none,own,1,unskilled - resident,2,none,yes,good
+no checking account,24,existing credits paid back duly till now,business,1258,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,1,real estate,25,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,717,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,52,none,own,3,skilled employee / official,1,none,yes,good
+no checking account,6,no credits taken/ all credits paid back duly,car (new),1204,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,unknown / no property,35,bank,rent,1,skilled employee / official,1,none,no,good
+... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,furniture/equipment,1925,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,26,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,radio/television,433,... < 100 DM,unemployed,3,female : divorced/separated/married,co-applicant,4,real estate,22,none,rent,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),666,... >= 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,4,real estate,39,none,own,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,furniture/equipment,2251,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",46,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,30,existing credits paid back duly till now,car (new),2150,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,2,unknown / no property,24,bank,own,1,skilled employee / official,1,none,yes,bad
+no checking account,24,delay in paying off in the past,furniture/equipment,4151,100 <= ... < 500 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,35,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,furniture/equipment,2030,unknown/ no savings account,4 <= ... < 7 years,2,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,60,delay in paying off in the past,radio/television,7418,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,none,1,real estate,27,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2684,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,35,none,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,12,all credits at this bank paid back duly,radio/television,2149,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,unknown / no property,29,none,for free,1,skilled employee / official,1,none,yes,bad
+no checking account,15,existing credits paid back duly till now,car (used),3812,100 <= ... < 500 DM,... < 1 year,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",23,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,11,critical account/ other credits existing (not at this bank),radio/television,1154,100 <= ... < 500 DM,unemployed,4,female : divorced/separated/married,none,4,real estate,57,none,own,3,unskilled - resident,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1657,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,27,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,radio/television,1603,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",55,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,18,critical account/ other credits existing (not at this bank),car (new),5302,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,36,none,for free,3,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),education,2748,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,57,bank,for free,3,unskilled - resident,1,none,yes,good
+no checking account,10,critical account/ other credits existing (not at this bank),car (new),1231,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,real estate,32,none,own,2,unskilled - resident,2,none,no,good
+0 <= ... < 200 DM,15,existing credits paid back duly till now,radio/television,802,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",37,none,own,1,skilled employee / official,2,none,yes,bad
+no checking account,36,critical account/ other credits existing (not at this bank),business,6304,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,real estate,36,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,1533,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",38,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,14,existing credits paid back duly till now,car (new),8978,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,45,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",no,bad
+no checking account,24,existing credits paid back duly till now,radio/television,999,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,car (new),2662,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,32,none,own,1,skilled employee / official,1,none,no,good
+no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,1402,500 <= ... < 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",37,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,48,all credits at this bank paid back duly,car (new),12169,unknown/ no savings account,unemployed,4,female : divorced/separated/married,co-applicant,4,unknown / no property,36,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,48,existing credits paid back duly till now,radio/television,3060,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,real estate,28,none,own,2,skilled employee / official,1,none,yes,bad
+... < 0 DM,30,existing credits paid back duly till now,repairs,11998,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,1,unknown / no property,34,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+no checking account,9,existing credits paid back duly till now,radio/television,2697,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,real estate,32,none,own,1,skilled employee / official,2,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,2404,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1262,unknown/ no savings account,... >= 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,49,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+no checking account,6,existing credits paid back duly till now,furniture/equipment,4611,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,32,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,24,existing credits paid back duly till now,radio/television,1901,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",29,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),car (used),3368,... >= 1000 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,23,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,furniture/equipment,1574,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,50,none,own,1,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,18,all credits at this bank paid back duly,radio/television,1445,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",49,bank,own,1,unskilled - resident,1,none,yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),furniture/equipment,1520,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,63,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),car (new),3878,100 <= ... < 500 DM,... < 1 year,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",37,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,47,existing credits paid back duly till now,car (new),10722,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,1,real estate,35,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+... < 0 DM,48,existing credits paid back duly till now,car (used),4788,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,2,none,yes,good
+0 <= ... < 200 DM,48,delay in paying off in the past,others,7582,100 <= ... < 500 DM,unemployed,2,female : divorced/separated/married,none,4,unknown / no property,31,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1092,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,guarantor,4,real estate,49,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,delay in paying off in the past,radio/television,1024,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,4,real estate,48,stores,own,1,skilled employee / official,1,none,yes,bad
+no checking account,12,existing credits paid back duly till now,business,1076,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,real estate,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",no,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,car (used),9398,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,24,critical account/ other credits existing (not at this bank),car (used),6419,... < 100 DM,... >= 7 years,2,female : divorced/separated/married,none,4,unknown / no property,44,none,for free,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,42,critical account/ other credits existing (not at this bank),car (used),4796,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,56,none,for free,1,skilled employee / official,1,none,yes,good
+no checking account,48,critical account/ other credits existing (not at this bank),business,7629,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",46,bank,own,2,management/ self-employed/ highly qualified employee/ officer,2,none,yes,good
+0 <= ... < 200 DM,48,existing credits paid back duly till now,furniture/equipment,9960,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,12,existing credits paid back duly till now,car (used),4675,unknown/ no savings account,... < 1 year,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",20,none,rent,1,skilled employee / official,1,none,yes,good
+no checking account,10,existing credits paid back duly till now,car (new),1287,unknown/ no savings account,... >= 7 years,4,female : divorced/separated/married,co-applicant,2,building society savings agreement/ life insurance,45,none,own,1,unskilled - resident,1,none,no,good
+no checking account,18,existing credits paid back duly till now,furniture/equipment,2515,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,4,real estate,43,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,21,critical account/ other credits existing (not at this bank),furniture/equipment,2745,... >= 1000 DM,4 <= ... < 7 years,3,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,6,existing credits paid back duly till now,car (new),672,... < 100 DM,unemployed,1,female : divorced/separated/married,none,4,real estate,54,none,own,1,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,36,no credits taken/ all credits paid back duly,radio/television,3804,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... >= 200 DM / salary assignments for at least 1 year,24,critical account/ other credits existing (not at this bank),car (new),1344,unknown/ no savings account,4 <= ... < 7 years,4,female : divorced/separated/married,none,2,real estate,37,bank,own,2,unskilled - resident,2,none,yes,bad
+... < 0 DM,10,critical account/ other credits existing (not at this bank),car (new),1038,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,co-applicant,3,building society savings agreement/ life insurance,49,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,48,critical account/ other credits existing (not at this bank),car (new),10127,500 <= ... < 1000 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,2,unknown / no property,44,bank,for free,1,skilled employee / official,1,none,yes,bad
+no checking account,6,existing credits paid back duly till now,furniture/equipment,1543,... >= 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,33,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,30,existing credits paid back duly till now,car (used),4811,unknown/ no savings account,4 <= ... < 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,24,stores,rent,1,unskilled - resident,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,radio/television,727,100 <= ... < 500 DM,... < 1 year,4,female : divorced/separated/married,none,3,unknown / no property,33,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,8,existing credits paid back duly till now,furniture/equipment,1237,... < 100 DM,1 <= ... < 4 years,3,female : divorced/separated/married,none,4,real estate,24,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,9,existing credits paid back duly till now,car (new),276,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,real estate,22,none,rent,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,48,existing credits paid back duly till now,others,5381,unknown/ no savings account,unemployed,3,female : divorced/separated/married,none,4,unknown / no property,40,bank,for free,1,unemployed/ unskilled - non-resident,1,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,furniture/equipment,5511,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,1,"car or other, not in attribute Savings account/bonds",25,stores,own,1,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,furniture/equipment,3749,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),685,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",25,bank,own,1,unskilled - resident,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,4,existing credits paid back duly till now,car (new),1494,unknown/ no savings account,... < 1 year,1,female : divorced/separated/married,none,2,real estate,29,none,own,1,unskilled - resident,2,none,no,good
+... < 0 DM,36,all credits at this bank paid back duly,furniture/equipment,2746,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",31,bank,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,708,... < 100 DM,1 <= ... < 4 years,2,female : divorced/separated/married,guarantor,3,building society savings agreement/ life insurance,38,none,own,1,unskilled - resident,2,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,furniture/equipment,4351,unknown/ no savings account,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,48,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),education,701,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,15,delay in paying off in the past,furniture/equipment,3643,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,27,none,own,2,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,30,critical account/ other credits existing (not at this bank),car (new),4249,... < 100 DM,unemployed,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,radio/television,1938,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,3,building society savings agreement/ life insurance,32,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,car (used),2910,... < 100 DM,4 <= ... < 7 years,2,female : divorced/separated/married,none,1,unknown / no property,34,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,2659,... >= 1000 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),car (new),1028,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,3,real estate,36,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,8,critical account/ other credits existing (not at this bank),car (new),3398,... < 100 DM,4 <= ... < 7 years,1,female : divorced/separated/married,none,4,real estate,39,none,own,2,unskilled - resident,1,none,no,good
+no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,5801,unknown/ no savings account,... >= 7 years,2,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,49,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,car (new),1525,... >= 1000 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,3,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,36,existing credits paid back duly till now,radio/television,4473,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,1068,... < 100 DM,... >= 7 years,4,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,2,none,yes,good
+... < 0 DM,24,critical account/ other credits existing (not at this bank),car (used),6615,... < 100 DM,unemployed,2,female : divorced/separated/married,none,4,unknown / no property,75,none,for free,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),education,1864,100 <= ... < 500 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,30,none,own,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,60,existing credits paid back duly till now,car (new),7408,100 <= ... < 500 DM,... < 1 year,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,24,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
+no checking account,48,critical account/ other credits existing (not at this bank),car (used),11590,100 <= ... < 500 DM,1 <= ... < 4 years,2,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",24,bank,rent,2,unskilled - resident,1,none,yes,bad
+... < 0 DM,24,no credits taken/ all credits paid back duly,furniture/equipment,4110,... < 100 DM,... >= 7 years,3,female : divorced/separated/married,none,4,unknown / no property,23,bank,rent,2,skilled employee / official,2,none,yes,bad
+... < 0 DM,6,critical account/ other credits existing (not at this bank),furniture/equipment,3384,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,4,real estate,44,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,13,existing credits paid back duly till now,radio/television,2101,... < 100 DM,... < 1 year,2,female : divorced/separated/married,guarantor,4,building society savings agreement/ life insurance,23,none,own,1,unskilled - resident,1,none,yes,good
+... < 0 DM,15,existing credits paid back duly till now,domestic appliances,1275,unknown/ no savings account,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",24,none,rent,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,4169,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,4,building society savings agreement/ life insurance,28,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,10,existing credits paid back duly till now,furniture/equipment,1521,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),education,5743,... < 100 DM,... < 1 year,2,female : divorced/separated/married,none,4,unknown / no property,24,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,21,existing credits paid back duly till now,furniture/equipment,3599,... < 100 DM,4 <= ... < 7 years,1,female : divorced/separated/married,none,4,"car or other, not in attribute Savings account/bonds",26,none,rent,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,radio/television,3213,500 <= ... < 1000 DM,... < 1 year,1,female : divorced/separated/married,none,3,real estate,25,none,rent,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,business,4439,... < 100 DM,... >= 7 years,1,female : divorced/separated/married,co-applicant,1,real estate,33,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,10,existing credits paid back duly till now,car (new),3949,... < 100 DM,... < 1 year,1,female : divorced/separated/married,guarantor,1,building society savings agreement/ life insurance,37,none,own,1,unskilled - resident,2,none,yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1459,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",43,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,13,critical account/ other credits existing (not at this bank),radio/television,882,... < 100 DM,... < 1 year,4,female : divorced/separated/married,guarantor,4,real estate,23,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,3758,500 <= ... < 1000 DM,unemployed,1,female : divorced/separated/married,none,4,unknown / no property,23,none,rent,1,unemployed/ unskilled - non-resident,1,none,yes,good
+no checking account,6,delay in paying off in the past,business,1743,100 <= ... < 500 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,real estate,34,none,own,2,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,9,critical account/ other credits existing (not at this bank),education,1136,... >= 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,3,unknown / no property,32,none,for free,2,skilled employee / official,2,none,yes,bad
+no checking account,9,existing credits paid back duly till now,domestic appliances,1236,... < 100 DM,... < 1 year,1,female : divorced/separated/married,none,4,real estate,23,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,furniture/equipment,959,... < 100 DM,1 <= ... < 4 years,1,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",29,none,own,1,skilled employee / official,1,none,no,bad
+no checking account,18,critical account/ other credits existing (not at this bank),car (used),3229,unknown/ no savings account,unemployed,2,female : divorced/separated/married,none,4,unknown / no property,38,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,no credits taken/ all credits paid back duly,radio/television,6199,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,building society savings agreement/ life insurance,28,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,10,existing credits paid back duly till now,education,727,500 <= ... < 1000 DM,... >= 7 years,4,female : divorced/separated/married,none,4,unknown / no property,46,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),1246,... < 100 DM,... < 1 year,4,female : divorced/separated/married,none,2,real estate,23,stores,own,1,unskilled - resident,1,none,yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,2331,unknown/ no savings account,... >= 7 years,1,female : divorced/separated/married,co-applicant,4,real estate,49,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,36,delay in paying off in the past,radio/television,4463,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,12,existing credits paid back duly till now,radio/television,776,... < 100 DM,1 <= ... < 4 years,4,female : divorced/separated/married,none,2,real estate,28,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,30,existing credits paid back duly till now,furniture/equipment,2406,... < 100 DM,4 <= ... < 7 years,4,female : divorced/separated/married,none,4,real estate,23,none,rent,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,18,existing credits paid back duly till now,education,1239,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,61,none,for free,1,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,radio/television,3399,unknown/ no savings account,... >= 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",37,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,delay in paying off in the past,car (new),2247,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",36,stores,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,6,existing credits paid back duly till now,furniture/equipment,1766,... < 100 DM,1 <= ... < 4 years,1,male : single,none,2,building society savings agreement/ life insurance,21,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,2473,... < 100 DM,unemployed,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",25,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,bad
+no checking account,12,existing credits paid back duly till now,business,1542,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",36,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),car (used),3850,... < 100 DM,4 <= ... < 7 years,3,male : single,none,1,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,3650,... < 100 DM,... < 1 year,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",22,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,3446,... < 100 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,2,none,yes,bad
+0 <= ... < 200 DM,18,existing credits paid back duly till now,furniture/equipment,3001,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,real estate,40,none,rent,1,skilled employee / official,1,none,yes,good
+no checking account,36,existing credits paid back duly till now,car (new),3079,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,real estate,36,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,6070,... < 100 DM,... >= 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",33,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,10,critical account/ other credits existing (not at this bank),furniture/equipment,2146,... < 100 DM,... < 1 year,1,male : single,none,3,real estate,23,none,rent,2,skilled employee / official,1,none,yes,good
+no checking account,60,critical account/ other credits existing (not at this bank),car (new),13756,unknown/ no savings account,... >= 7 years,2,male : single,none,4,unknown / no property,63,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,60,all credits at this bank paid back duly,others,14782,100 <= ... < 500 DM,... >= 7 years,3,male : single,none,4,unknown / no property,60,bank,for free,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,48,all credits at this bank paid back duly,business,7685,... < 100 DM,4 <= ... < 7 years,2,male : single,guarantor,4,"car or other, not in attribute Savings account/bonds",37,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,18,delay in paying off in the past,radio/television,2320,... < 100 DM,unemployed,2,male : single,none,3,real estate,34,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,7,delay in paying off in the past,radio/television,846,unknown/ no savings account,... >= 7 years,3,male : single,none,4,unknown / no property,36,none,for free,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,car (new),14318,... < 100 DM,... >= 7 years,4,male : single,none,2,unknown / no property,57,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,6,critical account/ other credits existing (not at this bank),car (new),362,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",52,none,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,20,existing credits paid back duly till now,furniture/equipment,2212,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",39,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,car (used),12976,... < 100 DM,unemployed,3,male : single,none,4,unknown / no property,38,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,22,existing credits paid back duly till now,car (new),1283,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,building society savings agreement/ life insurance,25,none,rent,1,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,car (new),1330,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,26,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,30,delay in paying off in the past,business,4272,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,26,none,own,2,unskilled - resident,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,2238,... < 100 DM,1 <= ... < 4 years,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",25,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,radio/television,1126,unknown/ no savings account,... < 1 year,4,male : single,none,2,real estate,21,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,7374,... < 100 DM,unemployed,4,male : single,none,4,building society savings agreement/ life insurance,40,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,15,critical account/ other credits existing (not at this bank),business,2326,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,bank,own,1,skilled employee / official,1,none,yes,good
+no checking account,9,existing credits paid back duly till now,business,1449,... < 100 DM,4 <= ... < 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,car (new),1820,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,983,... >= 1000 DM,... < 1 year,1,male : single,none,4,real estate,19,none,rent,1,unskilled - resident,1,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,car (new),3249,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,unknown / no property,39,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+... < 0 DM,6,critical account/ other credits existing (not at this bank),radio/television,1957,... < 100 DM,4 <= ... < 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,9,critical account/ other credits existing (not at this bank),furniture/equipment,2406,... < 100 DM,unemployed,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",31,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+0 <= ... < 200 DM,39,delay in paying off in the past,education,11760,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,3,unknown / no property,32,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,2578,... < 100 DM,unemployed,3,male : single,none,4,unknown / no property,55,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+... < 0 DM,36,critical account/ other credits existing (not at this bank),furniture/equipment,2348,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,building society savings agreement/ life insurance,46,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),1223,... < 100 DM,... >= 7 years,1,male : single,none,1,real estate,46,none,rent,2,skilled employee / official,1,none,yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,1516,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,1,real estate,43,none,own,2,unskilled - resident,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,radio/television,1473,... < 100 DM,... < 1 year,3,male : single,none,4,real estate,39,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),business,1887,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,real estate,28,bank,own,2,skilled employee / official,1,none,yes,good
+no checking account,24,delay in paying off in the past,business,8648,... < 100 DM,... < 1 year,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",27,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,14,delay in paying off in the past,car (new),802,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,2,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,18,delay in paying off in the past,car (new),2899,unknown/ no savings account,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",43,none,own,1,skilled employee / official,2,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,2039,... < 100 DM,... < 1 year,1,male : single,none,1,building society savings agreement/ life insurance,22,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),car (used),2197,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",43,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,15,existing credits paid back duly till now,radio/television,1053,... < 100 DM,... < 1 year,4,male : single,none,2,real estate,27,none,own,1,skilled employee / official,1,none,no,good
+no checking account,24,existing credits paid back duly till now,radio/television,3235,500 <= ... < 1000 DM,... >= 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,critical account/ other credits existing (not at this bank),car (new),939,500 <= ... < 1000 DM,4 <= ... < 7 years,4,male : single,none,2,real estate,28,none,own,3,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,1967,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",20,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,33,critical account/ other credits existing (not at this bank),car (used),7253,... < 100 DM,4 <= ... < 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",35,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),business,2292,... < 100 DM,unemployed,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",42,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,10,existing credits paid back duly till now,car (new),1597,500 <= ... < 1000 DM,1 <= ... < 4 years,3,male : single,none,2,unknown / no property,40,none,rent,1,unskilled - resident,2,none,no,good
+... < 0 DM,24,existing credits paid back duly till now,car (new),1381,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,35,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,36,critical account/ other credits existing (not at this bank),car (used),5842,... < 100 DM,... >= 7 years,2,male : single,none,2,building society savings agreement/ life insurance,35,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,car (new),2579,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,33,none,own,1,unskilled - resident,2,none,yes,bad
+... < 0 DM,18,delay in paying off in the past,education,8471,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",23,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,21,existing credits paid back duly till now,car (new),2782,500 <= ... < 1000 DM,4 <= ... < 7 years,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,car (new),1042,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,33,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,15,existing credits paid back duly till now,car (new),3186,... >= 1000 DM,4 <= ... < 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",20,none,rent,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (used),2028,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (new),958,... < 100 DM,4 <= ... < 7 years,2,male : single,none,3,real estate,47,none,own,2,unskilled - resident,2,none,yes,good
+no checking account,21,delay in paying off in the past,furniture/equipment,1591,100 <= ... < 500 DM,4 <= ... < 7 years,4,male : single,none,3,real estate,34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,2762,unknown/ no savings account,... >= 7 years,1,male : single,none,2,building society savings agreement/ life insurance,25,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,18,existing credits paid back duly till now,car (used),2779,... < 100 DM,1 <= ... < 4 years,1,male : single,none,3,"car or other, not in attribute Savings account/bonds",21,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,28,critical account/ other credits existing (not at this bank),radio/television,2743,... < 100 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",29,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1149,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,46,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,9,existing credits paid back duly till now,furniture/equipment,1313,... < 100 DM,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",20,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,18,critical account/ other credits existing (not at this bank),repairs,1190,... < 100 DM,unemployed,2,male : single,none,4,unknown / no property,55,none,for free,3,unemployed/ unskilled - non-resident,2,none,yes,bad
+no checking account,5,existing credits paid back duly till now,business,3448,... < 100 DM,4 <= ... < 7 years,1,male : single,none,4,real estate,74,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,others,11328,... < 100 DM,1 <= ... < 4 years,2,male : single,co-applicant,3,"car or other, not in attribute Savings account/bonds",29,bank,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,6,critical account/ other credits existing (not at this bank),furniture/equipment,1872,... < 100 DM,unemployed,4,male : single,none,4,unknown / no property,36,none,for free,3,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),repairs,2058,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,33,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,9,existing credits paid back duly till now,furniture/equipment,2136,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,25,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1484,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,1,real estate,25,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,6,existing credits paid back duly till now,repairs,660,500 <= ... < 1000 DM,4 <= ... < 7 years,2,male : single,none,4,real estate,23,none,rent,1,unskilled - resident,1,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),car (new),1287,... >= 1000 DM,... >= 7 years,4,male : single,none,4,real estate,37,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,42,critical account/ other credits existing (not at this bank),repairs,3394,... < 100 DM,unemployed,4,male : single,co-applicant,4,"car or other, not in attribute Savings account/bonds",65,none,own,2,unemployed/ unskilled - non-resident,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,all credits at this bank paid back duly,business,609,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,26,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,bad
+no checking account,12,existing credits paid back duly till now,car (new),1884,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",39,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1620,... < 100 DM,1 <= ... < 4 years,2,male : single,co-applicant,3,building society savings agreement/ life insurance,30,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,20,delay in paying off in the past,others,2629,... < 100 DM,1 <= ... < 4 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",29,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,education,719,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",41,bank,own,1,unskilled - resident,2,none,yes,bad
+0 <= ... < 200 DM,48,critical account/ other credits existing (not at this bank),furniture/equipment,5096,... < 100 DM,1 <= ... < 4 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,9,critical account/ other credits existing (not at this bank),education,1244,unknown/ no savings account,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,41,none,rent,2,unskilled - resident,1,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,car (new),1842,... < 100 DM,... < 1 year,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,7,existing credits paid back duly till now,radio/television,2576,... < 100 DM,1 <= ... < 4 years,2,male : single,guarantor,2,real estate,35,none,own,1,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,furniture/equipment,1424,unknown/ no savings account,... >= 7 years,3,male : single,none,4,real estate,55,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,15,delay in paying off in the past,repairs,1512,... >= 1000 DM,1 <= ... < 4 years,3,male : single,none,3,building society savings agreement/ life insurance,61,stores,own,2,skilled employee / official,1,none,yes,bad
+no checking account,36,critical account/ other credits existing (not at this bank),car (used),11054,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,6,existing credits paid back duly till now,radio/television,518,... < 100 DM,1 <= ... < 4 years,3,male : single,none,1,real estate,29,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,12,no credits taken/ all credits paid back duly,furniture/equipment,2759,... < 100 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,34,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,car (used),2670,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",35,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,existing credits paid back duly till now,car (new),4817,... < 100 DM,4 <= ... < 7 years,2,male : single,co-applicant,3,building society savings agreement/ life insurance,31,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,24,existing credits paid back duly till now,car (used),2679,... < 100 DM,... < 1 year,4,male : single,none,1,unknown / no property,29,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,11,critical account/ other credits existing (not at this bank),car (new),3905,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,36,none,rent,2,skilled employee / official,2,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,car (used),3386,... < 100 DM,... >= 7 years,3,male : single,none,4,unknown / no property,35,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,6,existing credits paid back duly till now,domestic appliances,343,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,27,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,radio/television,4594,... < 100 DM,... < 1 year,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",32,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,3620,... < 100 DM,1 <= ... < 4 years,1,male : single,guarantor,2,building society savings agreement/ life insurance,37,none,own,1,skilled employee / official,2,none,yes,good
+... < 0 DM,15,existing credits paid back duly till now,car (new),1721,... < 100 DM,... < 1 year,2,male : single,none,3,real estate,36,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,3017,... < 100 DM,... < 1 year,3,male : single,none,1,real estate,34,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,retraining,754,unknown/ no savings account,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,38,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,business,1950,... < 100 DM,4 <= ... < 7 years,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",34,stores,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,existing credits paid back duly till now,car (used),2924,... < 100 DM,1 <= ... < 4 years,3,male : single,guarantor,4,unknown / no property,63,bank,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,24,delay in paying off in the past,radio/television,1659,... < 100 DM,... < 1 year,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",29,none,rent,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+no checking account,48,delay in paying off in the past,radio/television,7238,unknown/ no savings account,... >= 7 years,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",32,bank,own,2,skilled employee / official,2,none,yes,good
+no checking account,33,delay in paying off in the past,business,2764,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,delay in paying off in the past,car (used),4679,... < 100 DM,4 <= ... < 7 years,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",35,none,own,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,3092,100 <= ... < 500 DM,... < 1 year,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",22,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,6,existing credits paid back duly till now,education,448,... < 100 DM,... < 1 year,4,male : single,none,4,building society savings agreement/ life insurance,23,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,9,existing credits paid back duly till now,car (new),654,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",28,none,own,1,unskilled - resident,1,none,yes,bad
+no checking account,6,existing credits paid back duly till now,retraining,1238,unknown/ no savings account,unemployed,4,male : single,none,4,building society savings agreement/ life insurance,36,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),radio/television,1245,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,18,no credits taken/ all credits paid back duly,furniture/equipment,3114,... < 100 DM,... < 1 year,1,male : single,none,4,building society savings agreement/ life insurance,26,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,39,existing credits paid back duly till now,car (used),2569,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,radio/television,5152,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",25,bank,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,business,1037,100 <= ... < 500 DM,4 <= ... < 7 years,3,male : single,none,4,real estate,39,none,own,1,unskilled - resident,1,none,yes,good
+... < 0 DM,15,critical account/ other credits existing (not at this bank),furniture/equipment,1478,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",44,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),radio/television,3573,... < 100 DM,1 <= ... < 4 years,1,male : single,none,1,real estate,23,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),1201,... < 100 DM,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,30,existing credits paid back duly till now,furniture/equipment,3622,... >= 1000 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,57,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,15,delay in paying off in the past,furniture/equipment,960,... >= 1000 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,30,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),car (new),1163,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,44,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,6,delay in paying off in the past,car (new),1209,... < 100 DM,unemployed,4,male : single,none,4,building society savings agreement/ life insurance,47,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,12,existing credits paid back duly till now,radio/television,3077,... < 100 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",52,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,car (new),3757,... < 100 DM,... >= 7 years,4,male : single,co-applicant,4,unknown / no property,62,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,10,existing credits paid back duly till now,car (new),1418,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,35,none,rent,1,unskilled - resident,1,none,no,good
+no checking account,6,existing credits paid back duly till now,car (new),3518,... < 100 DM,1 <= ... < 4 years,2,male : single,guarantor,3,building society savings agreement/ life insurance,26,none,rent,1,skilled employee / official,1,none,yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,1934,... < 100 DM,... >= 7 years,2,male : single,none,2,unknown / no property,26,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,27,no credits taken/ all credits paid back duly,business,8318,... < 100 DM,... >= 7 years,2,male : single,none,4,unknown / no property,42,none,for free,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1237,100 <= ... < 500 DM,1 <= ... < 4 years,1,male : single,none,1,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,368,unknown/ no savings account,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,38,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),2122,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,39,none,rent,2,unskilled - resident,2,none,no,good
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,2996,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",20,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,36,existing credits paid back duly till now,furniture/equipment,9034,100 <= ... < 500 DM,... < 1 year,4,male : single,co-applicant,1,unknown / no property,29,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),furniture/equipment,1585,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,40,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,radio/television,1301,... < 100 DM,... >= 7 years,4,male : single,guarantor,2,real estate,32,none,own,1,unskilled - resident,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,6,critical account/ other credits existing (not at this bank),car (new),1323,100 <= ... < 500 DM,... >= 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,24,existing credits paid back duly till now,car (new),3123,... < 100 DM,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,27,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,36,existing credits paid back duly till now,car (used),5493,... < 100 DM,... >= 7 years,2,male : single,none,4,unknown / no property,42,none,for free,1,skilled employee / official,2,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,9,existing credits paid back duly till now,radio/television,1126,100 <= ... < 500 DM,... >= 7 years,2,male : single,none,4,real estate,49,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),radio/television,1216,100 <= ... < 500 DM,... < 1 year,4,male : single,none,4,unknown / no property,38,bank,own,2,skilled employee / official,2,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,car (new),1207,... < 100 DM,... < 1 year,4,male : single,none,4,building society savings agreement/ life insurance,24,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,10,existing credits paid back duly till now,car (new),1309,unknown/ no savings account,1 <= ... < 4 years,4,male : single,guarantor,4,building society savings agreement/ life insurance,27,none,own,1,unskilled - resident,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,15,critical account/ other credits existing (not at this bank),car (used),2360,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",36,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,15,all credits at this bank paid back duly,car (new),6850,100 <= ... < 500 DM,unemployed,1,male : single,none,2,building society savings agreement/ life insurance,34,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,bad
+no checking account,24,existing credits paid back duly till now,radio/television,1413,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,28,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,39,existing credits paid back duly till now,car (used),8588,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",45,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,car (new),759,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,real estate,26,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,36,existing credits paid back duly till now,car (used),4686,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,unknown / no property,32,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,15,existing credits paid back duly till now,business,2687,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,building society savings agreement/ life insurance,26,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,delay in paying off in the past,radio/television,585,... < 100 DM,1 <= ... < 4 years,4,male : single,co-applicant,4,real estate,20,none,rent,2,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,car (new),2255,unknown/ no savings account,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,54,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),609,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,37,none,own,2,skilled employee / official,1,none,no,good
+... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),1361,... < 100 DM,... < 1 year,2,male : single,none,4,real estate,40,none,own,1,unskilled - resident,2,none,no,good
+no checking account,36,critical account/ other credits existing (not at this bank),furniture/equipment,7127,... < 100 DM,... < 1 year,2,male : single,none,4,building society savings agreement/ life insurance,23,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,6,existing credits paid back duly till now,car (new),1203,100 <= ... < 500 DM,... >= 7 years,3,male : single,none,2,building society savings agreement/ life insurance,43,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,6,critical account/ other credits existing (not at this bank),radio/television,700,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,36,none,for free,2,skilled employee / official,1,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),repairs,5507,... < 100 DM,... >= 7 years,3,male : single,none,4,unknown / no property,44,none,for free,2,skilled employee / official,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,radio/television,3190,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,24,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,48,no credits taken/ all credits paid back duly,furniture/equipment,7119,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,unknown / no property,53,none,for free,2,skilled employee / official,2,none,yes,bad
+no checking account,24,existing credits paid back duly till now,car (used),3488,100 <= ... < 500 DM,4 <= ... < 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",23,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,radio/television,1113,... < 100 DM,1 <= ... < 4 years,4,male : single,guarantor,4,real estate,26,none,own,1,unskilled - resident,2,none,yes,good
+0 <= ... < 200 DM,26,existing credits paid back duly till now,car (used),7966,... < 100 DM,... < 1 year,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),education,1532,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,4,critical account/ other credits existing (not at this bank),radio/television,1503,... < 100 DM,4 <= ... < 7 years,2,male : single,none,1,real estate,42,none,own,2,unskilled - resident,2,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,radio/television,2302,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",31,none,rent,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,6,existing credits paid back duly till now,car (new),662,... < 100 DM,... < 1 year,3,male : single,none,4,real estate,41,none,own,1,unskilled - resident,2,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,education,2273,... < 100 DM,4 <= ... < 7 years,3,male : single,none,1,"car or other, not in attribute Savings account/bonds",32,none,own,2,skilled employee / official,2,none,yes,good
+0 <= ... < 200 DM,15,existing credits paid back duly till now,car (new),2631,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,12,delay in paying off in the past,car (used),1503,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,41,none,rent,1,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,1311,100 <= ... < 500 DM,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,3105,unknown/ no savings account,... < 1 year,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,2,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,21,critical account/ other credits existing (not at this bank),education,2319,... < 100 DM,... < 1 year,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",33,none,rent,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,6,existing credits paid back duly till now,car (new),1374,unknown/ no savings account,unemployed,4,male : single,none,3,building society savings agreement/ life insurance,75,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,3612,... < 100 DM,... >= 7 years,3,male : single,none,4,building society savings agreement/ life insurance,37,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,48,existing credits paid back duly till now,car (new),7763,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,42,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,18,existing credits paid back duly till now,furniture/equipment,3049,... < 100 DM,... < 1 year,1,male : single,none,1,building society savings agreement/ life insurance,45,stores,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1534,... < 100 DM,... < 1 year,1,male : single,none,1,real estate,23,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,24,delay in paying off in the past,car (new),2032,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,60,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,30,existing credits paid back duly till now,furniture/equipment,6350,unknown/ no savings account,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,31,none,own,1,skilled employee / official,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,18,existing credits paid back duly till now,furniture/equipment,2864,... < 100 DM,1 <= ... < 4 years,2,male : single,none,1,real estate,34,none,own,1,unskilled - resident,2,none,yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),car (new),1255,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,61,none,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,24,delay in paying off in the past,car (new),1333,... < 100 DM,unemployed,4,male : single,none,2,real estate,43,none,for free,2,skilled employee / official,2,none,yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),car (new),2022,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",37,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,1552,... < 100 DM,4 <= ... < 7 years,3,male : single,none,1,"car or other, not in attribute Savings account/bonds",32,bank,own,1,skilled employee / official,2,none,yes,good
+... < 0 DM,12,all credits at this bank paid back duly,radio/television,626,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,24,bank,own,1,unskilled - resident,1,none,yes,bad
+no checking account,48,critical account/ other credits existing (not at this bank),car (used),8858,unknown/ no savings account,4 <= ... < 7 years,2,male : single,none,1,unknown / no property,35,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),repairs,996,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,real estate,23,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,6,all credits at this bank paid back duly,radio/television,1750,500 <= ... < 1000 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,45,bank,own,1,unskilled - resident,2,none,yes,good
+... < 0 DM,48,existing credits paid back duly till now,radio/television,6999,... < 100 DM,4 <= ... < 7 years,1,male : single,guarantor,1,real estate,34,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (new),1995,100 <= ... < 500 DM,... < 1 year,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",27,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,education,1199,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,building society savings agreement/ life insurance,67,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1331,... < 100 DM,... < 1 year,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",22,stores,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,18,no credits taken/ all credits paid back duly,car (new),2278,100 <= ... < 500 DM,... < 1 year,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,1,none,yes,bad
+no checking account,21,no credits taken/ all credits paid back duly,car (new),5003,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,4,building society savings agreement/ life insurance,29,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,3552,... < 100 DM,4 <= ... < 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,bank,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,1928,... < 100 DM,... < 1 year,2,male : single,none,2,real estate,31,none,own,2,unskilled - resident,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,car (used),2964,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,49,bank,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,24,all credits at this bank paid back duly,radio/television,1546,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,4,"car or other, not in attribute Savings account/bonds",24,bank,rent,1,unskilled - resident,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,6,delay in paying off in the past,radio/television,683,... < 100 DM,... < 1 year,2,male : single,none,1,building society savings agreement/ life insurance,29,bank,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,car (new),12389,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,4,unknown / no property,37,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,24,delay in paying off in the past,business,4712,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,37,bank,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,delay in paying off in the past,radio/television,1553,100 <= ... < 500 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,23,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,car (new),1372,... < 100 DM,4 <= ... < 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",36,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2578,... >= 1000 DM,... >= 7 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,48,existing credits paid back duly till now,radio/television,3979,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",41,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,48,existing credits paid back duly till now,radio/television,6758,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,3234,... < 100 DM,... < 1 year,4,male : single,none,4,real estate,23,none,rent,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+no checking account,30,critical account/ other credits existing (not at this bank),radio/television,5954,... < 100 DM,4 <= ... < 7 years,3,male : single,co-applicant,2,"car or other, not in attribute Savings account/bonds",38,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,car (used),5433,unknown/ no savings account,unemployed,2,male : single,none,4,building society savings agreement/ life insurance,26,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,15,existing credits paid back duly till now,business,806,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,building society savings agreement/ life insurance,22,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,1082,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,none,own,2,unskilled - resident,1,none,yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),furniture/equipment,2788,... < 100 DM,4 <= ... < 7 years,2,male : single,co-applicant,3,"car or other, not in attribute Savings account/bonds",24,bank,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,2930,... < 100 DM,4 <= ... < 7 years,2,male : single,none,1,real estate,27,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),education,1927,unknown/ no savings account,1 <= ... < 4 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,36,critical account/ other credits existing (not at this bank),car (new),2820,... < 100 DM,... < 1 year,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,none,own,2,skilled employee / official,1,none,yes,bad
+no checking account,24,existing credits paid back duly till now,retraining,937,... < 100 DM,... < 1 year,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",27,none,own,2,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),car (new),1056,... < 100 DM,... >= 7 years,3,male : single,guarantor,3,real estate,30,bank,own,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),car (new),3124,... < 100 DM,... < 1 year,1,male : single,none,3,real estate,49,bank,own,2,unskilled - resident,2,none,yes,good
+no checking account,9,existing credits paid back duly till now,furniture/equipment,1388,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,26,none,rent,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,repairs,2384,... < 100 DM,... < 1 year,4,male : single,none,1,unknown / no property,33,none,rent,1,unskilled - resident,1,none,yes,bad
+no checking account,12,existing credits paid back duly till now,car (new),2133,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,52,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,2039,... < 100 DM,1 <= ... < 4 years,1,male : single,none,4,real estate,20,bank,rent,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,9,critical account/ other credits existing (not at this bank),car (new),2799,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,36,none,rent,2,skilled employee / official,2,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1289,... < 100 DM,1 <= ... < 4 years,4,male : single,guarantor,1,building society savings agreement/ life insurance,21,none,own,1,unskilled - resident,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,domestic appliances,1217,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,47,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,12,critical account/ other credits existing (not at this bank),furniture/equipment,2246,... < 100 DM,... >= 7 years,3,male : single,none,3,building society savings agreement/ life insurance,60,none,own,2,skilled employee / official,1,none,yes,bad
+... < 0 DM,12,critical account/ other credits existing (not at this bank),radio/television,385,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,real estate,58,none,own,4,unskilled - resident,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,delay in paying off in the past,car (new),1965,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",42,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,21,existing credits paid back duly till now,business,1572,... >= 1000 DM,... >= 7 years,4,male : single,none,4,real estate,36,bank,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),2718,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,building society savings agreement/ life insurance,20,none,rent,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,24,all credits at this bank paid back duly,others,1358,unknown/ no savings account,... >= 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",40,stores,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,6,all credits at this bank paid back duly,car (new),931,100 <= ... < 500 DM,... < 1 year,1,male : single,none,1,building society savings agreement/ life insurance,32,stores,own,1,unskilled - resident,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,car (new),1442,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",23,none,rent,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,24,no credits taken/ all credits paid back duly,business,4241,... < 100 DM,1 <= ... < 4 years,1,male : single,none,4,real estate,36,none,own,3,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+no checking account,18,critical account/ other credits existing (not at this bank),car (new),2775,... < 100 DM,4 <= ... < 7 years,2,male : single,none,2,building society savings agreement/ life insurance,31,bank,own,2,skilled employee / official,1,none,yes,bad
+no checking account,24,delay in paying off in the past,business,3863,... < 100 DM,1 <= ... < 4 years,1,male : single,none,2,unknown / no property,32,none,for free,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,7,existing credits paid back duly till now,radio/television,2329,... < 100 DM,... < 1 year,1,male : single,guarantor,1,real estate,45,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,furniture/equipment,918,... < 100 DM,1 <= ... < 4 years,4,male : single,none,1,building society savings agreement/ life insurance,30,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,24,all credits at this bank paid back duly,education,1837,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,unknown / no property,34,bank,for free,1,unskilled - resident,1,none,yes,bad
+no checking account,36,existing credits paid back duly till now,furniture/equipment,3349,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... >= 200 DM / salary assignments for at least 1 year,10,existing credits paid back duly till now,furniture/equipment,1275,... < 100 DM,... < 1 year,4,male : single,none,2,building society savings agreement/ life insurance,23,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,2828,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,22,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),business,4526,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,74,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,radio/television,2671,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : single,co-applicant,4,unknown / no property,50,none,for free,1,skilled employee / official,1,none,yes,bad
+no checking account,18,existing credits paid back duly till now,radio/television,2051,... < 100 DM,... < 1 year,4,male : single,none,1,real estate,33,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,15,existing credits paid back duly till now,car (used),1300,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,45,bank,for free,1,skilled employee / official,2,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,domestic appliances,741,100 <= ... < 500 DM,unemployed,4,male : single,none,3,building society savings agreement/ life insurance,22,none,own,1,skilled employee / official,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,10,existing credits paid back duly till now,car (new),1240,100 <= ... < 500 DM,... >= 7 years,1,male : single,none,4,unknown / no property,48,none,for free,1,unskilled - resident,2,none,yes,bad
+... < 0 DM,21,existing credits paid back duly till now,radio/television,3357,... >= 1000 DM,... < 1 year,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",29,bank,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,24,all credits at this bank paid back duly,car (used),3632,... < 100 DM,1 <= ... < 4 years,1,male : single,guarantor,4,"car or other, not in attribute Savings account/bonds",22,bank,rent,1,skilled employee / official,1,none,no,good
+no checking account,18,delay in paying off in the past,furniture/equipment,1808,... < 100 DM,4 <= ... < 7 years,4,male : single,none,1,real estate,22,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,business,12204,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",48,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,60,delay in paying off in the past,radio/television,9157,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,2,unknown / no property,27,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),3676,... < 100 DM,1 <= ... < 4 years,1,male : single,none,3,real estate,37,none,rent,3,skilled employee / official,2,none,yes,good
+0 <= ... < 200 DM,30,existing credits paid back duly till now,furniture/equipment,3441,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : single,co-applicant,4,"car or other, not in attribute Savings account/bonds",21,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,12,existing credits paid back duly till now,car (new),640,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,49,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,21,critical account/ other credits existing (not at this bank),business,3652,... < 100 DM,4 <= ... < 7 years,2,male : single,none,3,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),car (new),1530,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,building society savings agreement/ life insurance,32,bank,own,2,skilled employee / official,1,none,yes,bad
+no checking account,48,existing credits paid back duly till now,business,3914,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,real estate,38,bank,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,1858,... < 100 DM,... < 1 year,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",22,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,radio/television,2600,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,65,none,for free,2,skilled employee / official,1,none,yes,bad
+no checking account,15,existing credits paid back duly till now,radio/television,1979,unknown/ no savings account,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",35,none,own,1,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,6,existing credits paid back duly till now,furniture/equipment,2116,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,41,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,9,all credits at this bank paid back duly,car (new),1437,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,3,unknown / no property,29,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,42,critical account/ other credits existing (not at this bank),furniture/equipment,4042,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,36,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,9,existing credits paid back duly till now,education,3832,unknown/ no savings account,... >= 7 years,1,male : single,none,4,real estate,64,none,own,1,unskilled - resident,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,radio/television,3660,... < 100 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,18,all credits at this bank paid back duly,furniture/equipment,1553,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",44,bank,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,15,existing credits paid back duly till now,radio/television,1444,unknown/ no savings account,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,23,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,9,existing credits paid back duly till now,furniture/equipment,1980,... < 100 DM,... < 1 year,2,male : single,co-applicant,2,"car or other, not in attribute Savings account/bonds",19,none,rent,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (new),1355,... < 100 DM,... < 1 year,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",25,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,bad
+no checking account,12,existing credits paid back duly till now,education,1393,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,47,bank,own,3,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,1376,500 <= ... < 1000 DM,4 <= ... < 7 years,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,60,delay in paying off in the past,radio/television,15653,... < 100 DM,4 <= ... < 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",21,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,1493,... < 100 DM,... < 1 year,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",34,none,own,1,skilled employee / official,2,none,yes,good
+... < 0 DM,42,delay in paying off in the past,radio/television,4370,... < 100 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,26,bank,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,bad
+... < 0 DM,18,existing credits paid back duly till now,education,750,... < 100 DM,unemployed,4,male : single,none,1,real estate,27,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,bad
+0 <= ... < 200 DM,15,existing credits paid back duly till now,repairs,1308,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",38,none,own,2,unskilled - resident,1,none,yes,good
+no checking account,15,existing credits paid back duly till now,education,4623,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,2,building society savings agreement/ life insurance,40,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,1851,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,2,"car or other, not in attribute Savings account/bonds",33,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,critical account/ other credits existing (not at this bank),radio/television,1880,... < 100 DM,4 <= ... < 7 years,4,male : single,none,1,building society savings agreement/ life insurance,32,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,36,delay in paying off in the past,business,7980,unknown/ no savings account,... < 1 year,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",27,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,30,no credits taken/ all credits paid back duly,furniture/equipment,4583,... < 100 DM,1 <= ... < 4 years,2,male : single,guarantor,2,real estate,32,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,12,existing credits paid back duly till now,car (new),1386,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,car (new),947,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,unknown / no property,38,bank,for free,1,skilled employee / official,2,none,yes,bad
+... < 0 DM,12,existing credits paid back duly till now,education,684,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,rent,1,unskilled - resident,2,none,yes,bad
+... < 0 DM,48,existing credits paid back duly till now,education,7476,... < 100 DM,4 <= ... < 7 years,4,male : single,none,1,unknown / no property,50,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,furniture/equipment,1922,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,37,none,own,1,unskilled - resident,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,car (new),2303,... < 100 DM,... >= 7 years,4,male : single,co-applicant,1,real estate,45,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,36,delay in paying off in the past,car (new),8086,100 <= ... < 500 DM,... >= 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",42,none,own,4,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),car (used),2346,... < 100 DM,4 <= ... < 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",35,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,14,existing credits paid back duly till now,car (new),3973,... < 100 DM,unemployed,1,male : single,none,4,unknown / no property,22,none,for free,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),888,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",41,bank,own,1,unskilled - resident,2,none,yes,bad
+no checking account,48,existing credits paid back duly till now,radio/television,10222,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",37,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,30,no credits taken/ all credits paid back duly,business,4221,... < 100 DM,1 <= ... < 4 years,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",28,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,6361,... < 100 DM,... >= 7 years,2,male : single,none,1,unknown / no property,41,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,radio/television,1297,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,real estate,23,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,car (new),900,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",23,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,21,existing credits paid back duly till now,furniture/equipment,2241,... < 100 DM,... >= 7 years,4,male : single,none,2,real estate,50,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,6,delay in paying off in the past,furniture/equipment,1050,... < 100 DM,unemployed,4,male : single,none,1,building society savings agreement/ life insurance,35,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,6,critical account/ other credits existing (not at this bank),education,1047,... < 100 DM,1 <= ... < 4 years,2,male : single,none,4,building society savings agreement/ life insurance,50,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),others,6314,... < 100 DM,unemployed,4,male : single,co-applicant,2,unknown / no property,27,bank,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,30,all credits at this bank paid back duly,furniture/equipment,3496,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",34,stores,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,48,all credits at this bank paid back duly,business,3609,... < 100 DM,1 <= ... < 4 years,1,male : single,none,1,real estate,27,stores,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),4843,... < 100 DM,... >= 7 years,3,male : single,co-applicant,4,building society savings agreement/ life insurance,43,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... >= 200 DM / salary assignments for at least 1 year,30,critical account/ other credits existing (not at this bank),radio/television,3017,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,47,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),business,4139,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,3,building society savings agreement/ life insurance,27,none,own,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
+no checking account,36,existing credits paid back duly till now,business,5742,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,60,existing credits paid back duly till now,car (new),10366,... < 100 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,42,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,6,critical account/ other credits existing (not at this bank),car (new),2080,500 <= ... < 1000 DM,1 <= ... < 4 years,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,21,delay in paying off in the past,business,2580,500 <= ... < 1000 DM,... < 1 year,4,male : single,none,2,real estate,41,bank,own,1,unskilled - resident,2,none,yes,bad
+no checking account,30,critical account/ other credits existing (not at this bank),radio/television,4530,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",26,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),furniture/equipment,5150,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,72,existing credits paid back duly till now,radio/television,5595,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,radio/television,2384,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,64,bank,rent,1,unskilled - resident,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,radio/television,1453,... < 100 DM,... < 1 year,3,male : single,none,1,real estate,26,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,6,existing credits paid back duly till now,education,1538,... < 100 DM,... < 1 year,1,male : single,none,2,unknown / no property,56,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,2279,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,37,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,15,delay in paying off in the past,radio/television,1478,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,33,bank,own,2,skilled employee / official,1,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,5103,... < 100 DM,... < 1 year,3,male : single,none,3,unknown / no property,47,none,for free,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,36,delay in paying off in the past,business,9857,100 <= ... < 500 DM,4 <= ... < 7 years,1,male : single,none,3,building society savings agreement/ life insurance,31,none,own,2,unskilled - resident,2,"yes, registered under the customers name",yes,good
+no checking account,60,existing credits paid back duly till now,car (new),6527,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,34,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,10,critical account/ other credits existing (not at this bank),radio/television,1347,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,2,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,36,delay in paying off in the past,car (new),2862,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,3,unknown / no property,30,none,for free,1,skilled employee / official,1,none,yes,good
+no checking account,9,existing credits paid back duly till now,radio/television,2753,100 <= ... < 500 DM,... >= 7 years,3,male : single,co-applicant,4,"car or other, not in attribute Savings account/bonds",35,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,car (new),3651,... >= 1000 DM,1 <= ... < 4 years,1,male : single,none,3,building society savings agreement/ life insurance,31,none,own,1,skilled employee / official,2,none,yes,good
+... < 0 DM,15,critical account/ other credits existing (not at this bank),furniture/equipment,975,... < 100 DM,1 <= ... < 4 years,2,male : single,none,3,building society savings agreement/ life insurance,25,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,15,existing credits paid back duly till now,repairs,2631,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,25,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,2896,100 <= ... < 500 DM,... < 1 year,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",29,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,6,critical account/ other credits existing (not at this bank),car (new),4716,unknown/ no savings account,... < 1 year,1,male : single,none,3,real estate,44,none,own,2,unskilled - resident,2,none,yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,2284,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,6,existing credits paid back duly till now,car (used),1236,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,4,building society savings agreement/ life insurance,50,none,rent,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1103,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,3,real estate,29,none,own,2,skilled employee / official,1,none,no,good
+no checking account,12,critical account/ other credits existing (not at this bank),car (new),926,... < 100 DM,unemployed,1,male : single,none,2,building society savings agreement/ life insurance,38,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1800,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",24,none,own,2,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,15,existing credits paid back duly till now,education,1905,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,furniture/equipment,1123,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",29,none,rent,1,unskilled - resident,1,none,yes,bad
+... < 0 DM,48,critical account/ other credits existing (not at this bank),car (used),6331,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,46,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,radio/television,1377,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,2,unknown / no property,47,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,30,delay in paying off in the past,business,2503,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,2,building society savings agreement/ life insurance,41,stores,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,27,existing credits paid back duly till now,business,2528,... < 100 DM,... < 1 year,4,male : single,none,1,building society savings agreement/ life insurance,32,none,own,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,15,existing credits paid back duly till now,car (new),5324,500 <= ... < 1000 DM,... >= 7 years,1,male : single,none,4,unknown / no property,35,none,for free,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,48,existing credits paid back duly till now,car (new),6560,100 <= ... < 500 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,24,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,12,no credits taken/ all credits paid back duly,furniture/equipment,2969,... < 100 DM,... < 1 year,4,male : single,none,3,building society savings agreement/ life insurance,25,none,rent,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,1206,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,25,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,2118,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,37,none,own,1,unskilled - resident,2,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,629,500 <= ... < 1000 DM,... >= 7 years,4,male : single,none,3,building society savings agreement/ life insurance,32,bank,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,6,all credits at this bank paid back duly,education,1198,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,35,none,for free,1,skilled employee / official,1,none,yes,bad
+no checking account,21,existing credits paid back duly till now,car (used),2476,unknown/ no savings account,... >= 7 years,4,male : single,none,4,real estate,46,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,9,critical account/ other credits existing (not at this bank),radio/television,1138,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,25,none,own,2,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,60,existing credits paid back duly till now,car (new),14027,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,unknown / no property,27,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,30,critical account/ other credits existing (not at this bank),car (used),7596,unknown/ no savings account,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",63,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,30,critical account/ other credits existing (not at this bank),radio/television,3077,unknown/ no savings account,... >= 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",40,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,18,existing credits paid back duly till now,radio/television,1505,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,unknown / no property,32,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,24,critical account/ other credits existing (not at this bank),radio/television,3148,unknown/ no savings account,1 <= ... < 4 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,20,no credits taken/ all credits paid back duly,car (used),6148,100 <= ... < 500 DM,... >= 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",31,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,9,no credits taken/ all credits paid back duly,radio/television,1337,... < 100 DM,... < 1 year,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,6,all credits at this bank paid back duly,education,433,... >= 1000 DM,... < 1 year,4,male : single,none,2,building society savings agreement/ life insurance,24,bank,rent,1,skilled employee / official,2,none,yes,bad
+... < 0 DM,12,existing credits paid back duly till now,car (new),1228,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,24,none,own,1,unskilled - resident,1,none,yes,bad
+0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,790,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,66,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,27,existing credits paid back duly till now,car (new),2570,... < 100 DM,1 <= ... < 4 years,3,male : single,none,3,real estate,21,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,6,critical account/ other credits existing (not at this bank),car (new),250,... >= 1000 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,41,bank,own,2,unskilled - resident,1,none,yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1316,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,47,none,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,radio/television,1882,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",25,bank,rent,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,48,all credits at this bank paid back duly,business,6416,... < 100 DM,... >= 7 years,4,male : single,none,3,unknown / no property,59,none,rent,1,skilled employee / official,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,24,critical account/ other credits existing (not at this bank),business,1275,... >= 1000 DM,1 <= ... < 4 years,2,male : single,none,4,real estate,36,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,delay in paying off in the past,radio/television,6403,... < 100 DM,... < 1 year,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,radio/television,1987,... < 100 DM,1 <= ... < 4 years,2,male : single,none,4,real estate,21,none,rent,1,unskilled - resident,2,none,yes,bad
+0 <= ... < 200 DM,8,existing credits paid back duly till now,radio/television,760,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,2,real estate,44,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,car (used),2603,... >= 1000 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,4,critical account/ other credits existing (not at this bank),car (new),3380,... < 100 DM,4 <= ... < 7 years,1,male : single,none,1,real estate,37,none,own,1,skilled employee / official,2,none,yes,good
+0 <= ... < 200 DM,36,all credits at this bank paid back duly,domestic appliances,3990,unknown/ no savings account,... < 1 year,3,male : single,none,2,unknown / no property,29,bank,own,1,unemployed/ unskilled - non-resident,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (used),11560,... < 100 DM,1 <= ... < 4 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",23,none,rent,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
+... < 0 DM,18,existing credits paid back duly till now,car (new),4380,100 <= ... < 500 DM,1 <= ... < 4 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",35,none,own,1,unskilled - resident,2,"yes, registered under the customers name",yes,good
+no checking account,6,critical account/ other credits existing (not at this bank),car (new),6761,... < 100 DM,4 <= ... < 7 years,1,male : single,none,3,unknown / no property,45,none,own,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,30,no credits taken/ all credits paid back duly,business,4280,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",26,none,rent,2,unskilled - resident,1,none,yes,bad
+... < 0 DM,24,all credits at this bank paid back duly,car (new),2325,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",32,bank,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,10,all credits at this bank paid back duly,radio/television,1048,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,23,stores,own,1,unskilled - resident,1,none,yes,good
+no checking account,21,existing credits paid back duly till now,radio/television,3160,unknown/ no savings account,... >= 7 years,4,male : single,none,3,building society savings agreement/ life insurance,41,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,2483,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,22,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,39,critical account/ other credits existing (not at this bank),furniture/equipment,14179,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,building society savings agreement/ life insurance,30,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,13,critical account/ other credits existing (not at this bank),business,1797,... < 100 DM,... < 1 year,3,male : single,none,1,building society savings agreement/ life insurance,28,bank,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,15,existing credits paid back duly till now,car (new),2511,... < 100 DM,unemployed,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",23,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,car (new),1274,... < 100 DM,... < 1 year,3,male : single,none,1,real estate,37,none,own,1,unskilled - resident,1,none,yes,bad
+no checking account,21,existing credits paid back duly till now,car (used),5248,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,3,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,15,existing credits paid back duly till now,car (used),3029,... < 100 DM,4 <= ... < 7 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,6,existing credits paid back duly till now,furniture/equipment,428,... < 100 DM,... >= 7 years,2,male : single,none,1,building society savings agreement/ life insurance,49,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,existing credits paid back duly till now,car (new),976,... < 100 DM,... < 1 year,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",23,none,own,1,unskilled - resident,1,none,yes,bad
+0 <= ... < 200 DM,12,existing credits paid back duly till now,business,841,100 <= ... < 500 DM,4 <= ... < 7 years,2,male : single,none,4,real estate,23,none,rent,1,unskilled - resident,1,none,yes,good
+no checking account,30,critical account/ other credits existing (not at this bank),radio/television,5771,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",25,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,12,delay in paying off in the past,repairs,1555,... >= 1000 DM,... >= 7 years,4,male : single,none,4,unknown / no property,55,none,for free,2,skilled employee / official,2,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,car (new),1285,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,4,unknown / no property,32,none,rent,1,skilled employee / official,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,6,critical account/ other credits existing (not at this bank),car (new),1299,... < 100 DM,1 <= ... < 4 years,1,male : single,none,1,real estate,74,none,own,3,unemployed/ unskilled - non-resident,2,none,no,good
+... >= 200 DM / salary assignments for at least 1 year,15,critical account/ other credits existing (not at this bank),radio/television,1271,unknown/ no savings account,1 <= ... < 4 years,3,male : single,none,4,unknown / no property,39,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,24,existing credits paid back duly till now,car (new),1393,... < 100 DM,1 <= ... < 4 years,2,male : single,guarantor,2,real estate,31,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),691,... < 100 DM,... >= 7 years,4,male : single,none,3,building society savings agreement/ life insurance,35,none,own,2,skilled employee / official,1,none,yes,bad
+no checking account,15,critical account/ other credits existing (not at this bank),car (new),5045,unknown/ no savings account,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",59,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,2124,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,real estate,24,none,rent,2,skilled employee / official,1,none,yes,bad
+... < 0 DM,12,existing credits paid back duly till now,radio/television,2214,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,building society savings agreement/ life insurance,24,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,21,critical account/ other credits existing (not at this bank),car (new),12680,unknown/ no savings account,... >= 7 years,4,male : single,none,4,unknown / no property,30,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),car (new),2463,100 <= ... < 500 DM,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,radio/television,1155,... < 100 DM,... >= 7 years,3,male : single,guarantor,3,real estate,40,bank,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,30,existing credits paid back duly till now,furniture/equipment,3108,... < 100 DM,... < 1 year,2,male : single,none,4,building society savings agreement/ life insurance,31,none,own,1,unskilled - resident,1,none,yes,bad
+no checking account,10,existing credits paid back duly till now,car (used),2901,unknown/ no savings account,... < 1 year,1,male : single,none,4,real estate,31,none,rent,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,critical account/ other credits existing (not at this bank),furniture/equipment,3617,... < 100 DM,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,3,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,1655,... < 100 DM,... >= 7 years,2,male : single,none,4,real estate,63,none,own,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,existing credits paid back duly till now,car (used),2812,unknown/ no savings account,... >= 7 years,2,male : single,none,4,real estate,26,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,36,critical account/ other credits existing (not at this bank),education,8065,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,unknown / no property,25,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,21,critical account/ other credits existing (not at this bank),car (used),3275,... < 100 DM,... >= 7 years,1,male : single,none,4,"car or other, not in attribute Savings account/bonds",36,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2223,100 <= ... < 500 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,52,bank,own,2,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,critical account/ other credits existing (not at this bank),car (new),1480,500 <= ... < 1000 DM,unemployed,2,male : single,none,4,unknown / no property,66,bank,for free,3,unemployed/ unskilled - non-resident,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,car (new),1371,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,real estate,25,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,36,critical account/ other credits existing (not at this bank),car (new),3535,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",37,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,existing credits paid back duly till now,radio/television,3509,... < 100 DM,4 <= ... < 7 years,4,male : single,guarantor,1,real estate,25,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,36,critical account/ other credits existing (not at this bank),car (used),5711,... >= 1000 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",38,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,repairs,3872,... < 100 DM,unemployed,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",67,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,39,critical account/ other credits existing (not at this bank),radio/television,4933,... < 100 DM,4 <= ... < 7 years,2,male : single,guarantor,2,real estate,25,none,own,2,skilled employee / official,1,none,yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),car (new),1940,... >= 1000 DM,... >= 7 years,4,male : single,none,4,real estate,60,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,no credits taken/ all credits paid back duly,retraining,1410,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,31,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),836,100 <= ... < 500 DM,... < 1 year,4,male : single,none,2,building society savings agreement/ life insurance,23,bank,own,1,unskilled - resident,1,none,yes,bad
+0 <= ... < 200 DM,20,existing credits paid back duly till now,car (used),6468,unknown/ no savings account,unemployed,1,male : single,none,4,real estate,60,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,18,existing credits paid back duly till now,business,1941,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,2,building society savings agreement/ life insurance,35,none,own,1,unskilled - resident,1,"yes, registered under the customers name",yes,good
+no checking account,22,existing credits paid back duly till now,radio/television,2675,500 <= ... < 1000 DM,... >= 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,48,critical account/ other credits existing (not at this bank),car (used),2751,unknown/ no savings account,... >= 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",38,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,48,delay in paying off in the past,education,6224,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,50,none,for free,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,40,critical account/ other credits existing (not at this bank),education,5998,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,unknown / no property,27,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,21,existing credits paid back duly till now,business,1188,... < 100 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,39,none,own,1,skilled employee / official,2,none,yes,bad
+no checking account,24,existing credits paid back duly till now,car (used),6313,unknown/ no savings account,... >= 7 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",41,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+no checking account,6,critical account/ other credits existing (not at this bank),furniture/equipment,1221,unknown/ no savings account,1 <= ... < 4 years,1,male : single,none,2,building society savings agreement/ life insurance,27,none,own,2,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,furniture/equipment,2892,... < 100 DM,... >= 7 years,3,male : single,none,4,unknown / no property,51,none,for free,1,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,furniture/equipment,3062,500 <= ... < 1000 DM,... >= 7 years,4,male : single,none,3,unknown / no property,32,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,9,existing credits paid back duly till now,furniture/equipment,2301,100 <= ... < 500 DM,... < 1 year,2,male : single,none,4,building society savings agreement/ life insurance,22,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,car (used),7511,unknown/ no savings account,... >= 7 years,1,male : single,none,4,building society savings agreement/ life insurance,51,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
+no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,1258,... < 100 DM,... < 1 year,2,male : single,none,4,building society savings agreement/ life insurance,22,none,rent,2,unskilled - resident,1,none,yes,good
+no checking account,24,delay in paying off in the past,car (new),717,unknown/ no savings account,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",54,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,car (new),1549,unknown/ no savings account,... < 1 year,4,male : single,none,2,real estate,35,none,own,1,unemployed/ unskilled - non-resident,1,none,yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),education,1597,... < 100 DM,... >= 7 years,4,male : single,none,4,unknown / no property,54,none,for free,2,skilled employee / official,2,none,yes,good
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),radio/television,1795,... < 100 DM,... >= 7 years,3,male : single,guarantor,4,real estate,48,bank,rent,2,unskilled - resident,1,"yes, registered under the customers name",yes,good
+... < 0 DM,20,critical account/ other credits existing (not at this bank),furniture/equipment,4272,... < 100 DM,... >= 7 years,1,male : single,none,4,building society savings agreement/ life insurance,24,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,976,unknown/ no savings account,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",35,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),7472,unknown/ no savings account,unemployed,1,male : single,none,2,real estate,24,none,rent,1,unemployed/ unskilled - non-resident,1,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,car (new),9271,... < 100 DM,4 <= ... < 7 years,2,male : single,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,590,... < 100 DM,... < 1 year,3,male : single,none,3,real estate,26,none,own,1,unskilled - resident,1,none,no,good
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,930,unknown/ no savings account,... >= 7 years,4,male : single,none,4,real estate,65,none,own,4,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,42,all credits at this bank paid back duly,car (used),9283,... < 100 DM,unemployed,1,male : single,none,2,unknown / no property,55,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,15,no credits taken/ all credits paid back duly,car (new),1778,... < 100 DM,... < 1 year,2,male : single,none,1,real estate,26,none,rent,2,unemployed/ unskilled - non-resident,1,none,yes,bad
+0 <= ... < 200 DM,8,existing credits paid back duly till now,business,907,... < 100 DM,... < 1 year,3,male : single,none,2,real estate,26,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,484,... < 100 DM,4 <= ... < 7 years,3,male : single,guarantor,3,real estate,28,bank,own,1,unskilled - resident,1,none,yes,good
+... < 0 DM,36,critical account/ other credits existing (not at this bank),car (used),9629,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",24,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,48,existing credits paid back duly till now,domestic appliances,3051,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",54,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,48,existing credits paid back duly till now,car (new),3931,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,unknown / no property,46,none,for free,1,skilled employee / official,2,none,yes,bad
+0 <= ... < 200 DM,36,delay in paying off in the past,car (new),7432,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,building society savings agreement/ life insurance,54,none,rent,1,skilled employee / official,1,none,yes,good
+no checking account,6,existing credits paid back duly till now,domestic appliances,1338,500 <= ... < 1000 DM,1 <= ... < 4 years,1,male : single,none,4,real estate,62,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1554,... < 100 DM,4 <= ... < 7 years,1,male : single,none,2,"car or other, not in attribute Savings account/bonds",24,none,rent,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,36,existing credits paid back duly till now,others,15857,... < 100 DM,unemployed,2,male : single,co-applicant,3,"car or other, not in attribute Savings account/bonds",43,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,radio/television,1345,... < 100 DM,1 <= ... < 4 years,4,male : single,none,3,real estate,26,bank,own,1,skilled employee / official,1,none,yes,bad
+no checking account,12,existing credits paid back duly till now,car (new),1101,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,27,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,12,existing credits paid back duly till now,radio/television,3016,... < 100 DM,1 <= ... < 4 years,3,male : single,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,2712,... < 100 DM,... >= 7 years,2,male : single,none,2,building society savings agreement/ life insurance,41,bank,own,1,skilled employee / official,2,none,yes,bad
+... < 0 DM,8,critical account/ other credits existing (not at this bank),car (new),731,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,47,none,own,2,unskilled - resident,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),furniture/equipment,3780,... < 100 DM,... < 1 year,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",35,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,21,critical account/ other credits existing (not at this bank),car (new),1602,... < 100 DM,... >= 7 years,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",30,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,critical account/ other credits existing (not at this bank),car (new),3966,... < 100 DM,... >= 7 years,1,male : single,none,4,real estate,33,bank,rent,3,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,18,no credits taken/ all credits paid back duly,business,4165,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",36,stores,own,2,skilled employee / official,2,none,yes,bad
+... < 0 DM,36,existing credits paid back duly till now,car (used),8335,unknown/ no savings account,... >= 7 years,3,male : single,none,4,unknown / no property,47,none,for free,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,48,delay in paying off in the past,business,6681,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,38,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,24,delay in paying off in the past,business,2375,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",44,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,18,existing credits paid back duly till now,car (new),1216,... < 100 DM,... < 1 year,4,male : single,none,3,"car or other, not in attribute Savings account/bonds",23,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,45,no credits taken/ all credits paid back duly,business,11816,... < 100 DM,... >= 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",29,none,rent,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,24,existing credits paid back duly till now,radio/television,5084,unknown/ no savings account,... >= 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,15,existing credits paid back duly till now,radio/television,2327,... < 100 DM,... < 1 year,2,male : single,none,3,real estate,25,none,own,1,unskilled - resident,1,none,yes,bad
+... < 0 DM,12,no credits taken/ all credits paid back duly,car (new),1082,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",48,bank,own,2,skilled employee / official,1,none,yes,bad
+no checking account,12,existing credits paid back duly till now,radio/television,886,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",21,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,4,existing credits paid back duly till now,furniture/equipment,601,... < 100 DM,... < 1 year,1,male : single,none,3,real estate,23,none,rent,1,unskilled - resident,2,none,yes,good
+... < 0 DM,24,critical account/ other credits existing (not at this bank),car (used),2957,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,63,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,critical account/ other credits existing (not at this bank),radio/television,2611,... < 100 DM,... >= 7 years,4,male : single,co-applicant,3,real estate,46,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,5179,... < 100 DM,4 <= ... < 7 years,4,male : single,none,2,building society savings agreement/ life insurance,29,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,21,delay in paying off in the past,car (used),2993,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,real estate,28,stores,own,2,unskilled - resident,1,none,yes,good
+no checking account,18,existing credits paid back duly till now,repairs,1943,... < 100 DM,... < 1 year,4,male : single,none,4,real estate,23,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,24,all credits at this bank paid back duly,business,1559,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",50,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,18,existing credits paid back duly till now,furniture/equipment,3422,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,47,bank,own,3,skilled employee / official,2,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,21,existing credits paid back duly till now,furniture/equipment,3976,unknown/ no savings account,4 <= ... < 7 years,2,male : single,none,3,"car or other, not in attribute Savings account/bonds",35,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,18,existing credits paid back duly till now,car (new),6761,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",68,none,rent,2,skilled employee / official,1,none,yes,bad
+no checking account,24,existing credits paid back duly till now,car (new),1249,... < 100 DM,... < 1 year,4,male : single,none,2,real estate,28,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,9,existing credits paid back duly till now,radio/television,1364,... < 100 DM,4 <= ... < 7 years,3,male : single,none,4,real estate,59,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,radio/television,709,... < 100 DM,... >= 7 years,4,male : single,none,4,real estate,57,stores,own,1,unskilled - resident,1,none,yes,bad
+... < 0 DM,20,critical account/ other credits existing (not at this bank),car (new),2235,... < 100 DM,1 <= ... < 4 years,4,male : single,guarantor,2,building society savings agreement/ life insurance,33,bank,rent,2,skilled employee / official,1,none,no,bad
+no checking account,24,critical account/ other credits existing (not at this bank),car (used),4042,unknown/ no savings account,4 <= ... < 7 years,3,male : single,none,4,building society savings agreement/ life insurance,43,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1471,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,unknown / no property,35,none,for free,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,18,all credits at this bank paid back duly,car (new),1442,... < 100 DM,4 <= ... < 7 years,4,male : single,none,4,unknown / no property,32,none,for free,2,unskilled - resident,2,none,yes,bad
+no checking account,36,delay in paying off in the past,car (new),10875,... < 100 DM,... >= 7 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",45,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,car (new),1474,100 <= ... < 500 DM,... < 1 year,4,male : single,none,3,real estate,33,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,10,existing credits paid back duly till now,retraining,894,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,3,building society savings agreement/ life insurance,40,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),furniture/equipment,3343,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,unknown / no property,28,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,15,existing credits paid back duly till now,car (new),3959,... < 100 DM,1 <= ... < 4 years,3,male : single,none,2,building society savings agreement/ life insurance,29,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,9,existing credits paid back duly till now,car (new),3577,100 <= ... < 500 DM,1 <= ... < 4 years,1,male : single,guarantor,2,real estate,26,none,rent,1,skilled employee / official,2,none,no,good
+no checking account,24,critical account/ other credits existing (not at this bank),car (used),5804,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,2,real estate,27,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,delay in paying off in the past,business,2169,... < 100 DM,1 <= ... < 4 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,24,existing credits paid back duly till now,radio/television,2439,... < 100 DM,... < 1 year,4,male : single,none,4,real estate,35,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,27,critical account/ other credits existing (not at this bank),furniture/equipment,4526,... >= 1000 DM,... < 1 year,4,male : single,none,2,real estate,32,stores,own,2,unskilled - resident,2,"yes, registered under the customers name",yes,good
+no checking account,10,existing credits paid back duly till now,furniture/equipment,2210,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,25,bank,rent,1,unskilled - resident,1,none,yes,bad
+no checking account,15,existing credits paid back duly till now,furniture/equipment,2221,500 <= ... < 1000 DM,1 <= ... < 4 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",20,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,radio/television,2389,... < 100 DM,... < 1 year,4,male : single,none,1,"car or other, not in attribute Savings account/bonds",27,stores,own,1,skilled employee / official,1,none,yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,3331,... < 100 DM,... >= 7 years,2,male : single,none,4,building society savings agreement/ life insurance,42,stores,own,1,skilled employee / official,1,none,yes,good
+no checking account,36,existing credits paid back duly till now,business,7409,unknown/ no savings account,... >= 7 years,3,male : single,none,2,building society savings agreement/ life insurance,37,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,652,... < 100 DM,... >= 7 years,4,male : single,none,4,building society savings agreement/ life insurance,24,none,rent,1,skilled employee / official,1,none,yes,good
+no checking account,36,delay in paying off in the past,furniture/equipment,7678,500 <= ... < 1000 DM,4 <= ... < 7 years,2,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,6,critical account/ other credits existing (not at this bank),car (new),1343,... < 100 DM,... >= 7 years,1,male : single,none,4,real estate,46,none,own,2,skilled employee / official,2,none,no,good
+... < 0 DM,24,critical account/ other credits existing (not at this bank),business,1382,100 <= ... < 500 DM,4 <= ... < 7 years,4,male : single,none,1,real estate,26,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,15,existing credits paid back duly till now,domestic appliances,874,unknown/ no savings account,... < 1 year,4,male : single,none,1,real estate,24,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,12,existing credits paid back duly till now,furniture/equipment,3590,... < 100 DM,1 <= ... < 4 years,2,male : single,co-applicant,2,building society savings agreement/ life insurance,29,none,own,1,unskilled - resident,2,none,yes,good
+0 <= ... < 200 DM,11,critical account/ other credits existing (not at this bank),car (new),1322,... >= 1000 DM,1 <= ... < 4 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",40,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,18,all credits at this bank paid back duly,radio/television,1940,... < 100 DM,... < 1 year,3,male : single,co-applicant,4,unknown / no property,36,bank,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,36,existing credits paid back duly till now,radio/television,3595,... < 100 DM,... >= 7 years,4,male : single,none,2,"car or other, not in attribute Savings account/bonds",28,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,9,existing credits paid back duly till now,car (new),1422,... < 100 DM,... < 1 year,3,male : single,none,2,unknown / no property,27,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,30,critical account/ other credits existing (not at this bank),radio/television,6742,unknown/ no savings account,4 <= ... < 7 years,2,male : single,none,3,building society savings agreement/ life insurance,36,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,car (used),7814,... < 100 DM,4 <= ... < 7 years,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",38,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,car (used),9277,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,4,unknown / no property,48,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,30,critical account/ other credits existing (not at this bank),car (new),2181,unknown/ no savings account,... >= 7 years,4,male : single,none,4,real estate,36,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1098,... < 100 DM,unemployed,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",65,none,own,2,unemployed/ unskilled - non-resident,1,none,yes,good
+0 <= ... < 200 DM,24,existing credits paid back duly till now,furniture/equipment,4057,... < 100 DM,4 <= ... < 7 years,3,male : single,none,3,"car or other, not in attribute Savings account/bonds",43,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,12,existing credits paid back duly till now,education,795,... < 100 DM,... < 1 year,4,male : single,none,4,building society savings agreement/ life insurance,53,none,own,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),business,2825,unknown/ no savings account,4 <= ... < 7 years,4,male : single,none,3,unknown / no property,34,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,48,existing credits paid back duly till now,business,15672,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",23,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,36,critical account/ other credits existing (not at this bank),car (new),6614,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",34,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,28,all credits at this bank paid back duly,car (used),7824,unknown/ no savings account,... < 1 year,3,male : single,guarantor,4,real estate,40,bank,rent,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,27,critical account/ other credits existing (not at this bank),business,2442,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",43,stores,own,4,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+no checking account,15,critical account/ other credits existing (not at this bank),radio/television,1829,... < 100 DM,... >= 7 years,4,male : single,none,4,"car or other, not in attribute Savings account/bonds",46,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,critical account/ other credits existing (not at this bank),car (new),2171,... < 100 DM,1 <= ... < 4 years,4,male : single,none,4,building society savings agreement/ life insurance,38,bank,own,2,unskilled - resident,1,none,no,good
+0 <= ... < 200 DM,36,critical account/ other credits existing (not at this bank),car (used),5800,... < 100 DM,1 <= ... < 4 years,3,male : single,none,4,"car or other, not in attribute Savings account/bonds",34,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,18,critical account/ other credits existing (not at this bank),radio/television,1169,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,3,building society savings agreement/ life insurance,29,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,36,delay in paying off in the past,car (used),8947,unknown/ no savings account,4 <= ... < 7 years,3,male : single,none,2,"car or other, not in attribute Savings account/bonds",31,stores,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+... < 0 DM,21,existing credits paid back duly till now,radio/television,2606,... < 100 DM,... < 1 year,4,male : single,none,4,building society savings agreement/ life insurance,28,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),furniture/equipment,1592,... >= 1000 DM,4 <= ... < 7 years,3,male : single,none,2,building society savings agreement/ life insurance,35,none,own,1,skilled employee / official,1,none,no,good
+no checking account,15,existing credits paid back duly till now,furniture/equipment,2186,unknown/ no savings account,4 <= ... < 7 years,1,male : single,none,4,real estate,33,bank,rent,1,unskilled - resident,1,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,furniture/equipment,4153,... < 100 DM,1 <= ... < 4 years,2,male : single,co-applicant,3,"car or other, not in attribute Savings account/bonds",42,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,16,critical account/ other credits existing (not at this bank),car (new),2625,... < 100 DM,... >= 7 years,2,male : single,guarantor,4,building society savings agreement/ life insurance,43,bank,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,20,critical account/ other credits existing (not at this bank),car (new),3485,unknown/ no savings account,... < 1 year,2,male : single,none,4,real estate,44,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,36,critical account/ other credits existing (not at this bank),car (used),10477,unknown/ no savings account,... >= 7 years,2,male : single,none,4,unknown / no property,42,none,for free,2,skilled employee / official,1,none,yes,good
+no checking account,15,existing credits paid back duly till now,radio/television,1386,unknown/ no savings account,1 <= ... < 4 years,4,male : single,none,2,real estate,40,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,1278,... < 100 DM,... >= 7 years,4,male : single,none,1,real estate,36,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,radio/television,1107,... < 100 DM,1 <= ... < 4 years,2,male : single,none,2,real estate,20,none,rent,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+... < 0 DM,21,existing credits paid back duly till now,car (new),3763,unknown/ no savings account,4 <= ... < 7 years,2,male : single,co-applicant,2,real estate,24,none,own,1,unskilled - resident,1,none,no,good
+0 <= ... < 200 DM,36,existing credits paid back duly till now,education,3711,unknown/ no savings account,1 <= ... < 4 years,2,male : single,none,2,"car or other, not in attribute Savings account/bonds",27,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,15,delay in paying off in the past,car (used),3594,... < 100 DM,... < 1 year,1,male : married/widowed,none,2,building society savings agreement/ life insurance,46,none,own,2,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,car (new),3195,unknown/ no savings account,1 <= ... < 4 years,1,male : married/widowed,none,2,real estate,33,none,own,1,unskilled - resident,1,none,yes,good
+no checking account,36,delay in paying off in the past,radio/television,4454,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,4,real estate,34,none,own,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),furniture/equipment,4736,... < 100 DM,... < 1 year,2,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",25,bank,own,1,unskilled - resident,1,none,yes,bad
+0 <= ... < 200 DM,30,existing credits paid back duly till now,radio/television,2991,unknown/ no savings account,... >= 7 years,2,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",25,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,11,existing credits paid back duly till now,business,2142,... >= 1000 DM,... >= 7 years,1,male : married/widowed,none,2,real estate,28,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,all credits at this bank paid back duly,business,3161,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,31,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,others,18424,... < 100 DM,1 <= ... < 4 years,1,male : married/widowed,none,2,building society savings agreement/ life insurance,32,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",no,bad
+no checking account,10,existing credits paid back duly till now,car (used),2848,100 <= ... < 500 DM,1 <= ... < 4 years,1,male : married/widowed,co-applicant,2,real estate,32,none,own,1,skilled employee / official,2,none,yes,good
+... < 0 DM,6,existing credits paid back duly till now,car (new),14896,... < 100 DM,... >= 7 years,1,male : married/widowed,none,4,unknown / no property,68,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,2359,100 <= ... < 500 DM,unemployed,1,male : married/widowed,none,1,building society savings agreement/ life insurance,33,none,own,1,skilled employee / official,1,none,yes,bad
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,3345,... < 100 DM,... >= 7 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,39,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+no checking account,18,critical account/ other credits existing (not at this bank),furniture/equipment,1817,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,unknown / no property,28,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,48,delay in paying off in the past,radio/television,12749,500 <= ... < 1000 DM,4 <= ... < 7 years,4,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",37,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,9,existing credits paid back duly till now,radio/television,1366,... < 100 DM,... < 1 year,3,male : married/widowed,none,4,building society savings agreement/ life insurance,22,none,rent,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,12,existing credits paid back duly till now,car (new),2002,... < 100 DM,4 <= ... < 7 years,3,male : married/widowed,none,4,building society savings agreement/ life insurance,30,none,rent,1,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,6872,... < 100 DM,... < 1 year,2,male : married/widowed,none,1,building society savings agreement/ life insurance,55,bank,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,12,all credits at this bank paid back duly,car (new),697,... < 100 DM,... < 1 year,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",46,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,18,critical account/ other credits existing (not at this bank),furniture/equipment,1049,... < 100 DM,... < 1 year,4,male : married/widowed,none,4,building society savings agreement/ life insurance,21,none,rent,1,skilled employee / official,1,none,yes,good
+... < 0 DM,48,existing credits paid back duly till now,car (used),10297,... < 100 DM,4 <= ... < 7 years,4,male : married/widowed,none,4,unknown / no property,39,stores,for free,3,skilled employee / official,2,"yes, registered under the customers name",yes,bad
+no checking account,30,existing credits paid back duly till now,radio/television,1867,unknown/ no savings account,... >= 7 years,4,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",58,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,12,delay in paying off in the past,car (new),1344,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,real estate,43,none,own,2,unskilled - resident,2,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,furniture/equipment,1747,... < 100 DM,... < 1 year,4,male : married/widowed,co-applicant,1,building society savings agreement/ life insurance,24,none,own,1,unskilled - resident,1,none,no,good
+0 <= ... < 200 DM,9,existing credits paid back duly till now,radio/television,1670,... < 100 DM,... < 1 year,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",22,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+no checking account,9,critical account/ other credits existing (not at this bank),car (new),1224,... < 100 DM,1 <= ... < 4 years,3,male : married/widowed,none,1,real estate,30,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),radio/television,522,500 <= ... < 1000 DM,... >= 7 years,4,male : married/widowed,none,4,building society savings agreement/ life insurance,42,none,own,2,skilled employee / official,2,"yes, registered under the customers name",yes,good
+... < 0 DM,12,existing credits paid back duly till now,radio/television,1498,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",23,bank,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,30,delay in paying off in the past,radio/television,1919,100 <= ... < 500 DM,... < 1 year,4,male : married/widowed,none,3,unknown / no property,30,stores,own,2,management/ self-employed/ highly qualified employee/ officer,1,none,yes,bad
+... >= 200 DM / salary assignments for at least 1 year,9,existing credits paid back duly till now,radio/television,745,... < 100 DM,1 <= ... < 4 years,3,male : married/widowed,none,2,real estate,28,none,own,1,unskilled - resident,1,none,yes,bad
+0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,2063,... < 100 DM,... < 1 year,4,male : married/widowed,none,3,"car or other, not in attribute Savings account/bonds",30,none,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,60,existing credits paid back duly till now,education,6288,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,4,unknown / no property,42,none,for free,1,skilled employee / official,1,none,yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),car (used),6842,unknown/ no savings account,1 <= ... < 4 years,2,male : married/widowed,none,4,building society savings agreement/ life insurance,46,none,own,2,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,car (new),3527,unknown/ no savings account,... < 1 year,2,male : married/widowed,none,3,building society savings agreement/ life insurance,45,none,own,1,management/ self-employed/ highly qualified employee/ officer,2,"yes, registered under the customers name",yes,good
+no checking account,10,existing credits paid back duly till now,car (new),1546,... < 100 DM,1 <= ... < 4 years,3,male : married/widowed,none,2,real estate,31,none,own,1,unskilled - resident,2,none,no,good
+no checking account,24,existing credits paid back duly till now,furniture/equipment,929,unknown/ no savings account,4 <= ... < 7 years,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",31,stores,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,4,critical account/ other credits existing (not at this bank),car (new),1455,... < 100 DM,4 <= ... < 7 years,2,male : married/widowed,none,1,real estate,42,none,own,3,unskilled - resident,2,none,yes,good
+... < 0 DM,15,existing credits paid back duly till now,furniture/equipment,1845,... < 100 DM,... < 1 year,4,male : married/widowed,guarantor,1,building society savings agreement/ life insurance,46,none,rent,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,48,no credits taken/ all credits paid back duly,car (new),8358,500 <= ... < 1000 DM,... < 1 year,1,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",30,none,own,2,skilled employee / official,1,none,yes,good
+... < 0 DM,24,all credits at this bank paid back duly,furniture/equipment,3349,500 <= ... < 1000 DM,... < 1 year,4,male : married/widowed,none,4,unknown / no property,30,none,for free,1,skilled employee / official,2,"yes, registered under the customers name",yes,bad
+no checking account,12,existing credits paid back duly till now,car (new),2859,unknown/ no savings account,unemployed,4,male : married/widowed,none,4,unknown / no property,38,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,18,existing credits paid back duly till now,furniture/equipment,1533,... < 100 DM,... < 1 year,4,male : married/widowed,co-applicant,1,building society savings agreement/ life insurance,43,none,own,1,unskilled - resident,2,none,yes,bad
+no checking account,24,existing credits paid back duly till now,radio/television,3621,100 <= ... < 500 DM,... >= 7 years,2,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",31,none,own,2,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,18,critical account/ other credits existing (not at this bank),business,3590,... < 100 DM,unemployed,3,male : married/widowed,none,3,"car or other, not in attribute Savings account/bonds",40,none,own,3,unemployed/ unskilled - non-resident,2,"yes, registered under the customers name",yes,good
+... < 0 DM,36,delay in paying off in the past,business,2145,... < 100 DM,4 <= ... < 7 years,2,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",24,none,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,24,existing credits paid back duly till now,car (used),4113,500 <= ... < 1000 DM,... < 1 year,3,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",28,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,36,existing credits paid back duly till now,furniture/equipment,10974,... < 100 DM,unemployed,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",26,none,own,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... < 0 DM,12,existing credits paid back duly till now,car (new),1893,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,guarantor,4,building society savings agreement/ life insurance,29,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,24,critical account/ other credits existing (not at this bank),radio/television,1231,... >= 1000 DM,... >= 7 years,4,male : married/widowed,none,4,building society savings agreement/ life insurance,57,none,rent,2,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,30,critical account/ other credits existing (not at this bank),radio/television,3656,unknown/ no savings account,... >= 7 years,4,male : married/widowed,none,4,building society savings agreement/ life insurance,49,stores,own,2,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,9,critical account/ other credits existing (not at this bank),radio/television,1154,... < 100 DM,... >= 7 years,2,male : married/widowed,none,4,real estate,37,none,own,3,unskilled - resident,1,none,yes,good
+... < 0 DM,28,existing credits paid back duly till now,car (new),4006,... < 100 DM,1 <= ... < 4 years,3,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",45,none,own,1,unskilled - resident,1,none,yes,bad
+0 <= ... < 200 DM,24,existing credits paid back duly till now,furniture/equipment,3069,100 <= ... < 500 DM,... >= 7 years,4,male : married/widowed,none,4,unknown / no property,30,none,for free,1,skilled employee / official,1,none,yes,good
+no checking account,6,critical account/ other credits existing (not at this bank),radio/television,1740,... < 100 DM,... >= 7 years,2,male : married/widowed,none,2,real estate,30,none,rent,2,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,21,delay in paying off in the past,car (new),2353,... < 100 DM,1 <= ... < 4 years,1,male : married/widowed,none,4,building society savings agreement/ life insurance,47,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,15,existing credits paid back duly till now,car (new),3556,unknown/ no savings account,1 <= ... < 4 years,3,male : married/widowed,none,2,unknown / no property,29,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,radio/television,2397,500 <= ... < 1000 DM,... >= 7 years,3,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",35,bank,own,2,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,6,existing credits paid back duly till now,repairs,454,... < 100 DM,... < 1 year,3,male : married/widowed,none,1,building society savings agreement/ life insurance,22,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,30,existing credits paid back duly till now,radio/television,1715,unknown/ no savings account,1 <= ... < 4 years,4,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",26,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,27,critical account/ other credits existing (not at this bank),radio/television,2520,500 <= ... < 1000 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,23,none,own,2,unskilled - resident,1,none,yes,bad
+no checking account,15,existing credits paid back duly till now,radio/television,3568,... < 100 DM,... >= 7 years,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",54,bank,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,42,existing credits paid back duly till now,radio/television,7166,unknown/ no savings account,4 <= ... < 7 years,2,male : married/widowed,none,4,building society savings agreement/ life insurance,29,none,rent,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... < 0 DM,11,critical account/ other credits existing (not at this bank),car (new),3939,... < 100 DM,1 <= ... < 4 years,1,male : married/widowed,none,2,real estate,40,none,own,2,unskilled - resident,2,none,yes,good
+0 <= ... < 200 DM,15,existing credits paid back duly till now,repairs,1514,100 <= ... < 500 DM,1 <= ... < 4 years,4,male : married/widowed,guarantor,2,real estate,22,none,own,1,skilled employee / official,1,none,yes,good
+no checking account,24,existing credits paid back duly till now,car (new),7393,... < 100 DM,1 <= ... < 4 years,1,male : married/widowed,none,4,building society savings agreement/ life insurance,43,none,own,1,unskilled - resident,2,none,yes,good
+... < 0 DM,24,all credits at this bank paid back duly,car (new),1193,... < 100 DM,unemployed,1,male : married/widowed,co-applicant,4,unknown / no property,29,none,rent,2,unemployed/ unskilled - non-resident,1,none,yes,bad
+... < 0 DM,60,existing credits paid back duly till now,business,7297,... < 100 DM,... >= 7 years,4,male : married/widowed,co-applicant,4,unknown / no property,36,none,rent,1,skilled employee / official,1,none,yes,bad
+no checking account,30,critical account/ other credits existing (not at this bank),radio/television,2831,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",33,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+... >= 200 DM / salary assignments for at least 1 year,24,existing credits paid back duly till now,radio/television,1258,500 <= ... < 1000 DM,1 <= ... < 4 years,3,male : married/widowed,none,3,"car or other, not in attribute Savings account/bonds",57,none,own,1,unskilled - resident,1,none,yes,good
+0 <= ... < 200 DM,6,existing credits paid back duly till now,radio/television,753,... < 100 DM,1 <= ... < 4 years,2,male : married/widowed,guarantor,3,real estate,64,none,own,1,skilled employee / official,1,none,yes,good
+0 <= ... < 200 DM,18,delay in paying off in the past,business,2427,unknown/ no savings account,... >= 7 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,42,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,24,delay in paying off in the past,car (new),2538,... < 100 DM,... >= 7 years,4,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",47,none,own,2,unskilled - resident,2,none,yes,bad
+0 <= ... < 200 DM,15,all credits at this bank paid back duly,car (new),1264,100 <= ... < 500 DM,1 <= ... < 4 years,2,male : married/widowed,none,2,building society savings agreement/ life insurance,25,none,rent,1,skilled employee / official,1,none,yes,bad
+0 <= ... < 200 DM,30,critical account/ other credits existing (not at this bank),furniture/equipment,8386,... < 100 DM,4 <= ... < 7 years,2,male : married/widowed,none,2,building society savings agreement/ life insurance,49,none,own,1,skilled employee / official,1,none,yes,bad
+no checking account,48,existing credits paid back duly till now,business,4844,... < 100 DM,unemployed,3,male : married/widowed,none,2,"car or other, not in attribute Savings account/bonds",33,bank,rent,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,bad
+... >= 200 DM / salary assignments for at least 1 year,21,existing credits paid back duly till now,car (new),2923,100 <= ... < 500 DM,1 <= ... < 4 years,1,male : married/widowed,none,1,"car or other, not in attribute Savings account/bonds",28,bank,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+... < 0 DM,36,existing credits paid back duly till now,car (used),8229,... < 100 DM,1 <= ... < 4 years,2,male : married/widowed,none,2,building society savings agreement/ life insurance,26,none,own,1,skilled employee / official,2,none,yes,bad
+no checking account,24,critical account/ other credits existing (not at this bank),furniture/equipment,2028,... < 100 DM,4 <= ... < 7 years,2,male : married/widowed,none,2,building society savings agreement/ life insurance,30,none,own,2,unskilled - resident,1,none,yes,good
+... < 0 DM,15,critical account/ other credits existing (not at this bank),furniture/equipment,1433,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,3,building society savings agreement/ life insurance,25,none,rent,2,skilled employee / official,1,none,yes,good
+... >= 200 DM / salary assignments for at least 1 year,42,no credits taken/ all credits paid back duly,business,6289,... < 100 DM,... < 1 year,2,male : married/widowed,none,1,building society savings agreement/ life insurance,33,none,own,2,skilled employee / official,1,none,yes,good
+no checking account,13,existing credits paid back duly till now,radio/television,1409,100 <= ... < 500 DM,unemployed,2,male : married/widowed,none,4,real estate,64,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,24,existing credits paid back duly till now,car (used),6579,... < 100 DM,unemployed,4,male : married/widowed,none,2,unknown / no property,29,none,for free,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+0 <= ... < 200 DM,24,critical account/ other credits existing (not at this bank),radio/television,1743,... < 100 DM,... >= 7 years,4,male : married/widowed,none,2,building society savings agreement/ life insurance,48,none,own,2,unskilled - resident,1,none,yes,good
+no checking account,12,critical account/ other credits existing (not at this bank),education,3565,unknown/ no savings account,... < 1 year,2,male : married/widowed,none,1,building society savings agreement/ life insurance,37,none,own,2,unskilled - resident,2,none,yes,good
+no checking account,15,all credits at this bank paid back duly,radio/television,1569,100 <= ... < 500 DM,... >= 7 years,4,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",34,bank,own,1,unskilled - resident,2,none,yes,good
+... < 0 DM,18,existing credits paid back duly till now,radio/television,1936,unknown/ no savings account,4 <= ... < 7 years,2,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",23,none,rent,2,unskilled - resident,1,none,yes,good
+... < 0 DM,36,existing credits paid back duly till now,furniture/equipment,3959,... < 100 DM,unemployed,4,male : married/widowed,none,3,building society savings agreement/ life insurance,30,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,car (new),2390,unknown/ no savings account,... >= 7 years,4,male : married/widowed,none,3,"car or other, not in attribute Savings account/bonds",50,none,own,1,skilled employee / official,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,furniture/equipment,1736,... < 100 DM,4 <= ... < 7 years,3,male : married/widowed,none,4,real estate,31,none,own,1,unskilled - resident,1,none,yes,good
+... < 0 DM,30,existing credits paid back duly till now,car (used),3857,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,4,building society savings agreement/ life insurance,40,none,own,1,management/ self-employed/ highly qualified employee/ officer,1,"yes, registered under the customers name",yes,good
+no checking account,12,existing credits paid back duly till now,radio/television,804,... < 100 DM,... >= 7 years,4,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",38,none,own,1,skilled employee / official,1,none,yes,good
+... < 0 DM,45,existing credits paid back duly till now,radio/television,1845,... < 100 DM,1 <= ... < 4 years,4,male : married/widowed,none,4,unknown / no property,23,none,for free,1,skilled employee / official,1,"yes, registered under the customers name",yes,bad
+0 <= ... < 200 DM,45,critical account/ other credits existing (not at this bank),car (used),4576,100 <= ... < 500 DM,unemployed,3,male : married/widowed,none,4,"car or other, not in attribute Savings account/bonds",27,none,own,1,skilled employee / official,1,none,yes,good
```

### Comparing `scorecardpy-0.1.9.2/scorecardpy/germancredit.py` & `scorecardpy-0.1.9.5/scorecardpy/germancredit.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,26 +33,26 @@
     # dat.dtypes
     '''
     DATA_FILE = pkg_resources.resource_filename('scorecardpy', 'data/germancredit.csv')
     
     dat = pd.read_csv(DATA_FILE)
     # categorical levels
     cate_levels = {
-            "status.of.existing.checking.account": ['... < 0 DM', '0 <= ... < 200 DM', '... >= 200 DM / salary assignments for at least 1 year', 'no checking account'], 
-            "credit.history": ["no credits taken/ all credits paid back duly", "all credits at this bank paid back duly", "existing credits paid back duly till now", "delay in paying off in the past", "critical account/ other credits existing (not at this bank)"], 
-            "savings.account.and.bonds": ["... < 100 DM", "100 <= ... < 500 DM", "500 <= ... < 1000 DM", "... >= 1000 DM", "unknown/ no savings account"],
-            "present.employment.since": ["unemployed", "... < 1 year", "1 <= ... < 4 years", "4 <= ... < 7 years", "... >= 7 years"], 
-            "personal.status.and.sex": ["male : divorced/separated", "female : divorced/separated/married", "male : single", "male : married/widowed", "female : single"], 
-            "other.debtors.or.guarantors": ["none", "co-applicant", "guarantor"], 
+            "status_of_existing_checking_account": ['... < 0 DM', '0 <= ... < 200 DM', '... >= 200 DM / salary assignments for at least 1 year', 'no checking account'], 
+            "credit_history": ["no credits taken/ all credits paid back duly", "all credits at this bank paid back duly", "existing credits paid back duly till now", "delay in paying off in the past", "critical account/ other credits existing (not at this bank)"], 
+            "savings_account_and_bonds": ["... < 100 DM", "100 <= ... < 500 DM", "500 <= ... < 1000 DM", "... >= 1000 DM", "unknown/ no savings account"],
+            "present_employment_since": ["unemployed", "... < 1 year", "1 <= ... < 4 years", "4 <= ... < 7 years", "... >= 7 years"], 
+            "personal_status_and_sex": ["male : divorced/separated", "female : divorced/separated/married", "male : single", "male : married/widowed", "female : single"], 
+            "other_debtors_or_guarantors": ["none", "co-applicant", "guarantor"], 
             "property": ["real estate",  "building society savings agreement/ life insurance",  "car or other, not in attribute Savings account/bonds",  "unknown / no property"],
-            "other.installment.plans": ["bank", "stores", "none"],
+            "other_installment_plans": ["bank", "stores", "none"],
             "housing": ["rent", "own", "for free"], 
             "job": ["unemployed/ unskilled - non-resident", "unskilled - resident", "skilled employee / official", "management/ self-employed/ highly qualified employee/ officer"],
             "telephone": ["none", "yes, registered under the customers name"], 
-            "foreign.worker": ["yes", "no"]}
+            "foreign_worker": ["yes", "no"]}
     # func of cate
     def cate_type(levels):
         return CategoricalDtype(categories=levels, ordered=True)
     # to cate
     for i in cate_levels.keys():
         dat[i] = dat[i].astype(cate_type(cate_levels[i]))
     # return
@@ -75,22 +75,22 @@
 
 ###### dtm ######
 # y
 y = dat['creditability']
 
 # x
 # numerical data
-xvar =  "credit.amount" # "foreign.worker # 'age.in.years' #'number.of.existing.credits.at.this.bank' # 
+xvar =  "credit_amount" # "foreign_worker # 'age_in_years' #'number_of_existing_credits_at_this_bank' # 
 x= dat1[xvar]
 spl_val = [2600, 9960, "6850%,%missing"]
 breaks = [2000, 4000, 6000]
 breaks = ['26%,%missing', 28, 35, 37]
 
 # categorical data
-xvar= 'purpose'#'housing' # "job" # "credit.amount"; #
+xvar= 'purpose'#'housing' # "job" # "credit_amount"; #
 x= dat[xvar] # pd.Categorical(dat[xvar], categories=['rent', 'own','for free']) 
 breaks = ["own", "for free%,%rent%,%missing"]
 breaks = ["own", "for free%,%rent"]
 
 
 dtm = pd.DataFrame({'y':y, 'variable':xvar, 'value':x})
 # dtm.value = None
```

### Comparing `scorecardpy-0.1.9.2/scorecardpy/info_ent_indx_gini.py` & `scorecardpy-0.1.9.5/scorecardpy/info_ent_indx_gini.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.2/scorecardpy/info_value.py` & `scorecardpy-0.1.9.5/scorecardpy/info_value.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.2/scorecardpy/one_hot.py` & `scorecardpy-0.1.9.5/scorecardpy/one_hot.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.2/scorecardpy/perf.py` & `scorecardpy-0.1.9.5/scorecardpy/perf.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.2/scorecardpy/scorecard.py` & `scorecardpy-0.1.9.5/scorecardpy/scorecard.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # -*- coding: utf-8 -*-
 
+import statsmodels.api as sm
+import pandas as pd
+
+def lr(dt, y, x):
+  # dty
+  dty = dt.loc[:,y] 
+  # dtx
+  dtx = dt.loc[:,x] 
+  dtx = sm.add_constant(dtx)
+  # logistic regression
+  lrfit = sm.GLM(
+    dty.astype(float), 
+    dtx.astype(float), 
+    family=sm.families.Binomial()
+  ).fit()
+  return lrfit
+
 import pandas as pd
 import numpy as np
 import re
 from .condition_fun import *
-from .woebin import woepoints_ply1
+from .woebin import woepoints_ply1, woebin_ply
 
 
 # coefficients in scorecard
 def ab(points0=600, odds0=1/19, pdo=50):
     # sigmoid function
     # library(ggplot2)
     # ggplot(data.frame(x = c(-5, 5)), aes(x)) + stat_function(fun = function(x) 1/(1+exp(-x)))
@@ -35,30 +52,33 @@
     b = pdo/np.log(2)
     a = points0 + b*np.log(odds0) #log(odds0/(1+odds0))
     
     return {'a':a, 'b':b}
 
 
 
-def scorecard(bins, model, xcolumns, points0=600, odds0=1/19, pdo=50, basepoints_eq0=False):
+def scorecard(bins, model, xcolumns, points0=600, odds0=1/19, pdo=50, basepoints_eq0=False, digits=0):
     '''
     Creating a Scorecard
     ------
     `scorecard` creates a scorecard based on the results from `woebin` 
-    and LogisticRegression of sklearn.linear_model
+    and LogisticRegression object from sklearn or statsmodels
     
     Params
     ------
     bins: Binning information generated from `woebin` function.
     model: A LogisticRegression model object.
     points0: Target points, default 600.
     odds0: Target odds, default 1/19. Odds = p/(1-p).
     pdo: Points to Double the Odds, default 50.
     basepoints_eq0: Logical, default is FALSE. If it is TRUE, the 
       basepoints will equally distribute to each variable.
+    digits: The number of digits after the decimal point for points 
+      calculation. Default 0.
+    
     
     Returns
     ------
     DataFrame
         scorecard dataframe
     
     Examples
@@ -105,38 +125,148 @@
     a = aabb['a'] 
     b = aabb['b']
     # odds = pred/(1-pred); score = a - b*log(odds)
     
     # bins # if (is.list(bins)) rbindlist(bins)
     if isinstance(bins, dict):
         bins = pd.concat(bins, ignore_index=True)
-    xs = [re.sub('_woe$', '', i) for i in xcolumns]
+  
     # coefficients
-    coef_df = pd.Series(model.coef_[0], index=np.array(xs))\
+    if str(type(model)) == "<class 'sklearn.linear_model._logistic.LogisticRegression'>":
+      coef_df = pd.Series(model.coef_[0], index=np.array([re.sub('_woe$', '', i) for i in xcolumns]))\
       .loc[lambda x: x != 0]#.reset_index(drop=True)
-    
+      coef_const = model.intercept_[0]
+    elif str(type(model)) == "<class 'statsmodels.genmod.generalized_linear_model.GLMResultsWrapper'>":
+      coef_df = model.summary2().tables[1].loc[:,'Coef.']
+      coef_const = coef_df['const']
+      coef_df = coef_df.drop('const')
+      coef_df.index = [re.sub('_woe$', '', i) for i in coef_df.index]
+      
     # scorecard
     len_x = len(coef_df)
-    basepoints = a - b*model.intercept_[0]
+    basepoints = a - b*coef_const
     card = {}
     if basepoints_eq0:
         card['basepoints'] = pd.DataFrame({'variable':"basepoints", 'bin':np.nan, 'points':0}, index=np.arange(1))
         for i in coef_df.index:
-            card[i] = bins.loc[bins['variable']==i,['variable', 'bin', 'woe']]\
-              .assign(points = lambda x: round(-b*x['woe']*coef_df[i] + basepoints/len_x))\
+            card[i] = bins.loc[bins['variable']==i, ['variable', 'bin', 'woe']]\
+              .assign(points = lambda x: round(-b*x['woe']*coef_df[i] + basepoints/len_x), ndigits=digits)\
               [["variable", "bin", "points"]]
     else:
-        card['basepoints'] = pd.DataFrame({'variable':"basepoints", 'bin':np.nan, 'points':round(basepoints)}, index=np.arange(1))
+        card['basepoints'] = pd.DataFrame({'variable':"basepoints", 'bin':np.nan, 'points':round(basepoints, ndigits=digits)}, index=np.arange(1))
         for i in coef_df.index:
-            card[i] = bins.loc[bins['variable']==i,['variable', 'bin', 'woe']]\
-              .assign(points = lambda x: round(-b*x['woe']*coef_df[i]))\
+            card[i] = bins.loc[bins['variable']==i, ['variable', 'bin', 'woe']]\
+              .assign(points = lambda x: round(-b*x['woe']*coef_df[i]), ndigits=digits)\
               [["variable", "bin", "points"]]
     return card
 
 
+def scorecard2(bins, dt, y, x=None, points0=600, odds0=1/19, pdo=50, basepoints_eq0=False, digits=0, 
+  return_prob = False, positive='bad|1', **kwargs): 
+    '''
+    Creating a Scorecard
+    ------
+    `scorecard2` creates a scorecard based on the results from woebin. It has 
+    the same function of scorecard, but without model object input.
+    
+    Params
+    ------
+    bins: Binning information generated from woebin function.
+    dt: A data frame with both x (predictor/feature) and y (response/label) variables.
+    y: Name of y variable.
+    x: Name of x variables. If it is None, then all variables in bins are used. Defaults to None.
+    points0: Target points, default 600.
+    odds0: Target odds, default 1/19. Odds = p/(1-p).
+    pdo: Points to Double the Odds, default 50.
+    basepoints_eq0: Logical, defaults to False. If it is True, the basepoints will equally distribute to each variable.
+    digits: The number of digits after the decimal point for points calculation. Default 0.
+    return_prob: Logical, defaults to False. If it is True, the predict probability will also return.
+    kwargs: Additional parameters.
+    
+    Returns
+    ------
+    A scorecard data frames
+    
+    Examples
+    ------
+    # load data
+    import scorecardpy as sc
+    dt = sc.germancredit()
+    
+    # filter variable via missing rate, iv, identical value rate
+    dtvf = sc.var_filter(dt, "creditability")
+    
+    # split into train and test
+    dtlst = sc.split_df(dtvf, y = 'creditability')
+    # binning
+    bins = sc.woebin(dtlst['train'], "creditability")
+    
+    # train only
+    ## create scorecard
+    card1 = sc.scorecard2(bins=bins, dt=dtlst['train'], y='creditability')
+    ## scorecard and predicted probability
+    cardprob1 = sc.scorecard2(bins=bins, dt=dtlst['train'], y='creditability', return_prob = True)
+    print(cardprob1.keys())
+    
+    # both train and test
+    ## create scorecard
+    card2 = sc.scorecard2(bins=bins, dt=dtlst, y='creditability')
+    ## scorecard and predicted probability
+    cardprob2 = sc.scorecard2(bins=bins, dt=dtlst, y='creditability', return_prob = True)
+    print(cardprob2.keys())
+    print(cardprob2['prob'].keys())
+    '''
+        
+  # data frame to list
+  if isinstance(dt, pd.DataFrame): dt = {'dat': dt}
+  # check y column
+  for i in dt.keys():
+    dt[i] = check_y(dt[i], y, positive)
+    
+  # dt0
+  dtfstkey = list(dt.keys())[0]
+  dt0 = dt[dtfstkey]
+
+  # bind bins
+  if isinstance(bins, dict): bins = pd.concat(bins, ignore_index=True)
+        
+  # check xs
+  x_bins = bins['variable'].unique()
+  if x is None: x = x_bins
+  x = x_variable(dt0,y,x)
+  x_woe = ['_'.join([i, 'woe']) for i in x]
+
+  # dt to woe
+  dt_woe = {}
+  for i in dt.keys():
+    dt_woe[i] = woebin_ply(dt[i], bins=bins, print_info=False, kwargs)
+  dt0_woe = dt_woe[dtfstkey]
+
+  # model
+  lrmodel = lr(dt0_woe, y=y, x=x_woe)
+
+  # scorecard
+  card = scorecard(bins = bins, model = lrmodel, xcolumns=x_woe, points0 = points0, odds0 = odds0, pdo = pdo, basepoints_eq0 = basepoints_eq0, digits = digits)
+  
+  # returns
+  if return_prob is True:
+    probdict = {}
+    for i in dt.keys():
+      dtx_woe = dt_woe[i].loc[:,x_woe] 
+      dtx_woe = sm.add_constant(dtx_woe)
+      probdict[i] = lrmodel.predict(dtx_woe)
+    rt = {
+      'card': card, 
+      'prob': probdict
+    }
+  else:
+    rt = card
+    
+  return rt
+
 
 def scorecard_ply(dt, card, only_total_score=True, print_step=0, replace_blank_na=True, var_kp = None):
     '''
     Score Transformation
     ------
     `scorecard_ply` calculates credit score using the results from `scorecard`.
```

### Comparing `scorecardpy-0.1.9.2/scorecardpy/split_df.py` & `scorecardpy-0.1.9.5/scorecardpy/split_df.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.2/scorecardpy/var_filter.py` & `scorecardpy-0.1.9.5/scorecardpy/var_filter.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.2/scorecardpy/woebin.py` & `scorecardpy-0.1.9.5/scorecardpy/woebin.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,28 +108,41 @@
             sv_df['value'] = sv_df['value'].astype(dtm['value'].dtypes)
             # sv_df['bin_chr'] = sv_df['bin_chr'].astype(dtm['value'].dtypes).astype(str)
             sv_df['bin_chr'] = np.where(
               np.isnan(sv_df['value']), sv_df['bin_chr'], 
               sv_df['value'].astype(dtm['value'].dtypes).astype(str))
             # sv_df = sv_df.assign(value = lambda x: x.value.astype(dtm['value'].dtypes))
         # dtm_sv & dtm
-        dtm_sv = pd.merge(dtm.fillna("missing"), sv_df[['value']].fillna("missing"), how='inner', on='value', right_index=True)
+        # dtm_sv = pd.merge(dtm.fillna("missing"), sv_df[['value']].fillna("missing"), how='inner', on='value', right_index=True)
+        if None in dtm.index.names and len(dtm.index.names)==1: 
+            dtm_index='index'
+        elif None in dtm.index.names and len(dtm.index.names)>1:
+            raise ValueError("multiindex's names contain Nonetype")
+        else:
+            dtm_index=dtm.index.names #update by ZK
+        
+        dtm_sv = pd.merge(
+          dtm.fillna("missing").reset_index(),
+          sv_df[['value']].fillna("missing"), 
+          how='inner', on='value'
+        ).set_index(dtm_index) #update by ZK
+
         dtm = dtm[~dtm.index.isin(dtm_sv.index)].reset_index() if len(dtm_sv.index) < len(dtm.index) else None
         # dtm_sv = dtm.query('value in {}'.format(sv_df['value'].tolist()))
         # dtm    = dtm.query('value not in {}'.format(sv_df['value'].tolist()))
         
         if dtm_sv.shape[0] == 0:
             return {'binning_sv':None, 'dtm':dtm}
         # binning_sv
         binning_sv = pd.merge(
-          dtm_sv.fillna('missing').groupby(['variable','value'])['y'].agg([n0, n1])\
+          dtm_sv.fillna('missing').groupby(['variable','value'], group_keys=False)['y'].agg([n0, n1])\
           .reset_index().rename(columns={'n0':'good','n1':'bad'}),
           sv_df.fillna('missing'), 
           on='value'
-        ).groupby(['variable', 'rowid', 'bin_chr']).agg({'bad':sum,'good':sum})\
+        ).groupby(['variable', 'rowid', 'bin_chr'], group_keys=False).agg({'bad':sum,'good':sum})\
         .reset_index().rename(columns={'bin_chr':'bin'})\
         .drop('rowid', axis=1)
     else:
         binning_sv = None
     # return
     return {'binning_sv':binning_sv, 'dtm':dtm}
     
@@ -141,15 +154,15 @@
         bin_list.remove('nan')
     binleft = set([re.match(r'\[(.+),(.+)\)', i).group(1) for i in bin_list]).difference(set(['-inf', 'inf']))
     binright = set([re.match(r'\[(.+),(.+)\)', i).group(2) for i in bin_list]).difference(set(['-inf', 'inf']))
     if binleft != binright:
         bstbrks = sorted(list(map(float, ['-inf'] + list(binright) + ['inf'])))
         labels = ['[{},{})'.format(bstbrks[i], bstbrks[i+1]) for i in range(len(bstbrks)-1)]
         dtm.loc[:,'bin'] = pd.cut(dtm['value'], bstbrks, right=False, labels=labels)
-        binning = dtm.groupby(['variable','bin'])['y'].agg([n0, n1])\
+        binning = dtm.groupby(['variable','bin'], group_keys=False)['y'].agg([n0, n1])\
           .reset_index().rename(columns={'n0':'good','n1':'bad'})
         # warnings.warn("The break points are modified into '[{}]'. There are empty bins based on the provided break points.".format(','.join(binright)))
         # binning
         # dtm['bin'] = dtm['bin'].astype(str)
     # return
     return binning
 
@@ -185,15 +198,15 @@
         bstbrks = ['-inf'] + list(set(bk_df.value.tolist()).difference(set([np.nan, '-inf', 'inf', 'Inf', '-Inf']))) + ['inf']
         bstbrks = sorted(list(map(float, bstbrks)))
         # cut
         labels = ['[{},{})'.format(bstbrks[i], bstbrks[i+1]) for i in range(len(bstbrks)-1)]
         dtm.loc[:,'bin'] = pd.cut(dtm['value'], bstbrks, right=False, labels=labels)
         dtm['bin'] = dtm['bin'].astype(str)
         
-        binning = dtm.groupby(['variable','bin'])['y'].agg([n0, n1])\
+        binning = dtm.groupby(['variable','bin'], group_keys=False)['y'].agg([n0, n1])\
           .reset_index().rename(columns={'n0':'good','n1':'bad'})
         # check empty bins for unmeric variable
         binning = check_empty_bins(dtm, binning)
         
         # sort bin
         binning = pd.merge(
           binning.assign(value=lambda x: [float(re.search(r"^\[(.*),(.*)\)", i).group(2)) if i != 'nan' else np.nan for i in binning['bin']] ),
@@ -208,15 +221,15 @@
               .reset_index()
     else:
         # merge binning with bk_df
         binning = pd.merge(
           dtm, 
           bk_df.assign(bin=lambda x: x.bin_chr),
           how='left', on='value'
-        ).fillna('missing').groupby(['variable', 'rowid', 'bin'])['y'].agg([n0,n1])\
+        ).fillna('missing').groupby(['variable', 'rowid', 'bin'], group_keys=False)['y'].agg([n0,n1])\
         .rename(columns={'n0':'good','n1':'bad'})\
         .reset_index().drop('rowid', axis=1)
     # return
     return {'binning_sv':binning_sv, 'binning':binning}
     
 
 # required in woebin2_init_bin # return pretty breakpoints
@@ -233,15 +246,15 @@
     Returns
     ------
     numpy.ndarray
         returns a breakpoints array
     '''
     # nicenumber
     def nicenumber(x):
-        exp = np.trunc(np.log10(abs(x)))
+        exp = np.floor(np.log10(abs(x)))
         f   = abs(x) / 10**exp
         if f < 1.5:
             nf = 1.
         elif f < 3.:
             nf = 2.
         elif f < 7.:
             nf = 5.
@@ -300,27 +313,27 @@
         brk = list(filter(lambda x: x>np.nanmin(xvalue) and x<=np.nanmax(xvalue), brk))
         brk = [float('-inf')] + sorted(brk) + [float('inf')]
         # initial binning datatable
         # cut
         labels = ['[{},{})'.format(brk[i], brk[i+1]) for i in range(len(brk)-1)]
         dtm.loc[:,'bin'] = pd.cut(dtm['value'], brk, right=False, labels=labels)#.astype(str)
         # init_bin
-        init_bin = dtm.groupby('bin')['y'].agg([n0, n1])\
+        init_bin = dtm.groupby('bin', group_keys=False)['y'].agg([n0, n1])\
         .reset_index().rename(columns={'n0':'good','n1':'bad'})
         # check empty bins for unmeric variable
         init_bin = check_empty_bins(dtm, init_bin)
         
         init_bin = init_bin.assign(
           variable = dtm['variable'].values[0],
           brkp = lambda x: [float(re.match('^\[(.*),.+', i).group(1)) for i in x['bin']],
           badprob = lambda x: x['bad']/(x['bad']+x['good'])
         )[['variable', 'bin', 'brkp', 'good', 'bad', 'badprob']]
     else: # other type variable
         # initial binning datatable
-        init_bin = dtm.groupby('value')['y'].agg([n0,n1])\
+        init_bin = dtm.groupby('value', group_keys=False)['y'].agg([n0,n1])\
         .rename(columns={'n0':'good','n1':'bad'})\
         .assign(
           variable = dtm['variable'].values[0],
           badprob = lambda x: x['bad']/(x['bad']+x['good'])
         ).reset_index()
         # order by badprob if is.character
         if dtm.value.dtype.name not in ['category', 'bool']:
@@ -341,16 +354,16 @@
         .query('(good==0) or (bad==0)')\
         .query('count == count.min()').iloc[0,]
         # set brkp to lead's or lag's
         shift_period = -1 if rm_brkp['merge_tolead'] else 1
         init_bin = init_bin.assign(brkp2  = lambda x: x['brkp'].shift(shift_period))\
         .assign(brkp = lambda x:np.where(x['brkp'] == rm_brkp['brkp'], x['brkp2'], x['brkp']))
         # groupby brkp
-        init_bin = init_bin.groupby('brkp').agg({
-          'variable':lambda x: np.unique(x),
+        init_bin = init_bin.groupby('brkp', group_keys=False).agg({
+          'variable':lambda x: np.unique(x)[0],
           'bin': lambda x: '%,%'.join(x),
           'good': sum,
           'bad': sum
         }).assign(badprob = lambda x: x['bad']/(x['good']+x['bad']))\
         .reset_index()
     # format init_bin
     if is_numeric_dtype(dtm['value']):
@@ -393,26 +406,26 @@
             # best break datatable
             labels = ['[{},{})'.format(bestbreaks_i[i], bestbreaks_i[i+1]) for i in range(len(bestbreaks_i)-1)]
             init_bin_all_breaks.loc[:,'bstbin'+str(i)] = pd.cut(init_bin_all_breaks['brkp'], bestbreaks_i, right=False, labels=labels)#.astype(str)
         # best break dt
         total_iv_all_brks = pd.melt(
           init_bin_all_breaks, id_vars=["variable", "good", "bad"], var_name='bstbin', 
           value_vars=['bstbin'+str(i) for i in breaks_set])\
-          .groupby(['variable', 'bstbin', 'value'])\
+          .groupby(['variable', 'bstbin', 'value'], group_keys=False)\
           .agg({'good':sum, 'bad':sum}).reset_index()\
           .assign(count=lambda x: x['good']+x['bad'])
           
-        total_iv_all_brks['count_distr'] = total_iv_all_brks.groupby(['variable', 'bstbin'])\
+        total_iv_all_brks['count_distr'] = total_iv_all_brks.groupby(['variable', 'bstbin'], group_keys=False)\
           ['count'].apply(lambda x: x/dtm_rows).reset_index(drop=True)
-        total_iv_all_brks['min_count_distr'] = total_iv_all_brks.groupby(['variable', 'bstbin'])\
+        total_iv_all_brks['min_count_distr'] = total_iv_all_brks.groupby(['variable', 'bstbin'], group_keys=False)\
           ['count_distr'].transform(lambda x: min(x))
           
         total_iv_all_brks = total_iv_all_brks\
           .assign(bstbin = lambda x: [float(re.sub('^bstbin', '', i)) for i in x['bstbin']] )\
-          .groupby(['variable','bstbin','min_count_distr'])\
+          .groupby(['variable','bstbin','min_count_distr'], group_keys=False)\
           .apply(lambda x: iv_01(x['good'], x['bad'])).reset_index(name='total_iv')
         # return 
         return total_iv_all_brks
     # binning add 1best break
     def binning_add_1bst(initial_binning, bestbreaks):
         if bestbreaks is None:
             bestbreaks_inf = [float('-inf'),float('inf')]
@@ -422,19 +435,19 @@
             bestbreaks_inf = [float('-inf')]+sorted(bestbreaks)+[float('inf')]
         
         labels = ['[{},{})'.format(bestbreaks_inf[i], bestbreaks_inf[i+1]) for i in range(len(bestbreaks_inf)-1)]
         binning_1bst_brk = initial_binning.assign(
           bstbin = lambda x: pd.cut(x['brkp'], bestbreaks_inf, right=False, labels=labels)
         )
         if is_numeric_dtype(dtm['value']):
-            binning_1bst_brk = binning_1bst_brk.groupby(['variable', 'bstbin'])\
+            binning_1bst_brk = binning_1bst_brk.groupby(['variable', 'bstbin'], group_keys=False)\
             .agg({'good':sum, 'bad':sum}).reset_index().assign(bin=lambda x: x['bstbin'])\
             [['bstbin', 'variable', 'bin', 'good', 'bad']]
         else:
-            binning_1bst_brk = binning_1bst_brk.groupby(['variable', 'bstbin'])\
+            binning_1bst_brk = binning_1bst_brk.groupby(['variable', 'bstbin'], group_keys=False)\
             .agg({'good':sum, 'bad':sum, 'bin':lambda x:'%,%'.join(x)}).reset_index()\
             [['bstbin', 'variable', 'bin', 'good', 'bad']]
         # format
         binning_1bst_brk['total_iv'] = iv_01(binning_1bst_brk.good, binning_1bst_brk.bad)
         binning_1bst_brk['bstbrkp'] = [float(re.match("^\[(.*),.+", i).group(1)) for i in binning_1bst_brk['bstbin']]
         # return
         return binning_1bst_brk
@@ -480,14 +493,16 @@
     dict
         returns a dict with initial binning and special_value binning
     '''
     # initial binning
     bin_list = woebin2_init_bin(dtm, init_count_distr=init_count_distr, breaks=breaks, spl_val=spl_val)
     initial_binning = bin_list['initial_binning']
     binning_sv = bin_list['binning_sv']
+    if initial_binning is None: # fix next condition npe
+        return {'binning_sv':binning_sv, 'binning':None}
     if len(initial_binning.index)==1: 
         return {'binning_sv':binning_sv, 'binning':initial_binning}
     # initialize parameters
     len_brks = len(initial_binning.index)
     bestbreaks = None
     IVt1 = IVt2 = 1e-10
     IVchg = 1 ## IV gain ratio
@@ -560,21 +575,21 @@
     # function to create a chisq column in initial_binning
     def add_chisq(initial_binning):
         chisq_df = pd.melt(initial_binning, 
           id_vars=["brkp", "variable", "bin"], value_vars=["good", "bad"],
           var_name='goodbad', value_name='a')\
         .sort_values(by=['goodbad', 'brkp']).reset_index(drop=True)
         ###
-        chisq_df['a_lag'] = chisq_df.groupby('goodbad')['a'].apply(lambda x: x.shift(1))#.reset_index(drop=True)
-        chisq_df['a_rowsum'] = chisq_df.groupby('brkp')['a'].transform(lambda x: sum(x))#.reset_index(drop=True)
-        chisq_df['a_lag_rowsum'] = chisq_df.groupby('brkp')['a_lag'].transform(lambda x: sum(x))#.reset_index(drop=True)
+        chisq_df['a_lag'] = chisq_df.groupby('goodbad', group_keys=False)['a'].apply(lambda x: x.shift(1))#.reset_index(drop=True)
+        chisq_df['a_rowsum'] = chisq_df.groupby('brkp', group_keys=False)['a'].transform(lambda x: sum(x))#.reset_index(drop=True)
+        chisq_df['a_lag_rowsum'] = chisq_df.groupby('brkp', group_keys=False)['a_lag'].transform(lambda x: sum(x))#.reset_index(drop=True)
         ###
         chisq_df = pd.merge(
           chisq_df.assign(a_colsum = lambda df: df.a+df.a_lag), 
-          chisq_df.groupby('brkp').apply(lambda df: sum(df.a+df.a_lag)).reset_index(name='a_sum'))\
+          chisq_df.groupby('brkp', group_keys=False).apply(lambda df: sum(df.a+df.a_lag)).reset_index(name='a_sum'))\
         .assign(
           e = lambda df: df.a_rowsum*df.a_colsum/df.a_sum,
           e_lag = lambda df: df.a_lag_rowsum*df.a_colsum/df.a_sum
         ).assign(
           ae = lambda df: (df.a-df.e)**2/df.e + (df.a_lag-df.e_lag)**2/df.e_lag
         ).groupby('brkp').apply(lambda x: sum(x.ae)).reset_index(name='chisq')
         # return
@@ -618,15 +633,15 @@
         else:
             break
         # set brkp to lead's or lag's
         shift_period = -1 if rm_brkp['merge_tolead'] else 1
         binning_chisq = binning_chisq.assign(brkp2  = lambda x: x['brkp'].shift(shift_period))\
         .assign(brkp = lambda x:np.where(x['brkp'] == rm_brkp['brkp'], x['brkp2'], x['brkp']))
         # groupby brkp
-        binning_chisq = binning_chisq.groupby('brkp').agg({
+        binning_chisq = binning_chisq.groupby('brkp', group_keys=False).agg({
           'variable':lambda x:np.unique(x),
           'bin': lambda x: '%,%'.join(x),
           'good': sum,
           'bad': sum
         }).assign(badprob = lambda x: x['bad']/(x['good']+x['bad']))\
         .reset_index()
         # update
@@ -746,15 +761,15 @@
       'not_numeric': [not is_numeric_dtype(dt[i]) for i in xs_all]
     })
     
     # breakslist of bins
     bins_breakslist = bins[~bins['breaks'].isin(["-inf","inf","missing"]) & ~bins['is_special_values']]
     bins_breakslist = pd.merge(bins_breakslist[['variable', 'breaks']], vars_class, how='left', on='variable')
     bins_breakslist.loc[bins_breakslist['not_numeric'], 'breaks'] = '\''+bins_breakslist.loc[bins_breakslist['not_numeric'], 'breaks']+'\''
-    bins_breakslist = bins_breakslist.groupby('variable')['breaks'].agg(lambda x: ','.join(x))
+    bins_breakslist = bins_breakslist.groupby('variable', group_keys=False)['breaks'].agg(lambda x: ','.join(x))
     
     if to_string:
         bins_breakslist = "breaks_list={\n"+', \n'.join('\''+bins_breakslist.index[i]+'\': ['+bins_breakslist[i]+']' for i in np.arange(len(bins_breakslist)))+"}"
         if save_string is not None:
             brk_lst_name = '{}_{}.py'.format(save_string, time.strftime('%Y%m%d_%H%M%S', time.localtime(time.time())))
             with open(brk_lst_name, 'w') as f:
                 f.write(bins_breakslist)
@@ -837,36 +852,36 @@
     
     # load data
     dat = sc.germancredit()
     
     # Example I
     # binning of two variables in germancredit dataset
     bins_2var = sc.woebin(dat, y = "creditability", 
-      x = ["credit.amount", "purpose"])
+      x = ["credit_amount", "purpose"])
     
     # Example II
     # binning of the germancredit dataset
     bins_germ = sc.woebin(dat, y = "creditability")
     
     # Example III
     # customizing the breakpoints of binning
     dat2 = pd.DataFrame({'creditability':['good','bad']}).sample(50, replace=True)
     dat_nan = pd.concat([dat, dat2], ignore_index=True)
     
     breaks_list = {
-      'age.in.years': [26, 35, 37, "Inf%,%missing"],
+      'age_in_years': [26, 35, 37, "Inf%,%missing"],
       'housing': ["own", "for free%,%rent"]
     }
     special_values = {
-      'credit.amount': [2600, 9960, "6850%,%missing"],
+      'credit_amount': [2600, 9960, "6850%,%missing"],
       'purpose': ["education", "others%,%missing"]
     }
     
     bins_cus_brk = sc.woebin(dat_nan, y="creditability",
-      x=["age.in.years","credit.amount","housing","purpose"],
+      x=["age_in_years","credit_amount","housing","purpose"],
       breaks_list=breaks_list, special_values=special_values)
     '''
     # start time
     start_time = time.time()
     
     # arguments
     ## print_info
@@ -1025,15 +1040,22 @@
         labels = ['[{},{})'.format(breaks_binx_other[i], breaks_binx_other[i+1]) for i in range(len(breaks_binx_other)-1)]
         
         dtx = dtx.assign(xi_bin = lambda x: pd.cut(x[x_i], breaks_binx_other, right=False, labels=labels))\
           .assign(xi_bin = lambda x: [i if (i != i) else str(i) for i in x['xi_bin']])
         # dtx.loc[:,'xi_bin'] = pd.cut(dtx[x_i], breaks_binx_other, right=False, labels=labels)
         # dtx.loc[:,'xi_bin'] = np.where(pd.isnull(dtx['xi_bin']), dtx['xi_bin'], dtx['xi_bin'].astype(str))
         #
-        mask = dtx[x_i].isin(binx_sv['V1'])
+        # mask = dtx[x_i].isin(binx_sv['V1'])
+        try:
+            # when binx_sv['V1'] is not int then cast type
+            mask = dtx[x_i].isin(binx_sv['V1'].astype('int'))
+        except:
+            # if can not cast then use as is
+            mask = dtx[x_i].isin(binx_sv['V1'])
+
         dtx.loc[mask,'xi_bin'] = dtx.loc[mask, x_i].astype(str)
         dtx = dtx[['xi_bin']].rename(columns={'xi_bin':x_i})
     ## to charcarter, na to missing
     if not is_string_dtype(dtx[x_i]):
         dtx.loc[:,x_i] = dtx.loc[:,x_i].astype(str).replace('nan', 'missing')
     # dtx.loc[:,x_i] = np.where(pd.isnull(dtx[x_i]), dtx[x_i], dtx[x_i].astype(str))
     dtx = dtx.replace(np.nan, 'missing').assign(rowid = dtx.index).sort_values('rowid')
@@ -1275,23 +1297,23 @@
     if isinstance(bins, dict):
         bins = pd.concat(bins, ignore_index=True)
     # good bad distr
     def gb_distr(binx):
         binx['good_distr'] = binx['good']/sum(binx['count'])
         binx['bad_distr'] = binx['bad']/sum(binx['count'])
         return binx
-    bins = bins.groupby('variable').apply(gb_distr)
+    bins = bins.groupby('variable', group_keys=False).apply(gb_distr)
     # x variable names
     if xs is None: xs = bins['variable'].unique()
     # plot export
     plotlist = {}
     for i in xs:
-        binx = bins[bins['variable'] == i].reset_index()
+        binx = bins[bins['variable'] == i].reset_index(drop=True)
         plotlist[i] = plot_bin(binx, title, show_iv)
-    return plotlist
+    return plotlist 
 
 
 
 # print basic information in woebin_adj
 def woebin_adj_print_basic_info(i, xs, bins, dt, bins_breakslist):
     '''
     print basic information of woebinnig in adjusting process
@@ -1410,18 +1432,18 @@
     if isinstance(bins, dict):
         bins = pd.concat(bins, ignore_index=True)
     # x variables
     xs_all = bins['variable'].unique()
     # adjust all variables
     if not adj_all_var:
         bins2 = bins.loc[~((bins['bin'] == 'missing') & (bins['count_distr'] >= count_distr_limit))].reset_index(drop=True)
-        bins2['badprob2'] = bins2.groupby('variable').apply(lambda x: x['badprob'].shift(1)).reset_index(drop=True)
+        bins2['badprob2'] = bins2.groupby('variable', group_keys=False).apply(lambda x: x['badprob'].shift(1)).reset_index(drop=True)
         bins2 = bins2.dropna(subset=['badprob2']).reset_index(drop=True)
         bins2 = bins2.assign(badprob_trend = lambda x: x.badprob >= x.badprob2)
-        xs_adj = bins2.groupby('variable')['badprob_trend'].nunique()
+        xs_adj = bins2.groupby('variable', group_keys=False)['badprob_trend'].nunique()
         xs_adj = xs_adj[xs_adj>1].index
     else:
         xs_adj = xs_all
     # length of adjusting variables
     xs_len = len(xs_adj)
     # special_values
     special_values = check_special_values(special_values, xs_adj)
@@ -1434,19 +1456,23 @@
         breaks_list = "{"+', '.join('\''+bins_breakslist.index[i]+'\': ['+bins_breakslist[i]+']' for i in np.arange(len(bins_breakslist)))+"}"
         return breaks_list
     # else 
     def menu(i, xs_len, x_i):
         print('>>> Adjust breaks for ({}/{}) {}?'.format(i, xs_len, x_i))
         print('1: next \n2: yes \n3: back')
         adj_brk = input("Selection: ")
-        adj_brk = int(adj_brk)
-        if adj_brk not in [0,1,2,3]:
-            warnings.warn('Enter an item from the menu, or 0 to exit.')
-            adj_brk = input("Selection: ")
-            adj_brk = int(adj_brk)
+        while isinstance(adj_brk,str):
+            if str(adj_brk).isdigit():
+                adj_brk = int(adj_brk)
+                if adj_brk not in [0,1,2,3]:
+                    warnings.warn('Enter an item from the menu, or 0 to exit.')               
+                    adj_brk = input("Selection: ")  
+            else: 
+                print('Input could not be converted to digit.')
+                adj_brk = input("Selection: ") #update by ZK 
         return adj_brk
         
     # init param
     i = 1
     breaks_list = None
     while i <= xs_len:
         breaks = stop_limit = None
```

### Comparing `scorecardpy-0.1.9.2/scorecardpy.egg-info/PKG-INFO` & `scorecardpy-0.1.9.5/scorecardpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,120 @@
 Metadata-Version: 2.1
 Name: scorecardpy
-Version: 0.1.9.2
+Version: 0.1.9.5
 Summary: Credit Risk Scorecard
 Home-page: http://github.com/shichenxie/scorecardpy
 Author: Shichen Xie
 Author-email: xie@shichen.name
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/shichenxie/scorecardpy/issues
 Project-URL: Source, https://github.com/shichenxie/scorecardpy/
-Description: # scorecardpy
-        
-        [![PyPI version](https://img.shields.io/pypi/pyversions/scorecardpy.svg)](https://pypi.python.org/pypi/scorecardpy)
-        [![PyPI release](https://img.shields.io/pypi/v/scorecardpy.svg)](https://pypi.python.org/pypi/scorecardpy)
-        [![Downloads](http://pepy.tech/badge/scorecardpy)](http://pepy.tech/project/scorecardpy)
-        [![Downloads](https://pepy.tech/badge/scorecardpy/month)](https://pepy.tech/project/scorecardpy/month)
-        
-        
-        This package is python version of R package [scorecard](https://github.com/ShichenXie/scorecard). 
-        Its goal is to make the development of traditional credit risk scorecard model easier and efficient by providing functions for some common tasks. 
-        - data partition (`split_df`)
-        - variable selection (`iv`, `var_filter`)
-        - weight of evidence (woe) binning (`woebin`, `woebin_plot`, `woebin_adj`, `woebin_ply`)
-        - scorecard scaling (`scorecard`, `scorecard_ply`)
-        - performance evaluation (`perf_eva`, `perf_psi`)
-        
-        ## Installation
-        
-        - Install the release version of `scorecardpy` from [PYPI](https://pypi.org/project/scorecardpy/) with:
-        ```
-        pip install scorecardpy
-        ```
-        
-        - Install the latest version of `scorecardpy` from [github](https://github.com/shichenxie/scorecardpy) with:
-        ```
-        pip install git+git://github.com/shichenxie/scorecardpy.git
-        ```
-        
-        ## Example
-        
-        This is a basic example which shows you how to develop a common credit risk scorecard:
-        
-        ``` python
-        # Traditional Credit Scoring Using Logistic Regression
-        import scorecardpy as sc
-        
-        # data prepare ------
-        # load germancredit data
-        dat = sc.germancredit()
-        
-        # filter variable via missing rate, iv, identical value rate
-        dt_s = sc.var_filter(dat, y="creditability")
-        
-        # breaking dt into train and test
-        train, test = sc.split_df(dt_s, 'creditability').values()
-        
-        # woe binning ------
-        bins = sc.woebin(dt_s, y="creditability")
-        # sc.woebin_plot(bins)
-        
-        # binning adjustment
-        # # adjust breaks interactively
-        # breaks_adj = sc.woebin_adj(dt_s, "creditability", bins) 
-        # # or specify breaks manually
-        breaks_adj = {
-            'age.in.years': [26, 35, 40],
-            'other.debtors.or.guarantors': ["none", "co-applicant%,%guarantor"]
-        }
-        bins_adj = sc.woebin(dt_s, y="creditability", breaks_list=breaks_adj)
-        
-        # converting train and test into woe values
-        train_woe = sc.woebin_ply(train, bins_adj)
-        test_woe = sc.woebin_ply(test, bins_adj)
-        
-        y_train = train_woe.loc[:,'creditability']
-        X_train = train_woe.loc[:,train_woe.columns != 'creditability']
-        y_test = test_woe.loc[:,'creditability']
-        X_test = test_woe.loc[:,train_woe.columns != 'creditability']
-        
-        # logistic regression ------
-        from sklearn.linear_model import LogisticRegression
-        lr = LogisticRegression(penalty='l1', C=0.9, solver='saga', n_jobs=-1)
-        lr.fit(X_train, y_train)
-        # lr.coef_
-        # lr.intercept_
-        
-        # predicted proability
-        train_pred = lr.predict_proba(X_train)[:,1]
-        test_pred = lr.predict_proba(X_test)[:,1]
-        
-        # performance ks & roc ------
-        train_perf = sc.perf_eva(y_train, train_pred, title = "train")
-        test_perf = sc.perf_eva(y_test, test_pred, title = "test")
-        
-        # score ------
-        card = sc.scorecard(bins_adj, lr, X_train.columns)
-        # credit score
-        train_score = sc.scorecard_ply(train, card, print_step=0)
-        test_score = sc.scorecard_ply(test, card, print_step=0)
-        
-        # psi
-        sc.perf_psi(
-          score = {'train':train_score, 'test':test_score},
-          label = {'train':y_train, 'test':y_test}
-        )
-        ```
-        
 Keywords: credit scorecard,woe binning,performace evaluation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# scorecardpy
+
+[![PyPI version](https://img.shields.io/pypi/pyversions/scorecardpy.svg)](https://pypi.python.org/pypi/scorecardpy)
+[![PyPI release](https://img.shields.io/pypi/v/scorecardpy.svg)](https://pypi.python.org/pypi/scorecardpy)
+[![Downloads](http://pepy.tech/badge/scorecardpy)](http://pepy.tech/project/scorecardpy)
+[![Downloads](https://pepy.tech/badge/scorecardpy/month)](https://pepy.tech/project/scorecardpy/month)
+
+
+This package is python version of R package [scorecard](https://github.com/ShichenXie/scorecard). 
+Its goal is to make the development of traditional credit risk scorecard model easier and efficient by providing functions for some common tasks. 
+- data partition (`split_df`)
+- variable selection (`iv`, `var_filter`)
+- weight of evidence (woe) binning (`woebin`, `woebin_plot`, `woebin_adj`, `woebin_ply`)
+- scorecard scaling (`scorecard`, `scorecard_ply`)
+- performance evaluation (`perf_eva`, `perf_psi`)
+
+## Installation
+
+- Install the release version of `scorecardpy` from [PYPI](https://pypi.org/project/scorecardpy/) with:
+```
+pip install scorecardpy
+```
+
+- Install the latest version of `scorecardpy` from [github](https://github.com/shichenxie/scorecardpy) with:
+```
+pip install git+git://github.com/shichenxie/scorecardpy.git
+```
+
+## Example
+
+This is a basic example which shows you how to develop a common credit risk scorecard:
+
+``` python
+# Traditional Credit Scoring Using Logistic Regression
+import scorecardpy as sc
+
+# data prepare ------
+# load germancredit data
+dat = sc.germancredit()
+
+# filter variable via missing rate, iv, identical value rate
+dt_s = sc.var_filter(dat, y="creditability")
+
+# breaking dt into train and test
+train, test = sc.split_df(dt_s, 'creditability').values()
+
+# woe binning ------
+bins = sc.woebin(dt_s, y="creditability")
+# sc.woebin_plot(bins)
+
+# binning adjustment
+# # adjust breaks interactively
+# breaks_adj = sc.woebin_adj(dt_s, "creditability", bins) 
+# # or specify breaks manually
+breaks_adj = {
+    'age.in.years': [26, 35, 40],
+    'other.debtors.or.guarantors': ["none", "co-applicant%,%guarantor"]
+}
+bins_adj = sc.woebin(dt_s, y="creditability", breaks_list=breaks_adj)
+
+# converting train and test into woe values
+train_woe = sc.woebin_ply(train, bins_adj)
+test_woe = sc.woebin_ply(test, bins_adj)
+
+y_train = train_woe.loc[:,'creditability']
+X_train = train_woe.loc[:,train_woe.columns != 'creditability']
+y_test = test_woe.loc[:,'creditability']
+X_test = test_woe.loc[:,train_woe.columns != 'creditability']
+
+# logistic regression ------
+from sklearn.linear_model import LogisticRegression
+lr = LogisticRegression(penalty='l1', C=0.9, solver='saga', n_jobs=-1)
+lr.fit(X_train, y_train)
+# lr.coef_
+# lr.intercept_
+
+# predicted proability
+train_pred = lr.predict_proba(X_train)[:,1]
+test_pred = lr.predict_proba(X_test)[:,1]
+
+# performance ks & roc ------
+train_perf = sc.perf_eva(y_train, train_pred, title = "train")
+test_perf = sc.perf_eva(y_test, test_pred, title = "test")
+
+# score ------
+card = sc.scorecard(bins_adj, lr, X_train.columns)
+# credit score
+train_score = sc.scorecard_ply(train, card, print_step=0)
+test_score = sc.scorecard_ply(test, card, print_step=0)
+
+# psi
+sc.perf_psi(
+  score = {'train':train_score, 'test':test_score},
+  label = {'train':y_train, 'test':y_test}
+)
+```
```

### Comparing `scorecardpy-0.1.9.2/scorecardpy.egg-info/SOURCES.txt` & `scorecardpy-0.1.9.5/scorecardpy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 scorecardpy/info_ent_indx_gini.py
 scorecardpy/info_value.py
 scorecardpy/one_hot.py
 scorecardpy/perf.py
 scorecardpy/scorecard.py
 scorecardpy/split_df.py
 scorecardpy/var_filter.py
+scorecardpy/vif.py
 scorecardpy/woebin.py
 scorecardpy.egg-info/PKG-INFO
 scorecardpy.egg-info/SOURCES.txt
 scorecardpy.egg-info/dependency_links.txt
 scorecardpy.egg-info/requires.txt
 scorecardpy.egg-info/top_level.txt
 scorecardpy/data/germancredit.csv
```

### Comparing `scorecardpy-0.1.9.2/setup.py` & `scorecardpy-0.1.9.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """A setuptools based setup module.
 See:
-https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 
 https://python-packaging.readthedocs.io/
 https://packaging.python.org/tutorials/distributing-packages/
 """
 
 # Always prefer setuptools over distutils
@@ -24,14 +23,15 @@
 # Get the version from __init__
 with open(path.join(here, 'scorecardpy/__init__.py'), encoding='utf-8') as f:
     __version__ = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read()).group(1)
 
 setup(
     name='scorecardpy',  # Required
     version=__version__,  # Required
+    package_dir={'scorecardpy':'scorecardpy'},
     description='Credit Risk Scorecard',  # Required
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='http://github.com/shichenxie/scorecardpy',  # Optional
     author='Shichen Xie',  # Optional
     author_email='xie@shichen.name',  # Optional
     classifiers=[  # Optional
@@ -51,18 +51,21 @@
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10'
     ],
     keywords='credit scorecard, woe binning, performace evaluation',  # Optional
     packages=['scorecardpy'],  # Required
-    install_requires=['numpy','pandas>=0.25.0','matplotlib','scikit-learn>=0.19.1'],  # Optional
+    install_requires=['numpy','pandas>=1.0.0','matplotlib','scikit-learn>=0.19.1', 'statsmodels', 'patsy'],  # Optional
     package_data={'scorecardpy': ['data/*.csv']},
     # data_files=[('scorecardpy': ['data/*.csv'])],  # Optional
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/shichenxie/scorecardpy/issues',
         'Source': 'https://github.com/shichenxie/scorecardpy/',
     },
 )
```

