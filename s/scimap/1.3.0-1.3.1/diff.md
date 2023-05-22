# Comparing `tmp/scimap-1.3.0.tar.gz` & `tmp/scimap-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-1.3.0.tar", max compression
+gzip compressed data, was "scimap-1.3.1.tar", max compression
```

## Comparing `scimap-1.3.0.tar` & `scimap-1.3.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.3.0/README.md
--rw-r--r--   0        0        0     2369 2023-05-21 01:05:13.360063 scimap-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/__init__.py
--rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/__main__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/cli/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-1.3.0/scimap/cli/_scimap_mcmicro.py
--rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-1.3.0/scimap/cli/test.py
--rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.3.0/scimap/helpers/__init__.py
--rwxr-xr-x   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.3.0/scimap/helpers/_addROI_omero.py
--rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.3.0/scimap/helpers/_add_roi_omero.py
--rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.3.0/scimap/helpers/_animate.py
--rwxr-xr-x   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.3.0/scimap/helpers/_classify.py
--rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.3.0/scimap/helpers/_dropFeatures.py
--rwxr-xr-x   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/helpers/_merge_adata_obs.py
--rwxr-xr-x   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/helpers/_rename.py
--rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.3.0/scimap/helpers/_scimap_to_csv.py
--rwxr-xr-x   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/helpers/add_roi_scatter.py
--rw-r--r--   0        0        0      588 2023-05-21 00:55:17.808850 scimap-1.3.0/scimap/plotting/__init__.py
--rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.3.0/scimap/plotting/_addROI_image.py
--rwxr-xr-x   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.3.0/scimap/plotting/_cluster_plots.py
--rwxr-xr-x   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/plotting/_foldchange.py
--rw-r--r--   0        0        0     9508 2023-05-20 22:41:36.638128 scimap-1.3.0/scimap/plotting/_gate_finder.py
--rw-r--r--   0        0        0     9403 2023-04-22 02:17:49.145882 scimap-1.3.0/scimap/plotting/_image_viewer.py
--rwxr-xr-x   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/plotting/_pie.py
--rwxr-xr-x   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.3.0/scimap/plotting/_spatial_distance.py
--rwxr-xr-x   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.3.0/scimap/plotting/_spatial_interaction.py
--rwxr-xr-x   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.3.0/scimap/plotting/_spatial_pscore.py
--rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/plotting/_spatial_scatter.py
--rwxr-xr-x   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.3.0/scimap/plotting/_stacked_barplot.py
--rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.3.0/scimap/plotting/_umap.py
--rwxr-xr-x   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.3.0/scimap/plotting/_voronoi.py
--rw-r--r--   0        0        0     8513 2023-05-21 00:45:22.122325 scimap-1.3.0/scimap/plotting/densityPlot2D.py
--rw-r--r--   0        0        0     8694 2023-05-21 00:57:39.732696 scimap-1.3.0/scimap/plotting/distPlot.py
--rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.3.0/scimap/plotting/lasso_selector.py
--rw-r--r--   0        0        0    11486 2023-05-21 00:55:01.189031 scimap-1.3.0/scimap/plotting/spatial_scatterPlot.py
--rw-r--r--   0        0        0      107 2023-04-20 01:30:26.953137 scimap-1.3.0/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     5078 2023-04-21 02:03:50.459976 scimap-1.3.0/scimap/preprocessing/_combat.py
--rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.3.0/scimap/preprocessing/_mcmicro_to_scimap.py
--rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.3.0/scimap/preprocessing/_rescale.py
--rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tests/_data/phenotype_workflow.csv
--rwxr-xr-x   0        0        0     1268 2023-05-06 14:45:48.623561 scimap-1.3.0/scimap/tests/test_helpers.py
--rwxr-xr-x   0        0        0      984 2023-05-06 14:46:01.108135 scimap-1.3.0/scimap/tests/test_preprocessing.py
--rwxr-xr-x   0        0        0     4673 2023-05-06 14:46:08.191066 scimap-1.3.0/scimap/tests/test_tools.py
--rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.3.0/scimap/tools/__init__.py
--rwxr-xr-x   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.3.0/scimap/tools/_cluster.py
--rwxr-xr-x   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.3.0/scimap/tools/_foldchange.py
--rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tools/_phenotype_cells.py
--rwxr-xr-x   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tools/_spatial_aggregate.py
--rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.3.0/scimap/tools/_spatial_cluster.py
--rwxr-xr-x   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tools/_spatial_count.py
--rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.3.0/scimap/tools/_spatial_distance.py
--rwxr-xr-x   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.3.0/scimap/tools/_spatial_expression.py
--rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.3.0/scimap/tools/_spatial_interaction.py
--rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.3.0/scimap/tools/_spatial_lda.py
--rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.3.0/scimap/tools/_spatial_pscore.py
--rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.3.0/scimap/tools/_spatial_similarity_search.py
--rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.3.0/scimap/tools/_umap.py
--rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 scimap-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2369 2023-05-22 14:12:06.920171 scimap-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.3.1/README.md
+-rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/__main__.py
+-rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/cli/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.000000 scimap-1.3.1/scimap/cli/_scimap_mcmicro.py
+-rw-r--r--   0        0        0      592 2023-04-20 14:28:51.000000 scimap-1.3.1/scimap/cli/test.py
+-rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.3.1/scimap/helpers/__init__.py
+-rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.3.1/scimap/helpers/_add_roi_omero.py
+-rw-r--r--   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.3.1/scimap/helpers/_addROI_omero.py
+-rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.3.1/scimap/helpers/_animate.py
+-rw-r--r--   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.3.1/scimap/helpers/_classify.py
+-rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.3.1/scimap/helpers/_dropFeatures.py
+-rw-r--r--   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/helpers/_merge_adata_obs.py
+-rw-r--r--   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/helpers/_rename.py
+-rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.3.1/scimap/helpers/_scimap_to_csv.py
+-rw-r--r--   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/helpers/add_roi_scatter.py
+-rw-r--r--   0        0        0      588 2023-05-21 00:55:17.000000 scimap-1.3.1/scimap/plotting/__init__.py
+-rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.3.1/scimap/plotting/_addROI_image.py
+-rw-r--r--   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.3.1/scimap/plotting/_cluster_plots.py
+-rw-r--r--   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/plotting/_foldchange.py
+-rw-r--r--   0        0        0     9508 2023-05-22 14:10:48.903765 scimap-1.3.1/scimap/plotting/_gate_finder.py
+-rw-r--r--   0        0        0     9403 2023-04-22 02:17:49.000000 scimap-1.3.1/scimap/plotting/_image_viewer.py
+-rw-r--r--   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/plotting/_pie.py
+-rw-r--r--   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.3.1/scimap/plotting/_spatial_distance.py
+-rw-r--r--   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.3.1/scimap/plotting/_spatial_interaction.py
+-rw-r--r--   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.3.1/scimap/plotting/_spatial_pscore.py
+-rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/plotting/_spatial_scatter.py
+-rw-r--r--   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.3.1/scimap/plotting/_stacked_barplot.py
+-rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.3.1/scimap/plotting/_umap.py
+-rw-r--r--   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.3.1/scimap/plotting/_voronoi.py
+-rw-r--r--   0        0        0     8513 2023-05-21 00:45:22.000000 scimap-1.3.1/scimap/plotting/densityPlot2D.py
+-rw-r--r--   0        0        0     8707 2023-05-21 01:13:28.000000 scimap-1.3.1/scimap/plotting/distPlot.py
+-rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.3.1/scimap/plotting/lasso_selector.py
+-rw-r--r--   0        0        0    11486 2023-05-21 00:55:01.000000 scimap-1.3.1/scimap/plotting/spatial_scatterPlot.py
+-rw-r--r--   0        0        0      107 2023-04-20 01:30:26.000000 scimap-1.3.1/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4932 2023-05-21 01:17:40.000000 scimap-1.3.1/scimap/preprocessing/_combat.py
+-rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.3.1/scimap/preprocessing/_mcmicro_to_scimap.py
+-rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.3.1/scimap/preprocessing/_rescale.py
+-rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/tests/_data/phenotype_workflow.csv
+-rw-r--r--   0        0        0     1268 2023-05-06 14:45:48.000000 scimap-1.3.1/scimap/tests/test_helpers.py
+-rw-r--r--   0        0        0      984 2023-05-06 14:46:01.000000 scimap-1.3.1/scimap/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     4673 2023-05-06 14:46:08.000000 scimap-1.3.1/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.3.1/scimap/tools/__init__.py
+-rw-r--r--   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.3.1/scimap/tools/_cluster.py
+-rw-r--r--   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.3.1/scimap/tools/_foldchange.py
+-rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/tools/_phenotype_cells.py
+-rw-r--r--   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/tools/_spatial_aggregate.py
+-rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.3.1/scimap/tools/_spatial_cluster.py
+-rw-r--r--   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.3.1/scimap/tools/_spatial_count.py
+-rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.3.1/scimap/tools/_spatial_distance.py
+-rw-r--r--   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.3.1/scimap/tools/_spatial_expression.py
+-rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.3.1/scimap/tools/_spatial_interaction.py
+-rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.3.1/scimap/tools/_spatial_lda.py
+-rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.3.1/scimap/tools/_spatial_pscore.py
+-rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.3.1/scimap/tools/_spatial_similarity_search.py
+-rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.3.1/scimap/tools/_umap.py
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 scimap-1.3.1/PKG-INFO
```

### Comparing `scimap-1.3.0/README.md` & `scimap-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/pyproject.toml` & `scimap-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "scimap"
-version = "1.3.0"
+version = "1.3.1"
 description = "Spatial Single-Cell Analysis Toolkit"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `scimap-1.3.0/scimap/cli/_scimap_mcmicro.py` & `scimap-1.3.1/scimap/cli/_scimap_mcmicro.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/cli/test.py` & `scimap-1.3.1/scimap/cli/test.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/_addROI_omero.py` & `scimap-1.3.1/scimap/helpers/_addROI_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/_add_roi_omero.py` & `scimap-1.3.1/scimap/helpers/_add_roi_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/_animate.py` & `scimap-1.3.1/scimap/helpers/_animate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/_classify.py` & `scimap-1.3.1/scimap/helpers/_classify.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/_dropFeatures.py` & `scimap-1.3.1/scimap/helpers/_dropFeatures.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/_merge_adata_obs.py` & `scimap-1.3.1/scimap/helpers/_merge_adata_obs.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/_rename.py` & `scimap-1.3.1/scimap/helpers/_rename.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/_scimap_to_csv.py` & `scimap-1.3.1/scimap/helpers/_scimap_to_csv.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/helpers/add_roi_scatter.py` & `scimap-1.3.1/scimap/helpers/add_roi_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/__init__.py` & `scimap-1.3.1/scimap/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_addROI_image.py` & `scimap-1.3.1/scimap/plotting/_addROI_image.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_cluster_plots.py` & `scimap-1.3.1/scimap/plotting/_cluster_plots.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_foldchange.py` & `scimap-1.3.1/scimap/plotting/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_gate_finder.py` & `scimap-1.3.1/scimap/plotting/_gate_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
                     name = None if channel_names is None else channel_names)
 
     # Add the seg mask
     if seg_mask is not None:
         viewer.add_labels(seg_m, name='segmentation mask', visible=False)
 
     # subset the gates to include only the image of interest
-    gates = gates.loc[adata.obs.index,]
+    gates = gates.loc[bdata.obs.index,]
 
     # Add gating layer
     def add_phenotype_layer (adata, gates, phenotype_layer,x,y,viewer,point_size):
         cells = gates[gates[phenotype_layer] == 1].index
         coordinates = adata[cells]
         # Flip Y axis if needed
         if flip_y is True:
@@ -267,10 +267,10 @@
         viewer.add_points(points, size=point_size, face_color='white',visible=False,name=phenotype_layer)
         #stop = time.time()
         #print(stop-start)
         
 
     # Run the function on all gating layer
     for i in gates.columns:
-        add_phenotype_layer (adata=adata, gates=gates, 
+        add_phenotype_layer (adata=bdata, gates=gates, 
                              phenotype_layer=i, x=x_coordinate, y=y_coordinate, 
                              viewer=viewer, point_size=point_size)
```

