# Comparing `tmp/pywhu3d-0.2.2-py3-none-any.whl.zip` & `tmp/pywhu3d-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 30736 bytes, number of entries: 18
+Zip file size: 31276 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-30 14:16 pywhu3d/__init__.py
--rw-r--r--  2.0 unx    12682 b- defN 23-Apr-23 14:35 pywhu3d/evaluation.py
--rw-r--r--  2.0 unx    23500 b- defN 23-Mar-04 06:47 pywhu3d/tool.py
+-rw-r--r--  2.0 unx    12694 b- defN 23-May-22 06:22 pywhu3d/evaluation.py
+-rw-r--r--  2.0 unx    25631 b- defN 23-May-22 06:26 pywhu3d/tool.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-30 14:17 pywhu3d/configs/__init__.py
 -rw-r--r--  2.0 unx     5172 b- defN 22-Dec-03 05:50 pywhu3d/configs/als_config.py
--rw-r--r--  2.0 unx     2285 b- defN 22-Oct-06 11:31 pywhu3d/configs/base_config.py
+-rw-r--r--  2.0 unx     2285 b- defN 22-Jan-25 02:28 pywhu3d/configs/base_config.py
 -rw-r--r--  2.0 unx    11576 b- defN 22-Nov-05 11:35 pywhu3d/configs/mls_config.py
 -rw-r--r--  2.0 unx    13768 b- defN 22-Nov-19 08:32 pywhu3d/configs/mls_config_pole.py
 -rw-r--r--  2.0 unx     7411 b- defN 22-Nov-05 11:35 pywhu3d/configs/paris_config.py
 -rw-r--r--  2.0 unx     4395 b- defN 22-Nov-05 11:35 pywhu3d/configs/s3dis_config.py
--rw-r--r--  2.0 unx     4283 b- defN 22-Oct-06 11:31 pywhu3d/configs/scannet_config.py
+-rw-r--r--  2.0 unx     4283 b- defN 20-Dec-31 16:00 pywhu3d/configs/scannet_config.py
 -rw-r--r--  2.0 unx     4740 b- defN 22-Nov-05 11:35 pywhu3d/configs/toronto_config.py
--rw-r--r--  2.0 unx      186 b- defN 22-Oct-06 11:31 pywhu3d/configs/wrap_configs.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1199 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1486 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/RECORD
-18 files, 93859 bytes uncompressed, 28302 bytes compressed:  69.8%
+-rw-r--r--  2.0 unx      186 b- defN 21-Jan-23 10:04 pywhu3d/configs/wrap_configs.py
+-rw-r--r--  2.0 unx     1076 b- defN 23-May-22 06:33 pywhu3d-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1199 b- defN 23-May-22 06:33 pywhu3d-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 06:33 pywhu3d-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-22 06:33 pywhu3d-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1486 b- defN 23-May-22 06:33 pywhu3d-0.2.3.dist-info/RECORD
+18 files, 96002 bytes uncompressed, 28842 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: pywhu3d/configs/toronto_config.py
 Comment: 
 
 Filename: pywhu3d/configs/wrap_configs.py
 Comment: 
 
-Filename: pywhu3d-0.2.2.dist-info/LICENSE
+Filename: pywhu3d-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: pywhu3d-0.2.2.dist-info/METADATA
+Filename: pywhu3d-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: pywhu3d-0.2.2.dist-info/WHEEL
+Filename: pywhu3d-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: pywhu3d-0.2.2.dist-info/top_level.txt
+Filename: pywhu3d-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pywhu3d-0.2.2.dist-info/RECORD
+Filename: pywhu3d-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywhu3d/evaluation.py

