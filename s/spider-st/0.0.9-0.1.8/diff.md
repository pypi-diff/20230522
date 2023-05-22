# Comparing `tmp/spider-st-0.0.9.tar.gz` & `tmp/spider-st-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-st-0.0.9.tar", last modified: Sun May 21 09:03:35 2023, max compression
+gzip compressed data, was "spider-st-0.1.8.tar", last modified: Mon May 22 11:07:35 2023, max compression
```

## Comparing `spider-st-0.0.9.tar` & `spider-st-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 09:03:35.126614 spider-st-0.0.9/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.9/LICENSE
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      598 2023-05-21 09:03:35.126614 spider-st-0.0.9/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.9/README.md
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 09:03:35.146613 spider-st-0.0.9/setup.cfg
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1572 2023-05-21 09:02:26.000000 spider-st-0.0.9/setup.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 09:03:35.122614 spider-st-0.0.9/spider/
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 09:03:35.122614 spider-st-0.0.9/spider/R_script/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/R_script/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/R_script/run_SPARKX.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/R_script/run_spatalk.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6149 2023-05-21 07:21:38.000000 spider-st-0.0.9/spider/SPIDER.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 09:03:35.122614 spider-st-0.0.9/spider/SpatialDE/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.9/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 09:03:35.122614 spider-st-0.0.9/spider/SpatialDE/_internal/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.9/spider/SpatialDE/aeh.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/de_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/io.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.9/spider/SpatialDE/svca.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       43 2023-05-21 07:39:43.000000 spider-st-0.0.9/spider/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/clustering.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/enrichment.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 09:03:35.122614 spider-st-0.0.9/spider/lrdb/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/lrdb/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     8280 2023-05-21 09:01:51.000000 spider-st-0.0.9/spider/preprocess.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26596 2023-05-21 09:02:20.000000 spider-st-0.0.9/spider/svi.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/trajectory.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/util.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 07:21:25.000000 spider-st-0.0.9/spider/version.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.9/spider/visualization.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 09:03:35.126614 spider-st-0.0.9/spider_st.egg-info/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      598 2023-05-21 09:03:35.000000 spider-st-0.0.9/spider_st.egg-info/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 09:03:35.000000 spider-st-0.0.9/spider_st.egg-info/SOURCES.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 09:03:35.000000 spider-st-0.0.9/spider_st.egg-info/dependency_links.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      313 2023-05-21 09:03:35.000000 spider-st-0.0.9/spider_st.egg-info/requires.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 09:03:35.000000 spider-st-0.0.9/spider_st.egg-info/top_level.txt
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:07:35.527437 spider-st-0.1.8/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-22 10:56:51.000000 spider-st-0.1.8/LICENSE
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      598 2023-05-22 11:07:35.527437 spider-st-0.1.8/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-22 10:56:51.000000 spider-st-0.1.8/README.md
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-22 11:07:35.527437 spider-st-0.1.8/setup.cfg
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1665 2023-05-22 11:01:29.000000 spider-st-0.1.8/setup.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:07:35.443438 spider-st-0.1.8/spider/
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:07:35.463438 spider-st-0.1.8/spider/R_script/
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/R_script/__init__.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)      480 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/R_script/run_SPARKX.R
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)      765 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/R_script/run_spatalk.R
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)     6411 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/SPIDER.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:07:35.463438 spider-st-0.1.8/spider/SpatialDE/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.1.8/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:07:35.463438 spider-st-0.1.8/spider/SpatialDE/_internal/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.1.8/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/io.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.1.8/spider/SpatialDE/svca.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)       26 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/__init__.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)     2889 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/clustering.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/enrichment.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:07:35.479437 spider-st-0.1.8/spider/lrdb/
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/lrdb/__init__.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)   125912 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/lrdb/lrpairs.tsv
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035) 71272041 2022-11-04 08:20:48.000000 spider-st-0.1.8/spider/lrdb/pathways.tsv
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)     7561 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/preprocess.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2918 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/reconstruction.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)    26819 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/svi.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)      996 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/trajectory.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)     3295 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/util.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)       21 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/version.py
+-rwxrwxr-x   0 lishiying  (1035) lishiying  (1035)    15524 2023-05-22 11:04:22.000000 spider-st-0.1.8/spider/visualization.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-22 11:07:35.527437 spider-st-0.1.8/spider_st.egg-info/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      598 2023-05-22 11:07:35.000000 spider-st-0.1.8/spider_st.egg-info/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1277 2023-05-22 11:07:35.000000 spider-st-0.1.8/spider_st.egg-info/SOURCES.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-22 11:07:35.000000 spider-st-0.1.8/spider_st.egg-info/dependency_links.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      308 2023-05-22 11:07:35.000000 spider-st-0.1.8/spider_st.egg-info/requires.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-22 11:07:35.000000 spider-st-0.1.8/spider_st.egg-info/top_level.txt
```

### Comparing `spider-st-0.0.9/LICENSE` & `spider-st-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/PKG-INFO` & `spider-st-0.1.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.9
+Version: 0.1.8
 Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.9/setup.py` & `spider-st-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import setuptools
 import os
