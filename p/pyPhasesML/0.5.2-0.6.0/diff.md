# Comparing `tmp/pyPhasesML-0.5.2.tar.gz` & `tmp/pyPhasesML-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.5.2.tar", last modified: Sat May  6 13:02:02 2023, max compression
+gzip compressed data, was "pyPhasesML-0.6.0.tar", last modified: Mon May 22 11:21:10 2023, max compression
```

## Comparing `pyPhasesML-0.5.2.tar` & `pyPhasesML-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.435993 pyPhasesML-0.5.2/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-06 13:02:02.434993 pyPhasesML-0.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.427992 pyPhasesML-0.5.2/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3744 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.430992 pyPhasesML-0.5.2/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17785 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.432993 pyPhasesML-0.5.2/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.433993 pyPhasesML-0.5.2/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.434993 pyPhasesML-0.5.2/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    18633 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.429992 pyPhasesML-0.5.2/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 13:02:02.435993 pyPhasesML-0.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-05-06 13:01:44.000000 pyPhasesML-0.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.302827 pyPhasesML-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-22 11:21:10.302827 pyPhasesML-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.298828 pyPhasesML-0.6.0/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4491 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.300827 pyPhasesML-0.6.0/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    18640 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.301828 pyPhasesML-0.6.0/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.301828 pyPhasesML-0.6.0/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.302827 pyPhasesML-0.6.0/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    18685 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.299827 pyPhasesML-0.6.0/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 11:21:10.303827 pyPhasesML-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-05-22 11:20:47.000000 pyPhasesML-0.6.0/setup.py
```

### Comparing `pyPhasesML-0.5.2/LICENSE` & `pyPhasesML-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/PKG-INFO` & `pyPhasesML-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.5.2
+Version: 0.6.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.5.2/README.md` & `pyPhasesML-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.6.0/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/DataSet.py` & `pyPhasesML-0.6.0/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.6.0/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.6.0/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/Model.py` & `pyPhasesML-0.6.0/pyPhasesML/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import csv
 from abc import ABC, abstractmethod
 from pathlib import Path
 
 from pyPhases.util.Optionizable import Optionizable
+from pyPhases.util.EventBus import EventBus
 
 from .DataSet import DataSet
 
 
 class MetricsDoesNotExist(Exception):
     pass
 
 class AdapterNotImplemented(Exception):
     pass
 
 
-class Model(ABC, Optionizable):
+class Model(ABC, Optionizable, EventBus):
     metrics = {
         "acc": {"name": "acc", "type": "max"},
         "binary_accuracy": {"name": "binary_accuracy", "type": "max"},
         "accuracy": {"name": "accuracy", "type": "max"},
         "kappa": {"name": "kappa", "type": "max"},
         "loss": {"name": "loss", "type": "min"},
     }
```

### Comparing `pyPhasesML-0.5.2/pyPhasesML/ModelManager.py` & `pyPhasesML-0.6.0/pyPhasesML/ModelManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import importlib
 
 from pyPhases import ConfigNotFoundException
+from pyPhases.util.EventBusStatic import EventBusStatic
 
 from .Model import Model
 
 
-class ModelManager:
+class ModelManager(EventBusStatic):
     model: Model = None
     modelOptions = None
     beforeBuild = None
     modelPath = None
 
     @staticmethod
     def getModel(forceReload=False) -> Model:
@@ -31,14 +32,15 @@
         if ModelManager.beforeBuild is not None:
             ModelManager.beforeBuild(model)
 
         model.init()
         model.define()
         model.build()
         ModelManager.model = model
+        ModelManager.trigger("modelLoaded", model)
 
     def validate(config):
         def checkValueInConfig(config, value, valuePath=None):
             checkDict = config if valuePath is None else config[valuePath]
 
             if value not in checkDict:
                 valuePath = value if valuePath is None else valuePath + "." + value
