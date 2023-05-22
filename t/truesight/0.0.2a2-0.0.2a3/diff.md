# Comparing `tmp/truesight-0.0.2a2.tar.gz` & `tmp/truesight-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truesight-0.0.2a2.tar", last modified: Fri May 19 19:19:03 2023, max compression
+gzip compressed data, was "truesight-0.0.2a3.tar", last modified: Mon May 22 18:09:04 2023, max compression
```

## Comparing `truesight-0.0.2a2.tar` & `truesight-0.0.2a3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:19:03.608434 truesight-0.0.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-19 19:19:03.608434 truesight-0.0.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-19 19:18:46.000000 truesight-0.0.2a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 19:19:03.608434 truesight-0.0.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-19 19:18:46.000000 truesight-0.0.2a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:19:03.608434 truesight-0.0.2a2/truesight/
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:19:03.608434 truesight-0.0.2a2/truesight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:04.820492 truesight-0.0.2a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 18:08:42.000000 truesight-0.0.2a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-22 18:09:04.820492 truesight-0.0.2a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-22 18:08:42.000000 truesight-0.0.2a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 18:09:04.820492 truesight-0.0.2a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-22 18:08:42.000000 truesight-0.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:04.820492 truesight-0.0.2a3/truesight/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:04.820492 truesight-0.0.2a3/truesight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/top_level.txt
```

### Comparing `truesight-0.0.2a2/PKG-INFO` & `truesight-0.0.2a3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-Metadata-Version: 2.1
-Name: truesight
-Version: 0.0.2a2
-Summary: Truesight is a python package for time series prediction using deep learning and statistical models.
-Home-page: https://github.com/renanklehm/true-sight
-Download-URL: https://github.com/renanklehm/true-sight/archive/refs/tags/v0.0.1-alpha.tar.gz
-Author: Renan Otvin Klehm
-Author-email: renanotivin@hotmail.com
-Keywords: time series,prediction
-Description-Content-Type: text/markdown
-
 # TrueSight ✨
 
-The TrueSight model is a hybrid forecasting tool that uses statistical forecasting models together with a Deep Neural Network (DNN) to make predictions. The TrueSight `Preprocessor` class is responsible for getting all the statistical forecasters in one place. It can handle forecasters from packages like `statsforecast`, `scikit-learn`, `pmdarima`, and others. You just need a class that accepts the `seasonal_length` parameter for the constructor and has a `.fit(x, y)` method
+The TrueSight model is a hybrid forecasting tool that uses statistical forecasting models together with a Deep Neural Network (DNN) to make predictions. The TrueSight `Preprocessor` class is responsible for getting all the statistical forecasters in one place. It can handle forecasters from packages like `statsforecast`, `scikit-learn`, `pmdarima`, and others. You just need to the `ModelWrapper` Class to standardize the method calls.
 
 All you need to do before using this package, is create a pandas dataframe with the following structure:
 
  - unique_id: A string that uniquely identifies each time series in the dataframe
  - ds: A datetime column with the date of each time step. The dates must be in the correct frequency for the date_freq parameter
  - y: The values of the time series
 
@@ -47,31 +36,40 @@
 from truesight.utils import get_input_shapes, generate_syntetic_data
 ```
 
 Load the data
 
 ``` python
 num_time_steps = 60
-seasonal_lenght = 12
+season_length = 12
 forecast_horizon = 12
-df = generate_syntetic_data(num_time_steps, seasonal_lenght, 100)
+df = generate_syntetic_data(num_time_steps, season_length, 100)
 ```
-Create and run the preprocessor class. You can include as many statistical models as you need in the `models` parameter. Just make sure they follow the syntax similar to `statsforecast`. However, keep in mind that more models mean longer processing time. It's important to set a fallback model in case any of the informed models fail to fit.
+Create and run the preprocessor class. You can include as many statistical models as you need in the `models` parameter, just make sure to use the `ModelWrapper` class. However, keep in mind that more models mean longer processing time. It's important to set a fallback model in case any of the informed models fail to fit.
 
 ``` python
 from statsforecast.models import SeasonalNaive, AutoETS