-os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
+# os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spider-st",
-    version="0.0.9",
+    version="0.1.8",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
     description="Identifying spatially variable interactions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     
-   package_data={'spider': ['lrdb/*.tsv'],
-                 'spider': ['R_script/*.R']},
+    # package_dir={"": "spider"},
+    
+    package_data={'lrdb': ['*.tsv'],
+                 'R_script': ['*.R']},
     
     install_requires=[
         'anndata>=0.8.0',
+        'numpy',
+        'Cython',
         'cellrank',
         'fa2',
         'gseapy',
         'h5py',
         'igraph',
         'leidenalg',
         'louvain',
@@ -43,23 +47,24 @@
         'pygco',
         'scanpy',
         'scgco',
         'scikit-learn',
         'scipy',
         'scvelo',
         'seaborn',
-        'sklearn',
+        # 'scikit-learn',
+        # 'sklearn',
         'somde',
         'somoclu',
         # 'spaotsc',
         'spatialde',
         'stlearn',
         'umap-learn',
         'statsmodels',
-        'importlib',
+        # 'importlib',
         'scprep',
         'squidpy',
         'magic-impute',
         'NaiveDE',
         'gpflow',
         'tensorflow>=2.12',
     ],
```

### Comparing `spider-st-0.0.9/spider/R_script/run_nnSVG.R` & `spider-st-0.1.8/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/R_script/run_spatalk.R` & `spider-st-0.1.8/spider/R_script/run_spatalk.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SPIDER.py` & `spider-st-0.1.8/spider/SPIDER.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from . import svi
 from . import preprocess
 from . import clustering
 from . import enrichment
 from . import visualization
 from . import util
 from . import trajectory
+from . import reconstruction
 
 class SPIDER():
     def __init__(self):
         self.svi = svi
         self.pp = preprocess
         self.cl = clustering
         self.er = enrichment
         self.vis = visualization
         self.util = util
         self.traj = trajectory
