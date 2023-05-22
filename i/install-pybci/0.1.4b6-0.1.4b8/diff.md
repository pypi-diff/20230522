# Comparing `tmp/install-pybci-0.1.4b6.tar.gz` & `tmp/install-pybci-0.1.4b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.1.4b6.tar", last modified: Sun May 21 22:57:16 2023, max compression
+gzip compressed data, was "install-pybci-0.1.4b8.tar", last modified: Mon May 22 01:00:17 2023, max compression
```

## Comparing `install-pybci-0.1.4b6.tar` & `install-pybci-0.1.4b8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 22:57:16.000000 install-pybci-0.1.4b6/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 22:57:16.634513 install-pybci-0.1.4b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-21 22:56:41.000000 install-pybci-0.1.4b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.362795 install-pybci-0.1.4b8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-22 01:00:17.362795 install-pybci-0.1.4b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.358795 install-pybci-0.1.4b8/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 01:00:17.000000 install-pybci-0.1.4b8/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.358795 install-pybci-0.1.4b8/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.358795 install-pybci-0.1.4b8/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.358795 install-pybci-0.1.4b8/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:00:17.362795 install-pybci-0.1.4b8/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14692 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 01:00:17.362795 install-pybci-0.1.4b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-22 00:59:46.000000 install-pybci-0.1.4b8/setup.py
```

### Comparing `install-pybci-0.1.4b6/LICENSE` & `install-pybci-0.1.4b8/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/PKG-INFO` & `install-pybci-0.1.4b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b6
+Version: 0.1.4b8
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `install-pybci-0.1.4b6/README.md` & `install-pybci-0.1.4b8/README.md`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.1.4b8/install_pybci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b6
+Version: 0.1.4b8
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `install-pybci-0.1.4b6/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.1.4b8/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/pybci/Configuration/EpochSettings.py` & `install-pybci-0.1.4b8/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.1.4b8/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.1.4b8/pybci/ThreadClasses/ClassifierThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.1.4b8/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.1.4b8/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.1.4b8/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/pybci/Utils/Classifier.py` & `install-pybci-0.1.4b8/pybci/Utils/Classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,18 @@
         if self.model != None: # maybe requires actual check for tensorflow model
             self.classifierLibrary = "tensor"
         elif self.clf != None: # maybe requires actual check for sklearn clf
             self.classifierLibrary = "sklearn"
 
     def TrainModel(self, features, targets):
         # check for nans and infs in feature creation, not here
-        if (len(np.array(features).shape) == 3):
-            features  = np.array(features).reshape(np.array(features).shape[0], -1)
-        else:
-            features = np.array(features)
+        #if (len(np.array(features).shape) == 3):
+        #    features  = np.array(features).reshape(np.array(features).shape[0], -1)
+        #else:
+        #    features = np.array(features)
         #features = np.where(np.isnan(features), 0, features)
         #self.targets = targets
         #print(features.shape)
         x_train, x_test, y_train, y_test = train_test_split(features, targets, shuffle = True, test_size=0.2)
         #print("training model")
         if self.classifierLibrary == "sklearn":
             if all(item == y_train[0] for item in y_train):
@@ -58,33 +58,37 @@
             # no classifier library selected, print debug?
             pass
 
     def TestModel(self, x):
         # needs check for nans and infs
         #print(x)
         #print(np.array(x).shape)
-        if (len(np.array(x).shape) == 2):
-            #x = np.array(x).reshape(np.array(x).shape[0], -1)
-            x = np.array([x.flatten()])
-        else:
-            x = np.array(x)
+        #if (len(np.array(x).shape) == 2):
+        #    #x = np.array(x).reshape(np.array(x).shape[0], -1)
+        #    x = np.array([x.flatten()])
+        #else:
+        #    x = np.array(x)
         #print(x)
         #print(x.shape)
         if self.classifierLibrary == "sklearn":
+            x = np.expand_dims(x, axis=0)
             return self.clf.predict(x)
             #print("we predict it's: "+str(self.y_pred))
         elif self.classifierLibrary == "tensor":
             # Predict the class labels for the test data
             #print(x)
-            #print(x.shape)
-            return self.model.predict(np.reshape(x, (1, len(x))))
-
+            x = np.expand_dims(x, axis=0)
+            predictions = self.model.predict(x)
+            if len (predictions[0]) == 1: # assume binary classification
+                return 1 if predictions[0] > 0.5 else 0
+            else:    # assume multi-classification
+                return np.argmax(predictions[0])
             #print("we predict it's: "+str(y_pred))
             # Convert the predicted probabilities to class labels
-            y_pred_classes = np.argmax(self.y_pred, axis=1)
+            #y_pred_classes = np.argmax(self.y_pred, axis=1)
             #print("if class label: "+str(y_pred_classes))
         else:
             print("no classifier library selected")
             # no classifier library selected, print debug?
             pass
 
 '''
```

