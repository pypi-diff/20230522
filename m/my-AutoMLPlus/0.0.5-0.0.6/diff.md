# Comparing `tmp/my_AutoMLPlus-0.0.5.tar.gz` & `tmp/my_AutoMLPlus-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_AutoMLPlus-0.0.5.tar", last modified: Sun May 21 23:48:03 2023, max compression
+gzip compressed data, was "my_AutoMLPlus-0.0.6.tar", last modified: Sun May 21 23:56:42 2023, max compression
```

## Comparing `my_AutoMLPlus-0.0.5.tar` & `my_AutoMLPlus-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:48:03.508232 my_AutoMLPlus-0.0.5/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:48:03.508232 my_AutoMLPlus-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-21 23:48:03.493116 my_AutoMLPlus-0.0.5/my_AutoMLPlus/
--rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus/__init__.py
--rw-rw-rw-   0        0        0     6650 2023-05-21 23:47:15.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus/data_preprocessing.py
--rw-rw-rw-   0        0        0     2272 2023-05-21 23:47:11.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus/ml_pipeline.py
--rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus/predictive_models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:48:03.506240 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:48:03.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-21 23:48:03.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:48:03.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 23:48:03.000000 my_AutoMLPlus-0.0.5/my_AutoMLPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 23:48:03.510227 my_AutoMLPlus-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      317 2023-05-21 23:47:54.000000 my_AutoMLPlus-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:56:42.333813 my_AutoMLPlus-0.0.6/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:56:42.334431 my_AutoMLPlus-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-21 23:56:42.319818 my_AutoMLPlus-0.0.6/my_AutoMLPlus/
+-rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus/__init__.py
+-rw-rw-rw-   0        0        0     6670 2023-05-21 23:56:02.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus/data_preprocessing.py
+-rw-rw-rw-   0        0        0     2246 2023-05-21 23:52:29.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus/ml_pipeline.py
+-rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus/predictive_models.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:56:42.332816 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:56:42.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-21 23:56:42.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 23:56:42.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 23:56:42.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 23:56:42.335809 my_AutoMLPlus-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      317 2023-05-21 23:56:22.000000 my_AutoMLPlus-0.0.6/setup.py
```

### Comparing `my_AutoMLPlus-0.0.5/my_AutoMLPlus/data_preprocessing.py` & `my_AutoMLPlus-0.0.6/my_AutoMLPlus/data_preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
 class DataFramePreprocessor:
     def __init__(self, object_columns, scaler=StandardScaler(), imputer=SimpleImputer()):
         self.object_columns = object_columns
         self.scaler = scaler
         self.imputer = imputer
 
-    def process(self, data):
+    def process(self, data, target):
         data = self.correct_text(data)
         data = self.drop_duplicates(data)
         data = self.apply_label_encoder(data)
         
-        X_train, X_test, y_train, y_test = self.split_data(data)
+        X_train, X_test, y_train, y_test = self.split_data(data, target)
         # Заполнение отсутствующих значений
         X_train_imputed, X_test_imputed = self.impute_missing_values(X_train, X_test, y_train)
         
         # Сохраняем имена столбцов
         self.columns = X_train_imputed.columns
         # Преобразуем numpy.ndarray обратно в DataFrame с сохранением имен столбцов
         X_train_imputed = pd.DataFrame(X_train_imputed, columns=self.columns)
@@ -58,16 +58,16 @@
 
     def apply_label_encoder(self, data):
         lew = LabelEncoderWrapper()
         data[self.object_columns] = lew.fit_transform(data[self.object_columns])
         return data
 
     @staticmethod
-    def split_data(data):
-        return train_test_split(data.drop(['target'], axis=1), data['target'], test_size=0.2, random_state=42)
+    def split_data(data, target):
+        return train_test_split(data.drop([target], axis=1), data[target], test_size=0.2, random_state=42)
 
     # Находим оптимальный метод заполнения пропущенных значений с помощью GridSearchCV
     def impute_missing_values(self, X_train, X_test, y_train):
         param_grid_imputer = {'strategy': ['mean', 'median', 'most_frequent', 'constant']}
         grid_search_imputer = GridSearchCV(self.imputer, param_grid=param_grid_imputer, cv=5, scoring='r2')
         grid_search_imputer.fit(X_train, y_train)
         best_imputer = grid_search_imputer.best_estimator_
```

### Comparing `my_AutoMLPlus-0.0.5/my_AutoMLPlus/ml_pipeline.py` & `my_AutoMLPlus-0.0.6/my_AutoMLPlus/ml_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from my_AutoMLPlus.predictive_models import ElasticNetModel
 from my_AutoMLPlus.predictive_models import RandomForestRegressorModel
 from my_AutoMLPlus.predictive_models import GradientBoostingRegressorModel
 from my_AutoMLPlus.predictive_models import LinearRegressionModel
 
 import warnings
 
-warnings.filterwarnings('ignore', message="Scoring failed")
+warnings.filterwarnings('ignore')
 
 class MyAutoML:
     def __init__(self, data: pd.DataFrame, target: str):
         self.data = data
         self.target = target
 
     def _preprocess_data(self):
```

### Comparing `my_AutoMLPlus-0.0.5/my_AutoMLPlus/predictive_models.py` & `my_AutoMLPlus-0.0.6/my_AutoMLPlus/predictive_models.py`

 * *Files identical despite different names*

