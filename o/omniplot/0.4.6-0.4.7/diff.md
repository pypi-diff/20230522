# Comparing `tmp/omniplot-0.4.6.tar.gz` & `tmp/omniplot-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplot-0.4.6.tar", last modified: Fri May  5 07:34:25 2023, max compression
+gzip compressed data, was "omniplot-0.4.7.tar", last modified: Mon May 22 02:44:37 2023, max compression
```

## Comparing `omniplot-0.4.6.tar` & `omniplot-0.4.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/
--rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-04-22 04:16:47.000000 omniplot-0.4.6/LICENSE
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-05-05 07:34:25.484147 omniplot-0.4.6/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)     3392 2023-04-30 04:35:53.000000 omniplot-0.4.6/README.md
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/omniplot/
--rw-rw-r--   0 koh       (1000) koh       (1000)      580 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/_adjustText.py
--rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-05-04 03:46:52.000000 omniplot-0.4.6/omniplot/_version.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/chipseq_utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/omniplot/cython_utils/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/cython_utils/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/data.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   101567 2023-05-05 07:29:10.000000 omniplot-0.4.6/omniplot/heatmap.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    12843 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/igraph_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    32121 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/networkplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    24258 2023-04-30 04:35:53.000000 omniplot-0.4.6/omniplot/plot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/plot_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    74812 2023-05-04 02:23:00.000000 omniplot-0.4.6/omniplot/proportion.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/regressionplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   134250 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/scatter.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/omniplot/scripts/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/scripts/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/scripts/gff2tss.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/statistics.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    44811 2023-04-23 08:15:37.000000 omniplot-0.4.6/omniplot/utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/omniplot.egg-info/
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)      711 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/SOURCES.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/dependency_links.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/requires.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/top_level.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-05-05 07:34:25.484147 omniplot-0.4.6/setup.cfg
--rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-22 04:16:47.000000 omniplot-0.4.6/setup.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/tests/
--rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-03-31 09:25:44.000000 omniplot-0.4.6/tests/test_chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     3033 2023-04-12 09:33:24.000000 omniplot-0.4.6/tests/test_network.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     5410 2023-04-29 06:16:08.000000 omniplot-0.4.6/tests/tests heatmap.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    14530 2023-05-05 07:21:22.000000 omniplot-0.4.6/tests/tests.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-22 02:44:37.833355 omniplot-0.4.7/
+-rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-04-22 04:16:47.000000 omniplot-0.4.7/LICENSE
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-05-22 02:44:37.833355 omniplot-0.4.7/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3392 2023-04-30 04:35:53.000000 omniplot-0.4.7/README.md
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-22 02:44:37.833355 omniplot-0.4.7/omniplot/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      580 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/_adjustText.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-05-22 02:42:51.000000 omniplot-0.4.7/omniplot/_version.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/chipseq_utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-22 02:44:37.833355 omniplot-0.4.7/omniplot/cython_utils/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/cython_utils/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/data.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   106673 2023-05-22 02:42:11.000000 omniplot-0.4.7/omniplot/heatmap.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    12843 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/igraph_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    32121 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/networkplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    27444 2023-05-21 06:17:28.000000 omniplot-0.4.7/omniplot/plot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/plot_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    74801 2023-05-07 11:59:55.000000 omniplot-0.4.7/omniplot/proportion.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    10715 2023-05-21 00:48:38.000000 omniplot-0.4.7/omniplot/regressionplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   134133 2023-05-21 00:28:37.000000 omniplot-0.4.7/omniplot/scatter.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-22 02:44:37.833355 omniplot-0.4.7/omniplot/scripts/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/scripts/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/scripts/gff2tss.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-04-22 04:16:47.000000 omniplot-0.4.7/omniplot/statistics.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    44620 2023-05-14 06:54:44.000000 omniplot-0.4.7/omniplot/utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-22 02:44:37.833355 omniplot-0.4.7/omniplot.egg-info/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-05-22 02:44:37.000000 omniplot-0.4.7/omniplot.egg-info/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)      734 2023-05-22 02:44:37.000000 omniplot-0.4.7/omniplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-05-22 02:44:37.000000 omniplot-0.4.7/omniplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-05-22 02:44:37.000000 omniplot-0.4.7/omniplot.egg-info/requires.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-05-22 02:44:37.000000 omniplot-0.4.7/omniplot.egg-info/top_level.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-05-22 02:44:37.833355 omniplot-0.4.7/setup.cfg
+-rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-22 04:16:47.000000 omniplot-0.4.7/setup.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-22 02:44:37.833355 omniplot-0.4.7/tests/
+-rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-03-31 09:25:44.000000 omniplot-0.4.7/tests/test_chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3033 2023-04-12 09:33:24.000000 omniplot-0.4.7/tests/test_network.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     5722 2023-05-22 02:37:42.000000 omniplot-0.4.7/tests/tests heatmap.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    10382 2023-05-21 06:16:17.000000 omniplot-0.4.7/tests/tests.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3789 2023-05-21 00:48:38.000000 omniplot-0.4.7/tests/tests_scatter.py
```

### Comparing `omniplot-0.4.6/LICENSE` & `omniplot-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/PKG-INFO` & `omniplot-0.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.4.6
+Version: 0.4.7
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.4.6/README.md` & `omniplot-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/__init__.py` & `omniplot-0.4.7/omniplot/__init__.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/_adjustText.py` & `omniplot-0.4.7/omniplot/_adjustText.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/chipseq.py` & `omniplot-0.4.7/omniplot/chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/chipseq_utils.py` & `omniplot-0.4.7/omniplot/chipseq_utils.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/heatmap.py` & `omniplot-0.4.7/omniplot/heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Union, Optional, Dict, List
 import matplotlib.collections as mc
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 import pandas as pd
 from matplotlib import cm
 from matplotlib.lines import Line2D
@@ -22,27 +21,28 @@
 from sklearn.decomposition import PCA, NMF, LatentDirichletAllocation
 from scipy.stats import fisher_exact
 from scipy.stats import zscore
 from itertools import combinations
 import os
 #script_dir = os.path.dirname( __file__ )
 #sys.path.append( script_dir )
-from omniplot.utils import * #
-from omniplot.utils import colormap_list, shape_list
 import scipy.stats as stats
-from joblib import Parallel, delayed
-from omniplot.chipseq_utils import _calc_pearson
 import itertools as it
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Rectangle, Circle,Ellipse, RegularPolygon, Polygon
 import copy
 import textwrap
 from matplotlib.artist import Artist
 from matplotlib.transforms import Affine2D
 import mpl_toolkits.axisartist.floating_axes as floating_axes