### Comparing `scimap-1.3.0/scimap/plotting/_image_viewer.py` & `scimap-1.3.1/scimap/plotting/_image_viewer.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_pie.py` & `scimap-1.3.1/scimap/plotting/_pie.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_spatial_distance.py` & `scimap-1.3.1/scimap/plotting/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_spatial_interaction.py` & `scimap-1.3.1/scimap/plotting/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_spatial_pscore.py` & `scimap-1.3.1/scimap/plotting/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_spatial_scatter.py` & `scimap-1.3.1/scimap/plotting/_spatial_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_stacked_barplot.py` & `scimap-1.3.1/scimap/plotting/_stacked_barplot.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_umap.py` & `scimap-1.3.1/scimap/plotting/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/_voronoi.py` & `scimap-1.3.1/scimap/plotting/_voronoi.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/densityPlot2D.py` & `scimap-1.3.1/scimap/plotting/densityPlot2D.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/distPlot.py` & `scimap-1.3.1/scimap/plotting/distPlot.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         ```python
         
         sm.pl.distPlot(adata, 
                      layer=None, 
                      markers=['CD45','CD3D','CD20'], 
                      plotGrid=True, 
                      ncols=5)
+        ```
     
     """
     
     # testing
     # layers=None; markers=None; plotGrid=True; ncols=None; color=None; figsize=(10, 10); fontsize=None; subset=None; imageid='imageid'; xticks=None; dpi=200; outputDir=None; 
     # outputFileName='distPlot.png'
     # color = {'markerA': '#000000', 'markerB': '#FF0000'}
```

