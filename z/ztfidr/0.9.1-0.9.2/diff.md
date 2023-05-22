# Comparing `tmp/ztfidr-0.9.1.tar.gz` & `tmp/ztfidr-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.9.1.tar", last modified: Tue May 16 08:43:34 2023, max compression
+gzip compressed data, was "ztfidr-0.9.2.tar", last modified: Mon May 22 15:03:34 2023, max compression
```

## Comparing `ztfidr-0.9.1.tar` & `ztfidr-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-16 08:43:34.907080 ztfidr-0.9.1/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.1/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-16 08:43:34.906956 ztfidr-0.9.1/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.1/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-16 08:43:34.907120 ztfidr-0.9.1/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-16 08:43:18.000000 ztfidr-0.9.1/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-16 08:43:34.906237 ztfidr-0.9.1/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-16 08:43:13.000000 ztfidr-0.9.1/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    14600 2023-05-16 08:41:57.000000 ztfidr-0.9.1/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.9.1/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.9.1/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)     3223 2023-05-07 16:40:33.000000 ztfidr-0.9.1/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.9.1/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    31049 2023-05-15 15:49:11.000000 ztfidr-0.9.1/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.1/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1170 2023-05-15 11:47:44.000000 ztfidr-0.9.1/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.1/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.1/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23521 2023-05-08 11:49:03.000000 ztfidr-0.9.1/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.9.1/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-16 08:43:34.906812 ztfidr-0.9.1/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-16 08:43:34.000000 ztfidr-0.9.1/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-16 08:43:34.000000 ztfidr-0.9.1/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-16 08:43:34.000000 ztfidr-0.9.1/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-16 08:43:34.000000 ztfidr-0.9.1/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-22 15:03:34.557697 ztfidr-0.9.2/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.2/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-22 15:03:34.557515 ztfidr-0.9.2/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.2/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-22 15:03:34.557746 ztfidr-0.9.2/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-22 15:03:14.000000 ztfidr-0.9.2/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-22 15:03:34.556571 ztfidr-0.9.2/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-22 15:03:09.000000 ztfidr-0.9.2/ztfidr/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    14854 2023-05-19 12:46:56.000000 ztfidr-0.9.2/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.9.2/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.9.2/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     3214 2023-05-22 14:53:09.000000 ztfidr-0.9.2/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.9.2/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    31049 2023-05-15 15:49:11.000000 ztfidr-0.9.2/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.2/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1170 2023-05-15 11:47:44.000000 ztfidr-0.9.2/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.2/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.2/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23610 2023-05-22 12:14:03.000000 ztfidr-0.9.2/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.9.2/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-22 15:03:34.557326 ztfidr-0.9.2/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-22 15:03:34.000000 ztfidr-0.9.2/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-22 15:03:34.000000 ztfidr-0.9.2/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-22 15:03:34.000000 ztfidr-0.9.2/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-22 15:03:34.000000 ztfidr-0.9.2/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.9.1/LICENSE` & `ztfidr-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/README.md` & `ztfidr-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/setup.py` & `ztfidr-0.9.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.9.1'
+VERSION = '0.9.2'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.9.1/ztfidr/io.py` & `ztfidr-0.9.2/ztfidr/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,23 +66,31 @@
                             "ztfdr2_targetlist.csv")
     if not load:
         return filepath
     
     return pandas.read_csv(filepath, **kwargs)
 
 def get_target_typing(load=True, index_col=0, sep=" ",
+                        from_datacreation=False,
                         clean=True, generic_typing=True,
                           **kwargs):
     """ """
