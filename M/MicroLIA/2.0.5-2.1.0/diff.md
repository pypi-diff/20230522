# Comparing `tmp/MicroLIA-2.0.5.tar.gz` & `tmp/MicroLIA-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MicroLIA-2.0.5.tar", last modified: Fri Apr 14 06:45:27 2023, max compression
+gzip compressed data, was "MicroLIA-2.1.0.tar", last modified: Mon May 22 20:42:30 2023, max compression
```

## Comparing `MicroLIA-2.0.5.tar` & `MicroLIA-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-14 06:45:27.257535 MicroLIA-2.0.5/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2022-10-18 03:09:36.000000 MicroLIA-2.0.5/LICENSE.txt
--rw-r--r--   0 daniel     (501) staff       (20)       37 2022-10-18 03:09:36.000000 MicroLIA-2.0.5/MANIFEST.in
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-14 06:45:27.240343 MicroLIA-2.0.5/MicroLIA/
--rwxr-xr-x   0 daniel     (501) staff       (20)      365 2022-08-12 15:04:07.000000 MicroLIA-2.0.5/MicroLIA/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)   172040 2023-04-14 06:01:24.000000 MicroLIA-2.0.5/MicroLIA/cnn_model.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-14 06:45:27.254087 MicroLIA-2.0.5/MicroLIA/data/
--rwxr-xr-x   0 daniel     (501) staff       (20)  1384833 2022-07-17 06:13:15.000000 MicroLIA-2.0.5/MicroLIA/data/Miras_vo.xml
--rwxr-xr-x   0 daniel     (501) staff       (20)       26 2022-07-17 06:13:15.000000 MicroLIA-2.0.5/MicroLIA/data/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    36126 2023-04-14 06:02:09.000000 MicroLIA-2.0.5/MicroLIA/data_augmentation.py
--rw-r--r--   0 daniel     (501) staff       (20)    12888 2023-04-14 06:05:32.000000 MicroLIA-2.0.5/MicroLIA/data_processing.py
--rw-r--r--   0 daniel     (501) staff       (20)    54677 2023-04-14 06:20:00.000000 MicroLIA-2.0.5/MicroLIA/ensemble_model.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     5250 2023-03-30 05:00:56.000000 MicroLIA-2.0.5/MicroLIA/extract_features.py
--rwxr-xr-x   0 daniel     (501) staff       (20)   117151 2023-03-30 03:46:20.000000 MicroLIA-2.0.5/MicroLIA/features.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     2719 2023-03-19 23:16:44.000000 MicroLIA-2.0.5/MicroLIA/noise_models.py
--rw-r--r--   0 daniel     (501) staff       (20)   130007 2023-04-14 05:58:12.000000 MicroLIA-2.0.5/MicroLIA/optimization.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     4419 2023-02-26 05:00:18.000000 MicroLIA-2.0.5/MicroLIA/quality_check.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    12914 2023-02-26 04:59:36.000000 MicroLIA-2.0.5/MicroLIA/simulate.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    25733 2023-04-14 06:18:09.000000 MicroLIA-2.0.5/MicroLIA/training_set.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-14 06:45:27.246483 MicroLIA-2.0.5/MicroLIA.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      572 2023-04-14 06:45:27.000000 MicroLIA-2.0.5/MicroLIA.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      569 2023-04-14 06:45:27.000000 MicroLIA-2.0.5/MicroLIA.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-04-14 06:45:27.000000 MicroLIA-2.0.5/MicroLIA.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)      178 2023-04-14 06:45:27.000000 MicroLIA-2.0.5/MicroLIA.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        9 2023-04-14 06:45:27.000000 MicroLIA-2.0.5/MicroLIA.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)      572 2023-04-14 06:45:27.257084 MicroLIA-2.0.5/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)     2641 2022-10-18 03:09:36.000000 MicroLIA-2.0.5/README.md
--rw-r--r--   0 daniel     (501) staff       (20)      417 2023-03-07 06:54:07.000000 MicroLIA-2.0.5/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-04-14 06:45:27.257665 MicroLIA-2.0.5/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)     1141 2023-04-14 06:43:17.000000 MicroLIA-2.0.5/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 20:42:30.682300 MicroLIA-2.1.0/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2022-10-18 03:09:36.000000 MicroLIA-2.1.0/LICENSE.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       24 2023-05-22 20:39:52.000000 MicroLIA-2.1.0/MANIFEST.in
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 20:42:30.668140 MicroLIA-2.1.0/MicroLIA/
+-rwxr-xr-x   0 daniel     (501) staff       (20)      365 2022-08-12 15:04:07.000000 MicroLIA-2.1.0/MicroLIA/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)   172657 2023-04-16 16:18:23.000000 MicroLIA-2.1.0/MicroLIA/cnn_model.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 20:42:30.680612 MicroLIA-2.1.0/MicroLIA/data/
+-rw-r--r--   0 daniel     (501) staff       (20)     6148 2023-05-22 19:33:40.000000 MicroLIA-2.1.0/MicroLIA/data/.DS_Store
+-rwxr-xr-x   0 daniel     (501) staff       (20)  1384833 2022-07-17 06:13:15.000000 MicroLIA-2.1.0/MicroLIA/data/Miras_vo.xml
+-rwxr-xr-x   0 daniel     (501) staff       (20)       26 2022-07-17 06:13:15.000000 MicroLIA-2.1.0/MicroLIA/data/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    36126 2023-04-14 06:02:09.000000 MicroLIA-2.1.0/MicroLIA/data_augmentation.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12888 2023-04-14 06:05:32.000000 MicroLIA-2.1.0/MicroLIA/data_processing.py
+-rw-r--r--   0 daniel     (501) staff       (20)    54677 2023-04-14 06:20:00.000000 MicroLIA-2.1.0/MicroLIA/ensemble_model.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     5250 2023-03-30 05:00:56.000000 MicroLIA-2.1.0/MicroLIA/extract_features.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)   117151 2023-03-30 03:46:20.000000 MicroLIA-2.1.0/MicroLIA/features.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     2719 2023-03-19 23:16:44.000000 MicroLIA-2.1.0/MicroLIA/noise_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)   130007 2023-04-14 05:58:12.000000 MicroLIA-2.1.0/MicroLIA/optimization.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     4419 2023-02-26 05:00:18.000000 MicroLIA-2.1.0/MicroLIA/quality_check.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    20101 2023-05-22 20:37:04.000000 MicroLIA-2.1.0/MicroLIA/simulate.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    25740 2023-05-22 20:21:37.000000 MicroLIA-2.1.0/MicroLIA/training_set.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 20:42:30.671665 MicroLIA-2.1.0/MicroLIA.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      593 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      193 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        9 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-22 20:42:30.681843 MicroLIA-2.1.0/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)     2641 2022-10-18 03:09:36.000000 MicroLIA-2.1.0/README.md
+-rw-r--r--   0 daniel     (501) staff       (20)      456 2023-05-22 20:31:54.000000 MicroLIA-2.1.0/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-22 20:42:30.682558 MicroLIA-2.1.0/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1162 2023-05-22 20:32:10.000000 MicroLIA-2.1.0/setup.py
```

### Comparing `MicroLIA-2.0.5/LICENSE.txt` & `MicroLIA-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/cnn_model.py` & `MicroLIA-2.1.0/MicroLIA/cnn_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1246,41 +1246,44 @@
         
         if savefig:
             plt.savefig('CNN_Training_History_'+metric+'.png', bbox_inches='tight', dpi=300)
             plt.clf()
         else:
             plt.show()
 