+import matplotlib.patheffects as patheffects
+from typing import Union, Optional, Dict, List
+
+from omniplot.utils import * #
+from omniplot.utils import colormap_list, shape_list
 
 __all__=["correlation", "triangle_heatmap", "complex_clustermap","dotplot", "heatmap"]
 def correlation(df: pd.DataFrame, 
                 category: Union[str, list]=[],
                 variables: List=[],
                 method="pearson",
                 palette: str="coolwarm",
@@ -95,63 +95,50 @@
     See Also
     --------
     Examples
     --------
     """
     original_index=df.index
     X, category=_separate_data(df, variables=variables, category=category)
-    # if len(category) !=0:
-    #
-    #     if type(category)==str:
-    #         category=[category]
-    #     #df=df.drop(category, axis=1)
-    #     valnames=list(set(df.columns) -set(category)) 
-    #     X = df[valnames].values
-    #     assert X.dtype==float, f"data must contain only float values except {category} column."
-    #
-    # else:    
-    #     X = df.values
-    #     assert X.dtype==float, "data must contain only float values."
-    if ztransform==True:
+    if ztransform is True:
         X=zscore(X, axis=0)
     if method=="pearson":
-        # dmat=Parallel(n_jobs=-1)(delayed(_calc_pearson)(ind, X) for ind in list(it.combinations(range(X.shape[0]), 2)))
-        # dmat=np.array(dmat)
-        # dmat=squareform(dmat)
-        # print(dmat)
-        # dmat+=np.identity(dmat.shape[0])
         dmat=np.corrcoef(X)
     else:
         dmat=squareform(pdist(X, method))
     if method=="pearson":
             ctitle="Pearson correlation"
     else:
         ctitle=method+" distance"    
-        
+
+    dfm=pd.DataFrame(data=dmat, columns=original_index,index=original_index)
+
+
+    colnames=dfm.columns
+
         
     if len(category) >0:
-        dfm=pd.DataFrame(data=dmat)
-        colnames=dfm.columns
         for cat in category:
             dfm[cat]=df[cat].values
         res=complex_clustermap(dfm,
                                heatmap_col=colnames, 
                                row_colors=category,
                                ztranform=False,
                                xticklabels=xticklabels,
                                yticklabels=yticklabels,
                                figsize=figsize,
                                ctitle=ctitle )
     else:
         
-        res=complex_clustermap(data=dmat,
+        res=complex_clustermap(dfm,
+                         heatmap_col=colnames, 
                          xticklabels=xticklabels,
                          yticklabels=yticklabels,
                    method="ward", 
-                   cmap=palette,
+                   heatmap_palette=palette,
                    col_cluster=True,
                    row_cluster=True,
                    figsize=figsize,
                    #rasterized=True,
                     #cbar_kws={"label":"Pearson correlation"}, 
                    #annot=show_values,
                    **clustermap_param)
@@ -214,15 +201,15 @@
     # Transformation matrix for rotating the heatmap.
     A = np.array([(y, x) for x in range(N, -1, -1) for y in range(N + 1)])
     t = np.array([[2**(-0.5), 2**(-0.5)], [-2**(-0.5), 2**(-0.5)]])
     A = np.dot(A, t)
     #t_ = np.array([[2**(-0.5), -2**(-0.5)], [2**(-0.5), 2**(-0.5)]])
     
     # -1.0 correlation is blue, 0.0 is white, 1.0 is red.
-    cmap = plt.cm.Reds
+    cmap = plt.get_cmap("Reds")
     #norm = mp.colors.BoundaryNorm(np.linspace(0, 10, 14), cmap.N)
     
     # This MUST be before the call to pl.pcolormesh() to align properly.
     ax.set_xticks([])
     ax.set_yticks([])
     
     X = A[:, 1].reshape(N + 1, N + 1)
@@ -1147,16 +1134,18 @@
                 rowplot_format: str="{x:.1f}",
                 colplot_format:  str="{x:.1f}",
                 
                 boxlabels: bool=False,
                 box_textwidth: Optional[int]=None,
                 box_max_lines: Optional[int]=None,
                 n_jobs: int=-1,
-                show_values: bool=False
-                ):
+                show_values: bool=False,
+                text_color: str="w",
+                val_format: str="",
+                )->Dict:
     """
     Drawing a heatmap. The function is mostly overlapping with the complex_clustermap, but has more flexibility, but may be slower.
     The main difference is this heatmap uses patch collections instead of pcolormech.  
     
     Parameters
     ----------
     df : pandas DataFrame
@@ -1296,17 +1285,38 @@
 
     rowplot_format: str, optional (default: "{x:.1f}")
         The format of y axis values of row plots/scatter/bar
 
     colplot_format:  str, optional (default: "{x:.1f}")
         The format of y axis values of row plots/scatter/bar
     
+    boxlabels: bool, optional (default: False)
+        Whether to add row labels boxed by clustering groups. 
+    
+    box_textwidth: int, optional
+        The number of charcters in one line of the boxlabels
+    
+    box_max_lines: Optional[int]=None,
+        The maximum number of lines in the boxlabels.
+    
+    n_jobs: int, optional (default: -1)
+        The number of threads to use for adding pathes/shapes to the heatmap.
+
+    show_values: bool, optional (default: False)
+        Whether to show values over the heatmap elements.
+
+    text_color: str="w",
+        The color of texts for value annotation.
+
+    val_format: str="",
+        The format of texts for value annotation. e.g., {x:.2f}
+
     Returns
     -------
-        {"row_clsuter":rclusters,"col_cluster":cclusters, "axes":axis_dict} : dict
+        {"row_clsuter":rclusters,"col_cluster":cclusters, "axes":axis_dict, "colsort":sortindexc,"rowsort":sortindexr} : dict
     Raises
     ------
     Notes
     -----
     References
     ----------
     See Also
@@ -1321,15 +1331,15 @@
     
     if col_split==True and row_split==True:
         raise Exception("Splitting both columns and rows may not be a good idea...")
     
     def _scale_size(x, size_scale, smin, smax):
         return size_scale*((x-smin)/(smax-smin))
     def _reverse_size(x, size_scale, smin, smax):
-        return (x/size_scale-0.01)*(smax-smin)+smin
+        return (x/size_scale)*(smax-smin)+smin
     
     margin=0.00
     sns.set_theme(style="white",font="Arial",font_scale=1.1)
     TBLR=['top','bottom','left','right']
     # Separating values into heatmap colors, sizes, ans category    
     lut={}
     if dtype=="numerical":
@@ -1350,18 +1360,20 @@
                 scX=np.array(shape_colors)
         if row_cluster==True or col_cluster==True:
             clustering_method="kmodes"
             print("Categorical variables are provided. 'kmodes' will be used for the clustering method.")
     
     rowplot_num=len(category)+len(row_colors)+\
         len(row_plot)+len(row_scatter)+len(row_bar)+row_axis+\
-        int(clustering_method=="kmeans" and row_cluster==True)+int(clustering_method=="kmodes" and row_cluster==True)
+        int(clustering_method=="kmeans" and row_cluster==True)+\
+        int(clustering_method=="kmodes" and row_cluster==True)
     colplot_num=len(col_colors)+len(col_plot)+\
         len(col_scatter)+len(col_bar)+col_axis+\
-        int(clustering_method=="kmeans" and col_cluster==True)+int(clustering_method=="kmodes" and col_cluster==True)
+        int(clustering_method=="kmeans" and col_cluster==True)+\
+        int(clustering_method=="kmodes" and col_cluster==True)
     Xshape=X.shape
     if np.sum(Xshape)>200:
         edgecolor=None
     show_legend=int(rowplot_num>0 or type(Xsize)!=type(None))
 
     if len(figsize)==0:
         figure_height=np.amin([np.amax([X.shape[0]/5, 3]), 10])
@@ -1371,103 +1383,45 @@
         else:
             figure_width=figure_height*X.shape[1]/X.shape[0]+int(boxlabels)*6
         figsize=[figure_width,figure_height,]
     print("figsize: ", figsize)
     fig=plt.figure(figsize=figsize, layout='constrained')
     
     # determining the size and positionn of axes
-    if col_ticklabels==True:
-        lmax = float(np.amax(list(map(len, list(collabels.astype(str)))))) 
-        lmax=np.amin([lmax/150, 0.3])
-    else:
-        lmax=0
-
-    if boxlabels==True:
-        row_ticklabels=False
-
-    xori=0.05
-    yori=0.11+lmax
-    lcatw=0.04
-    
-    legendw=0.15*show_legend
-    if boxlabels==True:
-        boxwidth=0.15
-    else:
-        boxwidth=0.
-    if row_cluster==True:
-        ltreew=0.15
-        ttreew=0.65-lcatw*rowplot_num-legendw-boxwidth
-    else:
-        ltreew=0
-        ttreew=0.75-lcatw*rowplot_num-legendw
-    
-    if col_cluster==True:
-        ltreeh=0.75-lmax
-        ttreeh=0.05
-    else:
-        ltreeh=0.8-lmax
-        ttreeh=0
-    if ttreew<0:
-        raise Exception("Too many things to plot. \
-                        Please reduce the number of \
-                        row-wise plots.")
-    hmapw=ttreew
-    hmaph=ltreeh
-    lcatx=xori+ltreew
-    tcaty=yori+ltreeh
-    tcath=0.025
-
-    hmapx=xori+ltreew+lcatw*rowplot_num
-    ttreey=yori+ltreeh+tcath*colplot_num
-    legendh=(3/Xshape[0])*hmaph
+    (xori, yori, 
+    boxwidth, 
+    legendw, legendh,
+    ltreew, ltreeh,  
+    ttreey, ttreew,  ttreeh, 
+    hmapx, hmapw, hmaph, 
+    lcatx, lcatw, 
+    tcaty, tcath, 
+    row_ticklabels)=_axis_loc_sizes(col_ticklabels, row_ticklabels,
+                    boxlabels, 
+                    row_cluster,col_cluster,
+                    show_legend,
+                    rowplot_num,colplot_num,
+                    collabels,
+                    Xshape)
     
     size_legend_num=3
     size_legend_elements=[]
     if type(Xsize)!=type(None):
-        smin=np.amin(Xsize)
-        smax=np.amax(Xsize)
-        _scaled=_scale_size(Xsize,1, smin, smax)
-        vmin, vmax=np.amin(_scaled), np.amax(_scaled)
-        print("scaled: ", vmin, vmax)
-        vinterval=(vmax-vmin)/(size_legend_num-1)
-        
-        if size_format=="":
-            if 1<np.abs(vmax)<=1000:
-                size_format="{x:.2f}"
-            elif 0<np.abs(vmax)<=1 or 1000<np.abs(vmax):
-                size_format="{x:.3E}"
-        sx=1
-        _sx=vmax*(hmaph/legendw)*size_legend_num/Xshape[1]
-        _sy=vmax*(hmaph/legendh)*size_legend_num/Xshape[0]
-        _sy=200
-        size_legend_elements.append(Rectangle((0 -0.5,0-0.5), 1, size_legend_num))
-
-        size_labels=[]
-        prev_top=0
-        for _i in range(size_legend_num):
-            s=vmin+_i*vinterval
-            if s <0.1:
-                s=0.1
-            sx=s*(hmapw/legendw)/Xshape[1]
-            sy=s*(hmaph/legendh)*size_legend_num/Xshape[0]
-            
-            if prev_top==0:
-                _yh=0
-            else:
-                _yh=prev_top+sy
-            if shape=="by_category":
-                size_legend_elements.append(_create_polygon("circle", 0, _i, sx,ry=sy))
-            else:
-                size_legend_elements.append(_create_polygon(shape, 0, _i, sx,ry=sy))
-
+        size_legend_elements, size_labels =_create_shape_legend_elements(Xsize, 
+                                                                        Xshape,
+                                                                        hmapw,
+                                                                        hmaph,
+                                                                        legendw,
+                                                                        legendh,
+                                                                        _scale_size,
+                                                                        _reverse_size,
+                                                                        size_legend_num,
+                                                                        shape,
+                                                                        size_format)
 
-            prev_top+=sy+0.1
-            _s=_reverse_size(s, 1, smin, smax)
-            size_labels.append([size_format.format(x=_s), _i])
-    
     # Row-wise clustering 
     legend_elements_dict={} 
     rclusters={}
     cclusters={}
     if row_cluster==True:
         if clustering_method=="hierarchical":
             # Drawing the left dendrogram
@@ -1528,18 +1482,23 @@
 
     # Column-wise clustering 
     if col_cluster==True:
         
         if clustering_method=="hierarchical":
             ax1=fig.add_axes([hmapx,ttreey,ttreew,ttreeh])
             X, Xsize, Zt, collabels, cclusters,=_dendrogram(X, 
-                                                                    Xsize, ax1,collabels,
-                                                                    treepalette ,
-                                                                    approx_clusternum_col, 
-                                                                    metric,method,above_threshold_color, "top")     
+                                                            Xsize, 
+                                                            ax1,
+                                                            collabels,
+                                                            treepalette ,
+                                                            approx_clusternum_col, 
+                                                            metric,
+                                                            method,
+                                                            above_threshold_color, 
+                                                            "top")     
             ax1.axis('off')
             ax1.margins(x=margin)
             sortindexc=Zt["leaves"]
             if len(shape_colors)>0:
                 scX=scX[:, sortindexc]
             ax_dict["toptree"]=ax1
         elif clustering_method=="kmeans":
