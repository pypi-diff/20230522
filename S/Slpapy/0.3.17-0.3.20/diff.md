# Comparing `tmp/Slpapy-0.3.17.tar.gz` & `tmp/Slpapy-0.3.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.3.17.tar", last modified: Thu May 18 04:12:47 2023, max compression
+gzip compressed data, was "Slpapy-0.3.20.tar", last modified: Mon May 22 01:44:53 2023, max compression
```

## Comparing `Slpapy-0.3.17.tar` & `Slpapy-0.3.20.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 04:12:47.761471 Slpapy-0.3.17/
--rw-rw-rw-   0        0        0      160 2023-05-18 04:12:47.760474 Slpapy-0.3.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 04:12:47.721578 Slpapy-0.3.17/Slpapy/
--rw-rw-rw-   0        0        0     4096 2023-05-18 04:12:28.000000 Slpapy-0.3.17/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.3.17/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:12:47.758480 Slpapy-0.3.17/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.17/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.17/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     6664 2023-05-18 03:04:42.000000 Slpapy-0.3.17/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:12:47.732549 Slpapy-0.3.17/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-05-18 04:12:47.000000 Slpapy-0.3.17/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-05-18 04:12:47.000000 Slpapy-0.3.17/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 04:12:47.000000 Slpapy-0.3.17/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-18 04:12:47.000000 Slpapy-0.3.17/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 04:12:47.000000 Slpapy-0.3.17/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 04:12:47.761471 Slpapy-0.3.17/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-05-18 03:10:06.000000 Slpapy-0.3.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 01:44:53.822870 Slpapy-0.3.20/
+-rw-rw-rw-   0        0        0      160 2023-05-22 01:44:53.821873 Slpapy-0.3.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 01:44:53.783975 Slpapy-0.3.20/Slpapy/
+-rw-rw-rw-   0        0        0     4164 2023-05-18 09:11:59.000000 Slpapy-0.3.20/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.3.20/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-22 01:44:53.819877 Slpapy-0.3.20/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.20/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.20/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     6754 2023-05-18 07:49:27.000000 Slpapy-0.3.20/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-22 01:44:53.793948 Slpapy-0.3.20/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-05-22 01:44:53.000000 Slpapy-0.3.20/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-05-22 01:44:53.000000 Slpapy-0.3.20/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 01:44:53.000000 Slpapy-0.3.20/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-22 01:44:53.000000 Slpapy-0.3.20/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 01:44:53.000000 Slpapy-0.3.20/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 01:44:53.822870 Slpapy-0.3.20/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-05-22 01:44:38.000000 Slpapy-0.3.20/setup.py
```

### Comparing `Slpapy-0.3.17/Slpapy/Data_reconstruction.py` & `Slpapy-0.3.20/Slpapy/Data_reconstruction.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,17 @@
     adata.obs_names = df.columns
     adata.var['m/z'] = df.index
     adata.var_names = ['lips' + str(x) for x in range(adata.n_vars)]
     print(adata.obs_names[:])
     print(adata.var_names[:])
 
     # 标注坐标位置
+    adata.obs["X_org"] = df1.x
+    adata.obs["Y_org"] = df1.y
+
     adata.obs["X"] = (df1.x.values-df1.x.values.min())//mm
     adata.obs["Y"] = (df1.y.values-df1.y.values.min())//mm
 
     # 标注mask
     if mask is not None:
         mask = str(mask)
         resave(mask, 10)
@@ -90,16 +93,16 @@
         del adata.var['mask']
 
 
     # 标注注释
     if annotation is not None:
         annotation = str(annotation)
         liball = pd.read_csv(f'{annotation}', )
-        #填充liball中的空值
-        liball = liball.fillna(method='unknow')
+        #填充liball中的空值为unknow
+        liball = liball.fillna('unknow')
         adata.var['m/zs'] = adata.var_names
         for i in liball.index:
             t = liball.loc[i, 'm/z']
             t = round(t, 2)
             for j in adata.var_names:
                 tt = adata.var.loc[j, 'm/z']
                 if round(tt, 2) == t:
```

### Comparing `Slpapy-0.3.17/Slpapy/MZ_ppm_match.py` & `Slpapy-0.3.20/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.3.20/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/Slpapy/processing_analyze.py` & `Slpapy-0.3.20/Slpapy/processing_analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         estimator.fit(
             np.c_[adata.X, preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])])
         label_pred = estimator.labels_  # 获取聚类标签
         adata.obs['KNNlableXY'] = label_pred.T
         adata.obs['KNNlableXY'] = adata.obs['KNNlableXY'].astype('category')
         sc.tl.rank_genes_groups(adata, 'KNNlableXY', method='wilcoxon')
         sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_KXY_Wilcoxon.png')
+        sc.pl.rank_genes_groups_dotplot(adata, n_genes=10, save='_dotplot_Wilcoxon.png')
         result = adata.uns['rank_genes_groups']
         groups = result['names'].dtype.names
         res = pd.DataFrame({group + '_' + key: result[key][group] for group in groups for key in
                             ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
         res.to_csv("dif.csv")
         sc.pl.pca_variance_ratio(adata, log=True, save='_KXY.png')
         sc.pl.umap(adata, color=['KNNlableXY'], save='_KXY.png')
```

### Comparing `Slpapy-0.3.17/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.3.20/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.17/setup.py` & `Slpapy-0.3.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Slpapy',
-    version='0.3.17',
+    version='0.3.20',
     author='yifan xu',
     author_email='xuyifan@westlake.edu.cn',
     description='Spatial_lipomic_and_proteomic_analysis',
     packages=find_packages(),
     install_requires=[
         'scanpy>=1.9.1',
         'anndata>=0.8.0',
```