### Comparing `scimap-1.3.0/scimap/plotting/lasso_selector.py` & `scimap-1.3.1/scimap/plotting/lasso_selector.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/plotting/spatial_scatterPlot.py` & `scimap-1.3.1/scimap/plotting/spatial_scatterPlot.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/preprocessing/_combat.py` & `scimap-1.3.1/scimap/preprocessing/_combat.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,72 +18,68 @@
 import numpy as np
 import argparse
 
 
 def combat(
     adata,
     batch='imageid',
-    layers=None,
+    layer=None,
     log=False,
     replaceOriginal=False,
     label='combat'):
     
     """
-    Parameters:
+Parameters:
+    adata (AnnData object):  
+        Annotated data matrix.
 
-        adata (AnnData object):  
-            Annotated data matrix.
+    batch (str, optional):  
+        The batch key or column in `adata.obs` that indicates the batches for each cell.
 
-        batch (str, optional):  
-            The batch key or column in `adata.obs` that indicates the batches for each cell.
+    layer (str or None, optional):
+        The layer in `adata.layers` that contains the expression data to correct. If None, 
+        `adata.X` is used. use `raw` to use the data stored in `adata.raw.X`
 
-        layers (str or None, optional):
-            The layer in `adata.layers` that contains the expression data to correct. If None, 
-            `adata.X` is used. use `raw` to use the data stored in `adata.raw.X`
+    log (bool, optional):  
+        Whether to log transform the data before applying ComBat. Generally use it with `raw`.
 
-        log (bool, optional):  
-            Whether to log transform the data before applying ComBat. Generally use it with `raw`.
+    replaceOriginal (bool, optional):
+        Whether to replace the original expression data in `adata` with the corrected data.
 
-        replaceOriginal (bool, optional):
-            Whether to replace the original expression data in `adata` with the corrected data.
+    label (str, optional):  
+        The prefix for the key in `adata` that will contain the corrected data. If `replaceOriginal` is `True`, this parameter has no effect.  
 
-        label (str, optional):  
-            The prefix for the key in `adata` that will contain the corrected data. If `replaceOriginal` is `True`, this parameter has no effect.  
+Returns:
+    adata (anndata):  
+        The corrected expression data is stored in a new layer `adata.layers['combat']`.
 
-    Returns:
+Examples:
 
-        adata (anndata):  
-            The corrected expression data is stored in a new layer `adata.layers['combat']`.
+    ```python
 
-    Examples:
+    # applying batch correction using raw data
+    adata = sm.pp.combat (adata,
+                    batch='imageid',
+                    layer='raw',
+                    log=True,
+                    replaceOriginal=False,
+                    label='combat')
 
-        ```python
+    # results will be available in adata.layers['combat']
 
-        # applying batch correction using raw data
-        adata = combat (adata,
-                        batch='imageid',
-                        layers='raw',
-                        log=True,
-                        replaceOriginal=False,
-                        label='combat')
-
-        # results will be available in adata.layers['combat']
-
-        ```
+    ```
     """
 
     # isolate the data
