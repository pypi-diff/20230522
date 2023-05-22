# Comparing `tmp/multimelt-0.1.tar.gz` & `tmp/multimelt-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimelt-0.1.tar", last modified: Thu Nov 10 16:07:57 2022, max compression
+gzip compressed data, was "multimelt-0.2.tar", last modified: Mon May 22 12:48:48 2023, max compression
```

## Comparing `multimelt-0.1.tar` & `multimelt-0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2022-11-10 16:07:57.035142 multimelt-0.1/
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    35149 2021-08-22 11:07:21.000000 multimelt-0.1/LICENSE
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     3402 2022-11-10 16:07:57.000000 multimelt-0.1/PKG-INFO
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2578 2022-09-07 10:13:34.000000 multimelt-0.1/README.rst
-drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2022-11-10 16:07:56.911137 multimelt-0.1/multimelt/
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    11422 2022-09-07 11:49:58.000000 multimelt-0.1/multimelt/T_S_profile_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)        0 2021-08-22 11:09:31.000000 multimelt-0.1/multimelt/__init__.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    16691 2022-09-01 09:53:04.000000 multimelt-0.1/multimelt/box_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     1890 2021-08-22 11:09:51.000000 multimelt-0.1/multimelt/constants.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    48142 2022-09-01 09:52:56.000000 multimelt-0.1/multimelt/create_isf_mask_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    91795 2022-09-28 10:11:43.000000 multimelt-0.1/multimelt/melt_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    30434 2022-09-28 10:11:43.000000 multimelt-0.1/multimelt/plume_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2223 2021-08-22 11:10:26.000000 multimelt-0.1/multimelt/useful_functions.py
-drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2022-11-10 16:07:57.023141 multimelt-0.1/multimelt.egg-info/
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     3402 2022-11-10 16:07:54.000000 multimelt-0.1/multimelt.egg-info/PKG-INFO
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)      424 2022-11-10 16:07:55.000000 multimelt-0.1/multimelt.egg-info/SOURCES.txt
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)        1 2022-11-10 16:07:55.000000 multimelt-0.1/multimelt.egg-info/dependency_links.txt
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)       47 2022-11-10 16:07:55.000000 multimelt-0.1/multimelt.egg-info/requires.txt
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)       10 2022-11-10 16:07:55.000000 multimelt-0.1/multimelt.egg-info/top_level.txt
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)       38 2022-11-10 16:07:57.000000 multimelt-0.1/setup.cfg
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2511 2022-09-07 10:23:33.000000 multimelt-0.1/setup.py
+drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 12:48:48.787328 multimelt-0.2/
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    35149 2021-08-22 11:07:21.000000 multimelt-0.2/LICENSE
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     3362 2023-05-22 12:48:48.000000 multimelt-0.2/PKG-INFO
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2558 2023-05-22 10:11:02.000000 multimelt-0.2/README.rst
+drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 12:48:48.583320 multimelt-0.2/multimelt/
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    11422 2022-09-07 11:49:58.000000 multimelt-0.2/multimelt/T_S_profile_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)        0 2021-08-22 11:09:31.000000 multimelt-0.2/multimelt/__init__.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    16843 2023-05-22 10:08:17.000000 multimelt-0.2/multimelt/box_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     1890 2021-08-22 11:09:51.000000 multimelt-0.2/multimelt/constants.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    71837 2023-05-22 12:20:40.000000 multimelt-0.2/multimelt/create_isf_mask_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    93979 2023-05-22 12:19:03.000000 multimelt-0.2/multimelt/melt_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    30434 2022-09-28 10:11:43.000000 multimelt-0.2/multimelt/plume_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2302 2023-05-22 10:08:53.000000 multimelt-0.2/multimelt/useful_functions.py
+drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 12:48:48.771327 multimelt-0.2/multimelt.egg-info/
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     3362 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/PKG-INFO
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)      424 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/SOURCES.txt
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)        1 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/dependency_links.txt
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)       52 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/requires.txt
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)       10 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/top_level.txt
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)       38 2023-05-22 12:48:48.000000 multimelt-0.2/setup.cfg
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2530 2023-05-22 12:23:51.000000 multimelt-0.2/setup.py
```

### Comparing `multimelt-0.1/LICENSE` & `multimelt-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multimelt-0.1/PKG-INFO` & `multimelt-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: multimelt
-Version: 0.1
+Version: 0.2
 Summary: Regroupment of the main existing ice shelf basal melt parameterisations
 Home-page: https://github.com/ClimateClara/multimelt
 Author: Clara Burgard
 Author-email: clara.burgard@univ-grenoble-alpes.fr
 License: GPL-3.0
 Project-URL: Source, https://github.com/ClimateClara/multimelt
 Project-URL: Tracker, https://github.com/ClimateClara/multimelt/issues
 Keywords: earth-sciences climate-modeling ice-sheet antarctica oceanography
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5
 License-File: LICENSE
@@ -65,16 +64,14 @@
 Don't hesitate to contact me if any questions arise: clara.burgard@univ-grenoble-alpes.fr
 
 How to cite multimelt
 ---------------------
 
 The detailed description of the application of the functions in multimelt is found in `Burgard et al., 2022`_ and should therefore, when used, be cited as follows:
 
-Burgard, C., Jourdain, N. C., Reese, R., Jenkins, A., and Mathiot, P.: An assessment of basal melt parameterisations for Antarctic ice shelves, The Cryosphere Discuss. [preprint], https://doi.org/10.5194/tc-2022-32, in review, 2022. 
-
-
-.. _`Burgard et al., 2022`: https://doi.org/10.5194/tc-2022-32
+Burgard, C., Jourdain, N. C., Reese, R., Jenkins, A., and Mathiot, P. (2022): An assessment of basal melt parameterisations for Antarctic ice shelves, The Cryosphere, https://doi.org/10.5194/tc-16-4931-2022. 
 
 
+.. _`Burgard et al., 2022`: https://doi.org/10.5194/tc-16-4931-2022
```

### Comparing `multimelt-0.1/README.rst` & `multimelt-0.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,14 @@
 Don't hesitate to contact me if any questions arise: clara.burgard@univ-grenoble-alpes.fr
 
 How to cite multimelt
 ---------------------
 
 The detailed description of the application of the functions in multimelt is found in `Burgard et al., 2022`_ and should therefore, when used, be cited as follows:
 
-Burgard, C., Jourdain, N. C., Reese, R., Jenkins, A., and Mathiot, P.: An assessment of basal melt parameterisations for Antarctic ice shelves, The Cryosphere Discuss. [preprint], https://doi.org/10.5194/tc-2022-32, in review, 2022. 
+Burgard, C., Jourdain, N. C., Reese, R., Jenkins, A., and Mathiot, P. (2022): An assessment of basal melt parameterisations for Antarctic ice shelves, The Cryosphere, https://doi.org/10.5194/tc-16-4931-2022. 
 
 
-.. _`Burgard et al., 2022`: https://doi.org/10.5194/tc-2022-32
+.. _`Burgard et al., 2022`: https://doi.org/10.5194/tc-16-4931-2022
```

### Comparing `multimelt-0.1/multimelt/T_S_profile_functions.py` & `multimelt-0.2/multimelt/T_S_profile_functions.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.1/multimelt/box_functions.py` & `multimelt-0.2/multimelt/box_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     
     # add a common dimension 'grid' along which to stack
     stacked_isf_points = isf_points_da.stack(grid=['y', 'x'])
     stacked_line = line_points_da.stack(grid=['y', 'x'])
     
     # remove nans
     filtered_isf_points = stacked_isf_points[stacked_isf_points>0]
+    #filtered_isf_points = stacked_isf_points.where(stacked_isf_points>0, drop=True)
+    #filtered_line = stacked_line.where(stacked_line>0, drop=True)
     filtered_line = stacked_line[stacked_line>0]
     
     # write out the y,x pairs behind the dimension 'grid'
     grid_isf_points = filtered_isf_points.indexes['grid'].to_frame().values.astype(float)
     grid_line = filtered_line.indexes['grid'].to_frame().values.astype(float)
     
     # create tree to line and compute distance
```

### Comparing `multimelt-0.1/multimelt/constants.py` & `multimelt-0.2/multimelt/constants.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.1/multimelt/create_isf_mask_functions.py` & `multimelt-0.2/multimelt/create_isf_mask_functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @author: Clara Burgard
 """
 
 import xarray as xr
 import numpy as np
 import pandas as pd
 from tqdm.notebook import tqdm, trange
+import cc3d
 #from tqdm import tqdm, trange
 import multimelt.plume_functions as pf
 import multimelt.useful_functions as uf
 import multimelt.box_functions as bf
 
 def read_isfmask_info(infile):
     
@@ -49,58 +50,298 @@
                 is_nb = int(ll[124:127])
                 is_name = str(ll[130:200])
             def_ismask.append([minlon,maxlon,minlat,maxlat,is_nb])
     res = np.array(def_ismask)
     return res
 
 
-def def_isf_mask(arr_def_ismask, file_msk, lon, lat, FRIS_one=True):
+def def_isf_mask(arr_def_ismask, file_msk, file_conc, lon, lat, FRIS_one=True, 
+                 mouginot_basins=False, variable_geometry=False, connectivity = 4, threshold = 4):
     
     """
     Define a mask for the individual ice shelves. 
     
     This function defines a mask for the individual ice shelves. I think it works for both stereographic and latlon grids but I have not tried the latter.
     
     Parameters
     ----------
     arr_def_ismask : np.array
-        Array containing minlon,maxlon,minlat,maxlat,is_nb.
+        Array containing minlon,maxlon,minlat,maxlat,is_nb or xr.Dataset with drainage basins
     file_msk : xr.DataArray
         Mask separating ocean (0), ice shelves (between 0 and 2, excluding 0 and 2), grounded ice (2) 
+    file_conc : xr.DataArray
+        Ice shelf concentration for each point (between 0 and 1)
     lon : xr.DataArray
         Longitude (depends on x,y for stereographic)
     lat : xr.DataArray
         Latitude (depends on x,y for stereographic)