-    def _plot_positive(self, index=0, channel=0, default_scale=False, vmin=None, vmax=None, cmap='gray', title=''):
+    def _plot_positive(self, index=0, channel=0, default_scale=True, vmin=None, vmax=None, cmap='gray', title=''):
         """
         Plots the sample in the ``positive`` class, located an the specified index.
 
         The channel parameter determines what filter to display, must be less than
         or equal to the ``img_num_channels`` - 1, or 'all', to plot a colorized image.
 
         The plotting procedure employs the matplotlib imshow display, with a robust
         vmin and vmax, unless these are set as arguments.
     
         Args:
             index (int): The index of the sample to be displayed. Defaults to 0.
             channel (int): The channel to plot, can be 0, 1, 2, or 'all'. Defaults to 0.  
             default_scale (bool): If True the figure will be generated using the matplotlib 
                 imshow display, using the default scaling. If False, the vmin and vmax arguments must
-                be input. Defaults to True. 
+                be input, otherwise a robust vmin and vmax will be calculated. Defaults to True. 
             vmin (float): The vmin to control the colorbar scaling.
             vmax (float): The vmax to control the colorbar scaling. 
             cmap (str): Colormap to use when generating the image.
             title (str, optional): Title displayed above the image. 
 
         Returns:
             AxesImage.
         """
 