@@ -1597,28 +1556,44 @@
                                            row_bar, 
                                            rowplot_format, 
                                            legend_elements_dict, 
                                            Xshape, 
                                            lcatx,lcatw,
                                            yori,hmaph, margin, 
                                            plotkw, scatterkw, barkw, catnum, ax_dict,row_axis=row_axis)
-    legend_elements_dict, catnum, axis_dict=_col_plot(sortindexc, fig, col_colors, col_plot, 
-                                            col_scatter, col_bar, 
+    legend_elements_dict, catnum, axis_dict=_col_plot(sortindexc, 
+                                                      fig, 
+                                                      col_colors, 
+                                                      col_plot, 
+                                            col_scatter, 
+                                            col_bar, 
                                             colplot_format,
                                             legend_elements_dict, 
-                                            Xshape, tcaty,tcath,hmapx,
-                                            hmapw, margin, plotkw, scatterkw, barkw, catnum, axis_dict, col_axis=col_axis)
+                                            Xshape, 
+                                            tcaty,
+                                            tcath,
+                                            hmapx,
+                                            hmapw, 
+                                            margin, 
+                                            plotkw, scatterkw, barkw, catnum, axis_dict, col_axis=col_axis)
     # Creating the heatmap
     # Calculating the maximum and minum values of the data if the data is numerical.
+    cmap=plt.get_cmap(palette)
+
     if dtype=="numerical":
-        cmap=plt.get_cmap(palette)
         Xmin=np.amin(X)
         Xmax=np.amax(X)
+        if val_format=="":
+            if 1<np.abs(Xmax)<=1000:
+                val_format="{x:.2f}"
+            elif 0<np.abs(Xmax)<=1 or 1000<np.abs(Xmax):
+                val_format="{x:.3E}"
+
+
     if len(shape_colors)>0:
-        cmap=plt.get_cmap(palette)
         scXmin=np.amin(scX)
         scXmax=np.amax(scX)
     if type(Xsize)!=type(None):
         Xsizemin=np.amin(Xsize)
         Xsizemax=np.amax(Xsize)
 
     # Creating the color legend lists if the data is categorical
@@ -1741,15 +1716,15 @@
 
 
             _r+=c
             _y+=_c
 
     #Drawing a heatmap
     pcolormesh=False
-    if Xshape[0]>1000 or Xshape[1]>1000:
+    if Xshape[0]>=512 or Xshape[1]>=512:
         pcolormesh=True
     if row_split==True and row_cluster==True:
         
         # print(cnums, _cnums)
         _y=0
         _r=0
         for i, (_c,c) in enumerate(zip(_cnums, cnums)):
@@ -1801,14 +1776,20 @@
                             ax,
                             row_ticklabels,
                             rowlabels[_r:_r+c], 
                             rowrot, 
                             col_ticklabels, 
                             collabels, 
                             colrot,rasterized, n_jobs=n_jobs)
+                if show_values==True:
+                    for (_xtmp, _ytmp), text in zip(row_col, Xsub.flatten()):
+                        txt=ax.text(_xtmp, _ytmp, val_format.format(x=text), color=text_color, ha="center",va="center")
+                        txt.set_path_effects([patheffects.withStroke(linewidth=1, foreground='black')])
+
+
                 ax.margins(x=margin,y=margin)
             ax.tick_params(pad=1,axis='both', which='both', length=0)
             
             if _y>0:
                 ax.set_xticks([])
                 
             _r+=c
@@ -1876,14 +1857,19 @@
                             ax,
                             row_ticklabels,
                             rowlabels, 
                             rowrot, 
                             col_ticklabels, 
                             collabels[_r:_r+c], 
                             colrot,rasterized, n_jobs=n_jobs)
+                if show_values==True:
+                    for (_xtmp, _ytmp), text in zip(row_col, Xsub.flatten()):
+                        txt=ax.text(_xtmp, _ytmp, val_format.format(x=text), color=text_color, ha="center",va="center")
+                        txt.set_path_effects([patheffects.withStroke(linewidth=1, foreground='black')])
+
                 ax.margins(x=margin,y=margin)
             ax.tick_params(pad=1,axis='both', which='both', length=0)
             if i<len(col_cnums)-1:
                 ax.set_yticks([])
             
             _r+=c
             _y+=hmapw*_c
@@ -1930,46 +1916,61 @@
                     facecolors=[_color_lut[u] for u in _X]
                 
             row_col=[ [j,i] for i in range(X.shape[0]) for j in range(X.shape[1])]
             
             _add_patches(facecolors, Xshape, shape, row_col, edgecolor, Xsize, 
                         _Xsize,ax,row_ticklabels,rowlabels, rowrot, 
                         col_ticklabels, collabels, colrot,rasterized,Xflatten=_X, n_jobs=n_jobs)
+            
+            if show_values==True:
+                for (_xtmp, _ytmp), text in zip(row_col, X.flatten()):
+                    txt=ax.text(_xtmp, _ytmp, val_format.format(x=text), color=text_color, ha="center",va="center")
+                    txt.set_path_effects([patheffects.withStroke(linewidth=1, foreground='black')])
+
             ax.margins(x=margin,y=margin)
         ax.tick_params(pad=1,axis='both', which='both', length=0)
         axis_dict["heatmap"]=ax
     
     #Setting categorical color legends
     legendnum=0
     if len(legend_elements_dict) >0:
         for legendnum, (cat, legend_elements) in enumerate(legend_elements_dict.items()):
             axlegend=fig.add_axes([hmapx+hmapw+boxwidth+0.01,ttreey-legendnum*0.15,legendw,legendh])
             axlegend.add_artist(axlegend.legend(handles=legend_elements, 
                                                 title=cat,bbox_to_anchor=(0.0,0.5),
                                                 loc="center left"))
             axlegend.axis('off')
             axis_dict["legend_"+cat]=axlegend
-    
+
+    if row_axis>0 or col_axis >0:
+        for i in range(row_axis):
+            legendnum+=1            
+            axlegend=fig.add_axes([hmapx+hmapw+boxwidth+0.01,ttreey-legendnum*0.15,legendw,legendh])
+            axlegend.axis('off')
+            axis_dict["row_legend"+str(i)]=axlegend
+        for i in range(col_axis):
+            legendnum+=1            
+            axlegend=fig.add_axes([hmapx+hmapw+boxwidth+0.01,ttreey-legendnum*0.15,legendw,legendh])
+            axlegend.axis('off')
+            axis_dict["col_legend"+str(i)]=axlegend
+
+
     if len(shape_legend_elements) >0:
-        if legendnum>0:
-            legendnum+=1
         for cat, legend_elements in shape_legend_elements.items():
+            legendnum+=1
+
             axlegend=fig.add_axes([hmapx+hmapw+boxwidth+0.01,ttreey-legendnum*0.15,legendw,legendh])
             axlegend.add_artist(axlegend.legend(legend_elements["ao"], 
             legend_elements["labels"],
             handler_map=legend_elements["handler"],
             title=cat,
             bbox_to_anchor=(0.0,0.5),
             loc="center left"))
-            # axlegend.add_artist(axlegend.legend(handles=legend_elements, 
-            #                                     title=cat,bbox_to_anchor=(0.0,0.5),
-            #                                     loc="center left"))
             axlegend.axis('off')
             axis_dict["legend_"+cat]=axlegend
-            legendnum+=1
 
     #Setting the size legend
     if type(Xsize)!=type(None):
         if legendnum>0:
             legendnum+=1
         axlegend=fig.add_axes([hmapx+hmapw+0.02,0.14,legendw,legendh])
         _pc = PatchCollection(size_legend_elements, edgecolor=["white"]+["darkgray"]*size_legend_num,
@@ -2018,51 +2019,69 @@
     # plt.subplots_adjust(**gridspec_kw)
     _save(save, "heatmap")
     if show==True:
         plt.show()
 
     return {"row_clsuter":rclusters,"col_cluster":cclusters, "axes":axis_dict, "colsort":sortindexc,"rowsort":sortindexr}
 
-def _add_patches(facecolors, Xshape, shape, row_col, edgecolor, Xsize, 
-                 _Xsize,ax,row_ticklabels,rowlabels, 
-                 rowrot, col_ticklabels, collabels, colrot,rasterized,Xflatten=None,n_jobs=-1):
+def _add_patches(facecolors: Union[List, np.ndarray], 
+                 Xshape: Union[List, tuple, np.ndarray], 
+                 shape: Union[str, dict], 
+                 row_col: list, 
+                 edgecolor, 
+                 Xsize, 
+                 _Xsize,
+                 ax: plt.Axes,
+                 row_ticklabels,
+                 rowlabels, 
+                 rowrot, 
+                 col_ticklabels, 
+                 collabels, 
+                 colrot,
+                 rasterized,
+                 Xflatten=None,
+                 n_jobs=-1):
     
     if type(Xsize)!=type(None):
         _row_col=np.array(row_col)
-        _shapes = [Rectangle((- 0.5,- 0.5), np.amax(_row_col[:,0])+1, np.amax(_row_col[:,1])+1)]
-        _pc = PatchCollection(_shapes, facecolor="w", alpha=1,
+        _shapes = [Rectangle((- 0.5,- 0.5), 
+                             np.amax(_row_col[:,0])+1, 
+                             np.amax(_row_col[:,1])+1)]
+        _pc = PatchCollection(_shapes, 
+                              facecolor="w", 
+                              alpha=1,
                     edgecolor="w")
         ax.add_collection(_pc)
 
     if type(shape)==dict:
-        # print(shape)
-        # print(Xflatten)
         if type(Xsize)!=type(None):
-            # shapes = [_create_polygon(shape[val], x,y, wh)
-            #             for (x, y), wh, val in zip(row_col, _Xsize,Xflatten)]
             shapes=Parallel(n_jobs=n_jobs)(delayed(_create_polygon)(
-                shape[val], x,y, wh) for (x, y), wh, val in zip(row_col, _Xsize,Xflatten))
-
+                shape[val], 
+                x,
+                y, 
+                wh) for (x, y), wh, val in zip(row_col, _Xsize,Xflatten))
 
         else:
-            # shapes = [_create_polygon(shape[val], x,y, 1)
-            #         for (x, y), val in zip(row_col,Xflatten)]
             shapes=Parallel(n_jobs=n_jobs)(delayed(_create_polygon)(
                 shape[val], x,y, 1) for (x, y), val in zip(row_col,Xflatten))
     else:
         if type(Xsize)!=type(None):            
             shapes = [_create_polygon(shape, x,y, wh)
                         for (x, y), wh in zip(row_col, _Xsize)]
-            shapes=Parallel(n_jobs=n_jobs)(delayed(_create_polygon)(shape, x,y, wh) for (x, y), wh in zip(row_col, _Xsize))
+            shapes=Parallel(n_jobs=n_jobs)(delayed(_create_polygon)(
+                shape, 
+                x,
+                y, 
+                wh) for (x, y), wh in zip(row_col, _Xsize))
         else:
-            shapes=Parallel(n_jobs=n_jobs)(delayed(_create_polygon)(shape, x,y, 1) for x, y in row_col)
-            
-            # shapes = [_create_polygon(shape, x,y, 1)
-            #             for x, y in row_col]
-
+            shapes=Parallel(n_jobs=n_jobs)(delayed(_create_polygon)(
+                shape, 
+                x,
+                y, 
+                1) for x, y in row_col)
     # Create patch collection with specified colour/alpha
     if edgecolor==None:
         pc = PatchCollection(shapes, facecolor=facecolors, alpha=1,
                         edgecolor=facecolors)
     else:
         pc = PatchCollection(shapes, facecolor=facecolors, alpha=1,
                         edgecolor=edgecolor)
@@ -2087,42 +2106,47 @@
     elif shape=="circle":
         return Ellipse((x, y),r, ry, **kwargs)
         
     elif shape=="triangle":
         vnum=3
         rs=[]
         for i in range(vnum):
-            rs.append([x+0.5*r*np.cos(np.pi/2+i*2*np.pi/vnum),y+0.5*ry*np.sin(np.pi/2+i*2*np.pi/vnum)])
+            rs.append([x+0.5*r*np.cos(np.pi/2+i*2*np.pi/vnum),
+                       y+0.5*ry*np.sin(np.pi/2+i*2*np.pi/vnum)])
         return Polygon(rs, **kwargs)
     elif shape=="star":
         rs=[]
         for i in range(5):
-            rs.append([x+0.5*r*np.cos(np.pi/2+(2*i)*2*np.pi/5),y+0.5*ry*np.sin(np.pi/2+(2*i)*2*np.pi/5)])
+            rs.append([x+0.5*r*np.cos(np.pi/2+(2*i)*2*np.pi/5),
+                       y+0.5*ry*np.sin(np.pi/2+(2*i)*2*np.pi/5)])
         return Polygon(rs, **kwargs)
     elif shape.startswith("polygon:"):
         _, vnum=shape.split(":")
         vnum=int(vnum)
         rs=[]
         for i in range(vnum):
-            rs.append([x+0.5*r*np.cos(np.pi/2+i*2*np.pi/vnum),y+0.5*ry*np.sin(np.pi/2+i*2*np.pi/vnum)])
+            rs.append([x+0.5*r*np.cos(np.pi/2+i*2*np.pi/vnum),
+                       y+0.5*ry*np.sin(np.pi/2+i*2*np.pi/vnum)])
 
         return Polygon(rs, **kwargs)
     elif shape.startswith("star:"):
         _, n, m=shape.split(":")
         n, m=int(n), int(m)
         rs=[]
         if n%m==0:
             l=n//m
             for _m in range(m):
                 
                 for _l in range(l+1):
-                    rs.append([x+0.5*r*np.cos(np.pi/2+(_l+_m/m)*2*np.pi/l),y+0.5*ry*np.sin(np.pi/2+(_l+_m/m)*2*np.pi/l)])
+                    rs.append([x+0.5*r*np.cos(np.pi/2+(_l+_m/m)*2*np.pi/l),
+                               y+0.5*ry*np.sin(np.pi/2+(_l+_m/m)*2*np.pi/l)])
         else:
             for i in range(n):
-                rs.append([x+0.5*r*np.cos(np.pi/2+(m*i)*2*np.pi/n),y+0.5*ry*np.sin(np.pi/2+(m*i)*2*np.pi/n)])
+                rs.append([x+0.5*r*np.cos(np.pi/2+(m*i)*2*np.pi/n),
+                           y+0.5*ry*np.sin(np.pi/2+(m*i)*2*np.pi/n)])
         return Polygon(rs, **kwargs)
     else:
         raise Exception["Unknown shape! you gave {}, but it only accepts 'rectangle', 'circle', 'star', 'polygon:n', 'star:n:m'".format(shape)]
 def _row_plot(df, 
               leaves, 
               fig, 
               category, 
@@ -2578,8 +2602,135 @@
                                    edgecolor='black', lw=1,
                                    transform=handlebox.get_transform())
         # patch = Ellipse([10, 3], 10, 10, facecolor=self.facecolor,
         #                            edgecolor='black', lw=1,
         #                            transform=handlebox.get_transform())
         handlebox.add_artist(patch)
         