-
+    FRIS_one : Boolean 
+        If True, Filchner-Ronne are considered as one ice-shelf
+    mouginot_basins : Boolean 
+        If True, arr_def_ismask is an xr.DataArray with drainage basins
+    variable_geometry : Boolean 
+        If True, arr_def_ismask
+    connectivity : int
+        4 or 8 for 2D, defines what is considered a "connected" point
+    threshold : int
+        Size of lonely pixel areas to remove
+        
     Returns
     -------
     new_mask : xr.DataArray
         Array showing the coverage of each ice shelf with the respective ID, open ocean is 1, land is 0
     """    
-
-    arr_def_general = arr_def_ismask[arr_def_ismask[:, 3] == -50]
-    arr_def_detail = arr_def_ismask[arr_def_ismask[:, 3] != -50]
     
-    isf_yes = (file_msk > 0) & (file_msk < 2)
-    isf_mask = file_msk.copy()
-    # is_mask0.plot()
-    for i, mm in enumerate(arr_def_general):
-        #print('general ' + str(i))
-        isf_mask = isf_mask.where(~(uf.in_range(lon, mm[0:2]) & uf.in_range(lat, mm[2:4])), int(mm[4]))
-    for i, mm in enumerate(arr_def_detail):
-        #print('detail ' + str(i))
-        isf_mask = isf_mask.where(~(uf.in_range(lon, mm[0:2]) & uf.in_range(lat, mm[2:4])), int(mm[4]))
-    isf_mask = isf_mask.where(isf_yes)
-    
-    if FRIS_one:
-        isf_mask = isf_mask.where(isf_mask != 21, 11) # Filchner (21) and Ronne (11) are combined
+    if mouginot_basins:
+        
+        isf_mask = file_msk.copy()
+        # only ice shelves
+        isf_only_mask = file_conc > 0
+        
+        #find connected components
+        dusted = cc3d.dust(isf_only_mask.values.astype(np.int64), 
+                   threshold = threshold, 
+                   connectivity = connectivity, 
+                   in_place = False)
+        
+        labels_out = cc3d.connected_components(dusted, 
+                                       connectivity = connectivity)
+        
+        labelled = xr.DataArray(labels_out, 
+                        coords = {"y": file_conc.y, "x": file_conc.x}, 
+                        dims = ["y", "x"],
+                        name = "labels")
+        
+        # assign ID for basins
+        isf_mask_basins = arr_def_ismask['ID_isf'].where(isf_only_mask > 0)
+        # cut connected areas to area covered by basin stuff
+        labelled_isf = labelled.where(np.isfinite(isf_mask_basins))
+        
+        # creating the mask
+        new_mask = isf_mask_basins.copy()
+        
+        new_mask = new_mask.where(
+            new_mask != 58, 57).where(
+            new_mask != 151, 99).where(
+            new_mask != 109, 107).where(
+            new_mask != 116, 5).where(
+            new_mask != 143, 97).where(
+            new_mask != 137, 99)
+        
+                    
+        arr_def_ismask['name_isf'].loc[{'Nisf': 57}] = 'Ross'
+        arr_def_ismask['name_isf'].loc[{'Nisf': 58}] = np.nan
+        
+        if FRIS_one:
+            new_mask = new_mask.where(new_mask != 104, 103)
+            arr_def_ismask['name_isf'].loc[{'Nisf': 103}] = 'Filchner-Ronne'
+            arr_def_ismask['name_isf'].loc[{'Nisf': 104}] = np.nan
+
+        arr_def_ismask['name_isf'] = arr_def_ismask['name_isf'].dropna('Nisf')
+        
+        # do some fine-tuning for overlapping ice shelves   
+        problem_regions = [2,3,8,9,10,13,23,26,27,28,29,32,34,38,44,46,50,57,59,60,
+                   63,70,71,72,73,74,76,77,78,83,84,85,89,91,96,103]
+        
+        for conn_label in range(1,labels_out.max()):
+            basins_conn_domain = arr_def_ismask['ID_isf'].where(labelled_isf == conn_label, drop=True)
+            max_label = basins_conn_domain.max().values
+            min_label = basins_conn_domain.min().values
+            
+            # for areas with two labels in problem regions, take the one with the most points
+            if max_label != min_label:
+                groups_isf = basins_conn_domain.groupby(basins_conn_domain)
+                groups_labels = groups_isf.groups.keys()
+                if groups_isf.count().ID_isf.count() > 1:
+                    if any(x in problem_regions for x in list(groups_labels)):
+                        #print(conn_label)
+                        #print(min_label,max_label)
+                        dominant_isf = groups_isf.count().idxmax().values
+                        if dominant_isf == 12:
+                            dominant_isf = 14
+                        #print(dominant_isf)
+                        new_mask = new_mask.where(labelled_isf != conn_label, dominant_isf)
+            
+        # other fine-tuning: if an ice shelf is split, keep the largest connected domain
+        dx = abs(file_conc.x[1] - file_conc.x[0])
+        dy = abs(file_conc.y[1] - file_conc.y[0])
+
+        split_regions = [70,77,83,89,103] 
+
+        for rreg in split_regions:
+            # look where there are the same labels in several unconnected domains
+            labels_same = list(new_mask.groupby(labelled_isf).groups) * (new_mask.groupby(labelled_isf).median() == rreg)
+            labels_same = labels_same[labels_same>0]
+
+            area_before = 0
+            for conn_label in labels_same:
+                # compute the area of the different unconnected areas
+                conc_for_area = file_conc.where(labelled_isf == conn_label, drop=True)
+                area_now = (conc_for_area * dx * dy).sum()
+                if area_now >= area_before:
+                    area_before = area_now
+                    largest_label = conn_label
+
+            # set the smaller areas to 159
+            for small_label in (labels_same.where(labels_same != largest_label).dropna('labels')):
+                new_mask = new_mask.where(labelled_isf != small_label, 159)
+
+        new_mask = new_mask + 1
+        new_mask_info = arr_def_ismask.copy()
+        new_mask_info['Nisf'] = new_mask_info['Nisf'] + 1
+        
+        new_mask = new_mask.where(file_msk != 0, 1).where(file_msk != 2, 0)
     
-    new_mask = isf_mask.where(file_msk != 0, 1).where(file_msk != 2, 0)
+    else:
+        
+        arr_def_general = arr_def_ismask[arr_def_ismask[:, 3] == -50]
+        arr_def_detail = arr_def_ismask[arr_def_ismask[:, 3] != -50]
+
+        isf_yes = (file_msk > 0) & (file_msk < 2)
+        isf_mask = file_msk.copy()
+        # is_mask0.plot()
+        for i, mm in enumerate(arr_def_general):
+            #print('general ' + str(i))
+            isf_mask = isf_mask.where(~(uf.in_range(lon, mm[0:2]) & uf.in_range(lat, mm[2:4])), int(mm[4]))
+        for i, mm in enumerate(arr_def_detail):
+            #print('detail ' + str(i))
+            isf_mask = isf_mask.where(~(uf.in_range(lon, mm[0:2]) & uf.in_range(lat, mm[2:4])), int(mm[4]))
+        isf_mask = isf_mask.where(isf_yes)
+
+        if FRIS_one:
+            isf_mask = isf_mask.where(isf_mask != 21, 11) # Filchner (21) and Ronne (11) are combined
+        
+        remaining_isf = (isf_mask > 0) & (isf_mask <= 1)
+        new_mask = isf_mask.where(~remaining_isf, 4)
+        new_mask = new_mask.where(file_msk != 0, 1).where(file_msk != 2, 0)
+        
+        if variable_geometry:
+            
+            print('YOU CHOSE VARIABLE GEOMETRY SO I NEED TO WORK A BIT MORE')
+            new_mask = new_mask.where(~((new_mask > 1) & (new_mask < 10)), 4)
+
+
+            dx = abs(new_mask.x[1] - new_mask.x[0]).values.astype(int)
+            dy = abs(new_mask.y[1] - new_mask.y[0]).values.astype(int)
+
+            ### SPECIAL REGIONS
+            new_mask = new_mask.where(new_mask != 102, 75)
+            new_mask = new_mask.where(new_mask != 103, 75)
+            new_mask = new_mask.where(new_mask != 114, 26)
+            new_mask = new_mask.where(new_mask != 81, 22)
+
+            print('I am separating splitted ice shelves')
+            ###### THIS BLOCK IS TO SEPARATE SPLIT REGIONS
+            threshold = 1
+            connectivity = 4
+
+            #find connected components
+            dusted = cc3d.dust(new_mask.values.astype(np.int64), 
+                       threshold = threshold, 
+                       connectivity = connectivity, 
+                       in_place = False)
+
+            labels_out = cc3d.connected_components(dusted, 
+                                           connectivity = connectivity)
+
+            labelled_isf = xr.DataArray(labels_out, 
+                            coords = {"y": file_conc.y, "x": file_conc.x}, 
+                            dims = ["y", "x"],
+                            name = "labels")
+
+            all_isf_list = np.array(list(new_mask.groupby(new_mask).groups))
+            isf_labels = all_isf_list[all_isf_list>9]
+
+            for rreg in isf_labels:
+                #print(rreg)
+                # look is one ice shelf is present in disconnected regions
+                isf_group = new_mask.where(new_mask==rreg)
+                label_group = labelled_isf.where(np.isfinite(isf_group))
+                label_group_list = np.array(list(label_group.groupby(label_group).groups))
+                label_group_list = label_group_list[label_group_list > 1]
+                if label_group_list.size > 0:
+                    if label_group_list.min() != label_group_list.max():
+                        area_before = 0
+                        for conn_label in label_group_list:
+                            # compute the area of the different unconnected areas
+                            conc_for_area = file_conc.where(labelled_isf == conn_label, drop=True)
+                            area_now = (conc_for_area * dx * dy).sum()
+                            if area_now >= area_before:
+                                area_before = area_now
+                                largest_label = conn_label
+
+                        # set the smaller areas to 4 
+                        for llabel in label_group_list:
+                            if llabel != largest_label:
+                                new_mask = new_mask.where(labelled_isf != llabel, 4)
+
+            print('I am filling ice-shelf regions that did not fit the initial limits')
+            ###### THIS BLOCK IS TO FILL THE "NEWLY ICE SHELF REGIONS"
+
+            #for n in range(4):
+            threshold = 1
+            connectivity = 4
+
+            scattered_reg_all_conc = file_conc.where(new_mask == 4) 
+            scattered_reg_all_mask = scattered_reg_all_conc > 0
+
+            #find connected components
+            dusted = cc3d.dust(scattered_reg_all_mask.values.astype(np.int64), 
+                       threshold = threshold, 
+                       connectivity = connectivity, 
+                       in_place = False)
+
+            labels_out_conc = cc3d.connected_components(dusted, 
+                                           connectivity = connectivity)
+
+            labelled = xr.DataArray(labels_out_conc, 
+                            coords = {"y": file_conc.y, "x": file_conc.x}, 
+                            dims = ["y", "x"],
+                            name = "labels")
+
+            # filter that checks the point around
+            weights_filter = np.zeros((3,3))
+            weights_filter[0,1] = 1
+            weights_filter[1,0] = 1
+            weights_filter[1,2] = 1
+            weights_filter[2,1] = 1
+
+            weights_da = xr.DataArray(data=weights_filter,dims=['y0','x0'])
+
+
+            for conn_label in range(1,labels_out_conc.max()+1):
+                dom_region = labelled.where(labelled == conn_label, drop=True)
+                dom_bounds_plus1 = np.array([dom_region.x.min().values - dx,dom_region.x.max().values + dx,dom_region.y.min().values - dy,dom_region.y.max().values + dy]).astype(int)
+                dom_plus1_mask = scattered_reg_all_mask.sel(x=range(dom_bounds_plus1[0],dom_bounds_plus1[1]+1,dx), y=range(dom_bounds_plus1[2],dom_bounds_plus1[3]+1,dy))
+                corr = pf.xr_nd_corr_v2(dom_plus1_mask, weights_filter)
+                only_contour = (corr ^ dom_plus1_mask)
+                neighboring_pixels = new_mask.where(only_contour)
+                if neighboring_pixels.max() > 9:
+                    neighbor_max = neighboring_pixels.where(neighboring_pixels > 9).max()
+                    neighbor_min = neighboring_pixels.where(neighboring_pixels > 9).min()
+                    if neighbor_max == neighbor_min:
+                        #print(neighbor_min.values)
+                        new_mask = new_mask.where(labelled != conn_label, neighbor_min)
+                    else:
+                        isf_cont = neighboring_pixels.where(neighboring_pixels > 1)
+                        isf_around = xr.DataArray(data=np.array(list(only_contour.groupby(isf_cont).groups))).assign_coords({'dim_0': np.array(list(only_contour.groupby(isf_cont).groups))})
+                        count_isf = (isf_cont == isf_around).sum(['x','y'])
+                        new_kisf = count_isf.dim_0.where(count_isf == count_isf.max(), drop=True).values[0]
+                        new_mask = new_mask.where(labelled != conn_label, new_kisf)
+    
+    
+    if mouginot_basins:
+        mask_file = xr.merge([new_mask.rename('ISF_mask'), 
+                              new_mask_info['name_isf'], 
+                              new_mask_info['name_reg'], 
+                              new_mask_info['Nisf_orig']])
+    else:
+        mask_file = new_mask
     
-    return new_mask
+    return mask_file
 
 def def_ground_mask(file_msk, dist, add_fac):
 
     """
     Define a mask for the Antarctic continent as such (not the islands). 
     
     This function defines the points that are part of the Antarctic continent as such (not the islands). 