-
-        data = self.positive_class[index]
+        if len(self.positive_class.shape) == 3:
+            data = self.positive_class.reshape(self.positive_class.shape[0], self.positive_class.shape[1], self.positive_class.shape[2], 1)
+            data = data[index]
+        else:
+            data = self.positive_class[index]
 
         if channel == 'all':
             if vmin is None and default_scale is False:
                 plot(data)
             else:
                 if default_scale is False:
                     plt.imshow(data[:,:,channel], vmin=vmin, vmax=vmax, cmap=cmap); plt.title(title); plt.show()
@@ -1295,40 +1298,44 @@
             if default_scale is False:
                 plt.imshow(data[:,:,channel], vmin=vmin, vmax=vmax, cmap=cmap); plt.title(title); plt.show()
             else:
                 plt.imshow(data[:,:,channel], cmap=cmap); plt.title(title); plt.show()
           
         return
 
-    def _plot_negative(self, index=0, channel=1, default_scale=False, vmin=None, vmax=None, cmap='gray', title=''):
+    def _plot_negative(self, index=0, channel=0, default_scale=True, vmin=None, vmax=None, cmap='gray', title=''):
         """
         Plots the sample in the ``negative`` class, located an the specified index.
 
         The channel parameter determines what filter to display, must be less than
         or equal to the ``img_num_channels`` - 1, or 'all', to plot a colorized image.
 
         The plotting procedure employs the matplotlib imshow display, with a robust
         vmin and vmax, unless these are set as arguments.
     
         Args:
             index (int): The index of the sample to be displayed. Defaults to 0.
             channel (int): The channel to plot, can be 0, 1, 2, or 'all'. Defaults to 0.  
             default_scale (bool): If True the figure will be generated using the matplotlib 
                 imshow display, using the default scaling. If False, the vmin and vmax arguments must
-                be input. Defaults to True.     
+                be input, otherwise a robust vmin and vmax will be calculated. Defaults to True. 
             cmap (str): Colormap to use when generating the image.
             vmin (float): The vmin to control the colorbar scaling.
             vmax (float): The vmax to control the colorbar scaling. 
             title (str, optional): Title displayed above the image. 
 
         Returns:
             AxesImage.
         """
 
-        data = self.negative_class[index]
+        if len(self.negative_class.shape) == 3:
+            data = self.negative_class.reshape(self.negative_class.shape[0], self.negative_class.shape[1], self.negative_class.shape[2], 1)
+            data = data[index]
+        else:
+            data = self.negative_class[index]
 
         if channel == 'all':
             if vmin is None and default_scale is False:
                 plot(data)
             else:
                 if default_scale is False:
                     plt.imshow(data[:,:,channel], vmin=vmin, vmax=vmax, cmap=cmap); plt.title(title); plt.show()
@@ -1339,14 +1346,15 @@
 
         if vmin is None and default_scale is False:
             plot(data[:,:,channel])
         else:   
             if default_scale is False:
                 plt.imshow(data[:,:,channel], vmin=vmin, vmax=vmax, cmap=cmap); plt.title(title); plt.show()
             else:
+                import pdb; pdb.set_trace()
                 plt.imshow(data[:,:,channel], vmin=vmin, vmax=vmax, cmap=cmap); plt.title(title); plt.show()
 
         return
 
 #Custom CNN model configured to genereate shallower CNNs than AlexNet
 
 def custom_model(positive_class, negative_class, img_num_channels=1, normalize=True,
```

### Comparing `MicroLIA-2.0.5/MicroLIA/data/Miras_vo.xml` & `MicroLIA-2.1.0/MicroLIA/data/Miras_vo.xml`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/data_augmentation.py` & `MicroLIA-2.1.0/MicroLIA/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/data_processing.py` & `MicroLIA-2.1.0/MicroLIA/data_processing.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/ensemble_model.py` & `MicroLIA-2.1.0/MicroLIA/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/extract_features.py` & `MicroLIA-2.1.0/MicroLIA/extract_features.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/features.py` & `MicroLIA-2.1.0/MicroLIA/features.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/noise_models.py` & `MicroLIA-2.1.0/MicroLIA/noise_models.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/optimization.py` & `MicroLIA-2.1.0/MicroLIA/optimization.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/quality_check.py` & `MicroLIA-2.1.0/MicroLIA/quality_check.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/MicroLIA/training_set.py` & `MicroLIA-2.1.0/MicroLIA/training_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     source_class_list=[]
     stats_list = []
 
     progess_bar = bar.FillingSquaresBar('Simulating variables......', max=n_class)
     for k in range(1,n_class+1):
         time = random.choice(timestamps)
         baseline = np.random.uniform(min_mag,max_mag)
-        mag, amplitude, period = simulate.variable(time,baseline)
+        mag, amplitude, period = simulate.rrlyr_variable(time, baseline)
            
         if noise is not None:
             mag, magerr = noise_models.add_noise(mag, noise, zp=zp, exptime=exptime)
         if noise is None:
            mag, magerr = noise_models.add_gaussian_noise(mag, zp=zp, exptime=exptime)
            
         source_class = ['VARIABLE']*len(time)
```

### Comparing `MicroLIA-2.0.5/MicroLIA.egg-info/PKG-INFO` & `MicroLIA-2.1.0/MicroLIA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicroLIA
-Version: 2.0.5
+Version: 2.1.0
 Summary: Machine learning classifier for microlensing
 Home-page: https://github.com/Professor-G/MicroLIA
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `MicroLIA-2.0.5/MicroLIA.egg-info/SOURCES.txt` & `MicroLIA-2.1.0/MicroLIA.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 MicroLIA/simulate.py
 MicroLIA/training_set.py
 MicroLIA.egg-info/PKG-INFO
 MicroLIA.egg-info/SOURCES.txt
 MicroLIA.egg-info/dependency_links.txt
 MicroLIA.egg-info/requires.txt
 MicroLIA.egg-info/top_level.txt
+MicroLIA/data/.DS_Store
 MicroLIA/data/Miras_vo.xml
 MicroLIA/data/__init__.py
```

### Comparing `MicroLIA-2.0.5/PKG-INFO` & `MicroLIA-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicroLIA
-Version: 2.0.5
+Version: 2.1.0
 Summary: Machine learning classifier for microlensing
 Home-page: https://github.com/Professor-G/MicroLIA
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `MicroLIA-2.0.5/README.md` & `MicroLIA-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.0.5/setup.py` & `MicroLIA-2.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 
 setup(
     name="MicroLIA",
-    version="2.0.5",
+    version="2.1.0",
     author="Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="Machine learning classifier for microlensing",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/MicroLIA",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
@@ -21,15 +21,15 @@
 		'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 		'Programming Language :: Python :: 3',	   
 ],
     packages=find_packages('.'),
     install_requires = ['numpy','scikit-learn', 'scikit-optimize', 'astropy','scipy','peakutils',
         'progress', 'matplotlib', 'optuna', 'boruta', 'BorutaShap', 'xgboost', 'scikit-plot',
-        'tensorflow', 'pandas', 'dill', 'opencv-python', 'imbalanced-learn'],
+        'tensorflow', 'pandas', 'dill', 'opencv-python', 'imbalanced-learn', 'gatspy', 'astroML'],
     python_requires='>=3.7,<4',
     include_package_data=True,
     test_suite="nose.collector",
     package_data={
     '': ['Miras_vo.xml'],
 },
```

