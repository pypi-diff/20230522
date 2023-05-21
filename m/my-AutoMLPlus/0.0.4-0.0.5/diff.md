# Comparing `tmp/my_AutoMLPlus-0.0.4.tar.gz` & `tmp/my_AutoMLPlus-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_AutoMLPlus-0.0.4.tar", last modified: Sun May 21 23:42:25 2023, max compression
+gzip compressed data, was "my_AutoMLPlus-0.0.5.tar", last modified: Sun May 21 23:48:03 2023, max compression
```

## Comparing `my_AutoMLPlus-0.0.4.tar` & `my_AutoMLPlus-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:42:25.622402 my_AutoMLPlus-0.0.4/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:42:25.622402 my_AutoMLPlus-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-21 23:42:25.607058 my_AutoMLPlus-0.0.4/my_AutoMLPlus/
--rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus/__init__.py
--rw-rw-rw-   0        0        0     6599 2023-05-21 18:47:16.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus/data_preprocessing.py
--rw-rw-rw-   0        0        0     2190 2023-05-21 23:41:49.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus/ml_pipeline.py
--rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus/predictive_models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:42:25.621402 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:42:25.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-21 23:42:25.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:42:25.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 23:42:25.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 23:42:25.624429 my_AutoMLPlus-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      317 2023-05-21 23:42:11.000000 my_AutoMLPlus-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:48:03.508232 my_AutoMLPlus-0.0.5/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:48:03.508232 my_AutoMLPlus-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-21 23:48:03.493116 my_AutoMLPlus-0.0.5/my_AutoMLPlus/
+-rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus/__init__.py
+-rw-rw-rw-   0        0        0     6650 2023-05-21 23:47:15.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus/data_preprocessing.py
+-rw-rw-rw-   0        0        0     2272 2023-05-21 23:47:11.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus/ml_pipeline.py
+-rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus/predictive_models.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:48:03.506240 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:48:03.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-21 23:48:03.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 23:48:03.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 23:48:03.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 23:48:03.510227 my_AutoMLPlus-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      317 2023-05-21 23:47:54.000000 my_AutoMLPlus-0.0.5/setup.py
```

### Comparing `my_AutoMLPlus-0.0.4/my_AutoMLPlus/data_preprocessing.py` & `my_AutoMLPlus-0.0.5/my_AutoMLPlus/data_preprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from sklearn.impute import SimpleImputer
 from sklearn.feature_selection import SelectKBest, f_regression, VarianceThreshold
 from sklearn.model_selection import GridSearchCV
 import pandas as pd
 import numpy as np
 from sklearn.model_selection import train_test_split
 from sklearn.feature_selection import RFECV
+from sklearn.linear_model import LinearRegression
 
 class LabelEncoderWrapper:
     def __init__(self):
         self.encoder_dict = defaultdict(LabelEncoder)
 
     def fit_transform(self, X):
         # Применение LabelEncoder к каждому объектному столбцу
```

### Comparing `my_AutoMLPlus-0.0.4/my_AutoMLPlus/ml_pipeline.py` & `my_AutoMLPlus-0.0.5/my_AutoMLPlus/ml_pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 from my_AutoMLPlus.data_preprocessing import DataFramePreprocessor
 from my_AutoMLPlus.predictive_models import ElasticNetModel
 from my_AutoMLPlus.predictive_models import RandomForestRegressorModel
 from my_AutoMLPlus.predictive_models import GradientBoostingRegressorModel
 from my_AutoMLPlus.predictive_models import LinearRegressionModel
 
+import warnings
+
+warnings.filterwarnings('ignore', message="Scoring failed")
+
 class MyAutoML:
     def __init__(self, data: pd.DataFrame, target: str):
         self.data = data
         self.target = target
 
     def _preprocess_data(self):
         # Обработка данных
```

### Comparing `my_AutoMLPlus-0.0.4/my_AutoMLPlus/predictive_models.py` & `my_AutoMLPlus-0.0.5/my_AutoMLPlus/predictive_models.py`

 * *Files identical despite different names*