@@ -114,23 +355,23 @@
     add_fac : int
        Defines additional iterations. Was introduced to get to the end of the Antarctic Peninsula, sometimes it would not get there otherwise. Current default is 100 but you are welcome to play around with it.
     Returns
     -------
     mask_ground : xr.DataArray
         Array showing the coverage of the Antarctic continent (0 for islands, 1 for ocean and ice shelves, 2 for mainland)
     """  
-
+    
     mask_10 = file_msk.where(file_msk == 2, 0).where(file_msk != 2,1) #set all ice shelves and open ocean to 0, set all grounded ice to 1
 
     mask_gnd = mask_10.where(mask_10>0, drop=True)
     mask_gnd = mask_gnd.where(mask_gnd>0,0)
     
     meshx_gnd, meshy_gnd = np.meshgrid(mask_gnd.x,mask_gnd.y)
-    meshx_gnd_da = mask_gnd.copy(data=meshx_gnd)
-    meshy_gnd_da = mask_gnd.copy(data=meshy_gnd)
+    meshx_gnd_da = mask_gnd.copy(data=np.broadcast_to(meshx_gnd, mask_gnd.shape))
+    meshy_gnd_da = mask_gnd.copy(data=np.broadcast_to(meshy_gnd, mask_gnd.shape))
     
     dx = abs(meshx_gnd_da.x[2] - meshx_gnd_da.x[1])
     dy = abs(meshx_gnd_da.y[2] - meshx_gnd_da.y[1])
     
     max_len_xy = max(len(meshx_gnd_da.x),len(meshx_gnd_da.y))
     half_range = round(max_len_xy/2)
     
@@ -142,20 +383,41 @@
     weights_filter[0,1] = 1
     weights_filter[1,0] = 1
     weights_filter[1,2] = 1
     weights_filter[2,1] = 1
     
     weights_da = xr.DataArray(data=weights_filter,dims=['y0','x0'])
     
-    iter_mask = mask_core.copy()
-    for n in tqdm(range(half_range+2*dist+add_fac)):
-        corr = pf.xr_nd_corr_v2(iter_mask, weights_filter)
-        iter_mask = iter_mask.where(~((corr >= 5) & (mask_core == 1)),5)
+    if 'time' in mask_gnd.dims:
+
+        iter_list = []
+        for tt,timet in enumerate(tqdm(mask_gnd.time)):
+
+            mask_core_tt = mask_core.isel(time=tt)
+            iter_mask = mask_core_tt.copy()
+            for n in range(half_range+2*dist+add_fac):
+                corr = pf.xr_nd_corr_v2(iter_mask, weights_filter)
+                iter_mask = iter_mask.where(~((corr >= 5) & (mask_core_tt == 1)),5)
+
+            iter_list.append(iter_mask)
+
+        iter_mask_all = xr.concat(iter_list,dim='time')
+        iter_mask_all = iter_mask_all.assign_coords({'time': mask_gnd.time})
+
+        mask_ground = iter_mask_all.where(iter_mask_all !=5, 2).reindex_like(mask_10)
+    
+    else:
+        
+        iter_mask = mask_core.copy()
+        for n in tqdm(range(half_range+2*dist+add_fac)):
+            corr = pf.xr_nd_corr_v2(iter_mask, weights_filter)
+            iter_mask = iter_mask.where(~((corr >= 5) & (mask_core == 1)),5)
 
-    mask_ground = iter_mask.where(iter_mask !=5, 2).reindex_like(mask_10)
+        mask_ground = iter_mask.where(iter_mask !=5, 2).reindex_like(mask_10)
+        
     mask_ground = mask_ground.where(mask_ground>0,0)
     
     return mask_ground
 
 def def_grounding_line(new_mask, mask_ground, ground_point, add_fac, dx, dy):
     
     """
@@ -198,73 +460,126 @@
     
     else: 
         
         mask_10 = mask_ground.where(mask_ground==2, 0) * 0.5
         weights_neighbors = np.array(([0, 1, 0], [1, 1, 1], [0, 1, 0]))
         xr_weights = xr.DataArray(data=weights_neighbors, dims=['y', 'x'])
 
-        xr_corr_neighbors = mask_10.copy(data=pf.nd_corr(mask_10,xr_weights))
+        if 'time' in mask_10.dims:
+
+            iter_list = []
+            for tt,timet in enumerate(tqdm(mask_10.time)):
+
+                mask_10_tt = mask_10.isel(time=tt)
+                xr_corr_neighbors = mask_10_tt.copy(data=pf.nd_corr(mask_10_tt,xr_weights))
+
+                new_mask_tt = new_mask.isel(time=tt)
+                mmask = (new_mask_tt>1).astype(int) + (xr_corr_neighbors>0).astype(int)
+                cut_gline = xr_corr_neighbors.where(mmask==2)
+                mask_gline_tt = new_mask_tt.where(cut_gline>0)#.load()
+
+                iter_list.append(mask_gline_tt)
+
+            mask_gline = xr.concat(iter_list,dim='time')
+            mask_gline = mask_gline.assign_coords({'time': mask_10.time})
         
-        mmask = (new_mask>1).astype(int) + (xr_corr_neighbors>0).astype(int)
-        cut_gline = xr_corr_neighbors.where(mmask==2)
-        mask_gline = new_mask.where(cut_gline>0)#.load()
-        #cut_gline = xr_corr_neighbors.where((new_mask>1) & (xr_corr_neighbors>0))
-        #mask_gline = new_mask.where(cut_gline>0).load()
+        else:
+            
+            xr_corr_neighbors = mask_10.copy(data=pf.nd_corr(mask_10,xr_weights))
+
+            mmask = (new_mask>1).astype(int) + (xr_corr_neighbors>0).astype(int)
+            cut_gline = xr_corr_neighbors.where(mmask==2)
+            mask_gline = new_mask.where(cut_gline>0)#.load()
         
         #################
         # fix the problems around Alexander Island (ice shelves with grounding line only on the island)
         mask_gline_orig = mask_gline.copy()
 
         larger_region = new_mask.sel(x=np.arange(-2998000.,0.5,dx),y=np.arange(2998000.,0,dy))
         mask_10_isl = larger_region.where(larger_region == 0, 5).where(larger_region != 0, 1)
         mask_isl = mask_10_isl.where(mask_10_isl == 1, 0) #set all ice shelves and open ocean to 0, set all grounded ice to 1
 
-        #meshx_gnd, meshy_gnd = np.meshgrid(mask_gnd.x,mask_gnd.y)
-        #meshx_gnd_da = mask_gnd.copy(data=meshx_gnd)
-        #meshy_gnd_da = mask_gnd.copy(data=meshy_gnd)
 
         core = mask_isl.sel(x=np.arange(-1938000.,-1900000., dx),y=np.arange(718000.,680000., dy)).reindex_like(mask_isl)
         mask_core = mask_isl.where(np.isnan(core),5)
 
         # filter that checks the point around
         weights_filter = np.zeros((3,3))
         weights_filter[0,1] = 1
         weights_filter[1,0] = 1
         weights_filter[1,2] = 1
         weights_filter[2,1] = 1
 
         weights_da = xr.DataArray(data=weights_filter,dims=['y0','x0'])
 
-        iter_mask = mask_core.copy()
-        for n in range(add_fac):
-            corr = pf.xr_nd_corr_v2(iter_mask, weights_filter)
-            iter_mask = iter_mask.where(~((corr >= 5) & (mask_core == 1)),5)
+        if 'time' in mask_10.dims:
+            
+            iter_list = []
+            for tt,timet in enumerate(tqdm(mask_gline_orig.time)):
+
+                    mask_core_tt = mask_core.isel(time=tt)
+                    iter_mask = mask_core_tt.copy()
+                    for n in range(add_fac):
+                        corr = pf.xr_nd_corr_v2(iter_mask, weights_filter)
+                        iter_mask = iter_mask.where(~((corr >= 5) & (mask_core_tt == 1)),5)
+
+                    iter_list.append(iter_mask)
+
+            iter_mask_all = xr.concat(iter_list,dim='time')
+            iter_mask_all = iter_mask_all.assign_coords({'time': mask_gline_orig.time})
+
+            mask_island = iter_mask_all.where(iter_mask_all !=5, 2)
+            
+        else:
+            
+            iter_mask = mask_core.copy()
+            for n in range(add_fac):
+                corr = pf.xr_nd_corr_v2(iter_mask, weights_filter)
+                iter_mask = iter_mask.where(~((corr >= 5) & (mask_core == 1)),5)
 
-        mask_island = iter_mask.where(iter_mask !=5, 2)
+            mask_island = iter_mask.where(iter_mask !=5, 2)
+            
         mask_island = mask_island.where(mask_island>0,0)
 
         ##########################################
 
         mask_10_island = mask_island.where(mask_island==2, 0) * 0.5
         weights_neighbors = np.array(([0, 1, 0], [1, 1, 1], [0, 1, 0]))
         xr_weights = xr.DataArray(data=weights_neighbors, dims=['y', 'x'])
+        
+        if 'time' in mask_10.dims:
+    
+            iter_list = []
+            for tt,timet in enumerate(tqdm(mask_10_island.time)):
+
+                mask_10_island_tt = mask_10_island.isel(time=tt)
+                xr_corr_neighbors = mask_10_island_tt.copy(data=pf.nd_corr(mask_10_island_tt,xr_weights))
+
+                cut_gline_tt = xr_corr_neighbors.where((larger_region.isel(time=tt)>1) & (xr_corr_neighbors>0))
 
-        xr_corr_neighbors = mask_10_island.copy(data=pf.nd_corr(mask_10_island,xr_weights))
+                iter_list.append(cut_gline_tt)
+
+            cut_gline = xr.concat(iter_list,dim='time')
+            cut_gline = cut_gline.assign_coords({'time': mask_10_island.time})
+            
+        else:
+            
+            xr_corr_neighbors = mask_10_island.copy(data=pf.nd_corr(mask_10_island,xr_weights))
 
-        cut_gline = xr_corr_neighbors.where((larger_region>1) & (xr_corr_neighbors>0))
+            cut_gline = xr_corr_neighbors.where((larger_region>1) & (xr_corr_neighbors>0))
+            
+    
         mask_gline_new = larger_region.where(cut_gline>0).reindex_like(mask_gline_orig)
+        mask_gline_final = mask_gline_orig.where(mask_gline_new != 54, mask_gline_new) # file_isf.Nisf.where(file_isf['isf_name'] == 'Bach', drop=True).values[0] (54)
+        mask_gline_final = mask_gline_final.where(mask_gline_new != 75, mask_gline_new) # file_isf.Nisf.where(file_isf['isf_name'] == 'Wilkins', drop=True).values[0] (75)
+        #mask_gline_final = mask_gline_final.where(mask_gline_new != 9, mask_gline_new) # only with Nico mask
+        #mask_gline_final = mask_gline_final.where(mask_gline_new != 98, mask_gline_new) # only with Nico mask - Verdi
+        #mask_gline_final = mask_gline_final.where(mask_gline_new != 99, mask_gline_new) # only with Nico mask - Brahms
+        #mask_gline_final = mask_gline_final.where(mask_gline_new != 100, mask_gline_new) # only with Nico mask - Mendelssohn
 
-        mask_gline_final = mask_gline_orig.where(mask_gline_new != 9, mask_gline_new)
-        mask_gline_final = mask_gline_final.where(mask_gline_new != 54, mask_gline_new)
-        mask_gline_final = mask_gline_final.where(mask_gline_new != 75, mask_gline_new)
-        mask_gline_final = mask_gline_final.where(mask_gline_new != 98, mask_gline_new)
-        mask_gline_final = mask_gline_final.where(mask_gline_new != 99, mask_gline_new)
-        mask_gline_final = mask_gline_final.where(mask_gline_new != 100, mask_gline_new)
-        
-        
     return mask_gline_final
 
 def def_ice_front(new_mask, file_msk):
 
     """
     Identify ice front points and assign ice shelf ID to these points. 
 
@@ -372,53 +687,61 @@
     return mask_pin2
 
 #latlonboundaryfile inputpath_metadata+'lonlat_masks.txt'
 #whole_ds.to_netcdf(outputpath+'BedMachineAntarctica_2020-07-15_v02_reduced5_isf_masks_and_info.nc')
 #outfile.to_netcdf(outputpath+'all_masks.nc','w')
 
 
-def create_isf_masks(file_map, file_msk, xx, yy, latlonboundary_file, outputpath, chunked, dx, dy, FRIS_one=True, ground_point='yes', write_ismask = 'yes', write_groundmask = 'yes', dist=150, add_fac=100):
-
+def create_isf_masks(file_map, file_msk, file_conc, xx, yy, latlonboundary_file, outputpath, chunked, dx, dy, FRIS_one=True, mouginot_basins=False, variable_geometry=False, ground_point='yes', write_ismask = 'yes', write_groundmask = 'yes', dist=150, add_fac=100, connectivity=4, threshold=4):
+ 
     """
     Identify the location of ice shelves, Antarctic mainland, grounding lines, ice fronts and pinning points. 
     
     This function creates masks identifying the location of ice shelves, Antarctic mainland, grounding lines, ice fronts and pinning points
     
     Parameters
     ----------
     file_map : xr.Dataset
         Dataset containing information about the grid
     file_msk : xr.DataArray
         Mask separating ocean (0), ice shelves (between 0 and 2, excluding 0 and 2), grounded ice (2)