```

### Comparing `pyPhasesML-0.5.2/pyPhasesML/Plugin.py` & `pyPhasesML-0.6.0/pyPhasesML/Plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,11 +11,12 @@
         self.project.systemExporter["ModelExporter"] = "pyPhasesML"
         self.project.systemExporter["MemmapRecordExporter"] = "pyPhasesML"
         
     def initPlugin(self):
         # reload the model everytime the config changed
         def updateModel(changedValue):
             ModelManager.loadModel(self.project)
+            self.project.trigger('modelLoaded', ModelManager.model)
 
         self.project.on("configChanged", updateModel)
 
         self.project.registerExporter(ModelExporter())
```

### Comparing `pyPhasesML-0.5.2/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.6.0/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.6.0/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.6.0/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.6.0/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import gc
 import math
 import os
-import pickle
 import timeit
 
 import numpy as np
 import psutil
 import torch
 import torch.optim as optim
-from pyPhases import CSVLogger
 from tqdm import tqdm
 
+from pyPhases import CSVLogger
+
 from ..DataSet import DataSet, TrainingSetLoader
 from ..Model import Model
 from ..scorer.ScorerTorch import ScorerTorch
 
 
 class ModelTorchAdapter(Model):
     model: torch.nn.Module
@@ -107,17 +107,20 @@
             results = s.scoreAllRecords()
 
             metrics = {m: results[m] for m in s.metrics}
             justPrint = []
 
             if "confusion" in s.results:
                 justPrint.append(s.results["confusion"])
+                
+            self.trigger("trainValidation", results, s)
 
             return metrics, justPrint
 
+        self.trigger("trainValidation", {}, s)
         return None, None
 
     def prepareTargetsForLoss(self, targets, oneHotDecoded=None):
         oneHotDecoded = self.oneHotDecoded if oneHotDecoded is None else oneHotDecoded
         mask = None
         if oneHotDecoded:
             targets = targets.reshape(-1, self.numClasses)
@@ -130,14 +133,15 @@
             if self.ignoreClassIndex is not None:
                 mask = targets != self.ignoreClassIndex
                 targets = targets[mask]
 
         return targets.float(), mask
 
     def train(self, dataset: TrainingSetLoader):
+        self.trigger("trainStart", self)
         if ModelTorchAdapter.useTensorBoard:
             from torch.utils.tensorboard import SummaryWriter
 
             self.summarywriter = SummaryWriter()
 
             for f, title in self.startFigures:
                 self.summarywriter.add_figure(title, f)
@@ -218,14 +222,17 @@
             smoothing = 0.05
         
         model = self.model
         lossCriterion = self.getLossFunction()
         i_epoch = self.startEpoch
         notImprovedSince = 0
         lastImprovdModel = None
+        
+        metricsValues, justPrint = self.evalValidation(dataset.validationData)
+        print(metricsValues)
 
         stopAfterNotImproving = 0 if self.stopAfterNotImproving is None else self.stopAfterNotImproving
 
         while self.maxEpochs is None or i_epoch < self.maxEpochs:
             # Put in train mode
             trainingStartTime = timeit.default_timer()
 
@@ -246,29 +253,41 @@
                 # check if there are any targets left
                 if len(targs) == 0:
                     continue
 
                 # for batchFeat in batchFeats:
                 output = model(batchFeats)
                 output = self.mapOutputForLoss(output, mask)
-                loss = lossCriterion(output, targs)
+                loss = lossCriterion(output, targs.reshape(1, 1))
                 ownStats = hasattr(lossCriterion, "stats")
 
                 if ownStats:
                     processList.set_postfix(ordered_dict=lossCriterion.stats)
                     for stat, value in lossCriterion.stats.items():
                         if stat not in runningStats:
                             runningStats[stat] = value
                         else:
                             runningStats[stat] += value
 
                 # Backpropagation
                 loss.backward()
                 # torch.nn.utils.clip_grad()
                 optimizer.step()
