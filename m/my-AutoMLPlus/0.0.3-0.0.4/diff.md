# Comparing `tmp/my_AutoMLPlus-0.0.3.tar.gz` & `tmp/my_AutoMLPlus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_AutoMLPlus-0.0.3.tar", last modified: Sun May 21 23:34:47 2023, max compression
+gzip compressed data, was "my_AutoMLPlus-0.0.4.tar", last modified: Sun May 21 23:42:25 2023, max compression
```

## Comparing `my_AutoMLPlus-0.0.3.tar` & `my_AutoMLPlus-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:34:47.778810 my_AutoMLPlus-0.0.3/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:34:47.778810 my_AutoMLPlus-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-21 23:34:47.764669 my_AutoMLPlus-0.0.3/my_AutoMLPlus/
--rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus/__init__.py
--rw-rw-rw-   0        0        0     6599 2023-05-21 18:47:16.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus/data_preprocessing.py
--rw-rw-rw-   0        0        0     2125 2023-05-21 23:33:44.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus/ml_pipeline.py
--rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus/predictive_models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:34:47.777605 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:34:47.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-21 23:34:47.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:34:47.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 23:34:47.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 23:34:47.780805 my_AutoMLPlus-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      317 2023-05-21 23:34:11.000000 my_AutoMLPlus-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:42:25.622402 my_AutoMLPlus-0.0.4/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:42:25.622402 my_AutoMLPlus-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-21 23:42:25.607058 my_AutoMLPlus-0.0.4/my_AutoMLPlus/
+-rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus/__init__.py
+-rw-rw-rw-   0        0        0     6599 2023-05-21 18:47:16.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus/data_preprocessing.py
+-rw-rw-rw-   0        0        0     2190 2023-05-21 23:41:49.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus/ml_pipeline.py
+-rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus/predictive_models.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:42:25.621402 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:42:25.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-21 23:42:25.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 23:42:25.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 23:42:25.000000 my_AutoMLPlus-0.0.4/my_AutoMLPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 23:42:25.624429 my_AutoMLPlus-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      317 2023-05-21 23:42:11.000000 my_AutoMLPlus-0.0.4/setup.py
```

### Comparing `my_AutoMLPlus-0.0.3/my_AutoMLPlus/data_preprocessing.py` & `my_AutoMLPlus-0.0.4/my_AutoMLPlus/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `my_AutoMLPlus-0.0.3/my_AutoMLPlus/ml_pipeline.py` & `my_AutoMLPlus-0.0.4/my_AutoMLPlus/ml_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pandas as pd
 from nbimporter import NotebookLoader
 from sklearn.preprocessing import StandardScaler
 from sklearn.impute import SimpleImputer
 from sklearn.metrics import r2_score
 
-from .data_preprocessing import DataFramePreprocessor
-from .predictive_models import ElasticNetModel
-from .predictive_models import RandomForestRegressorModel
-from .predictive_models import GradientBoostingRegressorModel
-from .predictive_models import LinearRegressionModel
+from my_AutoMLPlus.data_preprocessing import DataFramePreprocessor
+from my_AutoMLPlus.predictive_models import ElasticNetModel
+from my_AutoMLPlus.predictive_models import RandomForestRegressorModel
+from my_AutoMLPlus.predictive_models import GradientBoostingRegressorModel
+from my_AutoMLPlus.predictive_models import LinearRegressionModel
 
 class MyAutoML:
     def __init__(self, data: pd.DataFrame, target: str):
         self.data = data
         self.target = target
 
     def _preprocess_data(self):
```

### Comparing `my_AutoMLPlus-0.0.3/my_AutoMLPlus/predictive_models.py` & `my_AutoMLPlus-0.0.4/my_AutoMLPlus/predictive_models.py`

 * *Files identical despite different names*

