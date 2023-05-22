# Comparing `tmp/Slpapy-0.3.21.tar.gz` & `tmp/Slpapy-0.3.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.3.21.tar", last modified: Mon May 22 07:03:47 2023, max compression
+gzip compressed data, was "Slpapy-0.3.22.tar", last modified: Mon May 22 12:09:02 2023, max compression
```

## Comparing `Slpapy-0.3.21.tar` & `Slpapy-0.3.22.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 07:03:47.302919 Slpapy-0.3.21/
--rw-rw-rw-   0        0        0      160 2023-05-22 07:03:47.301922 Slpapy-0.3.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 07:03:47.268013 Slpapy-0.3.21/Slpapy/
--rw-rw-rw-   0        0        0     4531 2023-05-22 07:03:03.000000 Slpapy-0.3.21/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.3.21/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:03:47.299927 Slpapy-0.3.21/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.21/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.21/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     6754 2023-05-18 07:49:27.000000 Slpapy-0.3.21/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:03:47.276989 Slpapy-0.3.21/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-05-22 07:03:46.000000 Slpapy-0.3.21/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-05-22 07:03:47.000000 Slpapy-0.3.21/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 07:03:46.000000 Slpapy-0.3.21/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-22 07:03:46.000000 Slpapy-0.3.21/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 07:03:46.000000 Slpapy-0.3.21/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 07:03:47.302919 Slpapy-0.3.21/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-05-22 07:03:19.000000 Slpapy-0.3.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:02.545856 Slpapy-0.3.22/
+-rw-rw-rw-   0        0        0      160 2023-05-22 12:09:02.544857 Slpapy-0.3.22/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:02.507957 Slpapy-0.3.22/Slpapy/
+-rw-rw-rw-   0        0        0     4837 2023-05-22 12:08:25.000000 Slpapy-0.3.22/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.3.22/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:02.542864 Slpapy-0.3.22/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.22/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     6754 2023-05-18 07:49:27.000000 Slpapy-0.3.22/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:02.515935 Slpapy-0.3.22/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 12:09:02.545856 Slpapy-0.3.22/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-05-22 12:08:47.000000 Slpapy-0.3.22/setup.py
```

### Comparing `Slpapy-0.3.21/Slpapy/Data_reconstruction.py` & `Slpapy-0.3.22/Slpapy/Data_reconstruction.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     adata.obs_names = df.columns
     adata.var['m/z'] = df.index
     adata.var_names = ['lips' + str(x) for x in range(adata.n_vars)]
     print(adata.obs_names[:])
     print(adata.var_names[:])
 
     # 标注坐标位置
-    adata.obs["X_org"] = df1.x
-    adata.obs["Y_org"] = df1.y
+    adata.obs["X_org"] = df1.x.values
+    adata.obs["Y_org"] = df1.y.values
 
     adata.obs["X"] = (df1.x.values-df1.x.values.min())//mm
     adata.obs["Y"] = (df1.y.values-df1.y.values.min())//mm
 
     # 标注mask
     if mask is not None:
         mask = str(mask)
@@ -113,17 +113,24 @@
                     break
 
         adata.var_names = adata.var['m/zs']
         print(adata.var)
         del adata.var['m/zs']
 
         # 合并重复的m/z
-        duplicated_var = adata.var_names.duplicated(keep=False)
-        duplicated_var_names = adata.var_names[duplicated_var]
-        for var_name in duplicated_var_names:
-            adata[:, var_name].X = adata[:, var_name].X.sum(axis=0)
-        adata.var = adata.var.drop_duplicates()
-        adata.var_names = adata.var.index
+        if isinstance(adata.X, csr_matrix):
+            adata.X = adata.X.toarray()
 
+        df = pd.DataFrame(adata.X, columns=adata.var_names)
+        var = adata.var
+        # Step 2: 合并重复的列（基因）
+        merged_df = df.groupby(df.columns, axis=1).sum()
+        merged_var = var.groupby(var.index, axis=0).sum()
+        # Step 3: 创建新的anndata对象，用合并后的数据更新adata
+        adata_new = ad.AnnData(X=merged_df.values, obs=adata.obs, var=pd.DataFrame(index=merged_df.columns))
+
+        adata_new.obs = adata.obs
+        adata_new.var = merged_var
+        adata = adata_new
     # 保存adata
     adata.write(f'{XY}' + ".h5ad")
     return adata
```

### Comparing `Slpapy-0.3.21/Slpapy/MZ_ppm_match.py` & `Slpapy-0.3.22/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.3.22/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy/processing_analyze.py` & `Slpapy-0.3.22/Slpapy/processing_analyze.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.3.22/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.21/setup.py` & `Slpapy-0.3.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Slpapy',
-    version='0.3.21',
+    version='0.3.22',
     author='yifan xu',
     author_email='xuyifan@westlake.edu.cn',
     description='Spatial_lipomic_and_proteomic_analysis',
     packages=find_packages(),
     install_requires=[
         'scanpy>=1.9.1',
         'anndata>=0.8.0',
```