-        return patch
+        return patch
+    
+
+
+def _axis_loc_sizes(col_ticklabels: bool, 
+                    row_ticklabels: bool,
+                    boxlabels: bool, 
+                    row_cluster: bool,
+                    col_cluster: bool,
+                    show_legend: int,
+                    rowplot_num: int,
+                    colplot_num: int,
+                    collabels: np.ndarray,
+                    Xshape: Union[np.ndarray, list, tuple]) -> List:
+    # determining the size and positionn of axes
+
+
+    if col_ticklabels==True:
+        lmax = float(np.amax(list(map(len, list(collabels.astype(str)))))) 
+        lmax=np.amin([lmax/150, 0.3])
+    else:
+        lmax=0
+
+    if boxlabels==True:
+        row_ticklabels=False
+
+    xori=0.05
+    yori=0.11+lmax
+    lcatw=0.04
+    
+    legendw=0.15*show_legend
+    if boxlabels==True:
+        boxwidth=0.15
+    else:
+        boxwidth=0.
+    if row_cluster==True:
+        ltreew=0.15
+        ttreew=0.65-lcatw*rowplot_num-legendw-boxwidth
+    else:
+        ltreew=0
+        ttreew=0.75-lcatw*rowplot_num-legendw
+    
+    if col_cluster==True:
+        ltreeh=0.75-lmax
+        ttreeh=0.05
+    else:
+        ltreeh=0.8-lmax
+        ttreeh=0
+    if ttreew<0:
+        raise Exception("Too many things to plot. \
+                        Please reduce the number of \
+                        row-wise plots.")
+    hmapw=ttreew
+    hmaph=ltreeh
+    lcatx=xori+ltreew
+    tcaty=yori+ltreeh
+    tcath=0.025
+
+    hmapx=xori+ltreew+lcatw*rowplot_num
+    ttreey=yori+ltreeh+tcath*colplot_num
+    legendh=(3/Xshape[0])*hmaph
+
+    return (xori, yori, 
+            boxwidth, 
+            legendw, legendh,
+            ltreew, ltreeh,  
+            ttreey, ttreew,  ttreeh, 
+            hmapx, hmapw, hmaph, 
+            lcatx, lcatw, 
+            tcaty, tcath, 
+            row_ticklabels)
+
+
+def _create_shape_legend_elements(Xsize, 
+                                  Xshape,
+                                  hmapw,
+                                  hmaph,
+                                  legendw,
+                                  legendh,
+                                  _scale_size,
+                                  _reverse_size,
+                                  size_legend_num,
+                                  shape,
+                                  size_format):
+    size_legend_elements=[]
+    smin=np.amin(Xsize)
+    smax=np.amax(Xsize)
+    _scaled=_scale_size(Xsize,1, smin, smax)
+    vmin, vmax=np.amin(_scaled), np.amax(_scaled)
+    # print("scaled: ", vmin, vmax)
+    vinterval=(vmax-vmin)/(size_legend_num-1)
+    
+    if size_format=="":
+        if 1<np.abs(smax)<=1000:
+            size_format="{x:.2f}"
+        elif 0<np.abs(smax)<=1 or 1000<np.abs(smax):
+            size_format="{x:.3E}"
+    
+    
+
+    sx=1
+    size_legend_elements.append(Rectangle((0 -0.5,0-0.5), 1, size_legend_num))
+
+    size_labels=[]
+    prev_top=0
+    for _i in range(size_legend_num):
+        if _i==size_legend_num-1:
+            s=vmax
+        else:
+            s=vmin+_i*vinterval
+        if s <0.1:
+            s=0.1
+        sx=s*(hmapw/legendw)/Xshape[1]
+        sy=s*(hmaph/legendh)*size_legend_num/Xshape[0]
+        
+        if shape=="by_category":
+            size_legend_elements.append(_create_polygon("circle", 0, _i, sx,ry=sy))
+        else:
+            size_legend_elements.append(_create_polygon(shape, 0, _i, sx,ry=sy))
+
+
+        prev_top+=sy+0.1
+
+        _s=_reverse_size(s, 1, smin, smax)
+        size_labels.append([size_format.format(x=_s), _i])
+    
+
+    return size_legend_elements, size_labels
```

### Comparing `omniplot-0.4.6/omniplot/igraph_classes.py` & `omniplot-0.4.7/omniplot/igraph_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/networkplot.py` & `omniplot-0.4.7/omniplot/networkplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/plot.py` & `omniplot-0.4.7/omniplot/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from typing import Union, Optional, Dict, List
-import matplotlib.collections as mc
-import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 import pandas as pd
-from matplotlib import cm
-from matplotlib.lines import Line2D
-from scipy.cluster.hierarchy import leaves_list
-from scipy.cluster import hierarchy
-from collections import defaultdict
-import matplotlib.colors
-from natsort import natsort_keygen, natsorted
-from matplotlib.patches import Rectangle
+import matplotlib.pyplot as plt
+import copy
+# from matplotlib import cm
+# from matplotlib.lines import Line2D
+# from scipy.cluster.hierarchy import leaves_list
+# from scipy.cluster import hierarchy
+# from collections import defaultdict
+# import matplotlib.colors
+# from natsort import natsort_keygen, natsorted
+# from matplotlib.patches import Rectangle
 import scipy.cluster.hierarchy as sch
-import fastcluster as fcl
-
-import sys 
-import matplotlib as mpl
-from sklearn.cluster import KMeans, DBSCAN
-from sklearn.metrics import silhouette_score
+# import fastcluster as fcl
+# import sys 
+# import matplotlib as mpl
+# from sklearn.cluster import KMeans, DBSCAN
+# from sklearn.metrics import silhouette_score
 from scipy.spatial.distance import pdist, squareform
-from sklearn.decomposition import PCA, NMF, LatentDirichletAllocation
-from scipy.stats import fisher_exact
+# from scipy.stats import fisher_exact
 from scipy.stats import zscore
-from itertools import combinations
-import os
+# from itertools import combinations
+# import os
 #script_dir = os.path.dirname( __file__ )
 #sys.path.append( script_dir )
-from omniplot.utils import * #
 import scipy.stats as stats
-from joblib import Parallel, delayed
-from omniplot.chipseq_utils import _calc_pearson
-import itertools as it
+from matplotlib.ticker import StrMethodFormatter
+# from joblib import Parallel, delayed
+# from omniplot.chipseq_utils import _calc_pearson
+# import itertools as it
 from omniplot.scatter import *
 from omniplot.proportion import *
 from omniplot.heatmap import *
 from omniplot.utils import colormap_list, hatch_list, marker_list
+from omniplot.utils import * #
+
 # hatch_list: list = ['//', '\\\\', '||', '--', '++', 'xx', 'oo', 'OO', '..', '**','/o', '\\|', '|*', '-\\', '+o', 'x*', 'o-', 'O|', 'O.', '*-']
 # marker_list: list=['.', '_' , '+','|', 'x', 'v', '^', '<', '>', 's', 'p', '*', 'h', 'D', 'd', 'P', 'X','o', '1', '2', '3', '4','|', '_']
 
 
 
 
 plt.rcParams['font.family']= 'sans-serif'
@@ -651,10 +651,104 @@
                 ax.scatter(i+0.5*np.random.uniform(size=X.shape[0])-0.25, X, color=point_color, **point_kw)
     if orientation=="horizontal":
         ax.set_yticks(np.arange(len(mat)), labels=xlabels)
     elif orientation=="vertical":
         ax.set_xticks(np.arange(len(mat)), labels=xlabels, rotation=90)
         plt.subplots_adjust(bottom=0.2)
 