-    if layers is None:
+    if layer is None:
         data = pd.DataFrame(adata.X, index=adata.obs.index, columns=adata.var.index)
-    elif layers == 'raw':
+    elif layer == 'raw':
         data = pd.DataFrame(adata.raw.X, index=adata.obs.index, columns=adata.var.index)
     else:
-        data = pd.DataFrame(
-            adata.layers[layers], index=adata.obs.index, columns=adata.var.index
-        )
+        data = pd.DataFrame(adata.layers[layer], index=adata.obs.index, columns=adata.var.index)
 
     # log the data if requested
     if log is True:
         data = np.log1p(data)
 
     # isolate batch
     batchData = adata.obs[batch]
@@ -103,21 +99,21 @@
     batchCorrected = pycombat(data.T, batchData).T
 
     # add as a specific layer
     adata.layers[label] = batchCorrected
 
     # replace original
     if replaceOriginal is True:
-        if layers is None:
+        if layer is None:
             adata.X = batchCorrected
-        elif layers == 'raw':
+        elif layer == 'raw':
             del adata.raw
             adata.raw = ad.AnnData(batchCorrected, obs=adata.obs)
         else:
-            adata.layers[layers] = batchCorrected
+            adata.layers[layer] = batchCorrected
 
     # return adata
     return adata
 
 
 # Make the Function CLI compatable
 if __name__ == '__main__':
