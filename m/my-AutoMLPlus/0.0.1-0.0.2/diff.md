# Comparing `tmp/my_AutoMLPlus-0.0.1.tar.gz` & `tmp/my_AutoMLPlus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_AutoMLPlus-0.0.1.tar", last modified: Sun May 21 23:10:42 2023, max compression
+gzip compressed data, was "my_AutoMLPlus-0.0.2.tar", last modified: Sun May 21 23:26:28 2023, max compression
```

## Comparing `my_AutoMLPlus-0.0.1.tar` & `my_AutoMLPlus-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:10:42.438740 my_AutoMLPlus-0.0.1/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:10:42.438740 my_AutoMLPlus-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-21 23:10:42.419412 my_AutoMLPlus-0.0.1/my_AutoMLPlus/
--rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.1/my_AutoMLPlus/__init__.py
--rw-rw-rw-   0        0        0     6599 2023-05-21 18:47:16.000000 my_AutoMLPlus-0.0.1/my_AutoMLPlus/data_preprocessing.py
--rw-rw-rw-   0        0        0     1829 2023-05-21 18:47:47.000000 my_AutoMLPlus-0.0.1/my_AutoMLPlus/ml_pipeline.py
--rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.1/my_AutoMLPlus/predictive_models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:10:42.437800 my_AutoMLPlus-0.0.1/my_AutoMLPlus.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:10:42.000000 my_AutoMLPlus-0.0.1/my_AutoMLPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-21 23:10:42.000000 my_AutoMLPlus-0.0.1/my_AutoMLPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:10:42.000000 my_AutoMLPlus-0.0.1/my_AutoMLPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 23:10:42.000000 my_AutoMLPlus-0.0.1/my_AutoMLPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 23:10:42.440836 my_AutoMLPlus-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      317 2023-05-21 23:10:04.000000 my_AutoMLPlus-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:26:28.976545 my_AutoMLPlus-0.0.2/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:26:28.976804 my_AutoMLPlus-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-21 23:26:28.961387 my_AutoMLPlus-0.0.2/my_AutoMLPlus/
+-rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus/__init__.py
+-rw-rw-rw-   0        0        0     6599 2023-05-21 18:47:16.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus/data_preprocessing.py
+-rw-rw-rw-   0        0        0     1844 2023-05-21 23:21:41.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus/ml_pipeline.py
+-rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus/predictive_models.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:26:28.975490 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:26:28.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-21 23:26:28.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 23:26:28.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 23:26:28.000000 my_AutoMLPlus-0.0.2/my_AutoMLPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 23:26:28.978371 my_AutoMLPlus-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      317 2023-05-21 23:26:02.000000 my_AutoMLPlus-0.0.2/setup.py
```

### Comparing `my_AutoMLPlus-0.0.1/my_AutoMLPlus/data_preprocessing.py` & `my_AutoMLPlus-0.0.2/my_AutoMLPlus/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `my_AutoMLPlus-0.0.1/my_AutoMLPlus/ml_pipeline.py` & `my_AutoMLPlus-0.0.2/my_AutoMLPlus/ml_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 class MyAutoML:
     def __init__(self, data: pd.DataFrame, target: str):
         self.data = data
         self.target = target
 
     def _preprocess_data(self):
         # Обработка данных
-        object_columns = data.columns[data.dtypes == "object"]
+        object_columns = self.data.columns[self.data.dtypes == "object"]
         df_preprocessor = DataFramePreprocessor(object_columns, scaler=StandardScaler(), imputer=SimpleImputer())
-        X_train_selected, X_test_selected, y_train, y_test = df_preprocessor.process(data)
+        X_train_selected, X_test_selected, y_train, y_test = df_preprocessor.process(self.data)
 
         X_train_selected, X_test_selected, y_train, y_test = df_preprocessor.process(self.data, self.target)
         self.X_train_selected = X_train_selected
         self.X_test_selected = X_test_selected
         self.y_train = y_train
         self.y_test = y_test
```

### Comparing `my_AutoMLPlus-0.0.1/my_AutoMLPlus/predictive_models.py` & `my_AutoMLPlus-0.0.2/my_AutoMLPlus/predictive_models.py`

 * *Files identical despite different names*

