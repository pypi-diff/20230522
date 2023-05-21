# Comparing `tmp/install-pybci-0.1.4b5.tar.gz` & `tmp/install-pybci-0.1.4b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.1.4b5.tar", last modified: Sun May 21 11:14:36 2023, max compression
+gzip compressed data, was "install-pybci-0.1.4b6.tar", last modified: Sun May 21 22:57:16 2023, max compression
```

## Comparing `install-pybci-0.1.4b5.tar` & `install-pybci-0.1.4b6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-21 11:14:04.000000 install-pybci-0.1.4b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 11:14:04.000000 install-pybci-0.1.4b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-21 11:14:04.000000 install-pybci-0.1.4b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/setup.py
```

### Comparing `install-pybci-0.1.4b5/LICENSE` & `install-pybci-0.1.4b6/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/PKG-INFO` & `install-pybci-0.1.4b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b5
+Version: 0.1.4b6
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
-[![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)](https://github.com/LMBooth/pybci)
+[![pybci](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
```

### Comparing `install-pybci-0.1.4b5/README.md` & `install-pybci-0.1.4b6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
-[![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)](https://github.com/LMBooth/pybci)
+[![pybci](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
```

### Comparing `install-pybci-0.1.4b5/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.1.4b6/install_pybci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b5
+Version: 0.1.4b6
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
-[![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)](https://github.com/LMBooth/pybci)
+[![pybci](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
```

### Comparing `install-pybci-0.1.4b5/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.1.4b6/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/Configuration/EpochSettings.py` & `install-pybci-0.1.4b6/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.1.4b6/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.1.4b6/pybci/ThreadClasses/ClassifierThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.1.4b6/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.1.4b6/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.1.4b6/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/Utils/Classifier.py` & `install-pybci-0.1.4b6/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.1.4b6/pybci/Utils/FeatureExtractor.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/Utils/LSLScanner.py` & `install-pybci-0.1.4b6/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/pybci/pybci.py` & `install-pybci-0.1.4b6/pybci/pybci.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b5/setup.py` & `install-pybci-0.1.4b6/setup.py`

 * *Files identical despite different names*