```diff
@@ -12,15 +12,15 @@
 from rich.table import Column, Table
 from prettytable import PrettyTable as PT
 import xlwt
 from scipy import stats
 
 class Evaluator:
     def __init__(self, whu3d, pred):
-        assert len(pred) == 2, 'pred format wrong!'
+        assert len(pred[0][-1])==2, 'pred format wrong!'
         self.truth = []
         self.pred = []
         assert len(pred) == len(whu3d.scenes)
         for scene in whu3d.scenes:
             ins = whu3d.gt[scene]['semantics'].astype('int32')
             sem = whu3d.gt[scene]['instances'].astype('int32')
             self.truth.append(np.stack([ins, sem], axis=1))
@@ -32,15 +32,15 @@
         self.compute_ins_list = whu3d.compute_ins_list
         self.workbook = None
         self.eval_list = None
         self.info = None
         self.eval_table = None
 
     def set_gt(self, truth):
-        assert len(truth) == 2, 'gt format wrong!'
+        assert len(truth[0][-1]) == 2, 'gt format wrong!'
         self.truth = []
         for gt in truth:
             self.truth.append(gt.astype('int32'))
 
     def compute_metrics(self):
         seg_label_to_cat = self.label2cat
         compute_ins_list = self.compute_ins_list
```

## pywhu3d/tool.py

```diff
@@ -154,14 +154,77 @@
     '''
     vertex = np.array([tuple(points[i]) for i in range(points.shape[0])], dtype=dtype)
     el = ply.PlyElement.describe(vertex, 'vertex')
     data = ply.PlyData([el], text=False)
     data.write(path)
 
 
+import numpy as np
+from scipy import stats
+def block_merge(coords, pred, shape):
+    stride = 1 / shape
+    semantic = np.ones(shape + 1) * -1
+    instance = np.ones(shape + 1) * -1
+    semantic = semantic.astype(np.int32)
+    instance = instance.astype(np.int32)
+
+    batch_size = coords.shape[0]
+    npoints = coords.shape[1]
+    coords = coords / stride
+
+    merge_map = {'label': [], 'modes': []}
+    for b in range(batch_size):
+        xyz, labels = coords[b, ...].astype(np.float32), pred[b, ...].astype(np.int32)
+        xyz = xyz.astype(np.int32)
+        num_points = xyz.shape[0]
+
+        k = np.amax(labels[:, 1]) + 1
+        overlap = np.zeros([k, 1000])
+        # find label for each group
+        modes = {}
+        sizes = {}
+        for gid in range(k):
+            indices = (labels[:, 1] == gid)
+            mode = stats.mode(labels[indices, 0])[0]
+            try:
+                modes[gid] = int(mode)
+            except:
+                breakpoint()
+            sizes[gid] = np.sum(indices)
+        for i in range(num_points):
+            x, y, z = xyz[i]
+            gid = labels[i, 1]
+            if instance[x, y, z] >= 0 and semantic[x, y, z] == modes[gid]:
+                overlap[gid, instance[x, y, z]] += 1
+        label = np.argmax(overlap, axis=1)
+        n = np.amax(instance)
+        for gid in range(k):
+            count = np.amax(overlap[gid])
+            if count < 7 and sizes[gid] > 30:
+                n += 1
+                label[gid] = n
+        for i in range(num_points):
+            x, y, z = xyz[i]
+            gid = labels[i, 1]
+            if gid >= 0 and instance[x, y, z] < 0:
+                instance[x, y, z] = label[gid]
+                semantic[x, y, z] = modes[gid]
+        merge_map['label'].append({i: l for i, l in enumerate(label)})
+        merge_map['modes'].append(modes)
+
+    coords = coords.astype(np.int32)
+    for b in range(batch_size):
+        for i in range(npoints):
+            x, y, z = coords[b, i]
+            pred[b, i, 0] = semantic[x, y, z]
+            pred[b, i, 1] = instance[x, y, z]
+            # pred[b, i, 1] = x * 100 + y * 10 + z
+    return pred
+
+
 class WHU3D:
     def __init__(self,  data_root, data_type, format, scenes=[]):
         '''
         data_root: where is the data
         data_type: als, mls, image
         format: txt, ply, npy, h5, pickle
         [optional] scenes: a list of scenes
@@ -571,15 +634,14 @@
         whu3d.norm_coords()
         # self.compute_normals()
         whu3d.interprete_labels()
         whu3d.compute_normals(radius=0.8)
         whu3d.save_divided_blocks(out_dir='', num_points=600000, size=(20, 20), stride=10, threshold=100,
                                   show_points=False)
 
-
 if __name__ == '__main__':
     data_root = '/Users/hanxu/data/whu'
     # scenes = ['0404', '0940']
     whu3d = WHU3D(data_root=data_root, data_type='mls', format='txt')
     # whu3d.vis('0404', 'pc')
     whu3d.export_h5()
     whu3d.get_label_map()
```