+from sklearn.linear_model import LinearRegression
 from truesight.models import AdditiveDecomposition
+from truesight.utils import ModelWrapper
+
+models = [
+    ModelWrapper(LinearRegression, horizon=forecast_horizon, season_length=season_length), 
+    ModelWrapper(SeasonalNaive, horizon=forecast_horizon, season_length=season_length), 
+    ModelWrapper(AutoETS, horizon=forecast_horizon, season_length=season_length),
+    ModelWrapper(AdditiveDecomposition, horizon=forecast_horizon, season_length=season_length)
+]
 
 preprocessor = Preprocessor(df)
 X_train, Y_train, ids_train, X_val, Y_val, ids_val, models = preprocessor.make_dataset(
     forecast_horizon = 12, 
     season_length = 12,
     date_freq = "MS", 
-    models = [AdditiveDecomposition, AutoETS, SeasonalNaive], 
-    fallback_model = SeasonalNaive,
+    models = models, 
+    fallback_model = ModelWrapper(SeasonalNaive, horizon=forecast_horizon, season_length=season_length),
     verbose = True
     )
 ```
 
 Create the model
 
 ``` python
```

### Comparing `truesight-0.0.2a2/setup.py` & `truesight-0.0.2a3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'truesight',
     packages = ['truesight'],
-    version = 'v0.0.2a2',
+    version = 'v0.0.2a3',
     description = 'Truesight is a python package for time series prediction using deep learning and statistical models.',
     author = 'Renan Otvin Klehm',
     author_email = 'renanotivin@hotmail.com',
     url = 'https://github.com/renanklehm/true-sight',
     download_url = 'https://github.com/renanklehm/true-sight/archive/refs/tags/v0.0.1-alpha.tar.gz',
     keywords = ['time series', 'prediction'],
     classifiers = [],
```

### Comparing `truesight-0.0.2a2/truesight/core.py` & `truesight-0.0.2a3/truesight/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,23 +64,25 @@
             Y_val: np.ndarray, 
             batch_size: int = 128, 
             epochs: int = 100, 
             callbacks: list = [],
             save_best_model: bool = True,
             verbose: bool = True
         ):
+
         self.history = self.model.fit(
             x = X_train,
             y = Y_train,
             batch_size = batch_size,
             epochs = epochs,
             validation_data = [X_val, Y_val],
             callbacks = callbacks,
             verbose = verbose
             )