-    filepath = os.path.join(IDR_PATH, "tables/.dataset_creation/sample_def",
+    if not from_datacreation: # bases:
+        filepath = os.path.join(IDR_PATH, "tables/ztfdr2_classifications.csv")
+        sep = ","
+    else:
+        filepath = os.path.join(IDR_PATH, "tables/.dataset_creation/sample_def",
                             "ztfdr2_typing.csv")
     if not load:
         return filepath
     
     data = pandas.read_csv(filepath, index_col=index_col, sep=sep, **kwargs)
+    if not from_datacreation:
+        return data
+    
     if clean:
         data["typing"] = data["typing"].str.replace("[","", regex=False).str.replace("]","", regex=False).str.replace("'","") # clean
         data["typing"] = data["typing"].str.replace("sn ia", "snia").str.replace("not ia", "notia")
         data["typing"] = data["typing"].str.split(" ")
         
         data["ntypings"] = data["ntypings"].str.replace("[","", regex=False).str.replace("]","", regex=False).str.split(" ")
```

### Comparing `ztfidr-0.9.1/ztfidr/lightcurve.py` & `ztfidr-0.9.2/ztfidr/lightcurve.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/ztfidr/linefitter.py` & `ztfidr-0.9.2/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/ztfidr/plotting.py` & `ztfidr-0.9.2/ztfidr/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def show_hubble_standardisation(sample, fig=None,
                                 param="c", vmin=-0.2, vmax=0.3, cmap="coolwarm", 
                                 clear_axes=False):
     """ """
     from astropy.cosmology import Planck18
     data = sample.get_data(x1_range=[-4,4], c_range=[-0.3,0.8], goodcoverage=True)
-    data = data[data["classification"].isin(['ia(-norm)','ia-norm'])]
+    data = data[data["classification"].isin(['snia-norm'])]
     
     if fig is None:
         fig = plt.figure(figsize=[6,4])
     
     ax = fig.add_axes([0.1,0.15,0.8,0.75])
     cax = fig.add_axes([0.4,0.3,0.4,0.25])
 
@@ -48,17 +48,17 @@
 
     return fig
 
 
 def show_typingdistribution(sample, ax=None, fig=None):
     """ """
     dist_typing = sample.data.groupby("classification").size()
-    ia_norm = dist_typing[["ia-norm","ia(-norm)"]].sum()
-    ia_pec = dist_typing[["ia-91t","ia-91bg","ia-other"]].sum()
-    ia = dist_typing[["sn ia"]].sum()
+    ia_norm = dist_typing[["snia-norm"]].sum()
+    ia_pec = dist_typing[["snia-pec-91t","snia-pec-91bg","snia-pec"]].sum()
+    ia = dist_typing[["snia"]].sum()
     rest = dist_typing.sum() - (ia_norm+ia_pec+ia)
     if ax is None:
         if fig is None:
             fig = plt.figure(figsize=[7,3])
         ax = fig.add_subplot(111)
     else:
         fig = ax.figure
```

### Comparing `ztfidr-0.9.1/ztfidr/salt2.py` & `ztfidr-0.9.2/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/ztfidr/sample.py` & `ztfidr-0.9.2/ztfidr/sample.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/ztfidr/script.py` & `ztfidr-0.9.2/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/ztfidr/snid.py` & `ztfidr-0.9.2/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/ztfidr/spectroscopy.py` & `ztfidr-0.9.2/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/ztfidr/target.py` & `ztfidr-0.9.2/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.1/ztfidr/typing.py` & `ztfidr-0.9.2/ztfidr/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,18 +329,19 @@
             self.load_classification(**kwargs)
             
         data = self.get_classification_df()
         classification = self.data.groupby("target_name").first()[["classification","class_origin"]]
         data = data.join(classification)
         return data
     
-    def store_typing(self, **kwargs):
+    def store_typing(self, to_datacreation=True, **kwargs):
         """ """
         data = self.get_typing(**kwargs)
-        return data.to_csv( io.get_target_typing(False), sep=" ")
+        return data.to_csv( io.get_target_typing(False, from_datacreation=to_datacreation),
+                                sep=" ")
 
     def load_classification(self, **kwargs):
         """ """
         classifications = self.get_classification(**kwargs)
         self._data = self.data.join(classifications, on="target_name", how="outer")
         
     def get_classification(self,  min_review=2,
```

### Comparing `ztfidr-0.9.1/ztfidr/utils.py` & `ztfidr-0.9.2/ztfidr/utils.py`

 * *Files identical despite different names*