+        self.recon = reconstruction
         pass
 
     def prep(self,
             adata_input, work_dir, R_path,
             no_spatalk=False,
             cluster_key='type', 
             is_human=True, 
@@ -40,42 +42,42 @@
         lr_raw = preprocess.subset_lr(adata, no_spatalk, work_dir, cluster_key, is_human, overwrite, R_path)
         lr_df, adata = preprocess.subset_adata(adata, lr_raw)
         score = preprocess.score(adata, lr_df, interface_cell_pair, imputation)
         # Idata object construction
         idata = preprocess.idata_construct(score, interface_meta, lr_df, lr_raw, adata)
         return idata
 
-    def find_svi(self, idata, out_f, R_path, abstract=True, overwrite=False, n_neighbors=10, threshold=0.01, pattern_prune_threshold=0.0001):
+    def find_svi(self, idata, out_f, R_path, abstract=True, overwrite=False, n_neighbors=10, threshold=0.01, pattern_prune_threshold=0.0001, predefined_pattern_number=-1, svi_number=10):
         from os.path import exists
         from os import mkdir
         if not exists(out_f):
             print(f'Creating folder {out_f}')
             mkdir(out_f)
-        if len(idata) < 200:
-            print('number of interface is less than 200, skipping abstraction')
+        if len(idata) < 700:
+            print('number of interface is less than 700, skipping abstraction')
             abstract=False
         if abstract:
             som, idata, meta_idata = svi.abstract(idata, n_neighbors)
             svi.find_svi(meta_idata,out_f, overwrite, R_path, som=som) #generating results
             print('finished running all SVI tests')
-            svi_df, svi_df_strict = svi.combine_SVI(meta_idata,threshold=threshold)
+            svi_df, svi_df_strict = svi.combine_SVI(meta_idata,threshold=threshold, svi_number=svi_number)
             if (overwrite) | (not exists(f'{out_f}pattern.csv')):
-                svi.SVI_patterns(meta_idata, svi_df_strict, pattern_prune_threshold=pattern_prune_threshold)
+                svi.SVI_patterns(meta_idata, svi_df_strict, pattern_prune_threshold=pattern_prune_threshold, predefined_pattern_number=predefined_pattern_number)
                 pd.DataFrame(meta_idata.obsm['pattern_score']).to_csv(f'{out_f}pattern.csv')
                 meta_idata.var.to_csv(f'{out_f}membership.csv')
             else:
                 meta_idata.obsm['pattern_score'] = pd.read_csv(f'{out_f}pattern.csv', index_col=0).to_numpy()
                 meta_idata.var = pd.read_csv(f'{out_f}membership.csv', index_col=0)
             svi.meta_pattern_to_idata(idata, meta_idata)
             pd.DataFrame(meta_idata.obsm['pattern_score']).to_csv(f'{out_f}full_pattern.csv')
         else:
             svi.find_svi(idata, out_f, R_path, overwrite) #generating results
-            svi_df, svi_df_strict = svi.combine_SVI(idata,threshold=threshold)
+            svi_df, svi_df_strict = svi.combine_SVI(idata,threshold=threshold, svi_number=svi_number)
             if (overwrite) | (not exists(f'{out_f}pattern.csv')):
-                svi.SVI_patterns(idata, svi_df_strict, pattern_prune_threshold=pattern_prune_threshold)
+                svi.SVI_patterns(idata, svi_df_strict, pattern_prune_threshold=pattern_prune_threshold, predefined_pattern_number=predefined_pattern_number)
                 pd.DataFrame(idata.obsm['pattern_score']).to_csv(f'{out_f}pattern.csv')
                 idata.var.to_csv(f'{out_f}membership.csv')
             else:
                 idata.obsm['pattern_score'] = pd.read_csv(f'{out_f}pattern.csv', index_col=0)
                 idata.var = pd.read_csv(f'{out_f}membership.csv', index_col=0)   
             meta_idata = None
         idata.var[[f'pattern_correlation_{x}' for x in range(idata.obsm['pattern_score'].shape[1])]] = 0
```

### Comparing `spider-st-0.0.9/spider/SpatialDE/__init__.py` & `spider-st-0.1.8/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/distance_cache.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/gpflow_helpers.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/kernels.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/models.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/optimizer.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/score_test.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/sm_kernel.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/svca.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/tf_dataset.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/util.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/_internal/util_mixture.py` & `spider-st-0.1.8/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/aeh.py` & `spider-st-0.1.8/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/de_test.py` & `spider-st-0.1.8/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/dp_hmrf.py` & `spider-st-0.1.8/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/gaussian_process.py` & `spider-st-0.1.8/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/io.py` & `spider-st-0.1.8/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/SpatialDE/svca.py` & `spider-st-0.1.8/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/clustering.py` & `spider-st-0.1.8/spider/clustering.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import scanpy as sc
 import pandas as pd
 import numpy as np
 
 def supervised_spot_clust(idata, adata, label, portion=0.1, n_cluster=None, n_neighbors=100, min_dist=1):
     import umap
-    idata.uns['cell_meta'][label+'_int'] = idata.uns['cell_meta'][label].astype('category').cat.codes
-    masked_target = idata.uns['cell_meta'][label+'_int']
+    masked_target = idata.uns['cell_meta'][label].astype('category').cat.codes.to_numpy()
     np.random.seed(52)
     masked_target[np.random.choice(len(idata.uns['cell_meta'][label]), size=int(len(idata.uns['cell_meta'][label]) * portion), replace=False)] = -1
     embedding = umap.UMAP(n_neighbors=n_neighbors, min_dist=min_dist,random_state=52).fit_transform(idata.uns['cell_pattern'], y=masked_target)
     adata.obsm['X_umap'] = embedding
     sc.pp.neighbors(adata, n_neighbors=20, use_rep='X_umap')
     sc.tl.draw_graph(adata)
     flag = 1
```

### Comparing `spider-st-0.0.9/spider/enrichment.py` & `spider-st-0.1.8/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/preprocess.py` & `spider-st-0.1.8/spider/preprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         meta.celltype = "T"+meta.celltype.astype('str')
     meta.celltype = meta.celltype.str.replace(' ', '_')
     meta.celltype = meta.celltype.str.replace('-', '_')
     meta.to_csv(meta_f)
     species = 'Human' if is_human else 'Mouse'
     with resources.path("spider.R_script", "run_spatalk.R") as pw_fn:
         os.system(str(f'/bin/bash -c "{R_path} -f {pw_fn} {count_f} {meta_f} {species} {out_f}"'))
-        # os.system(str(f'/bin/bash -c "source /etc/profile;module load GCC/11.2.0 OpenMPI/4.1.1 R/4.2.0 Anaconda3/2022.05 R-bundle-Bioconductor/3.15-R-4.2.0;R -f {pw_fn} {count_f} {meta_f} {species} {out_f}"'))
     
 # imputation
 def impute_MAGIC(adata):
     magic_op = magic.MAGIC(n_jobs=5)
     inp = adata.to_df()
     inp = scprep.normalize.library_size_normalize(inp)
     inp = scprep.transform.sqrt(inp)
@@ -91,15 +90,15 @@
     l = lr_df['ligand'].to_numpy().flatten()
     r = lr_df['receptor'].to_numpy().flatten()
     sub_exp = exp_ref[np.concatenate((l, r))].to_numpy()
     sub_exp_rev = exp_ref[np.concatenate((r, l))].to_numpy()
     edge_exp_both = np.multiply(sub_exp[pairs[0]], sub_exp_rev[pairs[1]])
     # equation 2 in the manuscript
     print('scoring')
-    score = lr_df['score'].to_numpy()*np.sqrt(np.maximum(edge_exp_both[:, :int(len(l))], edge_exp_both[:, int(len(l)):]))
+    score = np.sqrt(np.maximum(edge_exp_both[:, :int(len(l))], edge_exp_both[:, int(len(l)):])) * lr_df['score'].to_numpy()
     return score
 
 def find_interfaces(adata, coord_type, n_neighs, cluster_key):
         pairs = find_pairs(adata, coord_type=coord_type, n_neighs=n_neighs)
         pairs_meta = meta(adata, cluster_key, pairs)
         return pairs, pairs_meta
 
@@ -113,31 +112,24 @@
     adata = adata[:, adata.var_names.isin(unique_lr)]
     sc.pp.filter_genes(adata, min_cells=1)
     sc.pp.normalize_total(adata, target_sum=1e4)
     genes = adata.var_names.tolist()
     lr_df = lr_df[lr_df['ligand'].isin(genes) & lr_df['receptor'].isin(genes)]
     return lr_df, adata
 
+
 def find_pairs(adata, coord_type='generic', n_neighs=6):
-    from sklearn.metrics import pairwise_distances
-    from scipy.sparse import triu
-    from scipy.spatial import Delaunay
     from squidpy.gr import spatial_neighbors
-    if coord_type=='grid':    
+    from scipy.sparse import triu
+    if coord_type == 'grid':
         spatial_neighbors(adata, coord_type=coord_type, n_neighs=n_neighs)
-        return np.transpose(triu(adata.obsp['spatial_connectivities']).nonzero()).T
     else:
-        print('non grid coordinate')
         spatial_neighbors(adata, coord_type=coord_type, delaunay=True, n_neighs=n_neighs)
-        potential_pairs = np.transpose(triu(adata.obsp['spatial_connectivities']).nonzero()).T
-        print('distance cutoff')
-        d = np.linalg.norm(adata.obsm['spatial'][potential_pairs[0]]-adata.obsm['spatial'][potential_pairs[1]], axis=1)
-        d = (d - d.mean()) / d.std()**2
-        potential_pairs = potential_pairs[:, d <= d.std()]
-        return potential_pairs
+    return np.transpose(triu(adata.obsp['spatial_connectivities']).nonzero()).T
+
 
 def meta(adata, cluster_key, pairs):
     # get label
     pairs_meta = pd.DataFrame()
     pairs_meta['A'] = adata.obs_names[pairs[0]]
     pairs_meta['B'] = adata.obs_names[pairs[1]]
     pairs_meta[['A_row', 'A_col']] = adata.obsm['spatial'][pairs[0]]
```

### Comparing `spider-st-0.0.9/spider/svi.py` & `spider-st-0.1.8/spider/svi.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,15 @@
                 n_jobs=10,
             )
             idata.uns['moranI_time'] = time.time()-t0
             idata.uns['moranI'].to_csv(f'{work_dir}moranI.csv')
         result = pd.read_csv(f'{work_dir}moranI.csv', index_col=0)
         idata.uns['moranI'] = result
         print(f'Added key moranI in idata.uns')
