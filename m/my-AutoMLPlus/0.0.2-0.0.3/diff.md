# Comparing `tmp/my_AutoMLPlus-0.0.2.tar.gz` & `tmp/my_AutoMLPlus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_AutoMLPlus-0.0.2.tar", last modified: Sun May 21 23:26:28 2023, max compression
+gzip compressed data, was "my_AutoMLPlus-0.0.3.tar", last modified: Sun May 21 23:34:47 2023, max compression
```

## Comparing `my_AutoMLPlus-0.0.2.tar` & `my_AutoMLPlus-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:26:28.976545 my_AutoMLPlus-0.0.2/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:26:28.976804 my_AutoMLPlus-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-21 23:26:28.961387 my_AutoMLPlus-0.0.2/my_AutoMLPlus/
--rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus/__init__.py
--rw-rw-rw-   0        0        0     6599 2023-05-21 18:47:16.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus/data_preprocessing.py
--rw-rw-rw-   0        0        0     1844 2023-05-21 23:21:41.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus/ml_pipeline.py
--rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus/predictive_models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:26:28.975490 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:26:28.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-21 23:26:28.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:26:28.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 23:26:28.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 23:26:28.978371 my_AutoMLPlus-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      317 2023-05-21 23:26:02.000000 my_AutoMLPlus-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:34:47.778810 my_AutoMLPlus-0.0.3/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:34:47.778810 my_AutoMLPlus-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-21 23:34:47.764669 my_AutoMLPlus-0.0.3/my_AutoMLPlus/
+-rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus/__init__.py
+-rw-rw-rw-   0        0        0     6599 2023-05-21 18:47:16.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus/data_preprocessing.py
+-rw-rw-rw-   0        0        0     2125 2023-05-21 23:33:44.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus/ml_pipeline.py
+-rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus/predictive_models.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:34:47.777605 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:34:47.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-21 23:34:47.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 23:34:47.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 23:34:47.000000 my_AutoMLPlus-0.0.3/my_AutoMLPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 23:34:47.780805 my_AutoMLPlus-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      317 2023-05-21 23:34:11.000000 my_AutoMLPlus-0.0.3/setup.py
```

### Comparing `my_AutoMLPlus-0.0.2/my_AutoMLPlus/data_preprocessing.py` & `my_AutoMLPlus-0.0.3/my_AutoMLPlus/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `my_AutoMLPlus-0.0.2/my_AutoMLPlus/ml_pipeline.py` & `my_AutoMLPlus-0.0.3/my_AutoMLPlus/ml_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import pandas as pd
 from nbimporter import NotebookLoader
 from sklearn.preprocessing import StandardScaler
 from sklearn.impute import SimpleImputer
 from sklearn.metrics import r2_score
 
+from .data_preprocessing import DataFramePreprocessor
+from .predictive_models import ElasticNetModel
+from .predictive_models import RandomForestRegressorModel
+from .predictive_models import GradientBoostingRegressorModel
+from .predictive_models import LinearRegressionModel
+
 class MyAutoML:
     def __init__(self, data: pd.DataFrame, target: str):
         self.data = data
         self.target = target
 
     def _preprocess_data(self):
         # Обработка данных
```

### Comparing `my_AutoMLPlus-0.0.2/my_AutoMLPlus/predictive_models.py` & `my_AutoMLPlus-0.0.3/my_AutoMLPlus/predictive_models.py`

 * *Files identical despite different names*