+                
+                
+                # with torch.no_grad():
+                    
+                #     for param, grad in zip(model.parameters(), model.parameters()):
+                #         if param.grad is not None:
+                #             grad *= (batchFeats[1].reshape(grad.shape) != 0).float()  # Zero out the gradient if input is zero
+
+                #     optimizer.step()
+
+                #     for param in model.parameters():
+                #         param.clamp_(0, 1)
 
                 # Perform one optimization step
                 currentBatchLoss = loss.data.cpu().numpy()
                 if np.isnan(currentBatchLoss):
                     model(batchFeats)
                     lossCriterion(output, targs)
                     raise Exception("batch loss should not be a number")
@@ -299,14 +318,15 @@
             runningStats = {n: v / batchesPerEpoch for n, v in runningStats.items()}
 
             i_epoch += 1
             trainingEndTime = timeit.default_timer()
 
             # Get validation accuracy
             metricsValues, justPrint = self.evalValidation(dataset.validationData)
+            print(metricsValues)
 
             metricStrings = []
             metricDiffStrings = []
             metricValuetrings = []
             improved = False
             modelId = "checkpointModel_%i_" % i_epoch
 
@@ -393,14 +413,15 @@
             print("Lowest Loss LR: %f" % minLr)
             print("Suggested LR range max bound: %f" % minLr)
             self.lr_find_lr = lr_find_lr
             self.lr_find_loss = lr_find_loss
 
         self.fullEpochs = i_epoch
         self.metricDefinitions = metricDefinitions
+        self.trigger("trainEnd", self)
         return lastImprovdModel
 
     def getModelPath(self):
         return self.logPath
 
     def build(self):
         torchSeed = 2
```

### Comparing `pyPhasesML-0.5.2/pyPhasesML/config.yaml` & `pyPhasesML-0.6.0/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.6.0/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.6.0/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.6.0/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.6.0/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.6.0/pyPhasesML/scorer/Scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,39 +244,39 @@
             classLikelyhood = predictionSoftMax[:, 1]
         else:
             classLikelyhood = max.reshape(-1)
         return classLikelyhood
 
     def getClassPrediction(self, prediction):
         likelyhood = self.getClassLikelyhood(prediction)
-        prediction = np.full(prediction.shape[0], 0)
-        prediction[likelyhood > self.threshold] = 1
-        return prediction
+        binPrediction = np.full(prediction.shape[0], 0)
+        binPrediction[likelyhood > self.threshold] = 1
+        return binPrediction
 
     def flattenPrediction(self, prediction, binaryLikelyHood=False, threshold=None):
         if binaryLikelyHood and self.numClasses != 2:
             raise Exception("Selected metric only support binary classification at the moment")
         useThreshold = threshold is not None and self.numClasses <= 2
 
         if useThreshold:
             return self.getClassPrediction(prediction)
 
         if self.isHotEncoded(prediction):
-            prediction = prediction.argmax(-1)
+            binPrediction = prediction.argmax(-1)
         else:
             threshhold = self.threshold if useThreshold is None else 0.5
-            prediction = prediction.reshape(-1)
+            binPrediction = prediction.copy().reshape(-1)
             if self.numClasses > 2:
-                prediction = np.floor(prediction)
-                prediction[prediction == self.numClasses] = self.numClasses - 1
-                return np.floor(prediction)
+                binPrediction = np.floor(binPrediction)
+                binPrediction[binPrediction == self.numClasses] = self.numClasses - 1
+                return np.floor(binPrediction)
             else:
-                prediction[prediction >= threshhold] = 1
-                prediction[prediction < threshhold] = 0
-        return prediction
+                binPrediction[binPrediction >= threshhold] = 1
+                binPrediction[binPrediction < threshhold] = 0
+        return binPrediction
 
     def getMetricScorer(self, metricName):
         def score(truth, prediction):
             prediction = self.prepareInput(prediction)
             truth = self.prepareInput(truth)
             prediction = self.preparePrediction(prediction)
             truth = self.prepareTruth(truth)
```

### Comparing `pyPhasesML-0.5.2/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.6.0/pyPhasesML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.5.2
+Version: 0.6.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.5.2/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.6.0/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.2/setup.py` & `pyPhasesML-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.5.2"[1:],
+    version="v0.6.0"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