+    file_conc : xr.DataArray
+        Ice shelf concentration for each point (between 0 and 1)
     xx : xr.DataArray
         x-coordinates for the domain.
     yy : xr.DataArray
         y-coordinates for the domain.
-    latlonboundary_file : str
-         Path to the csv-file containing the info. This function is tailored to the format of ``lonlat_masks.txt``.
+    latlonboundary_file : str 
+         Path to the csv-file containing the info. This function is tailored to the format of ``lonlat_masks.txt``. It takes the path to a netcdf-file if mouginot_basins is True.
     outputpath : str
         Path where the intermediate masks should be written to.
     chunked : int or False
         Size of chunks for dask when opening a netcdf into a dataset, if no need to chunk: False.
     dx : float
         Grid size in x direction, step from left to right (can be positive or negative depending on the initial coordinate).
     dy : float
         Grid size in x direction, step from left to right (can be positive or negative depending on the initial coordinate).
     FRIS_one : boolean
         True if Filchner-Ronne should be treated as one ice shelf, False if Filchner and Ronne should be separated.
+    mouginot_basins : Boolean 
+        If True, arr_def_ismask
     ground_point : str
         ``yes`` or ``no``. If ``yes``, the grounding line is defined on the ground points at the border to the ice shelf. If ``no``, the grounding line is defined on the ice shelf points at the border to the ground.
     write_ismask : str
         ``yes`` or ``no``. If ``yes``, compute the mask of the different ice shelves. If ``no``, read in the already existing file ``outputpath + 'preliminary_mask_file.nc'``.
     write_groundmask : str
         ``yes`` or ``no``. If ``yes``, compute the mask of mainland Antarctica. If ``no``, read in the already existing file ``outputpath + 'mask_ground.nc'``.
     dist : int
         Defines the size of the starting square for the ground mask - should be small if the resolution is coarse and high if the resolution is fine. Default is currently 150 but you can play around. A good indicator to see if it is too high is if you see the small upper tail of the Ross ice shelf or if it is masked as ground.
     add_fac : int
        Defines additional iterations for the propagation for the ground mask. Was introduced to get to the end of the Antarctic Peninsula, sometimes it would not get there otherwise. Current default is 100 but you are welcome to play around with it.
+    connectivity : int
+        4 or 8 for 2D, defines what is considered a "connected" point when looking at ice-shelves
+    threshold : int
+        Size of lonely pixel areas to remove for ice-shelf mask.
 
 
     Returns
     -------
     outfile : xr.Dataset
         Dataset containing all the produced masks: ISF_mask, GL_mask, IF_mask, PP_mask, ground_mask
     new_mask : xr.DataArray
@@ -446,24 +769,32 @@
     #####
     ##### PREPARE THE NETCDF WITH ICE SHELF NUMBERS AND THEIR FRONT, GROUNDING LINE AND PINNING POINT
     #####
 
     ### Read in the latlon boundaries of the ice shelves
 
     print('Reading in latlon boundaries')
-    arr_def_ismask = read_isfmask_info(latlonboundary_file)
+    if mouginot_basins:
+        arr_def_ismask = xr.open_dataset(latlonboundary_file)
+    else:
+        arr_def_ismask = read_isfmask_info(latlonboundary_file)
 
 
     ### Define the regional masks
 
     print('Define the regional masks')
 
     if write_ismask == 'yes':
-        new_mask = def_isf_mask(arr_def_ismask, file_msk, lon, lat, FRIS_one)
+        new_mask = def_isf_mask(arr_def_ismask, file_msk, file_conc, lon, lat, 
+                                FRIS_one, mouginot_basins, variable_geometry, connectivity, threshold)
         new_mask.to_netcdf(outputpath + 'preliminary_mask_file.nc', 'w')
+        
+        new_mask_info = new_mask
+        if mouginot_basins:
+            new_mask = new_mask['mask']
     else:
         print('read in from netcdf')
         if not chunked:
             new_mask_file = xr.open_mfdataset(outputpath + 'preliminary_mask_file.nc')
             #new_mask = new_mask_file['ls_mask012']
             new_mask = new_mask_file['mask']
         else:
@@ -555,17 +886,20 @@
     outfile['ground_mask'].attrs['units'] = '-'
 
     # Global attributes
     outfile.attrs['history'] = 'Created with create_isf_masks() by C. Burgard'
     outfile.attrs['projection'] = 'Polar Stereographic South (71S,0E)'
     outfile.attrs['proj4'] = '+init=epsg:3031'
     outfile.attrs['Note'] = 'isf ID and individual isf characteristics can be found in ice_shelf_metadata_complete.csv'
-    return outfile#, new_mask, mask_gline, mask_front
+    if mouginot_basins:
+        return outfile, new_mask_info # new_mask, mask_gline, mask_front
+    else:
+        return outfile
 
-def prepare_csv_metadata(file_metadata, file_metadata_GL_flux, file_conc, dx, dy, new_mask, FRIS_one):
+def prepare_csv_metadata(file_metadata, file_metadata_GL_flux, file_conc, dx, dy, new_mask, FRIS_one, mouginot_basins):
     
     """
     Prepare the metadata info (ice shelf names and observed melt rates). 
     
     This function creates a dataframe with the metadata for each ice shelf (name, area, observed melt rates from Rignot)
     
     Parameters
@@ -587,14 +921,17 @@
 
     Returns
     -------
     df1 : pandas.DataFrame
         DataFrame containing the following columns for each ice shelf: columns=['isf_name', 'region', 'isf_melt', 'melt_uncertainty','isf_area_rignot']
     """  
     
+    #if mouginot_basins:
+    #    new_mask = new_mask['mask']
+        
     ### Name, Area, Numbers from Rignot et al. 2013
     ismask_info = []
     file1 = open(file_metadata, 'r')
     Lines = file1.readlines()
     for ll in Lines:
         # print(ll)
         if ll[0] != '!':
@@ -606,64 +943,95 @@
             if ll[-2] == ';' or ll[132] == '!' or ll[132] == ' ':
                 is_area = np.nan
             else:
                 is_area = float(ll[148:155])
             if is_area == 1.:
                 is_area = np.nan
                 
-            ismask_info.append([is_nb0, is_name, is_region, is_melt_rate, is_melt_unc, is_area])
-            
+            if mouginot_basins:
+                if new_mask.Nisf.where(new_mask['Nisf_orig'] == is_nb0, drop=True):
+                    is_nb1 = new_mask.Nisf.where(new_mask['Nisf_orig'] == is_nb0, drop=True).values[0].astype(int)
+                    ismask_info.append([is_nb1, is_name, is_region, is_melt_rate, is_melt_unc, is_area])
+                elif is_name == 'Ross':
+                    is_nb1 = 59
+                    ismask_info.append([is_nb1, is_name, is_region, is_melt_rate, is_melt_unc, is_area])
+                elif is_name == 'Filchner':
+                    is_nb1 = 105
+                    ismask_info.append([is_nb1, is_name, is_region, is_melt_rate, is_melt_unc, is_area]) 
+                elif is_name == 'Ronne':
+                    is_nb1 = 104
+                    ismask_info.append([is_nb1, is_name, is_region, is_melt_rate, is_melt_unc, is_area]) 
+                #else:
+                #    ismask_info.append([is_nb0, is_name, is_region, is_melt_rate, is_melt_unc, is_area])
+            else:
+                ismask_info.append([is_nb0, is_name, is_region, is_melt_rate, is_melt_unc, is_area])
+
     arr_ismask_info = np.array(ismask_info)
     
     df = pd.DataFrame(arr_ismask_info[:, 1:6], index=arr_ismask_info[:, 0].astype(int),
                       columns=['isf_name', 'region', 'isf_melt', 'melt_uncertainty',
-                               'isf_area_rignot'])
+                               'isf_area_rignot'])        
+
     df['isf_melt'] = df['isf_melt'].astype(float)
     df['melt_uncertainty'] = df['melt_uncertainty'].astype(float)
     df['isf_area_rignot'] = df['isf_area_rignot'].astype(float)
     
-    if FRIS_one:
-        
+    if FRIS_one and not mouginot_basins:
+
         df['isf_name'].loc[11] = 'Filchner-Ronne'
         df['isf_melt'].loc[11] = df['isf_melt'].loc[11] + df['isf_melt'].loc[21]
         df['melt_uncertainty'].loc[11] = df['melt_uncertainty'].loc[11] + df['melt_uncertainty'].loc[21] # this might be a bit dodgy to add the uncertainties?
         df['isf_area_rignot'].loc[11] = df['isf_area_rignot'].loc[11] + df['isf_area_rignot'].loc[21] 
         df = df.drop(21)
+    
+    elif mouginot_basins:        
         
+        df['isf_name'].loc[104] = 'Filchner-Ronne'
+        df['isf_melt'].loc[104] = df['isf_melt'].loc[104] + df['isf_melt'].loc[105]
+        df['melt_uncertainty'].loc[104] = df['melt_uncertainty'].loc[104] + df['melt_uncertainty'].loc[105] # this might be a bit dodgy to add the uncertainties?
+        df['isf_area_rignot'].loc[104] = df['isf_area_rignot'].loc[104] + df['isf_area_rignot'].loc[105] 
+        df = df.drop(105)
     
     ### Compute area from our data
-    is_mask = new_mask.where(new_mask>1)
-    
+    if mouginot_basins:
+        is_mask = new_mask['mask'].where(new_mask['mask']>1)
+    else:
+        is_mask = new_mask.where(new_mask>1)
+        
     idx_da = xr.DataArray(data=df.index, dims=['Nisf']).chunk({'Nisf':1})
     
-    df['isf_area_here'] = file_conc.chunk({'x':1000,'y':1000}).where(is_mask == idx_da).sum(['x','y']) * abs(dx) * abs(dy) * 10 ** -6
-    
     
+    if 'time' not in file_conc.dims:    
+        df['isf_area_here'] = file_conc.chunk({'x':1000,'y':1000}).where(is_mask == idx_da).sum(['x','y']) * abs(dx) * abs(dy) * 10 ** -6
+
     ### Correct melt numbers using our area
     df1 = df.sort_index()
-    #print('here 1')
-    df1['isf_melt'] = df1['isf_melt'] * df1['isf_area_here'] / df1['isf_area_rignot']
-    #print('here 2')
-    df1['melt_uncertainty'] = df1['melt_uncertainty'] * df1['isf_area_here'] / df1['isf_area_rignot']
-    #print('here 3')
-    df1['ratio_isf_areas'] = df1['isf_area_here'] / df1['isf_area_rignot']
-    #print('here 4')
+        #print('here 1')
+        
+    if 'time' not in file_conc.dims: 
+        df1['isf_melt'] = df1['isf_melt'] * df1['isf_area_here'] / df1['isf_area_rignot']
+        #print('here 2')
+        df1['melt_uncertainty'] = df1['melt_uncertainty'] * df1['isf_area_here'] / df1['isf_area_rignot']
+        #print('here 3')
+        df1['ratio_isf_areas'] = df1['isf_area_here'] / df1['isf_area_rignot']
+        #print('here 4')
     
     # add grounding line flux as given by Rignot et al 2013
     GL_flux_pd = pd.read_csv(file_metadata_GL_flux, delimiter=';').dropna(how='all',axis=1).dropna(how='any',axis=0)
     df1['GL_flux'] = np.nan
