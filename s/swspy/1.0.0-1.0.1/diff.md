# Comparing `tmp/swspy-1.0.0.tar.gz` & `tmp/swspy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swspy-1.0.0.tar", last modified: Mon May 15 11:56:20 2023, max compression
+gzip compressed data, was "dist/swspy-1.0.1.tar", last modified: Mon May 22 09:25:19 2023, max compression
```

## Comparing `swspy-1.0.0.tar` & `swspy-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/
--rw-r--r--   0 eart0504   (502) staff       (20)     1397 2023-05-15 11:56:20.000000 swspy-1.0.0/PKG-INFO
--rw-r--r--   0 eart0504   (502) staff       (20)      665 2021-09-23 13:10:11.000000 swspy-1.0.0/README.md
--rw-r--r--   0 eart0504   (502) staff       (20)       38 2023-05-15 11:56:20.000000 swspy-1.0.0/setup.cfg
--rw-r--r--   0 eart0504   (502) staff       (20)      723 2023-05-15 11:54:59.000000 swspy-1.0.0/setup.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy/
--rw-r--r--   0 eart0504   (502) staff       (20)      436 2021-09-23 09:04:50.000000 swspy-1.0.0/swspy/__init__.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy/automate/
--rw-r--r--   0 eart0504   (502) staff       (20)      127 2021-09-23 09:03:55.000000 swspy-1.0.0/swspy/automate/__init__.py
--rw-r--r--   0 eart0504   (502) staff       (20)    15124 2022-07-11 11:27:06.000000 swspy-1.0.0/swspy/automate/automation_manager.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy/io/
--rw-r--r--   0 eart0504   (502) staff       (20)      126 2021-08-25 10:24:55.000000 swspy-1.0.0/swspy/io/__init__.py
--rw-r--r--   0 eart0504   (502) staff       (20)     9048 2021-12-03 10:26:14.000000 swspy-1.0.0/swspy/io/load.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy/splitting/
--rw-r--r--   0 eart0504   (502) staff       (20)      133 2023-04-04 15:14:25.000000 swspy-1.0.0/swspy/splitting/__init__.py
--rw-r--r--   0 eart0504   (502) staff       (20)     7008 2023-04-17 13:05:11.000000 swspy-1.0.0/swspy/splitting/forward_model.py
--rw-r--r--   0 eart0504   (502) staff       (20)   113994 2023-05-15 11:18:33.000000 swspy-1.0.0/swspy/splitting/split.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/
--rw-r--r--   0 eart0504   (502) staff       (20)     1397 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/PKG-INFO
--rw-r--r--   0 eart0504   (502) staff       (20)      340 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/SOURCES.txt
--rw-r--r--   0 eart0504   (502) staff       (20)        1 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/dependency_links.txt
--rw-r--r--   0 eart0504   (502) staff       (20)        6 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/top_level.txt
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/
+-rw-r--r--   0 eart0504   (502) staff       (20)     1053 2021-08-25 10:24:55.000000 swspy-1.0.1/LICENSE
+-rw-r--r--   0 eart0504   (502) staff       (20)     1447 2023-05-22 09:25:19.000000 swspy-1.0.1/PKG-INFO
+-rw-r--r--   0 eart0504   (502) staff       (20)      896 2023-05-19 14:16:55.000000 swspy-1.0.1/README.md
+-rw-r--r--   0 eart0504   (502) staff       (20)       38 2023-05-22 09:25:19.000000 swspy-1.0.1/setup.cfg
+-rw-r--r--   0 eart0504   (502) staff       (20)      723 2023-05-22 09:23:25.000000 swspy-1.0.1/setup.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy/
+-rw-r--r--   0 eart0504   (502) staff       (20)      436 2021-09-23 09:04:50.000000 swspy-1.0.1/swspy/__init__.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy/automate/
+-rw-r--r--   0 eart0504   (502) staff       (20)      127 2021-09-23 09:03:55.000000 swspy-1.0.1/swspy/automate/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)    15043 2023-05-19 14:05:48.000000 swspy-1.0.1/swspy/automate/automation_manager.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy/io/
+-rw-r--r--   0 eart0504   (502) staff       (20)      168 2023-05-19 14:02:00.000000 swspy-1.0.1/swspy/io/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     8958 2023-05-19 14:06:58.000000 swspy-1.0.1/swspy/io/load.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     5115 2023-05-19 14:00:58.000000 swspy-1.0.1/swspy/io/read_nonlinloc.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy/splitting/
+-rw-r--r--   0 eart0504   (502) staff       (20)      133 2023-04-04 15:14:25.000000 swspy-1.0.1/swspy/splitting/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     7008 2023-04-17 13:05:11.000000 swspy-1.0.1/swspy/splitting/forward_model.py
+-rw-r--r--   0 eart0504   (502) staff       (20)   120925 2023-05-22 09:15:48.000000 swspy-1.0.1/swspy/splitting/split.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/
+-rw-r--r--   0 eart0504   (502) staff       (20)     1447 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/PKG-INFO
+-rw-r--r--   0 eart0504   (502) staff       (20)      419 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/SOURCES.txt
+-rw-r--r--   0 eart0504   (502) staff       (20)        1 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/dependency_links.txt
+-rw-r--r--   0 eart0504   (502) staff       (20)        6 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/top_level.txt
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/tests/
+-rw-r--r--   0 eart0504   (502) staff       (20)     1725 2023-05-15 11:18:33.000000 swspy-1.0.1/tests/test_notebooks.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     3208 2023-05-02 08:15:38.000000 swspy-1.0.1/tests/test_synth.py
```

### Comparing `swspy-1.0.0/PKG-INFO` & `swspy-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 Metadata-Version: 2.1
 Name: swspy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for automatically calculating shear wave splitting for large earthquake catalogues.
 Home-page: https://github.com/TomSHudson/swspy/
 Author: Tom Hudson
 Author-email: thomas.hudson@earth.ox.ac.uk
 License: UNKNOWN