## Comparing `pywhu3d-0.2.2.dist-info/LICENSE` & `pywhu3d-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywhu3d-0.2.2.dist-info/METADATA` & `pywhu3d-0.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhu3d
-Version: 0.2.2
+Version: 0.2.3
 Summary: Example pywhu3d tool Package
 Home-page: https://github.com/astroy
 Author: Xu Han
 Author-email: hanxu@glad3d.com
 Keywords: whu3d,dataset,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `pywhu3d-0.2.2.dist-info/RECORD` & `pywhu3d-0.2.3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 pywhu3d/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pywhu3d/evaluation.py,sha256=Etj9-4kPt0f4Dw9IzL4Ryn-YE9iyuYKUNGPl4IKB00Y,12682
-pywhu3d/tool.py,sha256=4htM7mkMr_APbKODpEXKGeBrFVM5pwaykPVIoNHHQdA,23500
+pywhu3d/evaluation.py,sha256=YKLLYbuzpD6lQkJMB_91rXio9iw97ssXY307U9HgeI4,12694
+pywhu3d/tool.py,sha256=JSOKYNRau_F3BC9B4y7JzDN5HXUsA80nXCZ-wzwQkoI,25631
 pywhu3d/configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pywhu3d/configs/als_config.py,sha256=rA-T6OyyM085K8p7T_-iejYr3Xj7qEebI0YwleBiFXc,5172
 pywhu3d/configs/base_config.py,sha256=6UCAS9UCipC_h6quwik6KulWZkp2KxkTYbApRCrRiGQ,2285
 pywhu3d/configs/mls_config.py,sha256=StVuLEMN9gRyywnhMD7JpHBVCNN47PNf2swkRxegEOw,11576
 pywhu3d/configs/mls_config_pole.py,sha256=aTtouZrropJ_fbhUNcWjzdc-pTWV3fVeGE3IZ4_fldU,13768
 pywhu3d/configs/paris_config.py,sha256=JrBFXzUkLLMT20bRLlLIUqooXFWftu_qwa5avvG083Q,7411
 pywhu3d/configs/s3dis_config.py,sha256=bB8-j0um70lPLv03PeZvw-LkjKYLOc0bvzYVozsdFyw,4395
 pywhu3d/configs/scannet_config.py,sha256=dJjkjiP1l3VEWQ1Uluwd7lum_3LMvFt0l7TPz1NydgI,4283
 pywhu3d/configs/toronto_config.py,sha256=SxYgYKJ6bf7zaNlmszNdpwTy7126kCW9HsEwWT0xeXI,4740
 pywhu3d/configs/wrap_configs.py,sha256=9Lezbp6IStVpvS2BJiNm_qQ-9e9gyXT5TN-h_L4UbJg,186
-pywhu3d-0.2.2.dist-info/LICENSE,sha256=jAt62vPGMrWssYEKav2xAaDp8wjtKQScCguopKunN8Q,1076
-pywhu3d-0.2.2.dist-info/METADATA,sha256=oIU4lAYcBiLMr7ddKNsqHSQMKfbu5L5Eagb2AX3Ldhw,1199
-pywhu3d-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pywhu3d-0.2.2.dist-info/top_level.txt,sha256=XacQWDtHJRY_akQP8PPiX56iNHQ_epUiFTGekh1FP7g,8
-pywhu3d-0.2.2.dist-info/RECORD,,
+pywhu3d-0.2.3.dist-info/LICENSE,sha256=jAt62vPGMrWssYEKav2xAaDp8wjtKQScCguopKunN8Q,1076
+pywhu3d-0.2.3.dist-info/METADATA,sha256=TJ4JZoQjdxblFFbv3GSk7O_Wsn3kKdvPOi-5bitKjTU,1199
+pywhu3d-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pywhu3d-0.2.3.dist-info/top_level.txt,sha256=XacQWDtHJRY_akQP8PPiX56iNHQ_epUiFTGekh1FP7g,8
+pywhu3d-0.2.3.dist-info/RECORD,,
```