### Comparing `install-pybci-0.1.4b6/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.1.4b8/pybci/Utils/FeatureExtractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,75 +45,76 @@
             sr = samplerate of current device
         Returns:
             features = 2D numpy array of size (chs, (len(freqbands) + sum(True in self.featureChoices)))
             target = same as input target
         NOTE: Any channels with a constant value will generate warnings in any frequency based features (constant level == no frequency components).
         """
         #print(np.array(epoch).shape)
-        features = np.zeros((len(epoch),self.numFeatures))
+        numchs = len(epoch)
+        features = np.zeros(numchs * self.numFeatures)
         for k, ch in enumerate(epoch):
             if self.featureChoices.psdBand: # get custom average power within given frequency band from freqbands
                 freqs, psd = welch(ch, sr)
                 for l, band in enumerate(self.freqbands):
                     if len(freqs) > 0: # len(freqs) can be 0 if signal is all DC
                         idx_band = np.logical_and(freqs >= band[0], freqs <= band[1])
                         #if len(psd[idx_band]) == 1: # if freq band is only in one field just pass single value instead of calculating average
                         #print(ch)
                         bp = np.mean(psd[idx_band])
                         #else:
                         #    bp = simps(psd[idx_band], dx=(freqs[1]-freqs[0])) / (band[1] - band[0])
                             #bp = simpson(psd[idx_band], dx=freq_res)
-                        features[k][l] = bp
+                        features[(k*numchs)+l] = bp
                     else:
-                        features[k][l] = 0
+                        features[(k*numchs)+l] = 0
             else:
                 freqs, psd = welch(ch, sr)# calculate for mean and median
                 l = -1 # accounts for no freqbands being selected
             if self.featureChoices.meanPSD: # mean power
                 l += 1
-                if len(freqs) > 0: features[k][l] = np.mean(psd) # len(freqs) can be 0 if signal is all DC
-                else: features[k][l] = 0
+                if len(freqs) > 0: features[(k*numchs)+l] = np.mean(psd) # len(freqs) can be 0 if signal is all DC
+                else: features[(k*numchs)+l] = 0
             if self.featureChoices.medianPSD: # median Power
                 l += 1   
-                if len(freqs) > 0: features[k][l] = np.median(psd) # len(freqs) can be 0 if signal is all DC
-                else: features[k][l] = 0
+                if len(freqs) > 0: features[(k*numchs)+l] = np.median(psd) # len(freqs) can be 0 if signal is all DC
+                else: features[(k*numchs)+l] = 0
             if self.featureChoices.appr_entropy:  # Approximate entorpy(X,M,R) X = data, M is , R is 30% standard deviation of X 
                 l += 1
-                features[k][l] = ant.app_entropy(ch) 
+                features[(k*numchs)+l] = ant.app_entropy(ch) 
             if self.featureChoices.perm_entropy: # permutation_entropy
                 l += 1
-                features[k][l] = ant.perm_entropy(ch,normalize=True)
+                features[(k*numchs)+l] = ant.perm_entropy(ch,normalize=True)
             if self.featureChoices.spec_entropy:  # spectral Entropy
                 l += 1
-                features[k][l] = ant.spectral_entropy(ch, sf=sr, method='welch', nperseg = len(ch), normalize=True)
+                features[(k*numchs)+l] = ant.spectral_entropy(ch, sf=sr, method='welch', nperseg = len(ch), normalize=True)
             if self.featureChoices.svd_entropy:# svd Entropy
                 l += 1
-                features[k][l] = ant.svd_entropy(ch, normalize=True)
+                features[(k*numchs)+l] = ant.svd_entropy(ch, normalize=True)
             if self.featureChoices.samp_entropy: # sample Entropy
                 l += 1
-                features[k][l] = ant.sample_entropy(ch)
+                features[(k*numchs)+l] = ant.sample_entropy(ch)
             if self.featureChoices.rms: # rms
                 l += 1
-                features[k][l] = np.sqrt(np.mean(np.array(ch)**2))
+                features[(k*numchs)+l] = np.sqrt(np.mean(np.array(ch)**2))
             if self.featureChoices.variance: # variance
                 l += 1    
-                features[k][l] =  np.var(ch)
+                features[(k*numchs)+l] =  np.var(ch)
             if self.featureChoices.meanAbs: # Mean Absolute Value 
                 l += 1
-                features[k][l] = sum([np.linalg.norm(c) for c in ch])/len(ch)
+                features[(k*numchs)+l] = sum([np.linalg.norm(c) for c in ch])/len(ch)
             if self.featureChoices.waveformLength: # waveformLength
                 l += 1
-                features[k][l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
+                features[(k*numchs)+l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
             if self.featureChoices.zeroCross: # zeroCross
                 l += 1
-                features[k][l] = sum([1 if c*ch[inum+1]<0 else 0 for inum, c in enumerate(ch[:-1])])
+                features[(k*numchs)+l] = sum([1 if c*ch[inum+1]<0 else 0 for inum, c in enumerate(ch[:-1])])
             if self.featureChoices.slopeSignChange: # slopeSignChange
                 l += 1    
                 ssc = sum([1 if (c-ch[inum+1])*(c-ch[inum+1])>=0.1 else 0 for inum, c in enumerate(ch[:-1])])
-                features[k][l] = ssc
+                features[(k*numchs)+l] = ssc
         features[np.isnan(features)] = 0 # checks for nans
         features[features == np.inf] = 0 # checks for infs
         return features
     
 class GazeFeatureExtractor():
     def __init__(self):
         super().__init__()
```

### Comparing `install-pybci-0.1.4b6/pybci/Utils/LSLScanner.py` & `install-pybci-0.1.4b8/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b6/pybci/pybci.py` & `install-pybci-0.1.4b8/pybci/pybci.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .ThreadClasses.AsyncDataReceiverThread import AsyncDataReceiverThread
 from .ThreadClasses.MarkerThread import MarkerThread
 from .ThreadClasses.ClassifierThread import ClassifierThread
 from .Configuration.EpochSettings import GlobalEpochSettings, IndividualEpochSetting
 from .Configuration.FeatureSettings import GeneralFeatureChoices
 import queue, threading, copy
 import tensorflow as tf
+tf.get_logger().setLevel('ERROR')
 
 class PyBCI:
     printDebug = True   # boolean, used to toggle print statements from LSLScanner class
     globalEpochSettings = GlobalEpochSettings()
     customEpochSettings = {}
     minimumEpochsRequired = 10
     markerThread = []
@@ -47,14 +48,15 @@
         """
         self.streamCustomFeatureExtract = streamCustomFeatureExtract
         self.globalEpochSettings = globalEpochSettings
         self.customEpochSettings = customEpochSettings
         self.streamChsDropDict = streamChsDropDict
         self.lslScanner = LSLScanner(self, dataStreams, markerStream,streamTypes, markerTypes)
         self.printDebug = printDebug
+        #if self.printDebug == False:
         self.ConfigureMachineLearning(minimumEpochsRequired,  clf, model) # configure first, connect second
         self.Connect()
        
     def __enter__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, printDebug = True,
                  globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}, streamChsDropDict = {},
                  freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()): # with bci
         self.freqbands = freqbands
```

### Comparing `install-pybci-0.1.4b6/setup.py` & `install-pybci-0.1.4b8/setup.py`

 * *Files identical despite different names*

