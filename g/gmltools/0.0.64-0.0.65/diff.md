# Comparing `tmp/gmltools-0.0.64.tar.gz` & `tmp/gmltools-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.64.tar", last modified: Sun May 14 14:09:48 2023, max compression
+gzip compressed data, was "gmltools-0.0.65.tar", last modified: Mon May 22 08:03:14 2023, max compression
```

## Comparing `gmltools-0.0.64.tar` & `gmltools-0.0.65.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.905955 gmltools-0.0.64/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.64/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.64/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-05-14 14:09:48.904946 gmltools-0.0.64/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.64/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.604745 gmltools-0.0.64/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.64/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.64/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.64/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-05-14 14:09:21.000000 gmltools-0.0.64/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 14:09:48.905955 gmltools-0.0.64/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-05-14 14:09:10.000000 gmltools-0.0.64/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.544846 gmltools-0.0.64/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.616658 gmltools-0.0.64/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.64/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.64/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.661170 gmltools-0.0.64/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.64/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.64/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.788846 gmltools-0.0.64/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.64/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.64/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.64/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.64/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   119407 2023-05-14 14:08:53.000000 gmltools-0.0.64/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.64/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.64/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.839899 gmltools-0.0.64/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.64/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.64/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.64/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.901894 gmltools-0.0.64/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.64/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.64/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.64/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.64/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.643169 gmltools-0.0.64/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.952368 gmltools-0.0.65/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.65/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.65/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-05-22 08:03:14.951354 gmltools-0.0.65/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.65/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.632418 gmltools-0.0.65/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.65/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.65/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.65/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-05-22 08:02:30.000000 gmltools-0.0.65/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 08:03:14.952368 gmltools-0.0.65/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-05-22 08:02:08.000000 gmltools-0.0.65/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.551759 gmltools-0.0.65/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.667636 gmltools-0.0.65/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.65/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.65/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.763395 gmltools-0.0.65/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.65/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.65/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.830436 gmltools-0.0.65/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.65/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.65/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.65/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.65/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   126791 2023-05-22 08:00:36.000000 gmltools-0.0.65/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.65/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.65/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.875102 gmltools-0.0.65/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.65/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.65/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.65/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.945263 gmltools-0.0.65/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.65/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.65/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.65/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.65/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.738041 gmltools-0.0.65/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-05-22 08:03:13.000000 gmltools-0.0.65/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-22 08:03:14.000000 gmltools-0.0.65/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:03:13.000000 gmltools-0.0.65/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-22 08:03:13.000000 gmltools-0.0.65/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 08:03:13.000000 gmltools-0.0.65/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.64/LICENSE` & `gmltools-0.0.65/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/Models.ipynb` & `gmltools-0.0.65/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/PKG-INFO` & `gmltools-0.0.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.64
+Version: 0.0.65
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.64/README.md` & `gmltools-0.0.65/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.65/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/gmltools.yml` & `gmltools-0.0.65/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/mltools.yml` & `gmltools-0.0.65/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/pyproject.toml` & `gmltools-0.0.65/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.64"
+version = "0.0.65"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.64/setup.py` & `gmltools-0.0.65/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.64',
+    'version': '0.0.65',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.64/src/gmltools/To_Do.txt` & `gmltools-0.0.65/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/eda/eda.py` & `gmltools-0.0.65/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/models/bayes.py` & `gmltools-0.0.65/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.65/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/models/dummy_model.py` & `gmltools-0.0.65/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/models/model.py` & `gmltools-0.0.65/src/gmltools/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #REGRESSION
 from sklearn.ensemble import RandomForestRegressor
 from xgboost import XGBRegressor
 from sklearn.linear_model import LinearRegression
 from sklearn.neighbors import KNeighborsRegressor
 from sklearn.neural_network import MLPRegressor
 from sklearn.tree import DecisionTreeRegressor
+from sklearn.svm import SVR
 
 
 
 #PREPROCESSING
 from sklearn.pipeline import Pipeline
 from sklearn.compose import ColumnTransformer
 from sklearn.preprocessing import OneHotEncoder
