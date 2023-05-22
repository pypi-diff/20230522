# Comparing `tmp/install-pybci-0.1.4b8.tar.gz` & `tmp/install-pybci-0.1.4b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.1.4b8.tar", last modified: Mon May 22 01:00:17 2023, max compression
+gzip compressed data, was "install-pybci-0.1.4b9.tar", last modified: Mon May 22 11:54:25 2023, max compression
```

## Comparing `install-pybci-0.1.4b8.tar` & `install-pybci-0.1.4b9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.362795 install-pybci-0.1.4b8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-22 01:00:17.362795 install-pybci-0.1.4b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.358795 install-pybci-0.1.4b8/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.358795 install-pybci-0.1.4b8/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.358795 install-pybci-0.1.4b8/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.358795 install-pybci-0.1.4b8/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.362795 install-pybci-0.1.4b8/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14692 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 01:00:17.362795 install-pybci-0.1.4b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14692 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/setup.py
```

### Comparing `install-pybci-0.1.4b8/LICENSE` & `install-pybci-0.1.4b9/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/PKG-INFO` & `install-pybci-0.1.4b9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b8
+Version: 0.1.4b9
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
 
-[![pybci](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
+[![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
@@ -39,19 +39,16 @@
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI(minimumEpochsRequired = 4)
-while not bci.connected: # check to see if lsl marker and datastream are available
-    bci.Connect()
-    time.sleep(1)
-bci.TrainMode() # now both marker and datastreams available start training on received epochs
+bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
+bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
         currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
         if len(currentMarkers) > 1:  # check there is more then one marker type received
```

### Comparing `install-pybci-0.1.4b8/README.md` & `install-pybci-0.1.4b9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
-[![pybci](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
+[![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
@@ -15,19 +15,16 @@
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI(minimumEpochsRequired = 4)
-while not bci.connected: # check to see if lsl marker and datastream are available
-    bci.Connect()
-    time.sleep(1)
-bci.TrainMode() # now both marker and datastreams available start training on received epochs
+bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
+bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
         currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
         if len(currentMarkers) > 1:  # check there is more then one marker type received
```

### Comparing `install-pybci-0.1.4b8/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.1.4b9/install_pybci.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b8
+Version: 0.1.4b9
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
 
-[![pybci](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
+[![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
@@ -39,19 +39,16 @@
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI(minimumEpochsRequired = 4)
-while not bci.connected: # check to see if lsl marker and datastream are available
-    bci.Connect()
-    time.sleep(1)
-bci.TrainMode() # now both marker and datastreams available start training on received epochs
+bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
+bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
         currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
         if len(currentMarkers) > 1:  # check there is more then one marker type received
```

### Comparing `install-pybci-0.1.4b8/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.1.4b9/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/Configuration/EpochSettings.py` & `install-pybci-0.1.4b9/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.1.4b9/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.1.4b9/pybci/ThreadClasses/ClassifierThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.1.4b9/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.1.4b9/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.1.4b9/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/Utils/Classifier.py` & `install-pybci-0.1.4b9/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.1.4b9/pybci/Utils/FeatureExtractor.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/Utils/LSLScanner.py` & `install-pybci-0.1.4b9/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/pybci/pybci.py` & `install-pybci-0.1.4b9/pybci/pybci.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b8/setup.py` & `install-pybci-0.1.4b9/setup.py`

 * *Files identical despite different names*

