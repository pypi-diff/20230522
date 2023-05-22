# Comparing `tmp/iimcsim-0.0.3.tar.gz` & `tmp/iimcsim-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iimcsim-0.0.3.tar", last modified: Fri May 19 19:31:38 2023, max compression
+gzip compressed data, was "iimcsim-0.0.4.tar", last modified: Mon May 22 08:41:26 2023, max compression
```

## Comparing `iimcsim-0.0.3.tar` & `iimcsim-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:31:38.290997 iimcsim-0.0.3/
--rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4260 2023-05-19 19:31:38.290997 iimcsim-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsim-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      747 2023-05-19 19:31:38.292992 iimcsim-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 19:31:38.216198 iimcsim-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 19:31:38.271053 iimcsim-0.0.3/src/iimcsim/
--rw-rw-rw-   0        0        0     2431 2023-05-19 19:30:27.000000 iimcsim-0.0.3/src/iimcsim/MC.py
--rw-rw-rw-   0        0        0    11861 2023-05-19 11:37:00.000000 iimcsim-0.0.3/src/iimcsim/MonteCarlo.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.0.3/src/iimcsim/__init__.py
--rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.0.3/src/iimcsim/data_gen.py
--rw-rw-rw-   0        0        0      547 2023-05-19 19:30:22.000000 iimcsim-0.0.3/src/iimcsim/data_gen_run.py
--rw-rw-rw-   0        0        0     2486 2023-05-19 11:37:01.000000 iimcsim-0.0.3/src/iimcsim/shape_ext.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:31:38.289006 iimcsim-0.0.3/src/iimcsim.egg-info/
--rw-rw-rw-   0        0        0     4260 2023-05-19 19:31:38.000000 iimcsim-0.0.3/src/iimcsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-05-19 19:31:38.000000 iimcsim-0.0.3/src/iimcsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:31:38.000000 iimcsim-0.0.3/src/iimcsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 19:31:38.000000 iimcsim-0.0.3/src/iimcsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 08:41:26.520135 iimcsim-0.0.4/
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4260 2023-05-22 08:41:26.521140 iimcsim-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsim-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      747 2023-05-22 08:41:26.529188 iimcsim-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 08:41:26.008562 iimcsim-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 08:41:26.424758 iimcsim-0.0.4/src/iimcsim/
+-rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.0.4/src/iimcsim/MC.py
+-rw-rw-rw-   0        0        0    11861 2023-05-19 11:37:00.000000 iimcsim-0.0.4/src/iimcsim/MonteCarlo.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.0.4/src/iimcsim/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.0.4/src/iimcsim/data_gen.py
+-rw-rw-rw-   0        0        0      574 2023-05-22 07:30:47.000000 iimcsim-0.0.4/src/iimcsim/data_gen_run.py
+-rw-rw-rw-   0        0        0     2237 2023-05-22 08:36:01.000000 iimcsim-0.0.4/src/iimcsim/eda.py
+-rw-rw-rw-   0        0        0     2624 2023-05-22 08:34:48.000000 iimcsim-0.0.4/src/iimcsim/shape_ext.py
+-rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.0.4/src/iimcsim/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:41:26.511035 iimcsim-0.0.4/src/iimcsim.egg-info/
+-rw-rw-rw-   0        0        0     4260 2023-05-22 08:41:25.000000 iimcsim-0.0.4/src/iimcsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-05-22 08:41:25.000000 iimcsim-0.0.4/src/iimcsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:41:25.000000 iimcsim-0.0.4/src/iimcsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 08:41:25.000000 iimcsim-0.0.4/src/iimcsim.egg-info/top_level.txt
```

### Comparing `iimcsim-0.0.3/PKG-INFO` & `iimcsim-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsim Version: 0.0.3 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.0.4 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

### Comparing `iimcsim-0.0.3/README.md` & `iimcsim-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.3/setup.cfg` & `iimcsim-0.0.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 696d 6373 696d 0d0a 7665 7273   = iimcsim..vers
-00000020: 696f 6e20 3d20 302e 302e 330d 0a61 7574  ion = 0.0.3..aut
+00000020: 696f 6e20 3d20 302e 302e 340d 0a61 7574  ion = 0.0.4..aut
 00000030: 686f 7220 3d20 4a69 6761 7220 4268 616e  hor = Jigar Bhan
 00000040: 6465 7269 0d0a 6175 7468 6f72 5f65 6d61  deri..author_ema
 00000050: 696c 203d 206a 6967 6172 6268 616e 6465  il = jigarbhande
 00000060: 7269 4067 6d61 696c 2e63 6f6d 0d0a 6465  ri@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
 00000080: 636b 6167 6520 666f 7220 4d6f 6e74 652d  ckage for Monte-
 00000090: 4361 726c 6f20 7369 6d75 6c61 7469 6f6e  Carlo simulation
```

### Comparing `iimcsim-0.0.3/src/iimcsim/MC.py` & `iimcsim-0.0.4/src/iimcsim/MC.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,14 @@
     def get_mc_set(self, shape_list):
         data_X = []; data_X1 = []
         data_y = []; data_y1 = []
         CORR_pattern = []
         CH1_ind = []
         CH2_ind = []
         for i in tqdm(range(self.max_Rate)):
-            #print('samle_len : ', len(shape_list))
-            #print('rate : ', i)
-            #print('samp_size : ', self.sample_size)
             x, y, x1, y1, cor_pat, ch1_ind, ch2_ind = mc(shape_list, i, self.exe, self.sample_size).MC2()
             data_X.append(x); data_X1.append(x1)
             data_y.append(y); data_y1.append(y1)
             CORR_pattern.append(cor_pat)
             CH1_ind.append(ch1_ind)
             CH2_ind.append(ch2_ind)
         #data_X, data_y = mc(shape_list,2,10,100).MC2()
```

### Comparing `iimcsim-0.0.3/src/iimcsim/MonteCarlo.py` & `iimcsim-0.0.4/src/iimcsim/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.3/src/iimcsim/data_gen.py` & `iimcsim-0.0.4/src/iimcsim/data_gen.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.3/src/iimcsim/shape_ext.py` & `iimcsim-0.0.4/src/iimcsim/shape_ext.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,19 @@
         self.high_rate_file = high_rate_file
         self.path_to_save = path_to_save
         
     def generator(self, threshold=0, bin_num=2147483600):
         arr0 = -np.load(self.calib_file)[:bin_num] + threshold
         arr = np.where(arr0<0,0,arr0)
         arr_sub = arr-1
-        arr_w = np.where(arr_sub<0,0,arr_sub)#/np.max(arr_sub)
-        arr_threshold = arr_w.reshape(np.int(arr_w.shape[0]/100),100)
+        arr_threshold = np.where(arr_sub<0,0,arr_sub)#/np.max(arr_sub)
+        #print('calib_shape:',arr_w.shape)
+        #print('arr:',arr.shape)
+        #print('arr_sub_shape : ', arr_sub.shape)
+        #arr_threshold = arr_w.reshape(np.int(arr_w.shape[0]/100),100)
 
         rate = []
         ind = []
         val = []
         for i in range(arr_threshold.shape[0]):
             peak_val, peak_ind = find_peaks(arr_threshold[i], height=0)
             rate.append(len(peak_val))
```

### Comparing `iimcsim-0.0.3/src/iimcsim.egg-info/PKG-INFO` & `iimcsim-0.0.4/src/iimcsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsim Version: 0.0.3 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.0.4 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