@@ -234,14 +235,16 @@
                 self._model.fit(self.X_train, self.y_train, KNN__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             elif self.pipe.steps[-1][0] == 'LR':
                 self._model.fit(self.X_train, self.y_train, LR__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             elif self.pipe.steps[-1][0] == 'MLP':
                 self._model.fit(self.X_train, self.y_train, MLP__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             elif self.pipe.steps[-1][0] == 'DT':
                 self._model.fit(self.X_train, self.y_train, DT__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            elif self.pipe.steps[-1][0] == 'SVR':
+                self._model.fit(self.X_train, self.y_train, SVR__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
         else:
             self._model.fit(X=self.X_train, y=self.y_train, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
 
         return self._model
 
 
     
@@ -1770,14 +1773,114 @@
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
         
             print(self.model.best_params_)
 
+
+    def SVR(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+                            grid_params={'SVR__kernel':['linear','poly','rbf'],
+                                'SVR__C': [0.00001,0.0001,0.001,0.01,0.1,1,10,100,1000],
+                                'SVR__gamma':[0.0001,0.001,0.01,0.1,1,10]}, 
+                            random_params=None, random_n_iter=10, bayes_pbounds=None,
+                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None, n_jobs=-1,
+                            columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
+            
+
+            
+            """
+            This method performs a Decision Tree Regressor model with grid search or bayesian optimization.
+    
+            Parameters
+            ----------
+            X_train : pandas dataframe
+                Training set.
+    
+            y_train : pandas dataframe
+                Training set labels.
+    
+            ordinal_cat_cols : list, optional
+                List of ordinal categorical variables. The default is None.
+    
+            scoring : str, optional
+                Evaluation metric. The default is 'neg_mean_squared_error'.
+    
+            grid_params : dict, optional
+                Dictionary of parameters for grid search. The default is
+
+            cv : int, optional
+                Number of folds for cross validation. The default is 10.
+                For time series data, cv must be a TimeSeriesSplit object.
+            
+            random_params : dict, optional
+                Dictionary of parameters for random search. The default is None.
+            
+            random_n_iter : int, optional
+                Number of iterations for random search. The default is 10.
+            
+            bayes_pbounds : dict, optional
+                Dictionary of parameters for bayesian optimization. The default is None.
+
+            bayes_int_params : list, optional
+                List of parameters for bayesian optimization that are integers. The default is None.
+            
+            bayes_n_iter : int, optional
+                Number of iterations for bayesian optimization. The default is 30.
+            
+            random_state : int, optional
+                Random state. The default is None.
+            
+            n_jobs : int, optional
+                Number of jobs. The default is -1.
+            
+            Returns
+            -------
+            model_ : sklearn model
+                Trained model.
+            
+            """
+
+            print(" INFO: Agurments params must start as 'SVR__param'" + '\n' "INFO: Default params in Documentation for Decision Tree Regressor are: ", dt_default_params_reg)
+            print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
+            f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
+            f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
+            assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
+            assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter bounds"
+            assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
+            assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter bounds"
+            assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
+            assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
+            # DT__ is the prefix for every hyperparameter in the Decision Tree Regressor
+            if grid_params is not None and random_params is None and bayes_pbounds is None:
+                assert all('SVR__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'SVR__'"
+            elif random_params is not None:
+                assert all('SVR__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'SVR__'"
+            elif bayes_pbounds is not None:
+                assert all('SVR__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'SVR__'"
+                assert all('SVR__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'SVR__'"
+            
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            pipe = Pipeline(steps=[('Prep', preprocessor),
+                                ('SVR', SVR())]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+            
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
+
     
 
     def save(self,return_best_metrics:bool=True):
         """
         Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
 
         Parameters
```

### Comparing `gmltools-0.0.64/src/gmltools/models/models_info.py` & `gmltools-0.0.65/src/gmltools/models/models_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,10 +262,27 @@
     "max_leaf_nodes": None,
     "min_impurity_decrease": 0.0,
     "ccp_alpha": 0.0
 }
 
 
 
+svr_default_params_reg = {
+    'kernel': ['linear', 'poly', 'rbf', 'sigmoid', 'precomputed'],
+    'degree': 3,
+    'gamma': ['scale','auto', 0.001, 0.01, 0.1, 10],
+    'coef0': 0.0,
+    'tol': 1e-3,
+    'C':[0.0001,0.001,0.01,0.1,1,10],
+    'epsilon': 0.1,
+    'shrinking': True,
+    'cache_size': 200,
+    'verbose': False,
+    'max_iter': -1
+}
+
+
+
+
```

### Comparing `gmltools-0.0.64/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.65/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.65/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.65/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.65/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.65/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.65/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.64/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.65/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.64
+Version: 0.0.65
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.64/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.65/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