-    for idx_gl in GL_flux_pd.index:
-        for idx in df1.index:
-            if df1['isf_name'].loc[idx] == GL_flux_pd['Ice Shelf Name'].loc[idx_gl]:
-                df1['GL_flux'].loc[idx] = float(GL_flux_pd['Grounding line flux'].loc[idx_gl])
-    
+    if not mouginot_basins:
+        for idx_gl in GL_flux_pd.index:
+            for idx in df1.index:
+                if df1['isf_name'].loc[idx] == GL_flux_pd['Ice Shelf Name'].loc[idx_gl]:
+                    df1['GL_flux'].loc[idx] = float(GL_flux_pd['Grounding line flux'].loc[idx_gl])
+
     return df1
 
     
-def compute_dist_front_bot_ice(mask_gline, mask_front, file_draft, file_bed, df1, lon, lat):
+def compute_dist_front_bot_ice(mask_gline, mask_front, file_draft, file_bed, df1, lon, lat, dx=False, dy=False, new_mask=False, file_conc=False):
 
     """
     Compute the depth of the bedrock and of the ice draft at the ice front. 
     
     This function computes the average and maximum depth of the bedrock and of the ice draft at the ice front.
     
     Parameters
@@ -685,42 +1053,71 @@
         
     Returns
     -------
     df1 : pd.DataFrame
         DataFrame containing the following columns for each ice shelf: columns=['isf_name', 'region', 'isf_melt', 'melt_uncertainty','isf_area_rignot'] AND ['front_bot_depth_max','front_bot_depth_avg','front_ice_depth_min','front_ice_depth_avg','front_min_lat','front_max_lat','front_min_lon','front_max_lon']
     """ 
     
-    #print('here 6')
     file_draft = file_draft.where(file_draft<0,0)
     
     idx_da = xr.DataArray(data=df1.index, dims=['Nisf']).chunk({'Nisf': 1})
+
+    if 'time' in mask_front.dims:
+
+        ds1 = xr.Dataset()
+        
+        is_mask = new_mask.where(new_mask>1)
+        ds1['isf_area_here'] = file_conc.chunk({'x':1000,'y':1000}).where(is_mask == idx_da).sum(['x','y']) * abs(dx) * abs(dy) * 10 ** -6
+
+        #print('here 7')
+        ds1['front_bot_depth_max'] = -1*file_bed.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
+        ds1['front_bot_depth_avg'] = -1*file_bed.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).mean(['x','y'])
+        ds1['front_ice_depth_min'] = -1*file_draft.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
+        ds1['front_ice_depth_avg'] = -1*file_draft.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).mean(['x','y'])
+
+        #print('here 8')
+        ds1['front_min_lat'] = lat.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
+        ds1['front_max_lat'] = lat.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
+        ds1['front_min_lon'] = lon.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
+        ds1['front_max_lon'] = lon.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
+
+        #print('here 9')
+        # special treatment for Ross
+        ds1['front_max_lon'].loc[dict({'Nisf': 10})] = lon.where(mask_front == 10).where(lon < -100).max()
+        ds1['front_min_lon'].loc[dict({'Nisf': 10})] = lon.where(mask_front == 10).where(lon > 100).min()
+
+        ds_clean = ds1.where(ds1['isf_area_here'] > 0, drop= True)
+        
+        return ds_clean
+
+    else:
+
+        #print('here 7')
+        df1['front_bot_depth_max'] = -1*file_bed.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
+        df1['front_bot_depth_avg'] = -1*file_bed.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).mean(['x','y'])
+        df1['front_ice_depth_min'] = -1*file_draft.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
+        df1['front_ice_depth_avg'] = -1*file_draft.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).mean(['x','y'])
+
+        #print('here 8')
+        df1['front_min_lat'] = lat.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
+        df1['front_max_lat'] = lat.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
+        df1['front_min_lon'] = lon.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
+        df1['front_max_lon'] = lon.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
+
+        #print('here 9')
+        # special treatment for Ross
+        df1['front_max_lon'].loc[10] = lon.where(mask_front == 10).where(lon < -100).max()
+        df1['front_min_lon'].loc[10] = lon.where(mask_front == 10).where(lon > 100).min()
+
+        #print('here 10')
+        df_clean = df1[df1['isf_area_here'] > 0]
     
-    #print('here 7')
-    df1['front_bot_depth_max'] = -1*file_bed.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
-    df1['front_bot_depth_avg'] = -1*file_bed.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).mean(['x','y'])
-    df1['front_ice_depth_min'] = -1*file_draft.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
-    df1['front_ice_depth_avg'] = -1*file_draft.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).mean(['x','y'])
-    
-    #print('here 8')
-    df1['front_min_lat'] = lat.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
-    df1['front_max_lat'] = lat.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
-    df1['front_min_lon'] = lon.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).min(['x','y'])
-    df1['front_max_lon'] = lon.chunk({'x': 1000, 'y': 1000}).where(mask_front==idx_da).max(['x','y'])
-    
-    #print('here 9')
-    # special treatment for Ross
-    df1['front_max_lon'].loc[10] = lon.where(mask_front == 10).where(lon < -100).max()
-    df1['front_min_lon'].loc[10] = lon.where(mask_front == 10).where(lon > 100).min()
-    
-    #print('here 10')
-    df_clean = df1[df1['isf_area_here'] > 0]
-    
-    return df_clean
+        return df_clean
     
-def prepare_metadata(file_metadata, file_metadata_GL_flux, dx, dy, new_mask, mask_gline, mask_front, file_draft, file_bed, file_conc, lon, lat, outputpath, write_metadata = 'yes', FRIS_one=True):
+def prepare_metadata(file_metadata, file_metadata_GL_flux, dx, dy, new_mask, mask_gline, mask_front, file_draft, file_bed, file_conc, lon, lat, outputpath, write_metadata = 'yes', FRIS_one=True, mouginot_basins=True):
 
     """
     Prepare the metadata info into a csv. 
     
     This function creates a panda DataFrame with all metadata (1D) info about the individual ice shelves.
     
     Parameters
@@ -756,55 +1153,76 @@
     FRIS_one : boolean
         True if Filchner-Ronne should be treated as one ice shelf, False if Filchner and Ronne should be separated.
         
     Returns
     -------
     df1 : pandas.DataFrame
         DataFrame containing the following columns for each ice shelf: columns=['isf_name', 'region', 'isf_melt', 'melt_uncertainty','isf_area_rignot','front_bot_depth_max','front_bot_depth_avg','front_ice_depth_min','front_ice_depth_avg','front_min_lat','front_max_lat','front_min_lon','front_max_lon']
+    ds1 : xr.Dataset
+        xarray Dataset containing ['front_bot_depth_max','front_bot_depth_avg','front_ice_depth_min','front_ice_depth_avg','front_min_lat','front_max_lat','front_min_lon','front_max_lon'] if time dependent geometry.
     """  
 
     #####
     ##### PREPARE THE CSV WITH THE METADATA OF EACH ICE SHELF
     #####
 
     print('Prepare csv with metadata')
 
     ### Name, Area, Numbers from Rignot et al. 2013
     if write_metadata == 'yes':
-        df1 = prepare_csv_metadata(file_metadata, file_metadata_GL_flux, file_conc, dx, dy, new_mask, FRIS_one) 
-        df1 = compute_dist_front_bot_ice(mask_gline, mask_front, file_draft, file_bed, df1, lon, lat)
+        df1 = prepare_csv_metadata(file_metadata, file_metadata_GL_flux, file_conc, dx, dy, new_mask, 
+                                   FRIS_one, mouginot_basins) 
+        if 'time' not in new_mask.dims:
+            df1 = compute_dist_front_bot_ice(mask_gline, mask_front, file_draft, file_bed, df1, lon, lat)
         df1.to_csv(outputpath + "ice_shelf_metadata_complete.csv")
+        
+        if 'time' in new_mask.dims:
+            ds1 = compute_dist_front_bot_ice(mask_gline, mask_front, file_draft, file_bed, df1, lon, lat, dx, dy, new_mask, file_conc)
+            ds1.to_netcdf(outputpath + "ice_shelf_metadata_time_stuff.nc")
+        else:
+            ds1 = None
+
     else:
         print('read complete metadata from csv')
         df1 = pd.read_csv(outputpath + "ice_shelf_metadata_complete.csv", index_col=0)
-    return df1
+        if 'time' in new_mask.dims:
+            ds1 = xr.open_dataset(outputpath + "ice_shelf_metadata_time_stuff.nc")
+        else:
+            ds1 = None
+            
+    return df1, ds1
 
-def combine_mask_metadata(df1, outfile):
+def combine_mask_metadata(df1, outfile, ds_time=False):
 
     """
     Combine the metadata and the mask info into one netcdf. 
     
     This function combines the metadata and the mask info into one netcdf.
     
     Parameters
     ----------
     df1 : pandas.DataFrame
         DataFrame containing 1D info for each ice shelf
     outfile : xr.Dataset
         Dataset containing all the produced masks: ISF_mask, GL_mask, IF_mask, PP_mask, ground_mask
+    ds_time : xr.Dataset
+        Dataset containing metadata for each time step in the case there is a time evolution of the geometry
         
     Returns
     -------
     whole_ds : xr.Dataset
         Dataset containing all information from df1 and outfile 
     """  
     
     df_ds = df1.to_xarray()
     whole_ds = outfile.merge(df_ds)
     whole_ds = whole_ds.rename({"index": "Nisf"})
+    
+    if 'time' in outfile.dims:
+        whole_ds = whole_ds.merge(ds_time)
 
     whole_ds['Nisf'].attrs['standard_name'] = 'ice shelf ID'
     whole_ds['isf_name'].attrs['standard_name'] = 'ice shelf name'
     whole_ds['region'].attrs['standard_name'] = 'region'
     whole_ds['region'].attrs['long_name'] = 'Region name'
     whole_ds['isf_melt'].attrs['standard_name'] = 'ice shelf melt'
     whole_ds['isf_melt'].attrs['units'] = 'Gt/yr'
@@ -812,17 +1230,17 @@
     whole_ds['melt_uncertainty'].attrs['units'] = 'Gt/yr'
     whole_ds['isf_area_rignot'].attrs['standard_name'] = 'ice shelf area Rignot'
     whole_ds['isf_area_rignot'].attrs['units'] = 'km^2'
     whole_ds['isf_area_rignot'].attrs['long_name'] = 'Ice shelf area in Rignot et al 2013'
     whole_ds['isf_area_here'].attrs['standard_name'] = 'our ice shelf area'
     whole_ds['isf_area_here'].attrs['units'] = 'km^2'
     whole_ds['isf_area_here'].attrs['long_name'] = 'Ice shelf area computed from our mask'
-    whole_ds['ratio_isf_areas'].attrs['standard_name'] = 'ratio isf area here/Rignot'
-    whole_ds['ratio_isf_areas'].attrs['units'] = '-'
-    whole_ds['ratio_isf_areas'].attrs['long_name'] = 'Ratio between ice shelf area computed from our mask and area from Rignot et al 2013'
+    #whole_ds['ratio_isf_areas'].attrs['standard_name'] = 'ratio isf area here/Rignot'
+    #whole_ds['ratio_isf_areas'].attrs['units'] = '-'
+    #whole_ds['ratio_isf_areas'].attrs['long_name'] = 'Ratio between ice shelf area computed from our mask and area from Rignot et al 2013'
     whole_ds['GL_flux'].attrs['standard_name'] = 'grounding_line_flux'
     whole_ds['GL_flux'].attrs['units'] = 'Gt/yr'
     whole_ds['GL_flux'].attrs['long_name'] = 'Flux across grounding line from Rignot et al 2013'
     whole_ds['front_bot_depth_max'].attrs['standard_name'] = 'max depth between isf front and ocean bottom'
     whole_ds['front_bot_depth_max'].attrs['units'] = 'm'
     whole_ds['front_bot_depth_max'].attrs['long_name'] = 'Maximum depth between the ice shelf front and ocean bottom'
     whole_ds['front_bot_depth_avg'].attrs['standard_name'] = 'avg depth between isf front and ocean bottom'
