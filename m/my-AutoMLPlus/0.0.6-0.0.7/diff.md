# Comparing `tmp/my_AutoMLPlus-0.0.6.tar.gz` & `tmp/my_AutoMLPlus-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_AutoMLPlus-0.0.6.tar", last modified: Sun May 21 23:56:42 2023, max compression
+gzip compressed data, was "my_AutoMLPlus-0.0.7.tar", last modified: Sun May 21 23:59:56 2023, max compression
```

## Comparing `my_AutoMLPlus-0.0.6.tar` & `my_AutoMLPlus-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:56:42.333813 my_AutoMLPlus-0.0.6/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:56:42.334431 my_AutoMLPlus-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-21 23:56:42.319818 my_AutoMLPlus-0.0.6/my_AutoMLPlus/
--rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus/__init__.py
--rw-rw-rw-   0        0        0     6670 2023-05-21 23:56:02.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus/data_preprocessing.py
--rw-rw-rw-   0        0        0     2246 2023-05-21 23:52:29.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus/ml_pipeline.py
--rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus/predictive_models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:56:42.332816 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:56:42.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-21 23:56:42.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:56:42.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 23:56:42.000000 my_AutoMLPlus-0.0.6/my_AutoMLPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 23:56:42.335809 my_AutoMLPlus-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      317 2023-05-21 23:56:22.000000 my_AutoMLPlus-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:59:56.931967 my_AutoMLPlus-0.0.7/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:59:56.931967 my_AutoMLPlus-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-21 23:59:56.915432 my_AutoMLPlus-0.0.7/my_AutoMLPlus/
+-rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus/__init__.py
+-rw-rw-rw-   0        0        0     6670 2023-05-21 23:56:02.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus/data_preprocessing.py
+-rw-rw-rw-   0        0        0     2149 2023-05-21 23:58:57.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus/ml_pipeline.py
+-rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus/predictive_models.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:59:56.930968 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-21 23:59:56.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-21 23:59:56.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 23:59:56.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 23:59:56.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 23:59:56.933973 my_AutoMLPlus-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      317 2023-05-21 23:59:40.000000 my_AutoMLPlus-0.0.7/setup.py
```

### Comparing `my_AutoMLPlus-0.0.6/my_AutoMLPlus/data_preprocessing.py` & `my_AutoMLPlus-0.0.7/my_AutoMLPlus/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `my_AutoMLPlus-0.0.6/my_AutoMLPlus/ml_pipeline.py` & `my_AutoMLPlus-0.0.7/my_AutoMLPlus/ml_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         self.data = data
         self.target = target
 
     def _preprocess_data(self):
         # Обработка данных
         object_columns = self.data.columns[self.data.dtypes == "object"]
         df_preprocessor = DataFramePreprocessor(object_columns, scaler=StandardScaler(), imputer=SimpleImputer())
-        X_train_selected, X_test_selected, y_train, y_test = df_preprocessor.process(self.data)
 
         X_train_selected, X_test_selected, y_train, y_test = df_preprocessor.process(self.data, self.target)
         self.X_train_selected = X_train_selected
         self.X_test_selected = X_test_selected
         self.y_train = y_train
         self.y_test = y_test
```

### Comparing `my_AutoMLPlus-0.0.6/my_AutoMLPlus/predictive_models.py` & `my_AutoMLPlus-0.0.7/my_AutoMLPlus/predictive_models.py`

 * *Files identical despite different names*