+        
         if save_best_model: self.model.save(self.model_folder)
 
     def predict(
             self,
             X: list,
             n_repeats: int = 1,
             batch_size: int = 128,
```

### Comparing `truesight-0.0.2a2/truesight/metrics.py` & `truesight-0.0.2a3/truesight/metrics.py`

 * *Files identical despite different names*

### Comparing `truesight-0.0.2a2/truesight/preprocessing.py` & `truesight-0.0.2a3/truesight/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,22 @@
         groups = local_df.groupby("unique_id")
         return_df = []
         for unique_id, group in tqdm(groups, total = len(groups), disable = not verbose):
             output_dates = pd.date_range(group.ds.max(), periods = self.forecast_horizon + 1, freq = self.date_freq)[1:]
             output_ids = [unique_id] * len(output_dates)
             for model in models:
                 try:
-                    model = model(season_length = self.season_length)
                     model.fit(group['y'].to_numpy())
                 except:
                     if fallback_model is not None:
                         model = fallback_model(season_length = self.season_length)
                         model.fit(group['y'].to_numpy())
                     else:
                         raise Exception("Model fit failed. Please provide a fallback model.")
                 return_df.append(pd.DataFrame({
                     "unique_id": output_ids,
                     "ds": output_dates,
-                    model.__repr__(): model.predict(self.forecast_horizon)['mean'],
+                    model.__repr__(): model.predict(),
                 }))
         return_df = pd.concat(return_df)
         return_df = return_df.groupby(['unique_id', 'ds'], as_index = False).sum()
         return return_df
```

### Comparing `truesight-0.0.2a2/truesight.egg-info/PKG-INFO` & `truesight-0.0.2a3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: truesight
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: Truesight is a python package for time series prediction using deep learning and statistical models.
 Home-page: https://github.com/renanklehm/true-sight
 Download-URL: https://github.com/renanklehm/true-sight/archive/refs/tags/v0.0.1-alpha.tar.gz
 Author: Renan Otvin Klehm
 Author-email: renanotivin@hotmail.com
 Keywords: time series,prediction
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # TrueSight ✨
 
-The TrueSight model is a hybrid forecasting tool that uses statistical forecasting models together with a Deep Neural Network (DNN) to make predictions. The TrueSight `Preprocessor` class is responsible for getting all the statistical forecasters in one place. It can handle forecasters from packages like `statsforecast`, `scikit-learn`, `pmdarima`, and others. You just need a class that accepts the `seasonal_length` parameter for the constructor and has a `.fit(x, y)` method
+The TrueSight model is a hybrid forecasting tool that uses statistical forecasting models together with a Deep Neural Network (DNN) to make predictions. The TrueSight `Preprocessor` class is responsible for getting all the statistical forecasters in one place. It can handle forecasters from packages like `statsforecast`, `scikit-learn`, `pmdarima`, and others. You just need to the `ModelWrapper` Class to standardize the method calls.
 
 All you need to do before using this package, is create a pandas dataframe with the following structure:
 
  - unique_id: A string that uniquely identifies each time series in the dataframe
  - ds: A datetime column with the date of each time step. The dates must be in the correct frequency for the date_freq parameter
  - y: The values of the time series
 
@@ -47,31 +48,40 @@
 from truesight.utils import get_input_shapes, generate_syntetic_data
 ```
 
 Load the data
 
 ``` python
 num_time_steps = 60
-seasonal_lenght = 12
+season_length = 12
 forecast_horizon = 12
-df = generate_syntetic_data(num_time_steps, seasonal_lenght, 100)
+df = generate_syntetic_data(num_time_steps, season_length, 100)
 ```
-Create and run the preprocessor class. You can include as many statistical models as you need in the `models` parameter. Just make sure they follow the syntax similar to `statsforecast`. However, keep in mind that more models mean longer processing time. It's important to set a fallback model in case any of the informed models fail to fit.
+Create and run the preprocessor class. You can include as many statistical models as you need in the `models` parameter, just make sure to use the `ModelWrapper` class. However, keep in mind that more models mean longer processing time. It's important to set a fallback model in case any of the informed models fail to fit.
 
 ``` python
 from statsforecast.models import SeasonalNaive, AutoETS
+from sklearn.linear_model import LinearRegression
 from truesight.models import AdditiveDecomposition
+from truesight.utils import ModelWrapper
+
+models = [
+    ModelWrapper(LinearRegression, horizon=forecast_horizon, season_length=season_length), 
+    ModelWrapper(SeasonalNaive, horizon=forecast_horizon, season_length=season_length), 
+    ModelWrapper(AutoETS, horizon=forecast_horizon, season_length=season_length),
+    ModelWrapper(AdditiveDecomposition, horizon=forecast_horizon, season_length=season_length)
+]
 
 preprocessor = Preprocessor(df)
 X_train, Y_train, ids_train, X_val, Y_val, ids_val, models = preprocessor.make_dataset(
     forecast_horizon = 12, 
     season_length = 12,
     date_freq = "MS", 
-    models = [AdditiveDecomposition, AutoETS, SeasonalNaive], 
-    fallback_model = SeasonalNaive,
+    models = models, 
+    fallback_model = ModelWrapper(SeasonalNaive, horizon=forecast_horizon, season_length=season_length),
     verbose = True
     )
 ```
 
 Create the model
 
 ``` python
```

