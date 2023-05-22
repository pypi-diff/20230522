# Comparing `tmp/my_AutoMLPlus-0.0.7.tar.gz` & `tmp/my_AutoMLPlus-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_AutoMLPlus-0.0.7.tar", last modified: Sun May 21 23:59:56 2023, max compression
+gzip compressed data, was "my_AutoMLPlus-0.0.8.tar", last modified: Mon May 22 00:04:23 2023, max compression
```

## Comparing `my_AutoMLPlus-0.0.7.tar` & `my_AutoMLPlus-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:59:56.931967 my_AutoMLPlus-0.0.7/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:59:56.931967 my_AutoMLPlus-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-21 23:59:56.915432 my_AutoMLPlus-0.0.7/my_AutoMLPlus/
--rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus/__init__.py
--rw-rw-rw-   0        0        0     6670 2023-05-21 23:56:02.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus/data_preprocessing.py
--rw-rw-rw-   0        0        0     2149 2023-05-21 23:58:57.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus/ml_pipeline.py
--rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus/predictive_models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:59:56.930968 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-21 23:59:56.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-21 23:59:56.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:59:56.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 23:59:56.000000 my_AutoMLPlus-0.0.7/my_AutoMLPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 23:59:56.933973 my_AutoMLPlus-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      317 2023-05-21 23:59:40.000000 my_AutoMLPlus-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 00:04:23.897195 my_AutoMLPlus-0.0.8/
+-rw-rw-rw-   0        0        0      258 2023-05-22 00:04:23.897195 my_AutoMLPlus-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 00:04:23.882934 my_AutoMLPlus-0.0.8/my_AutoMLPlus/
+-rw-rw-rw-   0        0        0       68 2023-05-21 18:46:22.000000 my_AutoMLPlus-0.0.8/my_AutoMLPlus/__init__.py
+-rw-rw-rw-   0        0        0     6670 2023-05-21 23:56:02.000000 my_AutoMLPlus-0.0.8/my_AutoMLPlus/data_preprocessing.py
+-rw-rw-rw-   0        0        0     2169 2023-05-22 00:03:51.000000 my_AutoMLPlus-0.0.8/my_AutoMLPlus/ml_pipeline.py
+-rw-rw-rw-   0        0        0     1864 2023-05-21 18:48:18.000000 my_AutoMLPlus-0.0.8/my_AutoMLPlus/predictive_models.py
+drwxrwxrwx   0        0        0        0 2023-05-22 00:04:23.895202 my_AutoMLPlus-0.0.8/my_AutoMLPlus.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-22 00:04:23.000000 my_AutoMLPlus-0.0.8/my_AutoMLPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-22 00:04:23.000000 my_AutoMLPlus-0.0.8/my_AutoMLPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 00:04:23.000000 my_AutoMLPlus-0.0.8/my_AutoMLPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 00:04:23.000000 my_AutoMLPlus-0.0.8/my_AutoMLPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 00:04:23.898195 my_AutoMLPlus-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      317 2023-05-22 00:04:09.000000 my_AutoMLPlus-0.0.8/setup.py
```

### Comparing `my_AutoMLPlus-0.0.7/my_AutoMLPlus/data_preprocessing.py` & `my_AutoMLPlus-0.0.8/my_AutoMLPlus/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `my_AutoMLPlus-0.0.7/my_AutoMLPlus/ml_pipeline.py` & `my_AutoMLPlus-0.0.8/my_AutoMLPlus/ml_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 
         # Обучение и тестирование моделей
         models = [LinearRegressionModel(), ElasticNetModel(), RandomForestRegressorModel(), GradientBoostingRegressorModel()]
         # выбираем наилучшую модель
         best_model = None
         best_score = -float("inf")
         for model in models:
-            model.fit(X_train_selected, y_train)
-            y_pred = model.predict(X_test_selected)
-            r2 = r2_score(y_test, y_pred)
+            model.fit(self.X_train_selected, self.y_train)
+            y_pred = model.predict(self.X_test_selected)
+            r2 = r2_score(self.y_test, y_pred)
         
             if r2 > best_score:
                 best_model = model
                 best_score = r2
         
             print(f"{type(model).__name__} R²: {r2:.4f}")
```

### Comparing `my_AutoMLPlus-0.0.7/my_AutoMLPlus/predictive_models.py` & `my_AutoMLPlus-0.0.8/my_AutoMLPlus/predictive_models.py`

 * *Files identical despite different names*

