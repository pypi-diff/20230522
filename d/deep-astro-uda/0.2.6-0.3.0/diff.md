# Comparing `tmp/deep_astro_uda-0.2.6.tar.gz` & `tmp/deep_astro_uda-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_astro_uda-0.2.6.tar", max compression
+gzip compressed data, was "deep_astro_uda-0.3.0.tar", max compression
```

## Comparing `deep_astro_uda-0.2.6.tar` & `deep_astro_uda-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-05-07 23:05:47.006112 deep_astro_uda-0.2.6/LICENSE
--rw-r--r--   0        0        0    15627 2023-05-07 23:05:47.006312 deep_astro_uda-0.2.6/README.md
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.006474 deep_astro_uda-0.2.6/deep_astro_uda/__init__.py
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.006634 deep_astro_uda-0.2.6/deep_astro_uda/client/__init__.py
--rw-r--r--   0        0        0      544 2023-05-22 15:12:04.267152 deep_astro_uda-0.2.6/deep_astro_uda/client/astro_app.py
--rw-r--r--   0        0        0     1749 2023-05-22 15:29:01.285731 deep_astro_uda-0.2.6/deep_astro_uda/client/commands/demo_command.py
--rw-r--r--   0        0        0      228 2023-05-22 15:13:37.003588 deep_astro_uda-0.2.6/deep_astro_uda/client/commands/infer_command.py
--rw-r--r--   0        0        0     3741 2023-05-22 15:32:26.340255 deep_astro_uda-0.2.6/deep_astro_uda/client/commands/run_command.py
--rw-r--r--   0        0        0      754 2023-05-22 15:20:26.176305 deep_astro_uda-0.2.6/deep_astro_uda/client/options.py
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007013 deep_astro_uda-0.2.6/deep_astro_uda/configs/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-22 13:30:21.731901 deep_astro_uda-0.2.6/deep_astro_uda/configs/config.yaml
--rw-r--r--   0        0        0     2029 2023-05-22 15:34:02.169038 deep_astro_uda-0.2.6/deep_astro_uda/configs/config_functions.py
--rw-r--r--   0        0        0        0 2023-05-08 03:56:27.706969 deep_astro_uda-0.2.6/deep_astro_uda/data_utils/__init__.py
--rw-r--r--   0        0        0     2908 2023-05-08 05:07:18.180392 deep_astro_uda-0.2.6/deep_astro_uda/data_utils/download_data.py
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007291 deep_astro_uda-0.2.6/deep_astro_uda/dist/__init__.py
--rw-r--r--   0        0        0    10906 2023-05-07 23:05:47.007467 deep_astro_uda-0.2.6/deep_astro_uda/dist/deep_astro_uda-0.1.0.tar.gz
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007637 deep_astro_uda-0.2.6/deep_astro_uda/model/__init__.py
--rw-r--r--   0        0        0     6696 2023-05-22 12:36:09.942437 deep_astro_uda-0.2.6/deep_astro_uda/model/eval.py
--rw-r--r--   0        0        0     5632 2023-05-07 23:05:47.007756 deep_astro_uda-0.2.6/deep_astro_uda/model/get_loader.py
--rw-r--r--   0        0        0     4146 2023-05-07 23:05:47.007876 deep_astro_uda-0.2.6/deep_astro_uda/model/loss.py
--rw-r--r--   0        0        0      465 2023-05-07 23:05:47.007980 deep_astro_uda-0.2.6/deep_astro_uda/model/lr_schedule.py
--rw-r--r--   0        0        0     7913 2023-05-22 12:36:19.983415 deep_astro_uda-0.2.6/deep_astro_uda/model/train.py
--rw-r--r--   0        0        0      459 2023-05-22 13:15:04.892342 deep_astro_uda-0.2.6/deep_astro_uda/settings.py
--rw-r--r--   0        0        0     6468 2023-05-07 23:05:47.009742 deep_astro_uda-0.2.6/deep_astro_uda/tuner/tuner.py
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.008275 deep_astro_uda-0.2.6/deep_astro_uda/utils/__init__.py
--rw-r--r--   0        0        0      698 2023-05-07 23:05:47.008398 deep_astro_uda-0.2.6/deep_astro_uda/utils/utils.py
--rw-r--r--   0        0        0      450 2023-05-22 15:35:39.584895 deep_astro_uda-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    16225 1970-01-01 00:00:00.000000 deep_astro_uda-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-07 23:05:47.006112 deep_astro_uda-0.3.0/LICENSE
+-rw-r--r--   0        0        0    15627 2023-05-07 23:05:47.006312 deep_astro_uda-0.3.0/README.md
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.006474 deep_astro_uda-0.3.0/deep_astro_uda/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.006634 deep_astro_uda-0.3.0/deep_astro_uda/client/__init__.py
+-rw-r--r--   0        0        0      544 2023-05-22 15:12:04.267152 deep_astro_uda-0.3.0/deep_astro_uda/client/astro_app.py
+-rw-r--r--   0        0        0     1749 2023-05-22 15:29:01.285731 deep_astro_uda-0.3.0/deep_astro_uda/client/commands/demo_command.py
+-rw-r--r--   0        0        0      228 2023-05-22 15:13:37.003588 deep_astro_uda-0.3.0/deep_astro_uda/client/commands/infer_command.py
+-rw-r--r--   0        0        0     3741 2023-05-22 15:32:26.340255 deep_astro_uda-0.3.0/deep_astro_uda/client/commands/run_command.py
+-rw-r--r--   0        0        0      754 2023-05-22 15:20:26.176305 deep_astro_uda-0.3.0/deep_astro_uda/client/options.py
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007013 deep_astro_uda-0.3.0/deep_astro_uda/configs/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-22 13:30:21.731901 deep_astro_uda-0.3.0/deep_astro_uda/configs/config.yaml
+-rw-r--r--   0        0        0     2029 2023-05-22 15:34:02.169038 deep_astro_uda-0.3.0/deep_astro_uda/configs/config_functions.py
+-rw-r--r--   0        0        0        0 2023-05-08 03:56:27.706969 deep_astro_uda-0.3.0/deep_astro_uda/data_utils/__init__.py
+-rw-r--r--   0        0        0     2908 2023-05-08 05:07:18.180392 deep_astro_uda-0.3.0/deep_astro_uda/data_utils/download_data.py
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007291 deep_astro_uda-0.3.0/deep_astro_uda/dist/__init__.py
+-rw-r--r--   0        0        0    10906 2023-05-07 23:05:47.007467 deep_astro_uda-0.3.0/deep_astro_uda/dist/deep_astro_uda-0.1.0.tar.gz
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007637 deep_astro_uda-0.3.0/deep_astro_uda/model/__init__.py
+-rw-r--r--   0        0        0     6696 2023-05-22 12:36:09.942437 deep_astro_uda-0.3.0/deep_astro_uda/model/eval.py
+-rw-r--r--   0        0        0     5632 2023-05-07 23:05:47.007756 deep_astro_uda-0.3.0/deep_astro_uda/model/get_loader.py
+-rw-r--r--   0        0        0     4146 2023-05-07 23:05:47.007876 deep_astro_uda-0.3.0/deep_astro_uda/model/loss.py
+-rw-r--r--   0        0        0      465 2023-05-07 23:05:47.007980 deep_astro_uda-0.3.0/deep_astro_uda/model/lr_schedule.py
+-rw-r--r--   0        0        0     7913 2023-05-22 12:36:19.983415 deep_astro_uda-0.3.0/deep_astro_uda/model/train.py
+-rw-r--r--   0        0        0      459 2023-05-22 13:15:04.892342 deep_astro_uda-0.3.0/deep_astro_uda/settings.py
+-rw-r--r--   0        0        0     6468 2023-05-07 23:05:47.009742 deep_astro_uda-0.3.0/deep_astro_uda/tuner/tuner.py
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.008275 deep_astro_uda-0.3.0/deep_astro_uda/utils/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-07 23:05:47.008398 deep_astro_uda-0.3.0/deep_astro_uda/utils/utils.py
+-rw-r--r--   0        0        0      450 2023-05-22 15:36:58.755484 deep_astro_uda-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    16225 1970-01-01 00:00:00.000000 deep_astro_uda-0.3.0/PKG-INFO
```

### Comparing `deep_astro_uda-0.2.6/LICENSE` & `deep_astro_uda-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/README.md` & `deep_astro_uda-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/client/astro_app.py` & `deep_astro_uda-0.3.0/deep_astro_uda/client/astro_app.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/client/commands/demo_command.py` & `deep_astro_uda-0.3.0/deep_astro_uda/client/commands/demo_command.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/client/commands/run_command.py` & `deep_astro_uda-0.3.0/deep_astro_uda/client/commands/run_command.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/client/options.py` & `deep_astro_uda-0.3.0/deep_astro_uda/client/options.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/configs/config.yaml` & `deep_astro_uda-0.3.0/deep_astro_uda/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/configs/config_functions.py` & `deep_astro_uda-0.3.0/deep_astro_uda/configs/config_functions.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/data_utils/download_data.py` & `deep_astro_uda-0.3.0/deep_astro_uda/data_utils/download_data.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/dist/deep_astro_uda-0.1.0.tar.gz` & `deep_astro_uda-0.3.0/deep_astro_uda/dist/deep_astro_uda-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/model/eval.py` & `deep_astro_uda-0.3.0/deep_astro_uda/model/eval.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/model/get_loader.py` & `deep_astro_uda-0.3.0/deep_astro_uda/model/get_loader.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/model/loss.py` & `deep_astro_uda-0.3.0/deep_astro_uda/model/loss.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/model/train.py` & `deep_astro_uda-0.3.0/deep_astro_uda/model/train.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/tuner/tuner.py` & `deep_astro_uda-0.3.0/deep_astro_uda/tuner/tuner.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/deep_astro_uda/utils/utils.py` & `deep_astro_uda-0.3.0/deep_astro_uda/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.2.6/PKG-INFO` & `deep_astro_uda-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-astro-uda
-Version: 0.2.6
+Version: 0.3.0
 Summary: 
 Author: Ashia Lewis
 Author-email: pantagruelspendulum@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