-    except Exception as e:
-        print(e)
+    except:
         pass
 
 def svi_geary(idata, work_dir,overwrite=False):
     try:
         t0=time.time()
         n_perms=1000
         if (overwrite) | (not exists( f'{work_dir}gearyC.csv')):
@@ -100,16 +99,15 @@
                 n_jobs=10,
             )
             idata.uns['gearyC_time'] = time.time()-t0
             idata.uns['gearyC'].to_csv(f'{work_dir}gearyC.csv')
         result = pd.read_csv(f'{work_dir}gearyC.csv', index_col=0)
         idata.uns['gearyC'] = result
         print(f'Added key gearyC in idata.uns')
-    except Exception as e:
-        print(e)
+    except:
         pass
 
 def svi_nnSVG(idata, work_dir, R_path, overwrite=False):
     try:
         count_f = f'{work_dir}idata_count.csv'
         meta_f = f'{work_dir}idata_meta.csv'
         if (overwrite) | ((not exists(count_f)) & (not exists(meta_f))):
@@ -121,15 +119,14 @@
                 os.system(str(f'/bin/bash -c "{R_path} -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
             idata.uns['nnSVG_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}nnSVG.csv', index_col=0)
         idata.uns['nnSVG'] = result
         print(f'Added key nnSVG in idata.uns')
     except Exception as e:
         print(e)
-        pass
     
 def scGCO_sv(locs, data_norm, cellGraph, gmmDict, smooth_factor=10, unary_scale_factor=100, label_cost=10, algorithm='expansion'):
     from itertools import repeat
     from functools import reduce
     import operator
     import statsmodels.stats.multitest as multi
     import scGCO
@@ -180,16 +177,15 @@
             gmmDict= scGCO.gmm_model(data_norm)
             result_df= scGCO_sv(locs, data_norm, cellGraph,gmmDict)
             scGCO.write_result_to_csv(result_df, f'{work_dir}scGCO.csv')
             idata.uns['scGCO_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}scGCO.csv')
         idata.uns['scGCO'] = result
         print(f'Added key scGCO in idata.uns')
-    except Exception as e:
-        print(e)
+    except:
         pass
     
 def svi_SPARKX(idata, work_dir, R_path, overwrite=False):
     try:
         count_f = f'{work_dir}idata_count.csv'
         meta_f = f'{work_dir}idata_meta.csv'
         if (overwrite) | ((not exists(count_f)) & (not exists(meta_f))):
@@ -199,16 +195,15 @@
             t0=time.time()
             with resources.path("spider.R_script", "run_SPARKX.R") as pw_fn:
                 os.system(str(f'/bin/bash -c "{R_path} -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
             idata.uns['SPARKX_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SPARKX.csv', index_col=0)
         idata.uns['SPARKX'] = result
         print(f'Added key SPARKX in idata.uns')
-    except Exception as e:
-        print(e)
+    except:
         pass
     
 def svi_SpatialDE2(idata, work_dir, overwrite=False):
     try:
         # if (overwrite) | (not exists(f'{work_dir}SpatialDE.csv')) | (not exists(f'{work_dir}SpatialDE_individual.csv')):
         if (overwrite) | (not exists(f'{work_dir}SpatialDE.csv')):
             print('in')
@@ -218,16 +213,15 @@
             svg_full = pd.concat([svg_full.set_index('gene'), individual.loc[individual.groupby('gene').lengthscale.idxmin()].set_index('gene')], axis=1)
             svg_full.to_csv(f'{work_dir}SpatialDE.csv')
             individual.to_csv(f'{work_dir}SpatialDE_individual.csv')
             idata.uns['SpatialDE2_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SpatialDE.csv', index_col=0)
         idata.uns['SpatialDE'] = result
         print(f'Added key SpatialDE in idata.uns')
-    except Exception as e:
-        print(e)
+    except:
         pass 
     
 def svi_SOMDE(idata, work_dir, overwrite=False, som=None):
     try:
         if (overwrite) | (not exists(f'{work_dir}SOMDE.csv')):
             t0=time.time()
             if som is None:
@@ -241,25 +235,24 @@
             nres = som.norm()
             result, SVnum =som.run()
             result.to_csv(f'{work_dir}SOMDE.csv')
             idata.uns['SOMDE_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SOMDE.csv', index_col=0)
         idata.uns['SOMDE'] = result
         print(f'Added key SOMDE in idata.uns')
-    except Exception as e:
-        print(e)
+    except:
         pass
     
-def combine_SVI(idata, threshold):
+def combine_SVI(idata, threshold, svi_number):
     svi_df, svi_df_strict = combine_SVI_strict(idata,threshold=threshold)
-    if len(svi_df_strict) < 10:
-        print('Detected SVI number is less than 10, falling back to relaxed filtering.')
+    if len(svi_df_strict) <= svi_number:
+        print(f'Detected SVI number is less than {svi_number}, falling back to relaxed filtering.')
         svi_df, svi_df_strict = combine_SVI_Fisher(idata,threshold=threshold)
-    if len(svi_df_strict) < 10:
-        print('Detected SVI number is less than 10, falling back to use SOMDE result only.')
+    if len(svi_df_strict) <= svi_number:
+        print(f'Detected SVI number is less than {svi_number}, falling back to use SOMDE result only.')
         svi_df, svi_df_strict  = combine_SVI_somde(idata,threshold=threshold)
     return svi_df, svi_df_strict
 
 def combine_SVI_Fisher(idata, threshold=0.05):
     from scipy.stats import combine_pvalues
     methods = np.array(['SOMDE', 'SpatialDE', 'SPARKX', 'nnSVG', 'scGCO', 'gearyC', 'moranI'])[np.isin(['SOMDE', 'SpatialDE', 'SPARKX', 'nnSVG', 'scGCO', 'gearyC', 'moranI'],list(idata.uns.keys()))]
     df = []
@@ -346,51 +339,55 @@
 class dotdict(dict):
     """dot.notation access to dictionary attributes"""
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 # SVI pattern generation with Gaussian process mixture model
-def SVI_patterns(idata, svi_df_strict, iter=1000, pattern_prune_threshold=1e-8):
+def SVI_patterns(idata, svi_df_strict, iter=1000, pattern_prune_threshold=1e-8, predefined_pattern_number=-1):
     from spider import SpatialDE as SpatialDE2
     allsignifgenes = svi_df_strict.index.to_numpy()
     if 'lengthscale' in idata.uns['SpatialDE'].columns:
         l=idata.uns['SpatialDE'].loc[allsignifgenes]['lengthscale'].to_list()
         if len(np.unique(l)) < 2:
             allsignifgenes = np.intersect1d(allsignifgenes, idata.uns['SOMDE']['g'].to_numpy())
             l=idata.uns['SOMDE'].set_index('g').loc[allsignifgenes]['l'].to_list()
     else:
         l=idata.uns['SOMDE'].set_index('g').loc[allsignifgenes]['l'].to_list()
+
     pattern_number = 1000
-    if len(np.unique(l)) <= 1:
+    print(predefined_pattern_number)
+    if (len(np.unique(l)) <= 1) | (predefined_pattern_number != -1):
         pattern_number = -1
     for count in range(5):
         print(pattern_number, count, pattern_prune_threshold)
         if (pattern_number > 100) and (pattern_prune_threshold<1) and (count < 4):
             param_obj = SpatialDE2.SpatialPatternParameters(lengthscales=l,maxiter=iter, pattern_prune_threshold=pattern_prune_threshold)
             upper_patterns, _ = SpatialDE2.spatial_patterns(idata, genes=allsignifgenes, rng=np.random.default_rng(seed=45), params=param_obj, copy=False)
             pattern_number = upper_patterns.patterns.shape[1]
             pattern_prune_threshold = pattern_prune_threshold*100
             if pattern_number < 2:
                 pattern_number = -1
         elif (pattern_number < 100) and (pattern_number > 2):
             break
         else:
-            print(f'falling back to controlled pattern')
-            histology_results, patterns, prob = SVI_patterns_v1(idata, svi_df_strict)
+            print(f'using controlled pattern')
+            histology_results, patterns, prob = SVI_patterns_v1(idata, svi_df_strict, components=predefined_pattern_number)
             upper_patterns = dotdict({
                 'labels': histology_results['pattern'].to_numpy(),
                 'patterns': patterns.to_numpy(),
                 'pattern_probabilities': prob
             })
             pattern_number = patterns.shape[1]
+            histology_results['pattern'].to_csv('/home/lishiying/data6/01-interaction/results/DFPFC_paper/151673/patttern.csv')
             break
-
     print(f'eventually found {pattern_number} patterns')
     idata.var['label'] = -1
+    if len(upper_patterns.labels) !=  len(allsignifgenes):
+        allsignifgenes = svi_df_strict.index.to_numpy()
     idata.var.loc[allsignifgenes, 'label'] = upper_patterns.labels
     idata.var[[f'pattern_membership_{x}' for x in range(upper_patterns.pattern_probabilities.shape[1])]] = 0
     idata.var.loc[allsignifgenes, [f'pattern_membership_{x}' for x in range(upper_patterns.pattern_probabilities.shape[1])]] = upper_patterns.pattern_probabilities
     idata.obsm['pattern_score'] = upper_patterns.patterns
     idata.var[[f'pattern_correlation_{x}' for x in range(idata.obsm['pattern_score'].shape[1])]] = 0
     corr_df=pd.concat([idata.to_df(),pd.DataFrame(idata.obsm['pattern_score'],index=idata.obs_names)],axis=1).corr().loc[idata.var_names, range(idata.obsm['pattern_score'].shape[1])]
     idata.var[[f'pattern_correlation_{x}' for x in range(idata.obsm['pattern_score'].shape[1])]] = corr_df.to_numpy()
```

### Comparing `spider-st-0.0.9/spider/trajectory.py` & `spider-st-0.1.8/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.9/spider/visualization.py` & `spider-st-0.1.8/spider/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -299,26 +299,26 @@
     moran_df_svi['label'] = 'SVI genes'
     df = pd.concat([moran_df, moran_df_lr,moran_df_svi])
     print(moran_df.I.mean(),moran_df_lr.I.mean(), moran_df_svi.I.mean())
     sns.boxplot(data=df, x="label", y="I", order=["SVI genes", "LR genes",  "SVG",], palette={"SVI genes":"#098154","LR genes":  "#069af3",  "SVG": "#c72e29"})
     plt.title('Moran I')
     
     plt.subplot(1, 3, 2)
-    g=venn3(subsets = [set(gene_list_lri),set(genelist_lr),set(genelist)], #绘图数据集
-        set_labels = ('SVI genes', "LR genes",'SVG'), #设置组名
-        set_colors=("#098154","#069af3","#c72e29"),#设置圈的颜色，中间颜色不能修改
-        alpha=0.6,#透明度
-        normalize_to=1.0,#venn图占据figure的比例，1.0为占满
+    g=venn3(subsets = [set(gene_list_lri),set(genelist_lr),set(genelist)], #
+        set_labels = ('SVI genes', "LR genes",'SVG'), #
+        set_colors=("#098154","#069af3","#c72e29"),#
+        alpha=0.6,#
+        normalize_to=1.0,#
        )
     plt.title('Gene Overlap')
     plt.subplot(1, 3, 3)
-    g=venn3(subsets = [set(lri_pw_list),set(gene_lr_list),set(gene_pw_list)], #绘图数据集
-        set_labels = ('SVI genes', "LR genes",'SVG'), #设置组名
-        set_colors=("#098154","#069af3","#c72e29"),#设置圈的颜色，中间颜色不能修改
-        alpha=0.6,#透明度
-        normalize_to=1.0,#venn图占据figure的比例，1.0为占满
+    g=venn3(subsets = [set(lri_pw_list),set(gene_lr_list),set(gene_pw_list)], #
+        set_labels = ('SVI genes', "LR genes",'SVG'), #
+        set_colors=("#098154","#069af3","#c72e29"),#
+        alpha=0.6,#
+        normalize_to=1.0,#
        )
     plt.title('Enriched Pathway Overlap')
     
     merged_df = pd.concat(pathway_dfs)
 
     return merged_df,lri_pw_list,gene_lr_list,gene_pw_list
```

### Comparing `spider-st-0.0.9/spider_st.egg-info/PKG-INFO` & `spider-st-0.1.8/spider_st.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.9
+Version: 0.1.8
 Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.9/spider_st.egg-info/SOURCES.txt` & `spider-st-0.1.8/spider_st.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.cfg
 setup.py
 spider/SPIDER.py
 spider/__init__.py
 spider/clustering.py
 spider/enrichment.py
 spider/preprocess.py
+spider/reconstruction.py
 spider/svi.py
 spider/trajectory.py
 spider/util.py
 spider/version.py
 spider/visualization.py
 spider/R_script/__init__.py
 spider/R_script/run_SPARKX.R
@@ -32,12 +33,14 @@
 spider/SpatialDE/_internal/score_test.py
 spider/SpatialDE/_internal/sm_kernel.py
 spider/SpatialDE/_internal/svca.py
 spider/SpatialDE/_internal/tf_dataset.py
 spider/SpatialDE/_internal/util.py
 spider/SpatialDE/_internal/util_mixture.py
 spider/lrdb/__init__.py
+spider/lrdb/lrpairs.tsv
+spider/lrdb/pathways.tsv
 spider_st.egg-info/PKG-INFO
 spider_st.egg-info/SOURCES.txt
 spider_st.egg-info/dependency_links.txt
 spider_st.egg-info/requires.txt
 spider_st.egg-info/top_level.txt
```