-Description: # swspy
-        
-        A package for performing shear wave splitting in an automated manner. Based on the eigenvalue method of Silver and Chan (1991), with multi-windowing of Teanby et al (2004), coordinate system transformations from Walsh et al (2013), automation methods based on Wustefeld et al (2010), and some other additions.
-        
-        ## To cite:
-        
-        To be completed...
-        
-        
-        Zenodo citation:
-        TBC...
-        
-        ## Documentation:
-        
-        Will be published on readthedocs.org in due course, once the package becomes open source.
-        
-        In the meantime, to view the documentation, do:
-        
-        open docs/build/html/index.html 
-        
-        (or similar)
-        
-        ## Examples:
-        
-        Various example notebooks can be found in the examples directory.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# swspy
+
+A package for performing shear wave splitting in an automated manner. Based on the eigenvalue method of Silver and Chan (1991), with multi-windowing of Teanby et al (2004), coordinate system transformations from Walsh et al (2013), automation methods based on Wustefeld et al (2010), and some other additions.
+
+## To cite:
+
+If you find this package useful, please do consider citing it. The appropriate work to cite is a manuscript currently in review:
+Hudson, T.S., Asplet, J., Walker, A.M.. (in review) "Automated shear-wave splitting analysis for single- and multi- layer anisotropic media". Seismica.
+
+
+## Documentation:
+
+Full documentation for the package is available [here](https://swspy.readthedocs.io/en/latest/).
+
+## Examples:
+
+Various example notebooks can be found in the examples directory, including the examples contained in the paper: Hudson et al. (in review), Seismica.
+
```

### Comparing `swspy-1.0.0/setup.py` & `swspy-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="swspy",
-    version="1.0.0",
+    version="1.0.1",
     author="Tom Hudson",
     author_email="thomas.hudson@earth.ox.ac.uk",
     description="A package for automatically calculating shear wave splitting for large earthquake catalogues.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TomSHudson/swspy/",
     packages=setuptools.find_packages(),
```

### Comparing `swspy-1.0.0/swspy/automate/automation_manager.py` & `swspy-1.0.1/swspy/automate/automation_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import glob 
 import os, sys 
 from pathlib import Path
 import pandas as pd
 import gc 
-from NonLinLocPy import read_nonlinloc # For reading NonLinLoc data (can install via pip)
 
 class proc_many_events:
     """
     Class to process many events to calculate shear-wave splitting.
 
     Parameters
     ----------
@@ -187,15 +186,15 @@
         # Loop over events, processing:
         count = 0
         for nlloc_fname in nlloc_fnames:
             print(''.join(("Processing for event: ", str(count), "/", str(len(nlloc_fnames)))))
             count+=1
             # 1. Get waveform and other event data:
             try:
-                nlloc_hyp_data = read_nonlinloc.read_hyp_file(nlloc_fname)
+                nlloc_hyp_data = swspy.io.read_nonlinloc.read_hyp_file(nlloc_fname)
                 starttime = nlloc_hyp_data.origin_time - event_prepad
                 endtime = nlloc_hyp_data.origin_time + event_postpad
                 load_wfs_obj = swspy.io.load_waveforms(mseed_archive_dir, starttime=starttime, endtime=endtime, downsample_factor=self.downsample_factor, upsample_factor=self.upsample_factor)
                 load_wfs_obj.filter = self.filter
                 load_wfs_obj.filter_freq_min_max = self.filter_freq_min_max
                 st = load_wfs_obj.read_waveform_data()
             except Exception as e:
```

### Comparing `swspy-1.0.0/swspy/io/load.py` & `swspy-1.0.1/swspy/io/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import matplotlib.pyplot as plt
 import obspy
 from obspy import UTCDateTime as UTCDateTime
 import sys, os
 import glob
 import subprocess
 import gc
-from NonLinLocPy import read_nonlinloc # For reading NonLinLoc data (can install via pip)
 
 class load_waveforms:
     """
     A class to load waveforms from file or an archive.
 
     Notes:
     - Will currently only load archived data from the format year/jul_day/*station*
```

### Comparing `swspy-1.0.0/swspy/splitting/forward_model.py` & `swspy-1.0.1/swspy/splitting/forward_model.py`

 * *Files identical despite different names*

### Comparing `swspy-1.0.0/swspy/splitting/split.py` & `swspy-1.0.1/swspy/splitting/split.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 # Output variables:
 
 # Created by Tom Hudson, 30th July 2021
 
 #-----------------------------------------------------------------------------------------------------------------------------------------
 
 # Import neccessary modules:
+import swspy
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import pandas as pd 
 import numba 
-from numba import jit, set_num_threads, prange, float64, int64
+from numba import jit, njit, types, set_num_threads, prange, float64, int64
 from scipy import stats, interpolate
 from sklearn import cluster
 from sklearn.cluster import DBSCAN, KMeans, AgglomerativeClustering
 import obspy
 from obspy import UTCDateTime as UTCDateTime
 import sys, os
 import glob
 import subprocess
 import gc
-from NonLinLocPy import read_nonlinloc # For reading NonLinLoc data (can install via pip)
 import time 
 
 
 class CustomError(Exception):
     pass
 
 
@@ -364,14 +364,18 @@
     else:
         data_minmax = np.min(data)
     F = stats.f.ppf(1-alpha, k, dof)
     conf_bound = data_minmax * ( 1 + ( k / (dof - k) ) * F)
     return conf_bound
 
 
+# @jit((float64[:], float64[:], int64[:], int64[:], int64, int64, int64, float64, float64, float64[:,:,:], float64[:,:,:]), nopython=True, parallel=True)
+#@njit((types.float64[:], types.float64[:], types.int64[:], types.int64[:], types.int64, types.int64, types.int64, types.float64, types.float64, types.float64[:,:,:], types.float64[:,:,:]), parallel=True)
+# @jit(nopython=True, parallel=True)
+#@njit()#parallel=True)
 @jit((float64[:], float64[:], int64[:], int64[:], int64, int64, int64, float64, float64, float64[:,:,:], float64[:,:,:]), nopython=True, parallel=True)
 def _phi_dt_grid_search(data_arr_Q, data_arr_T, win_start_idxs, win_end_idxs, n_t_steps, n_angle_steps, n_win, fs, rotate_step_deg, 
                                     grid_search_results_all_win_EV, grid_search_results_all_win_XC):
     """Function to do numba accelerated grid search of phis and dts.
     Calculates splitting via eigenvalue (EV) (and also cross-correlation (XC) methods 
     if <grid_search_results_all_win_XC> is specified).
     Note: Currently takes absolute values of rotated, time-shifted waveforms to 
@@ -414,16 +418,15 @@
                     # Note: Use lambda2 divided by lambda1 as in Wuestefeld2010 (most stable):
                     grid_search_results_all_win_EV[grid_search_idx,i,j] = lambdas[0] / lambdas[1] 
 
                     # ================== Calculate splitting parameters via. XC method ==================
                     # if len(grid_search_results_all_win_XC) > 0:
                         # Calculate XC coeffecient and save to array:
                         # if np.std(rolled_rot_Q_curr)  * np.std(rolled_rot_T_curr) > 0. and len(rolled_rot_T_curr) > 0:
-                    grid_search_results_all_win_XC[grid_search_idx,i,j] = np.sum( np.abs(rolled_rot_Q_curr * rolled_rot_T_curr) / (np.std(rolled_rot_Q_curr) * 
-                                                                np.std(rolled_rot_T_curr))) / len(rolled_rot_T_curr)
+                    grid_search_results_all_win_XC[grid_search_idx,i,j] = np.sum( np.abs(rolled_rot_Q_curr * rolled_rot_T_curr) / (np.std(rolled_rot_Q_curr) * np.std(rolled_rot_T_curr))) / float(len(rolled_rot_T_curr))
 
     return grid_search_results_all_win_EV, grid_search_results_all_win_XC 
 
 
 @jit((float64[:], float64[:], int64[:], int64[:], int64, int64, int64, float64, float64, float64[:,:,:,:,:], float64[:,:,:,:,:]), nopython=True, parallel=True)
 def _phi_dt_grid_search_direct_multi_layer(data_arr_Q, data_arr_T, win_start_idxs, win_end_idxs, n_t_steps, n_angle_steps, n_win, fs, rotate_step_deg, 
                                     grid_search_results_all_win_EV, grid_search_results_all_win_XC):
@@ -629,15 +632,15 @@
             self.back_azis_all_stations = back_azis_all_stations
             self.receiver_inc_angles_all_stations = receiver_inc_angles_all_stations
             self.S_phase_arrival_times = S_phase_arrival_times
         # Define parameters:
         self.st = st 
         self.nonlinloc_event_path = nonlinloc_event_path
         if self.nonlinloc_event_path:
-            self.nonlinloc_hyp_data = read_nonlinloc.read_hyp_file(nonlinloc_event_path)
+            self.nonlinloc_hyp_data = swspy.io.read_nonlinloc.read_hyp_file(nonlinloc_event_path)
         if self.nonlinloc_event_path:
             self.origin_time = self.nonlinloc_hyp_data.origin_time
         else:
             self.origin_time = self.st[0].stats.starttime 
         if event_uid:
             self.event_uid = event_uid
         else:
@@ -702,15 +705,14 @@
             grid_search_results_all_win_XC = np.zeros((n_win**2, n_t_steps, n_angle_steps, n_t_steps, n_angle_steps), dtype=float)
         else:
             print("Error: n_layers = ", n_layers, "not supported (n_layers = 1 or 2 currently). Exiting.")
             sys.exit()
 
         # Perform grid search:
         if n_layers == 1:
-            set_num_threads(int(num_threads))
             grid_search_results_all_win_EV, grid_search_results_all_win_XC = _phi_dt_grid_search(data_arr_Q, data_arr_T, win_start_idxs, win_end_idxs, n_t_steps, n_angle_steps, n_win, fs, rotate_step_deg, grid_search_results_all_win_EV, grid_search_results_all_win_XC)
         elif n_layers == 2:
             set_num_threads(int(num_threads))
             grid_search_results_all_win_EV, grid_search_results_all_win_XC = _phi_dt_grid_search_direct_multi_layer(data_arr_Q, data_arr_T, win_start_idxs, win_end_idxs, 
                                                                                                         n_t_steps, n_angle_steps, n_win, fs, rotate_step_deg, 
                                                                                                         grid_search_results_all_win_EV, grid_search_results_all_win_XC)
 
@@ -740,16 +742,17 @@
             phis_labels = np.linspace(y_tmp[0], y_tmp[-1], interp_fac*len(y_tmp))
         else:
             error_surf = phi_dt_single_win
 
         # Find grid search array points where within confidence interval:
         # Use transverse component to calculate dof
         dof = calc_dof(tr_for_dof.data)
-        conf_bound = ftest(error_surf, dof, alpha=0.05, k=2)
-        # conf_bound = ftest(error_surf, dof, alpha=0.33, k=2)
+        #conf_bound = ftest(error_surf, dof, alpha=0.05, k=2) # (2 sigma)
+        conf_bound = ftest(error_surf, dof, alpha=0.003, k=2) # (3 sigma)
+        #conf_bound = ftest(error_surf, dof, alpha=0.32, k=2) # (1 sigma)
         conf_mask = error_surf <= conf_bound
 
         # Find lag dt error:
         # (= 1/2 (not 1/4) width of confidence box (see Silver1991))
         lag_mask = conf_mask.any(axis=1) #(axis=0) # Condense axis1 down along lag (axis0)
         true_idxs = np.where(lag_mask)[0]
         if len(true_idxs) == 0:
@@ -1084,14 +1087,19 @@
             If True, returns clustering data information. This is primarily used for 
             plotting. Default is False.
 
         num_threads : int
             Number of threads to use for parallel computing. Default is to use all 
             available threads on the system.
 
+        Returns
+        -------
+        self.sws_result_df : pandas DataFrame
+            A pandas DataFrame containing the key splitting results.
+
         """
         # Save any parameters to class object:
         self.coord_system = coord_system
         self.sws_method = sws_method
         
         # Perform initial parameter checks:
         if ( sws_method != "EV" ) and ( sws_method != "EV_and_XC" ):
@@ -1259,18 +1267,16 @@
         return self.sws_result_df
 
 
     def perform_sws_analysis_multi_layer(self, coord_system="ZNE", multi_layer_method="explicit", num_threads=numba.config.NUMBA_DEFAULT_NUM_THREADS):
         """Function to perform splitting analysis for a multi-layered medium. Currently 
          only a 2-layer medium is supported. Works in LQT coordinate system, therefore 
         supporting shear-wave-splitting in 3D.
-
         Currently doesn't support any method other than <sws_method> = EV and 
         doesn't support returning clustered data.
-
         Method assumes that apparent delay-time is longer than fast S-wave arrival duration.
         
         Parameters
         ----------
         coord_system : str
             Coordinate system to perform analysis in. Options are: LQT, ZNE. Will convert 
             splitting angles back into coordinates relative to ZNE whatever system it 
@@ -1284,14 +1290,23 @@
             expensive relative to explicit method, with many free parameters, as computation 
             scales as (n_phi * n_dt) ^ n-layers.
 
         num_threads : int
             Number of threads to use for parallel computing. Default is to use all 
             available threads on the system.
 
+        Returns
+        -------
+        self.sws_result_df : pandas DataFrame
+            A pandas DataFrame containing the key splitting results for an apparent splitting 
+            measurement (i.e. assuming only one layer).
+
+        self.sws_multi_layer_result_df pandas DataFrame
+            A pandas DataFrame containing the key splitting results for hte multi-layer result.
+
         """
         # Save any parameters to class object:
         self.coord_system = coord_system
 
         # Create datastores:
         sws_result_df_out = pd.DataFrame(data={'station': [], 'phi_from_Q': [], 'phi_from_N': [], 
                                                 'phi_from_U': [], 'phi_err': [], 'dt': [], 'dt_err': [], 
@@ -1301,14 +1316,16 @@
                                                 'phi1_from_U': [], 'phi1_err': [], 'dt1': [], 'dt1_err': [], 
                                                 'phi2_from_Q': [], 'phi2_from_N': [], 'phi2_from_U': [], 'phi2_err': [], 
                                                 'dt2': [], 'dt2_err': [], 
                                                 'src_pol_from_N': [], 'src_pol_from_U': [], 'src_pol_from_N_err': [], 
                                                 'src_pol_from_U_err': [], 'Q_w': [], 'lambda2/lambda1 ratio': [], 'lambda2/lambda1 ratio1': [], 
                                                 'lambda2/lambda1 ratio2': [], 'ray_back_azi': [], 'ray_inc': []})
         self.phi_dt_grid_average = {}
+        self.phi_dt_grid_average_layer1 = {}
+        self.phi_dt_grid_average_layer2 = {}
         self.event_station_win_idxs = {}
 
         # 0. Get initial, apparent splitting parameters:
         # (assuming single layer)
         self.perform_sws_analysis(coord_system=coord_system, sws_method="EV", return_clusters_data=True)
 
         # Calculate multi-layer splitting for all sstations:
@@ -1384,38 +1401,51 @@
                 # 2.a. For first window:
                 grid_search_results_all_win_EV_win1, lags_labels, phis_labels = self._calc_splitting_eig_val_method(tr_Q.data, tr_T.data, win_start_idxs_partition1, 
                                                                                                             win_end_idxs_partition1, sws_method="EV", num_threads=num_threads)
                 grid_search_results_all_win_EV_win1[grid_search_results_all_win_EV_win1==0] = 1 # Remove effect of any exact zero eigenvalues (spurious results), while preseerving indices
                 self.lags_labels = lags_labels 
                 self.phis_labels = phis_labels 
                 phis, lags, phi_errs, lag_errs, min_eig_ratios = self._get_phi_and_lag_errors(grid_search_results_all_win_EV_win1, tr_T)         
-                opt_phi_win1, opt_lag_win1, opt_phi_err_win1, opt_lag_err_win1, opt_eig_ratio1 = self._sws_win_clustering(lags, phis, lag_errs, phi_errs, 
-                                                                                                                        min_eig_ratios=min_eig_ratios, method="dbscan")
+                opt_phi_win1, opt_lag_win1, opt_phi_err_win1, opt_lag_err_win1, opt_eig_ratio1, clusters_dict1, min_var_idx1 = self._sws_win_clustering(lags, phis, lag_errs, phi_errs, 
+                                                                                                                        min_eig_ratios=min_eig_ratios, method="dbscan", return_clusters_data=True)
                 if not opt_phi_win1:
                     continue # If didn't cluster, skip station
                 # 2.b. For second window:
                 grid_search_results_all_win_EV_win2, lags_labels, phis_labels = self._calc_splitting_eig_val_method(tr_Q.data, tr_T.data, win_start_idxs_partition2, 
                                                                                                             win_end_idxs_partition2, sws_method="EV", num_threads=num_threads)
                 grid_search_results_all_win_EV_win2[grid_search_results_all_win_EV_win2==0] = 1 # Remove effect of any exact zero eigenvalues (spurious results), while preseerving indices
                 self.lags_labels = lags_labels 
                 self.phis_labels = phis_labels 
                 phis, lags, phi_errs, lag_errs, min_eig_ratios = self._get_phi_and_lag_errors(grid_search_results_all_win_EV_win2, tr_T)         
-                opt_phi_win2, opt_lag_win2, opt_phi_err_win2, opt_lag_err_win2, opt_eig_ratio2 = self._sws_win_clustering(lags, phis, lag_errs, phi_errs, 
-                                                                                                                        min_eig_ratios=min_eig_ratios, method="dbscan")
+                opt_phi_win2, opt_lag_win2, opt_phi_err_win2, opt_lag_err_win2, opt_eig_ratio2, clusters_dict2, min_var_idx2 = self._sws_win_clustering(lags, phis, lag_errs, phi_errs, 
+                                                                                                                        min_eig_ratios=min_eig_ratios, method="dbscan", return_clusters_data=True)
                 if not opt_phi_win2:
                     continue # If didn't cluster, skip station
+
                 # 2.c. Pick best (most linearised) result:
                 min_EV_both_wins = np.array([opt_eig_ratio1, opt_eig_ratio2])
                 min_EV_both_wins[min_EV_both_wins==0] = 1e6 # Remove effect of any exact zero eigenvalues (spurious results), while preseerving indices
                 best_win_idx = np.argmin(min_EV_both_wins)
                 opt_phi_layer2 = np.array([opt_phi_win1, opt_phi_win2])[best_win_idx]
                 opt_lag_layer2 = np.array([opt_lag_win1, opt_lag_win2])[best_win_idx]
                 opt_phi_err_layer2 = np.array([opt_phi_err_win1, opt_phi_err_win2])[best_win_idx]
                 opt_lag_err_layer2 = np.array([opt_lag_err_win1, opt_lag_err_win2])[best_win_idx]
                 opt_eig_ratio_layer2 = np.min(min_EV_both_wins)
+                if best_win_idx == 0:
+                    grid_search_results_all_win_EV_layer2 = grid_search_results_all_win_EV_win1
+                    self.clustering_info[station] = {}
+                    self.clustering_info[station]['layer2'] = {}
+                    self.clustering_info[station]['layer2']['min_var_idx'] = min_var_idx1
+                    self.clustering_info[station]['layer2']['clusters_dict'] = clusters_dict1
+                elif best_win_idx == 1:
+                    grid_search_results_all_win_EV_layer2 = grid_search_results_all_win_EV_win2
+                    self.clustering_info[station] = {}
+                    self.clustering_info[station]['layer2'] = {}
+                    self.clustering_info[station]['layer2']['min_var_idx'] = min_var_idx2
+                    self.clustering_info[station]['layer2']['clusters_dict'] = clusters_dict2
                     
                 # 3. Remove effect of layer 2 anisotropy:
                 st_ZNE_curr_sws_layer_2_removed = remove_splitting(st_ZNE_curr, opt_phi_layer2, opt_lag_layer2, back_azi, event_inclin_angle_at_station, return_BPA=False)
                 st_LQT_curr_sws_layer_2_removed = _rotate_ZNE_to_LQT(st_ZNE_curr_sws_layer_2_removed, back_azi, event_inclin_angle_at_station)
 
                 # 4. Find splitting parameters for layer 1:
                 # (by perform splitting for entire trace post layer 2 correction)
@@ -1423,16 +1453,20 @@
                 tr_T = st_LQT_curr_sws_layer_2_removed.select(station=station, channel="??T")[0]
                 grid_search_results_all_win_EV_layer1, lags_labels, phis_labels = self._calc_splitting_eig_val_method(tr_Q.data, tr_T.data, win_start_idxs, 
                                                                                                             win_end_idxs, sws_method="EV", num_threads=num_threads)
                 grid_search_results_all_win_EV_layer1[grid_search_results_all_win_EV_layer1==0] = 1 # Remove effect of any exact zero eigenvalues (spurious results), while preseerving indices
                 self.lags_labels = lags_labels 
                 self.phis_labels = phis_labels 
                 phis, lags, phi_errs, lag_errs, min_eig_ratios = self._get_phi_and_lag_errors(grid_search_results_all_win_EV_layer1, tr_T)         
-                opt_phi_layer1, opt_lag_layer1, opt_phi_err_layer1, opt_lag_err_layer1, opt_eig_ratio_layer1 = self._sws_win_clustering(lags, phis, lag_errs, phi_errs, 
-                                                                                                                                min_eig_ratios=min_eig_ratios, method="dbscan")
+                opt_phi_layer1, opt_lag_layer1, opt_phi_err_layer1, opt_lag_err_layer1, opt_eig_ratio_layer1, clusters_dict_layer1, min_var_idx_layer1 = self._sws_win_clustering(lags, phis, lag_errs, phi_errs, 
+                                                                                                                                min_eig_ratios=min_eig_ratios, method="dbscan", return_clusters_data=True)
+                # And write clustering info:
+                self.clustering_info[station]['layer1'] = {}
+                self.clustering_info[station]['layer1']['min_var_idx'] = min_var_idx_layer1
+                self.clustering_info[station]['layer1']['clusters_dict'] = clusters_dict_layer1
                 if not opt_phi_layer1:
                     continue # If didn't cluster, skip station
                 
                 # 5. And calculate source polarisation:
                 # Get wfs:
                 st_ZNE_curr_sws_corrected = remove_splitting(st_ZNE_curr_sws_layer_2_removed, opt_phi_layer1, opt_lag_layer1, back_azi, event_inclin_angle_at_station, 
                                                             return_BPA=False)
@@ -1467,14 +1501,15 @@
                 opt_phi_layer2, opt_lag_layer2 = self.phis_labels[abs_min_indices[2]], self.lags_labels[abs_min_indices[1]]
                 opt_phi_err_layer2, opt_lag_err_layer2 = 0, 0 # (Note: Currently don't calculate errors for this method)
                 opt_eig_ratio  = grid_search_result_multi_layer_inv[abs_min_indices[0], abs_min_indices[1], abs_min_indices[2], abs_min_indices[3], 
                                                                        abs_min_indices[4]]
                 opt_eig_ratio_layer1, opt_eig_ratio_layer2 = opt_eig_ratio, opt_eig_ratio
                 grid_search_results_all_win_EV_layer1 = grid_search_result_multi_layer_inv[:, abs_min_indices[1], abs_min_indices[2], 
                                                                                            :, :]
+                grid_search_results_all_win_EV_layer2 = np.zeros(np.shape(grid_search_results_all_win_EV_layer1)) # Set layer 2 to zeros, simply as can't untangle result.
                 del grid_search_result_multi_layer_inv
                 gc.collect()
 
                 # 5. And calculate source polarisation:
                 # Get wfs:
                 st_ZNE_curr_layer_2_corr = remove_splitting(st_ZNE_curr, opt_phi_layer2, opt_lag_layer2, back_azi, event_inclin_angle_at_station, 
                                                             return_BPA=False)
@@ -1535,14 +1570,16 @@
             sws_result_df_out = sws_result_df_out.append(df_tmp)
             try:
                 opt_phi_idx = np.where(self.phis_labels == opt_phi_layer1)[0][0]
                 opt_lag_idx = np.where(self.lags_labels == opt_lag_layer1)[0][0]
             except IndexError:
                 raise CustomError("Cannot find optimal phi or lag.")
             self.phi_dt_grid_average[station] = np.average(grid_search_results_all_win_EV_layer1, axis=0) # (lambda2 divided by lambda1 as in Wuestefeld2010 (most stable))
+            self.phi_dt_grid_average_layer1[station] = np.average(grid_search_results_all_win_EV_layer1, axis=0) # (lambda2 divided by lambda1 as in Wuestefeld2010 (most stable))
+            self.phi_dt_grid_average_layer2[station] = np.average(grid_search_results_all_win_EV_layer2, axis=0) # (lambda2 divided by lambda1 as in Wuestefeld2010 (most stable))
             self.event_station_win_idxs[station] = {}
             self.event_station_win_idxs[station]['win_start_idxs'] = win_start_idxs
             self.event_station_win_idxs[station]['win_end_idxs'] = win_end_idxs
 
         # And update one output df:
         self.sws_result_df = sws_result_df_out
 
@@ -1574,14 +1611,23 @@
                 dt_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt'])
                 phi_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_err'])
                 dt_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt_err'])
                 src_pol_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N'])
                 src_pol_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N_err'])
                 Q_w_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['Q_w'])
                 opt_eig_ratio_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['lambda2/lambda1 ratio'])
+                if self.sws_multi_layer_result_df is not None:
+                    dt_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt1'])
+                    dt_err_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt1_err'])
+                    dt_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt2'])
+                    dt_err_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt2_err'])
+                    phi_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi1_from_N'])
+                    phi_err_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi1_err'])
+                    phi_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi2_from_N'])
+                    phi_err_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi2_err'])
             except TypeError:
                 # If cannot get parameters becuase splitting clustering failed, skip station:
                 print("Cannot get splitting parameters because splitting clustering failed. Skipping station:", 
                         station)
                 continue
             # And get unncorrected P and A waveforms:
             tr_tmp_P = st_ZNE_curr.select(channel="??N")[0].copy()
@@ -1726,60 +1772,102 @@
             # Corr NE:
             ne_corr_ax.plot(st_ZNE_curr_sws_corrected.select(channel="??E")[0].data, 
                                                             st_ZNE_curr_sws_corrected.select(channel="??N")[0].data, c='#D73215')
             ne_corr_ax.set_xlim(-1.1*max_amp, 1.1*max_amp)
             ne_corr_ax.set_ylim(-1.1*max_amp, 1.1*max_amp)
 
             # phi - dt space:
-            Y, X = np.meshgrid(self.phis_labels, self.lags_labels)
-            Z = self.phi_dt_grid_average[station]
-            # phi_dt_ax.contourf(X, Y, Z, levels=10, cmap="magma")
-            CS = phi_dt_ax.contourf(X, Y, Z, levels=20, cmap="magma")
-            CS2 = phi_dt_ax.contour(CS, levels=CS.levels[1::2], colors='w', alpha=0.25)
-            phi_dt_ax.errorbar(dt_curr , phi_curr, xerr=dt_err_curr, yerr=phi_err_curr, c='g', capsize=5)
+            # Plot for single layer:
+            if self.sws_multi_layer_result_df is None:
+                Y, X = np.meshgrid(self.phis_labels, self.lags_labels)
+                Z = self.phi_dt_grid_average[station]
+                # phi_dt_ax.contourf(X, Y, Z, levels=10, cmap="magma")
+                CS = phi_dt_ax.contourf(X, Y, Z, levels=20, cmap="magma")
+                CS2 = phi_dt_ax.contour(CS, levels=CS.levels[1::2], colors='w', alpha=0.25)
+                phi_dt_ax.errorbar(dt_curr , phi_curr, xerr=dt_err_curr, yerr=phi_err_curr, c='g', capsize=5)
+            # Or plot for double layer:
+            else:
+                # Setup new axes:
+                phi_dt_ax_layer1 = phi_dt_ax.inset_axes([0, 0, 1.0, 0.5])#([0, 0, 0.5, 1.0])
+                phi_dt_ax_layer2 = phi_dt_ax.inset_axes([0, 0.5, 1.0, 0.5])#([0.5, 0, 0.5, 1.0])
+                # And plot data:
+                Y, X = np.meshgrid(self.phis_labels, self.lags_labels)
+                Z1 = self.phi_dt_grid_average_layer1[station]
+                Z2 = self.phi_dt_grid_average_layer2[station]
+                CS = phi_dt_ax_layer1.contourf(X, Y, Z1, levels=20, cmap="magma")
+                CS2 = phi_dt_ax_layer1.contour(CS, levels=CS.levels[1::2], colors='w', alpha=0.25)
+                phi_dt_ax_layer1.errorbar(dt_layer1 , phi_layer1, xerr=dt_err_layer1, yerr=phi_err_layer1, c='g', capsize=5)  
+                phi_dt_ax_layer1.set_xlim(self.lags_labels[0], self.lags_labels[-1])
+                phi_dt_ax_layer1.set_ylim(self.phis_labels[0], self.phis_labels[-1])
+                CS = phi_dt_ax_layer2.contourf(X, Y, Z2, levels=20, cmap="magma")
+                CS2 = phi_dt_ax_layer2.contour(CS, levels=CS.levels[1::2], colors='w', alpha=0.25)
+                phi_dt_ax_layer2.errorbar(dt_layer2 , phi_layer2, xerr=dt_err_layer2, yerr=phi_err_layer2, c='g', capsize=5)
+                phi_dt_ax_layer2.set_xlim(self.lags_labels[0], self.lags_labels[-1])
+                phi_dt_ax_layer2.set_ylim(self.phis_labels[0], self.phis_labels[-1])
+                # And sort axes:
+                phi_dt_ax_layer1.set_xlabel(r'$\delta t_{layer 1,2}$ ($s$)')
+                # phi_dt_ax_layer2.set_xlabel(r'$\delta t_{layer 2}$ ($s$)')
+                phi_dt_ax_layer2.get_xaxis().set_visible(False)
+                phi_dt_ax_layer1.set_ylabel(r'$\phi_{layer 1}$ from Q ($^o$)')
+                phi_dt_ax_layer2.set_ylabel(r'$\phi_{layer 2}$ from Q ($^o$)')
+                # phi_dt_ax_layer2.get_yaxis().set_visible(False)
 
             # Add clustering data if available:
             if self.clustering_info:
-                clust_idxs = list(self.clustering_info[station]['clusters_dict'].keys())
-                samp_idx_count = 0
-                for clust_idx in clust_idxs:
-                    # PLot cluster phis:
-                    y_tmp = self.clustering_info[station]['clusters_dict'][clust_idx]['phis']
-                    x_tmp = np.arange(samp_idx_count, samp_idx_count+len(y_tmp))
-                    y_err = self.clustering_info[station]['clusters_dict'][clust_idx]['phi_errs']
-                    cluster_results_ax_phi.errorbar(x_tmp, y_tmp, yerr=y_err, c='k', markersize=2.5, alpha=0.5)
-                    # And plot cluster dts:
-                    y_tmp = self.clustering_info[station]['clusters_dict'][clust_idx]['lags']
-                    x_tmp = np.arange(samp_idx_count, samp_idx_count+len(y_tmp))
-                    y_err = self.clustering_info[station]['clusters_dict'][clust_idx]['lag_errs']
-                    cluster_results_ax_dt.errorbar(x_tmp, y_tmp, yerr=y_err, c='k', markersize=2.5, alpha=0.5)                    
-                    # And update x sample count:
-                    samp_idx_count = samp_idx_count + len(y_tmp)
+                # Plot clustering for multi-layer explicit result, if exists:
+                if "layer1" in self.clustering_info[station]:
+                    clust_idxs = list(self.clustering_info[station]['layer1']['clusters_dict'].keys())
+                    samp_idx_count = 0
+                    for clust_idx in clust_idxs:
+                        samp_idx_count_overall = samp_idx_count
+                        for layer_id in ['layer1', 'layer2']:
+                            samp_idx_count = samp_idx_count_overall
+                            # PLot cluster phis:
+                            y_tmp = self.clustering_info[station][layer_id]['clusters_dict'][clust_idx]['phis']
+                            x_tmp = np.arange(samp_idx_count, samp_idx_count+len(y_tmp))
+                            y_err = self.clustering_info[station][layer_id]['clusters_dict'][clust_idx]['phi_errs']
+                            cluster_results_ax_phi.errorbar(x_tmp, y_tmp, yerr=y_err, markersize=2.5, alpha=0.5)
+                            # And plot cluster dts:
+                            y_tmp = self.clustering_info[station][layer_id]['clusters_dict'][clust_idx]['lags']
+                            x_tmp = np.arange(samp_idx_count, samp_idx_count+len(y_tmp))
+                            y_err = self.clustering_info[station][layer_id]['clusters_dict'][clust_idx]['lag_errs']
+                            cluster_results_ax_dt.errorbar(x_tmp, y_tmp, yerr=y_err, markersize=2.5, alpha=0.5)                    
+                            # And update x sample count:
+                            samp_idx_count = samp_idx_count + len(y_tmp)
+                # Or plot single clustering, if not explicit multi-layer result:
+                else:    
+                    clust_idxs = list(self.clustering_info[station]['clusters_dict'].keys())
+                    samp_idx_count = 0
+                    for clust_idx in clust_idxs:
+                        # PLot cluster phis:
+                        y_tmp = self.clustering_info[station]['clusters_dict'][clust_idx]['phis']
+                        x_tmp = np.arange(samp_idx_count, samp_idx_count+len(y_tmp))
+                        y_err = self.clustering_info[station]['clusters_dict'][clust_idx]['phi_errs']
+                        cluster_results_ax_phi.errorbar(x_tmp, y_tmp, yerr=y_err, c='k', markersize=2.5, alpha=0.5)
+                        # And plot cluster dts:
+                        y_tmp = self.clustering_info[station]['clusters_dict'][clust_idx]['lags']
+                        x_tmp = np.arange(samp_idx_count, samp_idx_count+len(y_tmp))
+                        y_err = self.clustering_info[station]['clusters_dict'][clust_idx]['lag_errs']
+                        cluster_results_ax_dt.errorbar(x_tmp, y_tmp, yerr=y_err, c='k', markersize=2.5, alpha=0.5)                    
+                        # And update x sample count:
+                        samp_idx_count = samp_idx_count + len(y_tmp)
                 # And set limits and labels:
                 cluster_results_ax_phi.set_ylim(-90, 90)
                 cluster_results_ax_dt.set_ylim(0, np.max(self.lags_labels))
                 cluster_results_ax_dt.set_xlabel("Cluster sample")
                 cluster_results_ax_phi.set_ylabel(r"$\phi$ ($^o$)")
                 cluster_results_ax_dt.set_ylabel(r"$\delta t$ ($s$)")
 
             # Add text:
             text_ax.text(0,0,"Event origin time : \n"+self.origin_time.strftime("%Y-%m-%dT%H:%M:%SZ"), fontsize='small')
             text_ax.text(0,-1,"Station : "+station, fontsize='small')
             # Plot intermediate post layer 2 correction (multi-layer splitting):
             if self.sws_multi_layer_result_df is not None:
-                dt_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt1'])
-                dt_err_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt1_err'])
-                dt_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt2'])
-                dt_err_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt2_err'])
                 text_ax.text(0,-2,r"$\delta$ $t_{layer 1}$ : "+str(dt_layer1)+" +/-"+str(round(dt_err_layer1, 5))+" $s$", fontsize='small')
                 text_ax.text(0,-3,r"$\delta$ $t_{layer 2}$ : "+str(dt_layer2)+" +/-"+str(round(dt_err_layer2, 5))+" $s$", fontsize='small')
-                phi_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi1_from_N'])
-                phi_err_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi1_err'])
-                phi_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi2_from_N'])
-                phi_err_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi2_err'])
                 text_ax.text(0,-4,r"$\phi_{layer 1}$ from N : "+"{0:0.1f}".format(phi_layer1)+"$^o$"+" +/-"+"{0:0.1f}".format(phi_err_layer1)+"$^o$", fontsize='small')
                 text_ax.text(0,-5,r"$\phi_{layer 2}$ from N : "+"{0:0.1f}".format(phi_layer2)+"$^o$"+" +/-"+"{0:0.1f}".format(phi_err_layer2)+"$^o$", fontsize='small')
                 text_ax.text(0,-6,''.join(("src pol from N: ","{0:0.1f}".format(src_pol_curr),"$^o$"," +/-","{0:0.1f}".format(src_pol_err_curr),"$^o$")), fontsize='small')
                 text_ax.text(0,-7,"Coord. sys. : "+self.coord_system, fontsize='small')
                 text_ax.text(0,-8,r"$\lambda_2$/$\lambda_1$: "+str(round(opt_eig_ratio_curr, 3)), fontsize='small')
                 if Q_w_curr <= 1.1:
                     text_ax.text(0,-9,"$Q_w$ : "+str(round(Q_w_curr, 3)), fontsize='small')
@@ -1807,15 +1895,17 @@
             ne_uncorr_ax.set_ylabel('N')
             ne_corr_ax.set_xlabel('E')
             ne_corr_ax.set_ylabel('N')
             phi_dt_ax.set_xlabel(r'$\delta$ t (s)')
             if self.sws_multi_layer_result_df is None:
                 phi_dt_ax.set_ylabel(r'$\phi$ from Q ($^o$)')
             else:
-                phi_dt_ax.set_ylabel(r'$\phi_{layer 1}$ from Q ($^o$)')
+                phi_dt_ax.set_ylabel(r'$\phi_{layer 1,2}$ from Q ($^o$)')
+                phi_dt_ax.get_xaxis().set_visible(False)
+                phi_dt_ax.get_yaxis().set_visible(False)
 
             # plt.colorbar()
             # plt.tight_layout()
             if outdir:
                 os.makedirs(outdir, exist_ok=True)
                 plt.savefig(os.path.join(outdir, ''.join((self.event_uid, "_", station, ".png"))), dpi=300)
             if suppress_direct_plotting:
```

### Comparing `swspy-1.0.0/swspy.egg-info/PKG-INFO` & `swspy-1.0.1/swspy.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 Metadata-Version: 2.1
 Name: swspy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for automatically calculating shear wave splitting for large earthquake catalogues.
 Home-page: https://github.com/TomSHudson/swspy/
 Author: Tom Hudson
 Author-email: thomas.hudson@earth.ox.ac.uk
 License: UNKNOWN
-Description: # swspy
-        
-        A package for performing shear wave splitting in an automated manner. Based on the eigenvalue method of Silver and Chan (1991), with multi-windowing of Teanby et al (2004), coordinate system transformations from Walsh et al (2013), automation methods based on Wustefeld et al (2010), and some other additions.
-        
-        ## To cite:
-        
-        To be completed...
-        
-        
-        Zenodo citation:
-        TBC...
-        
-        ## Documentation:
-        
-        Will be published on readthedocs.org in due course, once the package becomes open source.
-        
-        In the meantime, to view the documentation, do:
-        
-        open docs/build/html/index.html 
-        
-        (or similar)
-        
-        ## Examples:
-        
-        Various example notebooks can be found in the examples directory.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# swspy
+
+A package for performing shear wave splitting in an automated manner. Based on the eigenvalue method of Silver and Chan (1991), with multi-windowing of Teanby et al (2004), coordinate system transformations from Walsh et al (2013), automation methods based on Wustefeld et al (2010), and some other additions.
+
+## To cite:
+
+If you find this package useful, please do consider citing it. The appropriate work to cite is a manuscript currently in review:
+Hudson, T.S., Asplet, J., Walker, A.M.. (in review) "Automated shear-wave splitting analysis for single- and multi- layer anisotropic media". Seismica.
+
+
+## Documentation:
+
+Full documentation for the package is available [here](https://swspy.readthedocs.io/en/latest/).
+
+## Examples:
+
+Various example notebooks can be found in the examples directory, including the examples contained in the paper: Hudson et al. (in review), Seismica.
+
```