@@ -874,36 +1292,80 @@
     ######
     ###### DO THE COMPUTATION AND ADD THE DISTANCE TO THE DATASET
     ######
 
     whole_ds['dGL'] = whole_ds['ISF_mask'] * np.nan
     whole_ds['dIF'] = whole_ds['ISF_mask'] * np.nan
     whole_ds['dGL_dIF'] = whole_ds['ISF_mask'] * np.nan
+    
+    
 
     for kisf in tqdm(whole_ds['Nisf']):
 
-        if ~np.isnan(whole_ds['GL_mask'].where(whole_ds['GL_mask'] == kisf).max()):
-            domain = whole_ds['ISF_mask'].where(whole_ds['ISF_mask'] >= 0)
-            isf_area = whole_ds['ISF_mask'].where(whole_ds['ISF_mask'] == kisf).dropna('x', how='all').dropna('y',
-                                                                                                              how='all')
-            isf_gl = whole_ds['GL_mask'].where(whole_ds['GL_mask'] == kisf).dropna('x', how='all').dropna('y', how='all')
-            isf_if = whole_ds['IF_mask'].where(whole_ds['IF_mask'] == kisf).dropna('x', how='all').dropna('y', how='all')
-
-            # Compute distance from grounding line
-            xr_dist_to_gl = bf.distance_isf_points_from_line(domain, isf_area, isf_gl)
-            whole_ds['dGL'] = whole_ds['dGL'].where(np.isnan(xr_dist_to_gl), xr_dist_to_gl)
-
-            # Compute distance from ice front (for ice shelf points)
-            xr_dist_to_if = bf.distance_isf_points_from_line(domain, isf_area, isf_if)
-            whole_ds['dIF'] = whole_ds['dIF'].where(np.isnan(xr_dist_to_if), xr_dist_to_if)
-
-            domain_gl = whole_ds['GL_mask'].where(whole_ds['GL_mask'] >= 0)
-            # Compute distance from ice front (for grounding line)
-            xr_dist_dgl_if = bf.distance_isf_points_from_line(domain_gl, isf_gl, isf_if)
-            whole_ds['dGL_dIF'] = whole_ds['dGL_dIF'].where(np.isnan(xr_dist_dgl_if), xr_dist_dgl_if)
+        
+            
+        if 'time' in whole_ds.dims:
+            
+            whole_ds0 = whole_ds.isel(time=0)
+
+            if ~np.isnan(whole_ds0['GL_mask'].where(whole_ds0['GL_mask'] == kisf).max()):
+
+                #print(whole_ds.dims)
+
+                iter_list = []
+                for tt,timet in enumerate(whole_ds.time):
+
+                    whole_ds_tt = whole_ds.isel(time=tt).copy()
+
+                    domain = whole_ds_tt['ISF_mask'].where(whole_ds_tt['ISF_mask'] >= 0)
+                    isf_area = whole_ds_tt['ISF_mask'].where(whole_ds_tt['ISF_mask'] == kisf).dropna('x', how='all').dropna('y', how='all')
+                    isf_gl = whole_ds_tt['GL_mask'].where(whole_ds_tt['GL_mask'] == kisf).dropna('x', how='all').dropna('y', how='all')
+                    isf_if = whole_ds_tt['IF_mask'].where(whole_ds_tt['IF_mask'] == kisf).dropna('x', how='all').dropna('y', how='all')
+
+                    # Compute distance from grounding line
+                    xr_dist_to_gl = bf.distance_isf_points_from_line(domain, isf_area, isf_gl)
+                    whole_ds_tt['dGL'] = whole_ds_tt['dGL'].where(np.isnan(xr_dist_to_gl), xr_dist_to_gl)
+
+                    # Compute distance from ice front (for ice shelf points)
+                    xr_dist_to_if = bf.distance_isf_points_from_line(domain, isf_area, isf_if)
+                    whole_ds_tt['dIF'] = whole_ds_tt['dIF'].where(np.isnan(xr_dist_to_if), xr_dist_to_if)
+
+                    domain_gl = whole_ds_tt['GL_mask'].where(whole_ds_tt['GL_mask'] >= 0)
+                    # Compute distance from ice front (for grounding line)
+                    xr_dist_dgl_if = bf.distance_isf_points_from_line(domain_gl, isf_gl, isf_if)
+                    whole_ds_tt['dGL_dIF'] = whole_ds_tt['dGL_dIF'].where(np.isnan(xr_dist_dgl_if), xr_dist_dgl_if)
+
+                    iter_list.append(whole_ds_tt.chunk({'x': 500, 'y': 500}))
+
+                whole_ds_new = xr.concat(iter_list, dim='time')
+                whole_ds_new = whole_ds_new.assign_coords({'time': whole_ds.time})
+                whole_ds = whole_ds_new
+
+        else:
+            
+            if ~np.isnan(whole_ds['GL_mask'].where(whole_ds['GL_mask'] == kisf).max()):
+
+                domain = whole_ds['ISF_mask'].where(whole_ds['ISF_mask'] >= 0)
+                isf_area = whole_ds['ISF_mask'].where(whole_ds['ISF_mask'] == kisf).dropna('x', how='all').dropna('y',
+                                                                                                                  how='all')
+                isf_gl = whole_ds['GL_mask'].where(whole_ds['GL_mask'] == kisf).dropna('x', how='all').dropna('y', how='all')
+                isf_if = whole_ds['IF_mask'].where(whole_ds['IF_mask'] == kisf).dropna('x', how='all').dropna('y', how='all')
+
+                # Compute distance from grounding line
+                xr_dist_to_gl = bf.distance_isf_points_from_line(domain, isf_area, isf_gl)
+                whole_ds['dGL'] = whole_ds['dGL'].where(np.isnan(xr_dist_to_gl), xr_dist_to_gl)
+
+                # Compute distance from ice front (for ice shelf points)
+                xr_dist_to_if = bf.distance_isf_points_from_line(domain, isf_area, isf_if)
+                whole_ds['dIF'] = whole_ds['dIF'].where(np.isnan(xr_dist_to_if), xr_dist_to_if)
+
+                domain_gl = whole_ds['GL_mask'].where(whole_ds['GL_mask'] >= 0)
+                # Compute distance from ice front (for grounding line)
+                xr_dist_dgl_if = bf.distance_isf_points_from_line(domain_gl, isf_gl, isf_if)
+                whole_ds['dGL_dIF'] = whole_ds['dGL_dIF'].where(np.isnan(xr_dist_dgl_if), xr_dist_dgl_if)
 
     ######
     ###### UPDATE ATTRIBUTES
     ######
 
     # Variable attributes
     whole_ds['dGL'].attrs['units'] = 'm'
@@ -918,15 +1380,15 @@
 
     # Global attributes
     whole_ds.attrs['history'] = 'Created with combine_mask_metadata() by C. Burgard. dGL, dIF and dGL_dIF added by compute_distance_GL_IF_ISF()'
     
     return whole_ds
 
 
-def create_mask_and_metadata_isf(file_map, file_bed, file_msk, file_draft, file_conc, chunked, latlonboundary_file, outputpath, file_metadata, file_metadata_GL_flux, ground_point, FRIS_one=True, write_ismask = 'yes', write_groundmask = 'yes', write_outfile='yes', dist=150, add_fac=100, write_metadata = 'yes'):
+def create_mask_and_metadata_isf(file_map, file_bed, file_msk, file_draft, file_conc, chunked, latlonboundary_file, outputpath, file_metadata, file_metadata_GL_flux, ground_point, FRIS_one=True, mouginot_basins=False, variable_geometry=False, write_ismask = 'yes', write_groundmask = 'yes', write_outfile='yes', dist=150, add_fac=100, connectivity=4, threshold=4, write_metadata = 'yes'):
     
     """
     Create mask and metadata file for all ice shelves. 
     
     This function creates a dataset containing masks and metadata for the ice shelves in Antarctica. The input must be on a stereographic grid centered around Antarctica. 
     
     Parameters
@@ -977,23 +1439,41 @@
     xx = file_map['x']
     yy = file_map['y']
     dx = xx[2] - xx[1]
     dy = yy[2] - yy[1]
     
     print('--------- PREPARE THE MASKS --------------')
     if write_outfile == 'yes':
-        outfile = create_isf_masks(file_map, file_msk, xx, yy, latlonboundary_file, outputpath, chunked, dx, dy, FRIS_one, ground_point, write_ismask, write_groundmask, dist, add_fac)
-        outfile.to_netcdf(outputpath + 'outfile.nc', 'w')
+        if mouginot_basins:
+            outfile, new_mask_info = create_isf_masks(file_map, file_msk, file_conc, xx, yy, latlonboundary_file, outputpath, chunked, dx, dy, FRIS_one, mouginot_basins, variable_geometry, ground_point, write_ismask, write_groundmask, dist, add_fac, connectivity, threshold)
+            outfile.to_netcdf(outputpath + 'outfile.nc', 'w')
+            new_mask_info.to_netcdf(outputpath + 'new_mask_info.nc', 'w')
+        else:
+            outfile = create_isf_masks(file_map, file_msk, file_conc, xx, yy, latlonboundary_file, outputpath, chunked, dx, dy, FRIS_one, mouginot_basins, variable_geometry, ground_point, write_ismask, write_groundmask, dist, add_fac, connectivity, threshold)
+            outfile.to_netcdf(outputpath + 'outfile.nc', 'w')
     else:
         outfile = xr.open_dataset(outputpath + 'outfile.nc')
+        if mouginot_basins:
+            new_mask_info = xr.open_dataset(outputpath + 'new_mask_info.nc')
     
     print('--------- PREPARE THE METADATA --------------')
-    df1 = prepare_metadata(file_metadata, file_metadata_GL_flux, dx, dy, outfile['ISF_mask'], outfile['GL_mask'], outfile['IF_mask'], file_draft, file_bed, file_conc, outfile['longitude'], outfile['latitude'], outputpath, write_metadata, FRIS_one)
+    if 'time' in outfile.dims:
+        df1, ds1 = prepare_metadata(file_metadata, file_metadata_GL_flux, dx, dy, outfile['ISF_mask'], outfile['GL_mask'], outfile['IF_mask'], file_draft, file_bed, file_conc, outfile['longitude'], outfile['latitude'], outputpath, write_metadata, FRIS_one)
+    else:
+        if mouginot_basins:
+            df1, _ = prepare_metadata(file_metadata, file_metadata_GL_flux, dx, dy, new_mask_info, outfile['GL_mask'], outfile['IF_mask'], file_draft, file_bed, file_conc, outfile['longitude'], outfile['latitude'], outputpath, write_metadata, FRIS_one, mouginot_basins)
+        else:
+            df1, _ = prepare_metadata(file_metadata, file_metadata_GL_flux, dx, dy, outfile['ISF_mask'], outfile['GL_mask'], outfile['IF_mask'], file_draft, file_bed, file_conc, outfile['longitude'], outfile['latitude'], outputpath, write_metadata, FRIS_one, mouginot_basins)
+
+
     print('--------- COMBINE MASK AND METADATA --------------')
-    whole_ds = combine_mask_metadata(df1, outfile)
+    if 'time' in outfile.dims:
+        whole_ds = combine_mask_metadata(df1, outfile, ds1)
+    else:
+        whole_ds = combine_mask_metadata(df1, outfile)
     print('--------- COMPUTE DISTANCE TO GROUNDING LINE AND ICE FRONT --------------')
     whole_ds = compute_distance_GL_IF_ISF(whole_ds)
     
     return whole_ds
```

### Comparing `multimelt-0.1/multimelt/melt_functions.py` & `multimelt-0.2/multimelt/melt_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -739,15 +739,14 @@
         Mterm = compute_Mterm(T_in, S_in, Tf, c_rho_1, c_tau, gamma, E0, alpha, thermal_forcing)
         
     melt_rate = Mterm * M_hat * rho_sw/rho_i
     
     return melt_rate
 
 
-
     
 def plume_param_modif(theta_isf,salinity_isf,ice_draft_points,front_bot_dep_max_isf,zGL_isf,alpha_isf,conc_isf,dGL_isf,gamma,E0):
     
     """
     Apply the plume parametrization with modifications (from Burgard et al. 2022).
     
     This function computes the basal melt based on a plume parameterisation (see Lazeroms et al. 2018 and Lazeroms et al. 2019) with modifications from pers. comm. between A. Jenkins and C. Burgard & N. Jourdain.
