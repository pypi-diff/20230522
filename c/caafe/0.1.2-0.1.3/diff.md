# Comparing `tmp/caafe-0.1.2.tar.gz` & `tmp/caafe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caafe-0.1.2.tar", last modified: Sat May 20 09:25:09 2023, max compression
+gzip compressed data, was "caafe-0.1.3.tar", last modified: Mon May 22 12:38:51 2023, max compression
```

## Comparing `caafe-0.1.2.tar` & `caafe-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 09:25:09.129420 caafe-0.1.2/
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-20 09:23:35.000000 caafe-0.1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-20 09:25:09.129420 caafe-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2088 2023-05-20 09:23:35.000000 caafe-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 09:25:09.128420 caafe-0.1.2/caafe/
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11664 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/caafe.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/caafe_evaluate.py
--rw-r--r--   0 root         (0) root         (0)    11093 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/data.py
--rw-r--r--   0 root         (0) root         (0)     4399 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/evaluate.py
--rw-r--r--   0 root         (0) root         (0)     3605 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/feature_extension_baselines.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/metrics.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/plotting.py
--rw-r--r--   0 root         (0) root         (0)     4467 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)     7895 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/run_llm_code.py
--rw-r--r--   0 root         (0) root         (0)     5270 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/sklearn_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 09:25:09.129420 caafe-0.1.2/caafe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 09:25:09.129420 caafe-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1182 2023-05-20 09:25:03.000000 caafe-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 09:25:09.129420 caafe-0.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 09:23:35.000000 caafe-0.1.2/tests/test_sklearn_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:38:51.724153 caafe-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-22 12:37:19.000000 caafe-0.1.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     6349 2023-05-22 12:38:51.724153 caafe-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5505 2023-05-22 12:37:19.000000 caafe-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:38:51.723153 caafe-0.1.3/caafe/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11664 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/caafe.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/caafe_evaluate.py
+-rw-r--r--   0 root         (0) root         (0)    11101 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/data.py
+-rw-r--r--   0 root         (0) root         (0)     4399 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/feature_extension_baselines.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/plotting.py
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     7895 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/run_llm_code.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2023-05-22 12:37:19.000000 caafe-0.1.3/caafe/sklearn_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:38:51.724153 caafe-0.1.3/caafe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6349 2023-05-22 12:38:51.000000 caafe-0.1.3/caafe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-22 12:38:51.000000 caafe-0.1.3/caafe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 12:38:51.000000 caafe-0.1.3/caafe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-22 12:38:51.000000 caafe-0.1.3/caafe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-22 12:38:51.000000 caafe-0.1.3/caafe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 12:38:51.724153 caafe-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-05-22 12:37:39.000000 caafe-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:38:51.724153 caafe-0.1.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 12:37:19.000000 caafe-0.1.3/tests/test_sklearn_wrapper.py
```

### Comparing `caafe-0.1.2/caafe/caafe.py` & `caafe-0.1.3/caafe/caafe.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.2/caafe/caafe_evaluate.py` & `caafe-0.1.3/caafe/caafe_evaluate.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.2/caafe/data.py` & `caafe-0.1.3/caafe/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             data=np.concatenate([X, np.expand_dims(y, -1)], -1), columns=ds[4]
         )
         cat_features = ds[3]
         for c in cat_features:
             if len(np.unique(df.iloc[:, c])) > 50:
                 cat_features.remove(c)
                 continue
-            df.iloc[:, c] = df.iloc[:, c].astype("int32")
+            df[df.columns[c]] = df[df.columns[c]].astype("int32")
         return df.infer_objects()
 
     ds = copy.deepcopy(ds)
 
     X = ds[1].numpy() if type(ds[1]) == torch.Tensor else ds[1]
     y = ds[2].numpy() if type(ds[2]) == torch.Tensor else ds[2]
     X_train, X_test, y_train, y_test = train_test_split(
```

### Comparing `caafe-0.1.2/caafe/evaluate.py` & `caafe-0.1.3/caafe/evaluate.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.2/caafe/feature_extension_baselines.py` & `caafe-0.1.3/caafe/feature_extension_baselines.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.2/caafe/metrics.py` & `caafe-0.1.3/caafe/metrics.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.2/caafe/plotting.py` & `caafe-0.1.3/caafe/plotting.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.2/caafe/preprocessing.py` & `caafe-0.1.3/caafe/preprocessing.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.2/caafe/run_llm_code.py` & `caafe-0.1.3/caafe/run_llm_code.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.2/setup.py` & `caafe-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="caafe",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     description="Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Noah Hollmann, Samuel Müller, Frank Hutter",
     author_email="noah.homa@gmail.com",
     url="https://github.com/automl/CAAFE",
```