@@ -126,15 +122,15 @@
     parser.add_argument(
         '--batch',
         type=str,
         default='imageid',
         help='The batch key or column in `adata.obs` that indicates the batches for each cell.',
     )
     parser.add_argument(
-        '--layers',
+        '--layer',
         type=str,
         default=None,
         help='The layer in `adata.layers` that contains the expression data to correct. If None, `adata.X` is used. use `raw` to use the data stored in `adata.raw.X`',
     )
     parser.add_argument(
         '--log',
         type=bool,
@@ -153,11 +149,11 @@
         default='combat',
         help='The prefix for the key in `adata` that will contain the corrected data. If `replaceOriginal` is True, this parameter has no effect.',
     )
     args = parser.parse_args()
     combat(
         adata=args.adata,
         batch=args.batch,
-        layers=args.layers,
+        layer=args.layer,
         log=args.log,
         replaceOriginal=args.replaceOriginal,
         label=args.label)
```

### Comparing `scimap-1.3.0/scimap/preprocessing/_mcmicro_to_scimap.py` & `scimap-1.3.1/scimap/preprocessing/_mcmicro_to_scimap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/preprocessing/_rescale.py` & `scimap-1.3.1/scimap/preprocessing/_rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tests/_data/example_data.csv` & `scimap-1.3.1/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tests/_data/example_data.h5ad` & `scimap-1.3.1/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tests/_data/phenotype_workflow.csv` & `scimap-1.3.1/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tests/test_helpers.py` & `scimap-1.3.1/scimap/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tests/test_preprocessing.py` & `scimap-1.3.1/scimap/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tests/test_tools.py` & `scimap-1.3.1/scimap/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/__init__.py` & `scimap-1.3.1/scimap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_cluster.py` & `scimap-1.3.1/scimap/tools/_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_foldchange.py` & `scimap-1.3.1/scimap/tools/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_phenotype_cells.py` & `scimap-1.3.1/scimap/tools/_phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_aggregate.py` & `scimap-1.3.1/scimap/tools/_spatial_aggregate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_cluster.py` & `scimap-1.3.1/scimap/tools/_spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_count.py` & `scimap-1.3.1/scimap/tools/_spatial_count.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_distance.py` & `scimap-1.3.1/scimap/tools/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_expression.py` & `scimap-1.3.1/scimap/tools/_spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_interaction.py` & `scimap-1.3.1/scimap/tools/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_lda.py` & `scimap-1.3.1/scimap/tools/_spatial_lda.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_pscore.py` & `scimap-1.3.1/scimap/tools/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_spatial_similarity_search.py` & `scimap-1.3.1/scimap/tools/_spatial_similarity_search.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/scimap/tools/_umap.py` & `scimap-1.3.1/scimap/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.0/PKG-INFO` & `scimap-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimap
-Version: 1.3.0
+Version: 1.3.1
 Summary: Spatial Single-Cell Analysis Toolkit
 Home-page: https://pypi.org/project/scimap/
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.7,<3.11
```