@@ -865,44 +864,74 @@
     Returns
     -------
     T_corrected : array
         Corrected temperature profile in degrees C.
     """
     
     #print('T_correction!')
-    if isf_name in ['Filchner','Ronne']: #1
-        T_correction= 0.100282
+    if isf_name in ['Filchner','Ronne','Filchner-Ronne']: #1
+        T_correction= 0.17475163929428827 # Best
+        # T_correction = 0.0743606316460328 # Max
+        # T_correction = 0.5244083302228169 # Min
     elif isf_name in ['Stancomb Brunt','Riiser-Larsen']: #2
-        T_correction= -0.149999
+        T_correction= -0.0255081029413049 # Best
+        # T_correction = -0.12548257518694172 # Max
+        # T_correction = 0.1501077396062951 # Min
     elif isf_name in ['Fimbul','Ekstrom']: #3
-        T_correction= -0.339190
+        T_correction= -0.2395108534458497 # Best
+        # T_correction = -0.3148726679812903 # Max
+        # T_correction = -0.08954377969106031 # Min
     elif isf_name in ['Roi Baudouin','Nivl','Lazarev','Borchgrevink','Jelbart','Prince Harald']: #4
-        T_correction= -0.230268
+        T_correction= -0.2395108534458497 # Best
+        # T_correction = -0.2302679118230881 # Max
+        # T_correction = 0.019731915700313518 # Min
     elif isf_name in ['Amery']: #6
-        T_correction= -0.225311
+        T_correction= -0.1499489774269802 # Best
+        # T_correction = -0.2253108845620384 # Max
+        # T_correction = 0.02450222960220194 # Min
     elif isf_name in ['West','Shackleton','Tracy Tremenchus']: #7
-        T_correction= -0.099989
+        T_correction= 0.07451035394701355 # Best 
+        # T_correction = -0.025540487708914258 # Max
+        # T_correction = 0.27447478156728833 # Min
     elif isf_name in ['Totten','Moscow Univ.']: #8
-        T_correction= -1.321668
+        T_correction= -1.1254891863236058 # Best 
+        # T_correction = -1.2739265689483057 # Max
+        # T_correction = -0.9255087879987864 # Min
     elif isf_name in ['Cook']: #9
-        T_correction= -0.508674
+        T_correction= -0.3921345255042934 # Best
+        # T_correction = -0.4564870583860179 # Max
+        # T_correction = -0.32351184947581224 # Min
     elif isf_name in ['Ross']: #12
-        T_correction= 0.249697
+        T_correction= 0.3496226730326237 # Best
+        # T_correction = 0.17430680792175826 # Max
+        # T_correction = 0.7497004029068532 # Min
     elif isf_name in ['Getz','Nickerson','Sulzberger','Dotson']: #13
-        T_correction= -1.299967
+        T_correction= -1.1000717723391031 # Best
+        # T_correction = -1.2500222564940329 # Max
+        # T_correction = -0.8500613833763373 # Min
     elif isf_name in ['Pine Island','Thwaites','Crosson']: #14
-        T_correction= -1.775460
+        T_correction= -1.3499828424718645 # Best
+        # T_correction = -1.67548468708992 # Max
+        # T_correction = -0.92548468708992 # Min
     elif isf_name in ['Cosgrove','Abbot','Venable']: #15
-        T_correction= -1.999992
+        T_correction= -1.9999923008093563 # Best
+        # T_correction = -1.9999923008093563 # Max
+        # T_correction = -1.9999923008093563 # Min
     elif isf_name in ['Wilkins','Stange','Bach','George VI']: #16
-        T_correction= -1.999993
+        T_correction= -1.9999930749714996 # Best
+        # T_correction = -1.9999930749714996 # Max
+        # T_correction = -1.6999787982359889 # Min
     elif isf_name in ['Larsen C']: #18
-        T_correction= -0.507423
+        T_correction= -0.3819311957529061 # Best
+        # T_correction = -0.4819107321859564 # Max
+        # T_correction = -0.15736237917388785 # Min
     elif isf_name in ['Larsen D']: #19
-        T_correction= -0.292285
+        T_correction= -0.14732530277455758 # Best
+        # T_correction = -0.1616054051436846 # Max
+        # T_correction = -0.09932079835170393 # Min
     
     T_corrected = T_in + T_correction
     return T_corrected
 
 def PICO_and_PICOP_param(T_in,S_in,box_location,box_depth_below_surface,box_area_whole,nD,spatial_coord,isf_cell_area,
                          gamma, E0, C,
                          picop='no',pism_version='no',zGL=None,alpha=None,ice_draft_neg=None):
@@ -1283,15 +1312,15 @@
         da_out = da_in.copy()
     else:
         da_out = xr.concat([da_out, da_in], dim=dim)
     return da_out
 
 
 
-def calculate_melt_rate_2D_simple_1isf(kisf, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, U_param=True):
+def calculate_melt_rate_2D_simple_1isf(kisf, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, U_param=True, HUB=False):
     
     """
     Function to compute melt from simple parameterisations for one ice shelf.
         
     Parameters
     ----------
     kisf : int
@@ -1323,14 +1352,17 @@
     # decide on the depth to which to extrapolate the entry temperature
     if mparam[-6::]=='bottom':
         mparam0 = mparam[:-7:]
         # deepest entrance point
         #depth_of_int = geometry_isf_1D['front_bot_depth_max'] # deepest point of the entrance
         depth_of_int = geometry_isf_1D['front_bot_depth_avg']
         depth_of_int.where(geometry_isf_2D)
+    elif HUB:
+        mparam0 = mparam
+        depth_of_int = geometry_isf_2D['ice_draft_pos'].where(geometry_isf_2D['ice_draft_pos']<geometry_isf_2D['HUB_depth'], geometry_isf_2D['HUB_depth'])
     else:
         mparam0 = mparam
         # either the depth of the draft or the deepest entrance point
         depth_of_int = geometry_isf_2D['ice_draft_pos'].where(geometry_isf_2D['ice_draft_pos']<geometry_isf_1D['front_bot_depth_max'], geometry_isf_1D['front_bot_depth_max']) # ice draft depth or deepest entrance depth
     
     #print('here1')
     # extrapolate temperature and salinity at the given depth
@@ -1422,15 +1454,15 @@
     isf_cell_area = geometry_isf_2D['grid_cell_area_weighted']
     
     front_bot_dep_max_isf = geometry_info_1D['front_bot_depth_max'].sel(Nisf=kisf)
     theta_isf = T_S_profile['theta_ocean'].sel(Nisf=kisf)
     salinity_isf = T_S_profile['salinity_ocean'].sel(Nisf=kisf)
     
     zGL_cavity_pos = -1*zGL_isf.sel(option='cavity') 
-    
+
     if mparam == 'lazero19':
         
         moption = 'lazero'
         zGL = zGL_isf.sel(option=moption)
         zGL_pos = -1*zGL
         alpha = alpha_isf.sel(option=moption)
         
@@ -1457,15 +1489,14 @@
         S0_mean_cav = uf.weighted_mean(S0_loc, ['mask_coord'], conc_isf)
         #print(kisf)
         #print(T0_mean_cav)
         #print(S0_mean_cav)
         
         melt_rate = plume_param(T0_mean_cav, S0_mean_cav, -1*ice_draft_pos_isf, zGL.squeeze().drop('option'), alpha.squeeze().drop('option'), 
                               gamma, E0)
-
     
     elif mparam == 'lazero19_modif':
         melt_rate = plume_param_modif(theta_isf,salinity_isf,
                                        ice_draft_pos_isf,front_bot_dep_max_isf,zGL_isf,alpha_isf,conc_isf,dGL_isf,
                                        gamma,E0)
     
     return melt_rate
@@ -1631,15 +1662,16 @@
                                        pism_version, picop_opt)
 
     return m_out
 
 
 def calculate_melt_rate_2D_1isf(kisf, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, 
                                 U_param=True, C=None, E0=None, angle_option='lazero',
-                                box_charac_2D=None, box_charac_1D=None, box_tot=None, box_tot_option='box_nb_tot', pism_version='no', picop_opt='no', gamma_plume=None, T_corrections=False):
+                                box_charac_2D=None, box_charac_1D=None, box_tot=None, box_tot_option='box_nb_tot', pism_version='no', picop_opt='no', gamma_plume=None, 
+                                T_corrections=False, HUB=False):
 
         """
         Wrap function to point to the right melt parameterisation for one ice shelf.
 
         Parameters
         ----------
         kisf : int
@@ -1691,15 +1723,15 @@
         filled_TS = T_S_profile.ffill(dim='depth')
         if mparam in ['linear_local', 'quadratic_local', 'quadratic_local_locslope','quadratic_local_cavslope',
                       'quadratic_mixed_mean', 'quadratic_mixed_locslope','quadratic_mixed_cavslope',
                      'linear_local_bottom', 'quadratic_local_bottom', 'quadratic_local_locslope_bottom','quadratic_local_cavslope_bottom',
                       'quadratic_mixed_mean_bottom', 'quadratic_mixed_locslope_bottom','quadratic_mixed_cavslope_bottom']:
             #print('Computing simple '+mparam+' melt rates and writing to file')
             melt_rate_2D_isf = calculate_melt_rate_2D_simple_1isf(kisf, filled_TS, geometry_info_2D, geometry_info_1D, 
-                                                                  isf_stack_mask, mparam, gamma, U_param)
+                                                                  isf_stack_mask, mparam, gamma, U_param, HUB)
         elif mparam in ['lazero19', 'lazero19_modif']:
             #print('Computing plume '+mparam+' melt rates and writing to file')
             if E0 is None:
                 print('Careful! I did not receive a E0, I am using the default value!')
                 E0 = E0_lazero
             melt_rate_2D_isf = calculate_melt_rate_2D_plumes_1isf(kisf, filled_TS, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, E0)
         elif picop_opt in ['2018','2019']:
@@ -1740,14 +1772,15 @@
     
     
 def calculate_melt_rate_2D_all_isf(nisf_list, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, 
                                    U_param=True, C=None, E0=None, angle_option='lazero',
                                    box_charac_2D=None, box_charac_1D=None, box_tot=None, box_tot_option='box_nb_tot', pism_version='no', picop_opt='no',
                                    gamma_plume=None, T_corrections=False,
                                    options_2D=['melt_m_ice_per_y','melt_m_we_per_y'],
+                                   HUB=False,
                                    verbose=True):
     
     
     """
     Wrap function to loop over all ice shelves and combine result to a map.
 
     Parameters
@@ -1769,15 +1802,15 @@
     U_param : Boolean
         If ``True`` we use the complex parameterisation of U, if ``False``, this is "only" equal to (rho_sw * c_po) / (rho_i * L_i). Relevant for simple parameterisations only.
     C : float
         Circulation parameter C (Sv m3 kg-1 = m6 kg-1 s-1) in [0.1;9]*1.e6.
     E0 : float
         Entrainment coefficient.
     angle_option : str
-        Slope to be used, choice between "cavity" (cavity slope), "lazero" (lazeroms18), "local" (local slope)
+        Slope to be used, choice between "cavity" (cavity), "lazero" (lazeroms18), "local" (local)
     box_charac_2D : xarray.Dataset
         Dataset containing relevant 2D box characteristics for all ice shelves.
     box_charac_1D : xarray.Dataset
         Dataset containing relevant 1D box characteristics for all ice shelves.
     box_tot : int
         Either the total number of boxes being used if box_tot_option='box_nb_tot' or the configuration to use if box_tot_option='nD_config'.
     box_tot_option : str