+def lineplot(df: pd.DataFrame,
+             x: str="", 
+             y: Union[str, list]="", 
+             variables: Union[str, list]="",
+             split: bool=False,
+             ax: plt.Axes=None,
+             palette: Union[str, dict]="tab20b",
+             xlabel: str="",
+             ylabel: str="",
+             xunit: str="",
+             yunit: Union[str, dict]="",
+             xformat: str="",
+             yformat: str="",
+             logscalex: bool=False,
+             logscaley: bool=False,
+             title: str="",
+             plotkw: dict={},
+             show_legend: bool=True,
+             bbox_to_anchor: Union[list, tuple]=[1.05, 1],
+             right=0.75,
+             left=0.15,
+             bottom=0.15,
+             figsize: list=[],
+             rows_cols: list=[]) ->Dict:
+
+    if len(y)==0 and len(variables)==0:
+        raise Exception("Provide y or variables option")
+    elif len(variables)!=0:
+        y=copy.deepcopy(variables)
+
+    if isinstance(y, str):
+        y=[copy.deepcopy(y)]
+
+    if len(x)==0:
+        X=list(df.index)
+        x=df.index.name
+    else:
+        X=df[x]
+
+    
+    if isinstance(palette, str):
+        cmap=plt.get_cmap(palette, len(y))
+        lut={}
+        for i, _y in enumerate(y):
+            lut[_y]=cmap(i)
+    else:
+        lut=copy.deepcopy(palette)
+    if split==False:
+        if len(figsize)==0:
+            figsize=[6,4]
+        if isinstance(ax, type(None)):
+            fig, ax=plt.subplots(figsize=figsize)
+        for _y in y:
+            ax.plot(X, df[_y], color=lut[_y], label=_y, **plotkw)
+        _set_axis(ax,x, xlabel, ylabel, xunit, yunit, xformat, yformat,logscalex,logscaley, title)
+
+        if show_legend==True:
+            plt.legend(bbox_to_anchor=bbox_to_anchor)
+            plt.subplots_adjust(right=right, bottom=bottom, left=left)
+    else:
+        plotnum=len(y)
+        if len(rows_cols)==0:
+            rows_cols=[plotnum//2+int(plotnum%2!=0), 2]
+        if len(figsize)==0:
+            figsize=[6,4*(plotnum//2+int(plotnum%2!=0))]
+        if isinstance(ax, type(None)):
+            fig, ax=plt.subplots(nrows=rows_cols[0], ncols=rows_cols[1], figsize=figsize)
+        axes=ax.flatten()
+        for _ax, _y in zip(axes, y):
+            _ax.plot(X, df[_y], color=lut[_y], **plotkw)
+            _set_axis(_ax,x, xlabel, _y, xunit, yunit, xformat, yformat,logscalex,logscaley, "")
+        fig.suptitle(title)
+        plt.tight_layout(h_pad=5)
+def _set_axis(ax,x, xlabel, ylabel, xunit, yunit, xformat, yformat,logscalex,logscaley, title):
+    if xlabel !="":
+        ax.set_xlabel(xlabel)
+    else:
+        ax.set_xlabel(x)
+    if ylabel!="":
+        ax.set_ylabel(ylabel)
+    ax.set_title(title)
+    if yunit!="":
+        ax.text(0, 1, "({})".format(yunit), transform=ax.transAxes, ha="right")
+    if xunit!="":
+        ax.text(1, 0, "({})".format(xunit), transform=ax.transAxes, ha="left",va="top")
+    if xformat!="":
+        
+        ax.xaxis.set_major_formatter(StrMethodFormatter(xformat))
+    if yformat !="":
+        ax.yaxis.set_major_formatter(StrMethodFormatter(yformat))
+    if logscalex==True:
+        ax.set_xscale("log")
+    if logscaley==True:
+        ax.set_yscale("log")
 
 if __name__=="__main__":
     pass
```

### Comparing `omniplot-0.4.6/omniplot/plot_classes.py` & `omniplot-0.4.7/omniplot/plot_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/proportion.py` & `omniplot-0.4.7/omniplot/proportion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1035,16 +1035,18 @@
                   ncols: int=2,
                   ignore: float=0.05,
                   show_values: bool=True,
                   title: str="",
                   hatch: bool=False,
                   figsize: list=[],
                   show_legend:bool=False,
-                  bbox_to_anchor: list=[1.1, 1],
-                  right: float=0.7,bottom=0.1) ->Dict:
+                  bbox_to_anchor: list=[1, 1],
+                  right: float=0.8,
+                  bottom=0.1,
+                  top=0.9,left=0.1) ->Dict:
     """
     Drawing a nice pichart by counting the occurrence of values from pandas dataframe. if you want to draw a pie chart from numerical values, try nice_piechart_num.
     
     Parameters
     ----------
     df : pandas DataFrame
 
@@ -1106,16 +1108,20 @@
         fig, axes=plt.subplots(nrows=nrows, ncols=ncols, figsize=figsize)
     if title !="":
         fig.suptitle(title)
 
     axes=axes.flatten()
     for cat, ax in zip(category, axes):
         u, c=np.unique(df[cat], return_counts=True)
-        
-        srt=np.argsort(c)[::-1]
+        if order=="largest":
+            srt=np.argsort(c)[::-1]
+        elif order=="smallest":
+            srt=np.argsort(c)
+        else:
+            srt=np.arange(len(c))
         u=u[srt]
         c=c[srt]
         _c=c/np.sum(c)
         
         
         
         _cmap=plt.get_cmap(palette, c.shape[0])
@@ -1124,47 +1130,44 @@
             if _c[j]<ignore:
                 colors[j]=[0,0,0,1]
                 u[j]=""
                 continue
             if show_values==True:
                 u[j]=u[j]+"\n("+str(100*np.round(_c[j],1))+"%)"
         if hatch==True:
-            ax.pie(c, labels=u, 
+            piekw=dict(labels=u, 
                 counterclock=False,
                 startangle=90, 
                 colors=colors,
                 radius=1.25,
                 hatch=hatch_list[:c.shape[0]],
                 labeldistance=None)
-            ax.legend(bbox_to_anchor=[1,1])
         else:
-            if show_legend==True:
-                ax.pie(c, labels=u, 
+            piekw=dict(labels=u, 
                     counterclock=False,
                     startangle=90, 
                     colors=colors,
                     radius=1.25,
                     labeldistance=None)
-                ax.legend(bbox_to_anchor=[1,1])
-            else:
-                ax.pie(c, labels=u, 
-                    counterclock=False,
-                    startangle=90, 
-                    colors=colors,
-                    labeldistance=0.6,
-                    radius=1.25)
+        ax.pie(c, **piekw)
+        if show_legend==True or hatch==True:
+            ax.legend(bbox_to_anchor=bbox_to_anchor)
+
+
+
+
         ax.set_title(cat,backgroundcolor='lavender',pad=10)
     
 
 
     if len(category)!=ncols*nrows:
         for i in range(ncols*nrows-len(category)):
             fig.delaxes(axes[-(i+1)])
     # plt.tight_layout(h_pad=1)
-    plt.subplots_adjust(top=0.9,wspace=0.5)
+    plt.subplots_adjust(wspace=0.6, left=left, right=right, bottom=bottom,top=top)
     if title !="":
         fig.suptitle(title)
     return {"axes":ax}
 
 
 def nice_piechart_num(df: pd.DataFrame,
                       variables: List[str]=[],
```

### Comparing `omniplot-0.4.6/omniplot/regressionplot.py` & `omniplot-0.4.7/omniplot/regressionplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 import pandas as pd
 from matplotlib import cm
 from matplotlib.lines import Line2D
 from collections import defaultdict
-import matplotlib.colors
 import sys 
 import matplotlib as mpl
 from scipy.spatial.distance import pdist, squareform
 from scipy.stats import zscore
 from itertools import combinations
 
 import os
```

### Comparing `omniplot-0.4.6/omniplot/scatter.py` & `omniplot-0.4.7/omniplot/scatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from typing import Union, Optional, Dict, List
-import matplotlib.collections as mc
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 import pandas as pd
-from matplotlib import cm
 from matplotlib.lines import Line2D
 from scipy.cluster.hierarchy import leaves_list
 from scipy.cluster import hierarchy
 from collections import defaultdict
-import matplotlib.colors
 from natsort import natsort_keygen
 from matplotlib.patches import Rectangle
 import scipy.cluster.hierarchy as sch
 import fastcluster as fcl
 from matplotlib.patches import Patch
 import sys 
 import matplotlib as mpl
@@ -23,26 +20,25 @@
 from sklearn.decomposition import PCA, NMF, LatentDirichletAllocation
 from scipy.stats import fisher_exact
 from scipy.stats import zscore
 from itertools import combinations
 import os
 #script_dir = os.path.dirname( __file__ )
 #sys.path.append( script_dir )
-from omniplot.utils import *
 import scipy.stats as stats
 from joblib import Parallel, delayed
-from omniplot.chipseq_utils import _calc_pearson
 import itertools as it
 from matplotlib.ticker import StrMethodFormatter
 import statsmodels.api as sm
 from sklearn.linear_model import RANSACRegressor
-from matplotlib import colors
-from omniplot._adjustText import adjust_text
 import copy
 from sklearn import metrics
+from omniplot.utils import *
+from omniplot._adjustText import adjust_text
+from omniplot.chipseq_utils import _calc_pearson
 
 
 plt.rcParams['font.family']= 'sans-serif'
 plt.rcParams['font.sans-serif'] = ['Arial']
 plt.rcParams['svg.fonttype'] = 'none'
 sns.set_theme(font="Arial")
```

### Comparing `omniplot-0.4.6/omniplot/scripts/gff2tss.py` & `omniplot-0.4.7/omniplot/scripts/gff2tss.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/statistics.py` & `omniplot-0.4.7/omniplot/statistics.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/omniplot/utils.py` & `omniplot-0.4.7/omniplot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -744,20 +744,14 @@
                 
                 start=(2*np.pi/360)*_rotl*0.5+(2*np.pi/360)*_rot*0.5
                 theta=(2*np.pi/360)*((_rotr*0.5+_rot*0.5)-(_rotl*0.5+_rot*0.5))
                 #print(start, theta,_rotl, _rotr)
                 #print(start, theta, innerrad, outerrad,10, _colorlist[i])
                 _baumkuchen(ax, start, theta, innerrad, outerrad,10, _colorlist[i] ) #,edgecolor = "gray",linewidth=0.5)
                 
-            # patches, texts =plt.pie(colorpos, colors=_colorlist,
-            #         radius=outerrad,
-            #         counterclock=True,
-            #         startangle=label_coords[0][2]*0.5)
-            # circle=plt.Circle((0,0),innerrad, fc='white')
-            # plt.gca().add_patch(circle)
             labelnames.append(labelname)
             colorlabels_legend[labelname]={}
             colorlabels_legend[labelname]["colors"]=_cmp(np.linspace(0, 1, type_num))
             colorlabels_legend[labelname]["labels"]=ucolors
             classcounter+=1
         
         if colorlabels_legend!=None:
@@ -819,17 +813,17 @@
         for i, r in enumerate(row_plot):
             g.ax_row_colors.plot(r[leaves_list(g.dendrogram_row.linkage)]/np.amax(r)+i, np.arange(r.shape[0])+0.5)
         g.ax_row_colors.invert_xaxis()
         
     else:
         g=sns.clustermap(df,method=method,**kwargs)
     if color_var>0:
-        cmap = cm.nipy_spectral(np.linspace(0, 1, color_var))
+        cmap = plt.get_cmap("nipy_spectral")(np.linspace(0, 1, color_var))
     else:
-        cmap = cm.nipy_spectral(np.linspace(0, 1, approx_clusternum+5))
+        cmap = plt.get_cmap("nipy_spectral")(np.linspace(0, 1, approx_clusternum+5))
     hierarchy.set_link_color_palette([matplotlib.colors.rgb2hex(rgb[:3]) for rgb in cmap])
     lbranches=np.array(g.dendrogram_row.dendrogram["dcoord"])[:,:2]
     rbranches=np.array(g.dendrogram_row.dendrogram["dcoord"])[:,2:]
     thre=np.linspace(0, np.amax(g.dendrogram_row.dendrogram["dcoord"]), 100)[::-1]
     for t in thre:
         #print(np.sum(lbranches[:,1]>t),np.sum(rbranches[:,0]>t),np.sum(lbranches[:,0]>t),np.sum(rbranches[:,1]>t))
         crossbranches=np.sum(lbranches[:,1]>t)+np.sum(rbranches[:,0]>t)-np.sum(lbranches[:,0]>t)-np.sum(rbranches[:,1]>t)
@@ -869,15 +863,18 @@
     y_mean = np.mean(Y)
     numerator = np.sum((X - x_mean)*(Y - y_mean))
     denominator = ( np.sum((X - x_mean)**2) * np.sum((Y - y_mean)**2) )**.5
     correlation_coef = numerator / denominator
     r2 = correlation_coef**2
     return r2
 
-def _ci_pi(X: np.ndarray,Y: np.ndarray, plotline_X: np.ndarray, y_model: np.ndarray) -> list:
+def _ci_pi(X: np.ndarray,
+           Y: np.ndarray, 
+           plotline_X: np.ndarray, 
+           y_model: np.ndarray) -> list:
     x_mean = np.mean(X)
     y_mean = np.mean(Y)
     n = X.shape[0]                        # number of samples
     m = 2                             # number of parameters
     dof = n - m                       # degrees of freedom
     t = stats.t.ppf(0.975, dof)       # Students statistic of interval confidence
     residual = Y - y_model
@@ -967,32 +964,34 @@
                 plt.savefig(save+"_"+suffix+".pdf")
 
 
 from sklearn.decomposition import TruncatedSVD
 from sklearn.pipeline import make_pipeline
 from sklearn.random_projection import SparseRandomProjection
 
-def _get_embedding(method="umap",param={}):
+def _get_embedding(method: str="umap",
+                   param: dict={}):
     
-    
-    defaul_params={"tsne": dict(n_components=2,n_iter=500,
-                                n_iter_without_progress=150,
-                                perplexity=10,
-                                n_jobs=2,
-                                random_state=42),
-                "random_projection": dict(n_components=2, random_state=42, eigen_solver="arpack"),
-                "svd": dict(n_components=2),
-                "random_trees": dict(n_estimators=200, max_depth=5, random_state=42),
-                "mds": dict(n_components=2, n_init=1, max_iter=120, n_jobs=2, normalized_stress="auto"),
-                "lle": dict(n_neighbors=5, n_components=2, ),
-                "isomap":dict(n_neighbors=4, n_components=2),
-                "linear_discriminant":dict(n_components=2),
-                "random_projection": dict(n_components=2, random_state=42),
-                "nca": dict(n_components=2, init="pca", random_state=42),
-                "umap": dict(min_dist=0.25,n_neighbors=15)}
+    defaul_params={
+        "tsne": dict(n_components=2,n_iter=500,
+                     n_iter_without_progress=150,
+                     perplexity=10,
+                     n_jobs=2,
+                     random_state=42),
+        "random_projection": dict(n_components=2, random_state=42, eigen_solver="arpack"),
+        "svd": dict(n_components=2),
+        "random_trees": dict(n_estimators=200, max_depth=5, random_state=42),
+        "mds": dict(n_components=2, n_init=1, max_iter=120, n_jobs=2, normalized_stress="auto"),
+        "lle": dict(n_neighbors=5, n_components=2, ),
+        "isomap":dict(n_neighbors=4, n_components=2),
+        "linear_discriminant":dict(n_components=2),
+        "random_projection": dict(n_components=2, random_state=42),
+        "nca": dict(n_components=2, init="pca", random_state=42),
+        "umap": dict(min_dist=0.25,n_neighbors=15)
+        }
     if len(param)!=0:
         params={method: param}
     else:
         params=defaul_params
     from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
     from sklearn.ensemble import RandomTreesEmbedding
     from sklearn.manifold import (
@@ -1045,55 +1044,56 @@
         import umap 
         embedding=umap.UMAP(**params[method])
     else:
         raise Exception(f"Medthod {method} does not exist.")
     return embedding
 
 
-def _separate_data(df, variables=[], 
-                   category=""):
+def _separate_data(df: pd.DataFrame, 
+                   variables: list=[], 
+                   category: str="")->List:
     if len(variables) !=0:
         x = np.array(df[variables].values)
         if len(category) !=0:
-            if type(category)==str:
+            if isinstance(category, str):
                 category=[category]
             #category_val=df[category].values
         
         #if x.dtype!=np.number: 
         if np.issubdtype(x.dtype, np.number)==False:
             raise TypeError(f"variables must contain only float values. {x.dtype} was given")
     elif len(category) !=0:
-        if type(category)==str:
+        if isinstance(category, str):
             category=[category]
         #category_val=df[category].values
         df=df.drop(category, axis=1)
         x = np.array(df.values)
         if x.dtype!=np.number: 
             raise TypeError(f"data must contain only float values except {category} column. \
         or you can specify the numeric variables with the option 'variables'.")
         
     else:    
         x = df.values
         #category_val=[]
         if x.dtype!=float: 
             raise TypeError(f"data must contain only float values. \
-        or you can specify the numeric variables with the option 'variables'.")
+                            or you can specify the numeric variables with the option 'variables'.")
         
     return x, category
 
 def _separate_cdata(df, variables=[], 
                    category=""):
     if len(variables) !=0:
         x = np.array(df[variables].values)
         if len(category) !=0:
-            if type(category)==str:
+            if isinstance(category, str):
                 category=[category]
 
     elif len(category) !=0:
-        if type(category)==str:
+        if isinstance(category, str):
             category=[category]
         #category_val=df[category].values
         df=df.drop(category, axis=1)
         x = np.array(df.values)
         
     else:    
         x = df.values
@@ -1104,25 +1104,26 @@
 def _create_color_markerlut(df, cat, palette, markers=[]):
     # print(type(palette))
     color_lut={}
     marker_lut={}
     if df[cat].isnull().values.any():
         df[cat]=df[cat].fillna("NA")
     uniq_labels=sorted(list(set(df[cat])))
-    if type(palette)==str:
+    if isinstance(palette, str):
         _cmap=plt.get_cmap(palette, len(uniq_labels))
         
         color_lut={u: _cmap(i) for i, u in enumerate(uniq_labels)}
         
         if len(markers)!=0:
             if len(markers) < len(uniq_labels):
                 while len(markers) < len(uniq_labels):
                     markers.extend(markers)
             marker_lut={u: markers[i] for i, u in enumerate(uniq_labels)}
-    elif type(palette)==dict:
+    elif isinstance(palette, dict):
         color_lut=copy.deepcopy(palette)
     else:
-        raise TypeError("Unexpected type of the palette option. It must be either a matplot colormap name or the dictionary of a color look up table")
+        raise TypeError("Unexpected type of the palette option. It must be either a matplot \
+                        colormap name or the dictionary of a color look up table")
 
 
     return color_lut, marker_lut
```

### Comparing `omniplot-0.4.6/omniplot.egg-info/PKG-INFO` & `omniplot-0.4.7/omniplot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.4.6
+Version: 0.4.7
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.4.6/omniplot.egg-info/SOURCES.txt` & `omniplot-0.4.7/omniplot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 omniplot.egg-info/top_level.txt
 omniplot/cython_utils/__init__.py
 omniplot/scripts/__init__.py
 omniplot/scripts/gff2tss.py
 tests/test_chipseq.py
 tests/test_network.py
 tests/tests heatmap.py
-tests/tests.py
+tests/tests.py
+tests/tests_scatter.py
```

### Comparing `omniplot-0.4.6/setup.py` & `omniplot-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/tests/test_chipseq.py` & `omniplot-0.4.7/tests/test_chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/tests/test_network.py` & `omniplot-0.4.7/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.6/tests/tests heatmap.py` & `omniplot-0.4.7/tests/tests heatmap.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 
 test="triangle_heatmap"
 test="radialtree"
 test="regression"
 test="correlation"
 test="complex_clustermap"
 test="heatmap"
-test="heatmap"
+test="correlation"
 if test=="correlation":
     df=sns.load_dataset("penguins")
     df=df.dropna(axis=0)
     
+    op.correlation(df,variables=["bill_length_mm","bill_depth_mm","flipper_length_mm"], method="pearson", ztransform=True)
         
-    op.correlation(df, category=["species", "island","sex"], method="pearson", ztransform=True)
+    # op.correlation(df, category=["species", "island","sex"], method="pearson", ztransform=True)
     plt.show()
 
 elif test=="dotplot":
     df=pd.DataFrame({"Experiments":["exp1","exp1","exp1","exp1","exp2","exp2","exp3"],
                         "GO":["nucleus","cytoplasm","chromosome","DNA binding","chromosome","RNA binding","RNA binding"],
                         "FDR":[10,1,5,3,1,2,0.5],
                         "odds":[3.3,1.1,2.5,2.1,0.8,2.3,0.9]})
@@ -60,61 +61,69 @@
                         row_plot=["body_mass_g"],
                         row_bar=["body_mass_g"],
                         col_colors=["features"],
                         approx_clusternum=3,
                         marginalsum=True, title="Penguins")
     plt.show()
 elif test=="heatmap":
-    from PIL import Image
-    im=Image.open("/home/koh/Pictures/wave128.jpg").convert("LA")
-    df=pd.DataFrame(np.array(im)[:,:,0][::-1])
-    op.heatmap(df, shape="triangle",row_cluster=False, col_cluster=False,
-    ztranform=False, row_plot={"mean": df.mean(axis=1)}, row_ticklabels=False, col_ticklabels=False)
+    # from PIL import Image
+    # im=Image.open("/home/koh/Pictures/wave128.jpg").convert("LA")
+    # df=pd.DataFrame(np.array(im)[:,:,0][::-1])
+    # op.heatmap(df, shape="triangle",row_cluster=False, col_cluster=False,
+    # ztranform=False, row_plot={"mean": df.mean(axis=1)}, row_ticklabels=False, col_ticklabels=False)
     
     
-    df=sns.load_dataset("penguins")
+    # df=sns.load_dataset("penguins")
     
-    df=df.dropna(axis=0)
-    df=df.reset_index(drop=True)
-    res=op.heatmap(df=df,boxlabels=True, 
-    variables=["bill_length_mm","bill_depth_mm","flipper_length_mm"],
-    row_split=True, clustering_method="kmeans",
-               category=["species", "island"],
-               col_colors={"colors": ["bill","bill","flipper"]}, 
-               row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3)
-    op.heatmap(df=df, dtype="categorical", variables=["species", "island", "sex"],
-               row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3,column_wise_color=True) 
+    # df=df.dropna(axis=0)
+    # df=df.reset_index(drop=True)
+    # res=op.heatmap(df=df,boxlabels=True, 
+    # variables=["bill_length_mm","bill_depth_mm","flipper_length_mm"],
+    # row_split=True, clustering_method="kmeans",
+    #            category=["species", "island"],
+    #            col_colors={"colors": ["bill","bill","flipper"]}, 
+    #            row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3)
+    # op.heatmap(df=df, dtype="categorical", variables=["species", "island", "sex"],
+    #            row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3,column_wise_color=True) 
     # _df=df.sample(n=50, replace=False, random_state=1)
     # _df=_df.reset_index(drop=True)
     # op.heatmap(df=_df, 
     # dtype="categorical", 
     # variables=["species", "island", "sex"],
     #            row_plot=["body_mass_g"], 
     #            shape="by_category", shape_colors=np.arange(25*3).reshape([25,3]),
     #            row_ticklabels=False, 
     #            approx_clusternum=3,
     #            column_wise_color=True, sizes=np.arange(25*3).reshape([25,3])) 
 
-    mat=np.concatenate([0.25*np.random.uniform(0,1,size=[10, 25]),0.5*np.random.uniform(0,1,size=[15, 25]),
-                        np.random.uniform(0,1,size=[15, 25])])
-    mat=np.concatenate([mat, np.random.uniform(0,1,size=[40, 15])], axis=1)
-    print(mat.shape)
-    df=pd.DataFrame(mat)
-    res=op.heatmap(df, sizes=mat, size_title="random",cbar_title="random colors",
-               col_split=True,
-               row_plot={"mean": mat.mean(axis=1)}, 
-               row_scatter={"uniform": np.random.uniform(size=mat.shape[0])}, 
-               row_axis=2,
-               col_bar={"range": np.arange(mat.shape[1])},
-               
-               edgecolor=None, approx_clusternum=3, ztranform=False)
-    print(res.keys())
-    ax=res["axes"]["row_0"]
-    op.violinplot2(mat[res["rowsort"]], ax=ax,orientation="horizontal")
-    ax.set_xlabel("violin")
-    res["axes"]["row_0"].set_ylim(-0.5, mat.shape[0]-0.5)
-    # # op.heatmap(df, shape="circle", sizes=mat, edgecolor=None, approx_clusternum=3, row_split=True, ztranform=False)
-    # mat=np.arange(50).reshape([5,10]).astype(np.float)
+    # mat=np.concatenate([0.25*np.random.uniform(0,1,size=[10, 25]),0.5*np.random.uniform(0,1,size=[15, 25]),
+    #                     np.random.uniform(0,1,size=[15, 25])])
+    # mat=np.concatenate([mat, np.random.uniform(0,1,size=[40, 15])], axis=1)
+    # print(mat.shape)
     # df=pd.DataFrame(mat)
-    # op.heatmap(df, shape="circle", sizes=mat, row_cluster=False,col_cluster=False, edgecolor=None, approx_clusternum=3, ztranform=False, row_split=True)
-    print(res["axes"].keys())
+    # res=op.heatmap(df, sizes=mat, size_title="random",cbar_title="random colors",
+    #            col_split=True,
+    #            row_plot={"mean": mat.mean(axis=1)}, 
+    #            row_scatter={"uniform": np.random.uniform(size=mat.shape[0])}, 
+    #            row_axis=2,
+    #            col_bar={"range": np.arange(mat.shape[1])},
+               
+    #            edgecolor=None, approx_clusternum=3, ztranform=False)
+    # print(res.keys())
+    # ax=res["axes"]["row_0"]
+    # op.violinplot2(mat[res["rowsort"]], ax=ax,orientation="horizontal")
+    # ax.set_xlabel("violin")
+    # res["axes"]["row_0"].set_ylim(-0.5, mat.shape[0]-0.5)
+    # op.heatmap(df, shape="circle", sizes=mat, edgecolor=None, approx_clusternum=3, row_split=True, ztranform=False)
+    mat=np.arange(50).reshape([5,10]).astype(np.float)
+    df=pd.DataFrame(mat)
+    op.heatmap(df,
+               shape="circle",
+               show_values=True, 
+               sizes=mat,
+               row_cluster=False,
+               col_cluster=False,
+               edgecolor=None,
+               approx_clusternum=3,
+               ztranform=False,
+               row_split=True)
     plt.show()
```

