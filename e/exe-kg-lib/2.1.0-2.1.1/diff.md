# Comparing `tmp/exe_kg_lib-2.1.0.tar.gz` & `tmp/exe_kg_lib-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exe_kg_lib-2.1.0.tar", max compression
+gzip compressed data, was "exe_kg_lib-2.1.1.tar", max compression
```

## Comparing `exe_kg_lib-2.1.0.tar` & `exe_kg_lib-2.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34283 2023-05-22 09:12:03.358684 exe_kg_lib-2.1.0/LICENSE.md
--rw-r--r--   0        0        0    15902 2023-05-22 09:12:03.358684 exe_kg_lib-2.1.0/README.md
--rw-r--r--   0        0        0       27 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/__init__.py
--rw-r--r--   0        0        0      102 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/__init__.py
--rw-r--r--   0        0        0     1253 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/data_entity.py
--rw-r--r--   0        0        0      788 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/entity.py
--rw-r--r--   0        0        0    32574 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/exe_kg.py
--rw-r--r--   0        0        0      773 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/kg_schema.py
--rw-r--r--   0        0        0     3528 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/task.py
--rw-r--r--   0        0        0     1914 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/README.md
--rw-r--r--   0        0        0        0 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/__init__.py
--rw-r--r--   0        0        0     5619 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/ml_tasks.py
--rw-r--r--   0        0        0     1967 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/statistic_tasks.py
--rw-r--r--   0        0        0     3108 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/visual_tasks.py
--rw-r--r--   0        0        0        0 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/cli/__init__.py
--rw-r--r--   0        0        0      938 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/cli/main.py
--rw-r--r--   0        0        0        0 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/shacl/__init__.py
--rw-r--r--   0        0        0     1967 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/shacl/base_shape_graph_generator.py
--rw-r--r--   0        0        0    26612 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/shacl/shacl_shape_graph.ttl
--rw-r--r--   0        0        0      108 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/__init__.py
--rw-r--r--   0        0        0     3130 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/cli_utils.py
--rw-r--r--   0        0        0     7290 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/kg_creation_utils.py
--rw-r--r--   0        0        0      809 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/kg_validation_utils.py
--rw-r--r--   0        0        0     6378 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/query_utils.py
--rw-r--r--   0        0        0      679 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/string_utils.py
--rw-r--r--   0        0        0        0 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/task_utils/__init__.py
--rw-r--r--   0        0        0     2660 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/task_utils/ml_utils.py
--rw-r--r--   0        0        0     2606 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/task_utils/statistic_utils.py
--rw-r--r--   0        0        0     2388 2023-05-22 09:12:03.362684 exe_kg_lib-2.1.0/exe_kg_lib/utils/task_utils/visual_utils.py
--rw-r--r--   0        0        0     4184 2023-05-22 09:12:25.059020 exe_kg_lib-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    17344 1970-01-01 00:00:00.000000 exe_kg_lib-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34283 2023-05-22 14:31:05.871165 exe_kg_lib-2.1.1/LICENSE.md
+-rw-r--r--   0        0        0    15902 2023-05-22 14:31:05.871165 exe_kg_lib-2.1.1/README.md
+-rw-r--r--   0        0        0       27 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/__init__.py
+-rw-r--r--   0        0        0     1253 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/data_entity.py
+-rw-r--r--   0        0        0      788 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/entity.py
+-rw-r--r--   0        0        0    32574 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/exe_kg.py
+-rw-r--r--   0        0        0      773 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/kg_schema.py
+-rw-r--r--   0        0        0     3528 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/task.py
+-rw-r--r--   0        0        0     1914 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/__init__.py
+-rw-r--r--   0        0        0     5619 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/ml_tasks.py
+-rw-r--r--   0        0        0     1967 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/statistic_tasks.py
+-rw-r--r--   0        0        0     3108 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/visual_tasks.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/cli/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/shacl/__init__.py
+-rw-r--r--   0        0        0     1967 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/shacl/base_shape_graph_generator.py
+-rw-r--r--   0        0        0    26612 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/shacl/shacl_shape_graph.ttl
+-rw-r--r--   0        0        0      108 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/__init__.py
+-rw-r--r--   0        0        0     3130 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/cli_utils.py
+-rw-r--r--   0        0        0     7290 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/kg_creation_utils.py
+-rw-r--r--   0        0        0      809 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/kg_validation_utils.py
+-rw-r--r--   0        0        0     6378 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/query_utils.py
+-rw-r--r--   0        0        0      679 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/string_utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/task_utils/__init__.py
+-rw-r--r--   0        0        0     2660 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/task_utils/ml_utils.py
+-rw-r--r--   0        0        0     2606 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/task_utils/statistic_utils.py
+-rw-r--r--   0        0        0     2388 2023-05-22 14:31:05.875165 exe_kg_lib-2.1.1/exe_kg_lib/utils/task_utils/visual_utils.py
+-rw-r--r--   0        0        0     4184 2023-05-22 14:31:27.455124 exe_kg_lib-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    17344 1970-01-01 00:00:00.000000 exe_kg_lib-2.1.1/PKG-INFO
```

### Comparing `exe_kg_lib-2.1.0/LICENSE.md` & `exe_kg_lib-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/README.md` & `exe_kg_lib-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 1. **ML pipeline**: Loads features and labels from an input CSV dataset, splits the data, trains and tests a k-NN model, and visualizes the prediction errors.
 2. **Statistics pipeline**: Loads a feature from an input CSV dataset, normalizes it, and plots its values (before and after normalization) using a scatter plot.
 3. **Visualization pipeline**: Loads a feature from an input CSV dataset and plots its values using a line plot.
 
 Under the hood, **ExeKGLib** uses well-known Python libraries for data processing and visualization and performing predictions such as [pandas](https://pandas.pydata.org/), [matplotlib](https://matplotlib.org/), and [scikit-learn](https://scikit-learn.org/).
 
-**ExeKGLib** is part of the following paper submitted to ESWC 2023:<br>
+**ExeKGLib** is part of the following paper submitted to ISWC 2023:<br>
 _Klironomos A., Zhou B., Tan Z., Zheng Z., Gad-Elrab M., Paulheim H., Kharlamov E.: **ExeKGLib: A Python Library for Machine Learning Analytics based on Knowledge Graphs**_
 
 [//]: # (--8<-- [end:overview])
 
 Detailed information (installation, documentation etc.) about **ExeKGLib** can be found in [its website](https://boschresearch.github.io/ExeKGLib/) and basic information is shown below.
 
 ## Installation
```

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/data_entity.py` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/data_entity.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/entity.py` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/entity.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/exe_kg.py` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/exe_kg.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/kg_schema.py` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/kg_schema.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/task.py` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/task.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/README.md` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/README.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/ml_tasks.py` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/ml_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/statistic_tasks.py` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/statistic_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/classes/tasks/visual_tasks.py` & `exe_kg_lib-2.1.1/exe_kg_lib/classes/tasks/visual_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/cli/main.py` & `exe_kg_lib-2.1.1/exe_kg_lib/cli/main.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/shacl/base_shape_graph_generator.py` & `exe_kg_lib-2.1.1/exe_kg_lib/shacl/base_shape_graph_generator.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/shacl/shacl_shape_graph.ttl` & `exe_kg_lib-2.1.1/exe_kg_lib/shacl/shacl_shape_graph.ttl`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/utils/cli_utils.py` & `exe_kg_lib-2.1.1/exe_kg_lib/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/utils/kg_creation_utils.py` & `exe_kg_lib-2.1.1/exe_kg_lib/utils/kg_creation_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/utils/kg_validation_utils.py` & `exe_kg_lib-2.1.1/exe_kg_lib/utils/kg_validation_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/utils/query_utils.py` & `exe_kg_lib-2.1.1/exe_kg_lib/utils/query_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/utils/string_utils.py` & `exe_kg_lib-2.1.1/exe_kg_lib/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/utils/task_utils/ml_utils.py` & `exe_kg_lib-2.1.1/exe_kg_lib/utils/task_utils/ml_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/utils/task_utils/statistic_utils.py` & `exe_kg_lib-2.1.1/exe_kg_lib/utils/task_utils/statistic_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/exe_kg_lib/utils/task_utils/visual_utils.py` & `exe_kg_lib-2.1.1/exe_kg_lib/utils/task_utils/visual_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.1.0/pyproject.toml` & `exe_kg_lib-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exe-kg-lib"
-version = "2.1.0" # not used when bumping version via poe bump-version-tag or cd.yaml
+version = "2.1.1" # not used when bumping version via poe bump-version-tag or cd.yaml
 description = "Library for executable ML pipelines represented by KGs."
 license = "AGPL-3.0"
 authors = ["Antonis Klironomos <antonis.klironomos@de.bosch.com>", "Mohamed Gad-Elrab <mohamed.gad-elrab@de.bosch.com>"]
 
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Developers",
```

### Comparing `exe_kg_lib-2.1.0/PKG-INFO` & `exe_kg_lib-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exe-kg-lib
-Version: 2.1.0
+Version: 2.1.1
 Summary: Library for executable ML pipelines represented by KGs.
 Home-page: https://boschresearch.github.io/ExeKGLib
 License: AGPL-3.0
 Author: Antonis Klironomos
 Author-email: antonis.klironomos@de.bosch.com
 Maintainer: Antonis Klironomos
 Maintainer-email: antonis.klironomos@de.bosch.com
@@ -52,15 +52,15 @@
 
 1. **ML pipeline**: Loads features and labels from an input CSV dataset, splits the data, trains and tests a k-NN model, and visualizes the prediction errors.
 2. **Statistics pipeline**: Loads a feature from an input CSV dataset, normalizes it, and plots its values (before and after normalization) using a scatter plot.
 3. **Visualization pipeline**: Loads a feature from an input CSV dataset and plots its values using a line plot.
 
 Under the hood, **ExeKGLib** uses well-known Python libraries for data processing and visualization and performing predictions such as [pandas](https://pandas.pydata.org/), [matplotlib](https://matplotlib.org/), and [scikit-learn](https://scikit-learn.org/).
 
-**ExeKGLib** is part of the following paper submitted to ESWC 2023:<br>
+**ExeKGLib** is part of the following paper submitted to ISWC 2023:<br>
 _Klironomos A., Zhou B., Tan Z., Zheng Z., Gad-Elrab M., Paulheim H., Kharlamov E.: **ExeKGLib: A Python Library for Machine Learning Analytics based on Knowledge Graphs**_
 
 [//]: # (--8<-- [end:overview])
 
 Detailed information (installation, documentation etc.) about **ExeKGLib** can be found in [its website](https://boschresearch.github.io/ExeKGLib/) and basic information is shown below.
 
 ## Installation
```