@@ -1813,15 +1846,15 @@
         list_loop = nisf_list
         
     for kisf in list_loop:
         #print(kisf, n)
         
         melt_rate_2D_isf = calculate_melt_rate_2D_1isf(kisf, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, 
                                                        U_param, C, E0, angle_option, 
-                                                       box_charac_2D, box_charac_1D, box_tot, box_tot_option, pism_version, picop_opt, gamma_plume, T_corrections)
+                                                       box_charac_2D, box_charac_1D, box_tot, box_tot_option, pism_version, picop_opt, gamma_plume, T_corrections, HUB)
         
         if n == 0:
             ds_melt_rate_2D_all = melt_rate_2D_isf.squeeze().drop('Nisf')
         else:
             ds_melt_rate_2D_all = ds_melt_rate_2D_all.combine_first(melt_rate_2D_isf).squeeze().drop('Nisf')
         n = n+1
         
@@ -1912,14 +1945,15 @@
 def calculate_melt_rate_1D_and_2D_all_isf(nisf_list, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, 
                                           U_param=True, C=None, E0=None, angle_option='lazero',
                                           box_charac_2D=None, box_charac_1D=None, box_tot=None, box_tot_option='box_nb_tot', pism_version='no', picop_opt='no',
                                           gamma_plume=None, T_corrections=False,
                                           options_2D=['melt_m_ice_per_y','melt_m_we_per_y'],
                                           options_1D=['melt_m_ice_per_y_avg', 'melt_m_ice_per_y_min', 'melt_m_ice_per_y_max', 'melt_we_per_y_tot',
                                                      'melt_we_per_y_avg','melt_Gt_per_y_tot'],
+                                          HUB=False,
                                           verbose=True):
     
     """
     Function to process input information and call the 2D and 1D functions to compute melt rate variables.
 
     Parameters
     ----------
@@ -1940,15 +1974,15 @@
     U_param : Boolean
         If ``True`` we use the complex parameterisation of U, if ``False``, this is "only" equal to (rho_sw * c_po) / (rho_i * L_i). Relevant for simple parameterisations only.
     C : float
         Circulation parameter C (Sv m3 kg-1 = m6 kg-1 s-1) in [0.1;9]*1.e6.
     E0 : float
         Entrainment coefficient.
     angle_option : str
-        Slope to be used, choice between "cavity" (cavity slope), "lazero" (lazeroms18), "local" (local slope)
+        Slope to be used, choice between "cavity" (cavity), "lazero" (lazeroms18), "local" (local)
     box_charac_2D : xarray.Dataset
         Dataset containing relevant 2D box characteristics for all ice shelves.
     box_charac_1D : xarray.Dataset
         Dataset containing relevant 1D box characteristics for all ice shelves.
     box_tot : int
         Either the total number of boxes being used if box_tot_option='box_nb_tot' or the configuration to use if box_tot_option='nD_config'.
     box_tot_option : str
@@ -1978,30 +2012,31 @@
     
     if verbose:
         time_start = time.time()
         print('WELCOME! AS YOU WISH, I WILL COMPUTE MELT RATES FOR THE PARAMETERISATION "'+mparam+'" FOR '+str(len(nisf_list))+' ICE SHELVES')
     
     ds_2D = calculate_melt_rate_2D_all_isf(nisf_list, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, U_param, C, E0, angle_option,
                                            box_charac_2D, box_charac_1D, box_tot, box_tot_option, pism_version, picop_opt, gamma_plume, T_corrections,
-                                           options_2D, verbose)
+                                           options_2D, HUB, verbose)
     
     ds_1D = calculate_melt_rate_1D_all_isf(nisf_list, ds_2D, geometry_info_2D, isf_stack_mask, options_1D, verbose)
     
     if verbose:
         timelength = time.time() - time_start
         print("I AM DONE! IT TOOK: "+str(round(timelength,2))+" seconds.")
         
     return ds_2D, ds_1D
 
 
 def calculate_melt_rate_Gt_and_box1_all_isf(nisf_list, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam, gamma, 
                                           U_param=True, C=None, E0=None, angle_option='lazero',
                                           box_charac_2D=None, box_charac_1D=None, box_tot=None, box_tot_option='box_nb_tot', pism_version='no', picop_opt='no',
                                           gamma_plume=None, T_corrections=False,
-                                          tuning_mode=False,  
+                                          tuning_mode=False, 
+                                          HUB=False,
                                           verbose=True):
     
     """
     Function to process input information and call the 2D and 1D functions to compute melt rate variables.
 
     Parameters
     ----------
@@ -2022,15 +2057,15 @@
     U_param : Boolean
         If ``True`` we use the complex parameterisation of U, if ``False``, this is "only" equal to (rho_sw * c_po) / (rho_i * L_i). Relevant for simple parameterisations only.
     C : float
         Circulation parameter C (Sv m3 kg-1 = m6 kg-1 s-1) in [0.1;9]*1.e6.
     E0 : float
         Entrainment coefficient.
     angle_option : str
-        Slope to be used, choice between "cavity" (cavity slope), "lazero" (lazeroms18), "local" (local slope)
+        Slope to be used, choice between "cavity" (cavity), "lazero" (lazeroms18), "local" (local)
     box_charac_2D : xarray.Dataset
         Dataset containing relevant 2D box characteristics for all ice shelves.
     box_charac_1D : xarray.Dataset
         Dataset containing relevant 1D box characteristics for all ice shelves.
     box_tot : int
         Either the total number of boxes being used if box_tot_option='box_nb_tot' or the configuration to use if box_tot_option='nD_config'.
     box_tot_option : str
@@ -2062,15 +2097,15 @@
     if verbose:
         list_loop = tqdm(nisf_list)
     else:
         list_loop = nisf_list
 
     if box_charac_2D and box_charac_1D:
         box_loc_config2 = box_charac_2D['box_location'].sel(box_nb_tot=box_charac_1D['nD_config'].sel(config=2))
-        box1 = box_loc_config2.where(box_loc_config2==1).isel(Nisf=0).drop('Nisf')
+        box1 = box_loc_config2.where(box_loc_config2==1).isel(Nisf=1).drop('Nisf')
     elif not box_charac_2D:
         return print('You have not given me the 2D box characteristics! :( ')
     elif not box_charac_1D:
         return print('You have not given me the 1D box characteristics! :( ')
 
     melt1D_Gt_per_yr_list = []
     if not tuning_mode:
@@ -2081,15 +2116,15 @@
 
         geometry_isf_2D = uf.choose_isf(geometry_info_2D,isf_stack_mask, kisf)
 
         melt_rate_2D_isf = calculate_melt_rate_2D_1isf(kisf, T_S_profile, geometry_info_2D, geometry_info_1D, isf_stack_mask, mparam,
                                                        gamma, 
                                                        U_param, C, E0, angle_option, 
                                                        box_charac_2D, box_charac_1D, box_tot, box_tot_option, 
-                                                       pism_version, picop_opt, gamma_plume, T_corrections)
+                                                       pism_version, picop_opt, gamma_plume, T_corrections, HUB)
 
         melt_rate_2D_isf_m_per_y = melt_rate_2D_isf * yearinsec
         melt_rate_1D_isf_Gt_per_y = (melt_rate_2D_isf_m_per_y * geometry_isf_2D['grid_cell_area_weighted']).sum(dim=['mask_coord']) * rho_i / 10**12
         if 'option' in melt_rate_1D_isf_Gt_per_y.coords:
             melt_rate_1D_isf_Gt_per_y = melt_rate_1D_isf_Gt_per_y.drop('option')
         melt1D_Gt_per_yr_list.append(melt_rate_1D_isf_Gt_per_y)
```

### Comparing `multimelt-0.1/multimelt/plume_functions.py` & `multimelt-0.2/multimelt/plume_functions.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.1/multimelt/useful_functions.py` & `multimelt-0.2/multimelt/useful_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,30 @@
     R = 6.371e6
     a =   np.sin(np.deg2rad(lat1-lat2)*0.5)**2 + np.cos(np.deg2rad(lat2)) * np.cos(np.deg2rad(lat1)) * np.sin(np.deg2rad(lon1-lon2)*0.5)**2    
     return abs( 2 * R * np.atan2( np.sqrt(a), np.sqrt(1-a) ) ) # distance in meters
 
 def change_coord_latlon_to_stereo(meshlon,meshlat):
     ### Transformation from latlon to stereo
     trans_tostereo = Transformer.from_crs("EPSG:4326", "EPSG:3031", always_xy=True)
-    meshx, meshy = trans_tolonlat.transform(meshlon,meshlat)
+    meshx, meshy = trans_tostereo.transform(meshlon,meshlat)
     return meshx, meshy
 
 def change_coord_stereo_to_latlon(meshx,meshy):
     ### Transformation from latlon to stereo
     trans_tolonlat = Transformer.from_crs("EPSG:3031", "EPSG:4326", always_xy=True)
     meshlon,meshlat = trans_tolonlat.transform(meshx,meshy)
     return meshlon, meshlat
 
 def cut_domain_stereo(var_to_cut, map_lim_x, map_lim_y):
     var_cutted = var_to_cut.sel(x=var_to_cut.x.where(in_range(var_to_cut.x,map_lim_x),drop=True), y=var_to_cut.y.where(in_range(var_to_cut.y,map_lim_y),drop=True))
     return var_cutted
 
 def weighted_mean(data, dims, weights):
-    return (data*weights).sum(dim=dims)/weights.sum(dim=dims)
+    weight_sum = weights.sum(dim=dims) # to avoid dividing by zero
+    return (data*weights).sum(dim=dims)/weight_sum.where(weight_sum != 0)
 
 def create_stacked_mask(isfmask_2D, nisf_list, dims_to_stack, new_dim):
     # create stacked indices to select the different ice shelves
     # based on https://xarray.pydata.org/en/stable/indexing.html#more-advanced-indexing
     stacked_mask = isfmask_2D.stack(z=(dims_to_stack))
     
     new_coord_mask = stacked_mask.z.where(stacked_mask==nisf_list).dropna(how='all',dim='z')
```

### Comparing `multimelt-0.1/multimelt.egg-info/PKG-INFO` & `multimelt-0.2/multimelt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: multimelt
-Version: 0.1
+Version: 0.2
 Summary: Regroupment of the main existing ice shelf basal melt parameterisations
 Home-page: https://github.com/ClimateClara/multimelt
 Author: Clara Burgard
 Author-email: clara.burgard@univ-grenoble-alpes.fr
 License: GPL-3.0
 Project-URL: Source, https://github.com/ClimateClara/multimelt
 Project-URL: Tracker, https://github.com/ClimateClara/multimelt/issues
 Keywords: earth-sciences climate-modeling ice-sheet antarctica oceanography
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5
 License-File: LICENSE
@@ -65,16 +64,14 @@
 Don't hesitate to contact me if any questions arise: clara.burgard@univ-grenoble-alpes.fr
 
 How to cite multimelt
 ---------------------
 
 The detailed description of the application of the functions in multimelt is found in `Burgard et al., 2022`_ and should therefore, when used, be cited as follows:
 
-Burgard, C., Jourdain, N. C., Reese, R., Jenkins, A., and Mathiot, P.: An assessment of basal melt parameterisations for Antarctic ice shelves, The Cryosphere Discuss. [preprint], https://doi.org/10.5194/tc-2022-32, in review, 2022. 
-
-
-.. _`Burgard et al., 2022`: https://doi.org/10.5194/tc-2022-32
+Burgard, C., Jourdain, N. C., Reese, R., Jenkins, A., and Mathiot, P. (2022): An assessment of basal melt parameterisations for Antarctic ice shelves, The Cryosphere, https://doi.org/10.5194/tc-16-4931-2022. 
 
 
+.. _`Burgard et al., 2022`: https://doi.org/10.5194/tc-16-4931-2022
```

### Comparing `multimelt-0.1/setup.py` & `multimelt-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 setuptools.setup(
 	
     #The project's name
     name='multimelt',
     
     #The project's version 
-    version='0.1',
+    version='0.2',
     
     #The project's metadata
     author='Clara Burgard',
     author_email='clara.burgard@univ-grenoble-alpes.fr',
     description='Regroupment of the main existing ice shelf basal melt parameterisations',
     long_description=long_description,
     
@@ -67,13 +67,14 @@
 	
     install_requires=[
           'numpy',
           'xarray',
           'pandas',
           'tqdm',
           'scipy',
+          'cc3d',
           'gsw',
           'pyproj',
-          'dask'
+          'dask',
       ],
 
 )
```

