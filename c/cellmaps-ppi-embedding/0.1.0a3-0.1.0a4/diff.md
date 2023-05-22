# Comparing `tmp/cellmaps_ppi_embedding-0.1.0a3.tar.gz` & `tmp/cellmaps_ppi_embedding-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_ppi_embedding-0.1.0a3.tar", last modified: Sat May 20 00:06:46 2023, max compression
+gzip compressed data, was "dist/cellmaps_ppi_embedding-0.1.0a4.tar", last modified: Mon May 22 19:40:12 2023, max compression
```

## Comparing `cellmaps_ppi_embedding-0.1.0a3.tar` & `cellmaps_ppi_embedding-0.1.0a4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.011741 cellmaps_ppi_embedding-0.1.0a3/
--rw-r--r--   0 churas     (504) staff       (20)      192 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a3/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3707 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a3/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-20 00:06:46.011869 cellmaps_ppi_embedding-0.1.0a3/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3743 2023-05-15 16:46:17.000000 cellmaps_ppi_embedding-0.1.0a3/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.005870 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/
--rw-r--r--   0 churas     (504) staff       (20)      296 2023-05-19 23:36:32.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     4915 2023-05-20 00:05:39.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      139 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    10725 2023-05-20 00:04:55.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.007478 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      981 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       23 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.010694 cellmaps_ppi_embedding-0.1.0a3/docs/
--rw-r--r--   0 churas     (504) staff       (20)      623 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/Makefile
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/authors.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6093 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a3/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      290 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      972 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1238 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      470 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      820 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       81 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4400 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      792 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      725 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      405 2023-05-20 00:06:46.012305 cellmaps_ppi_embedding-0.1.0a3/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1860 2023-05-15 16:48:06.000000 cellmaps_ppi_embedding-0.1.0a3/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.011561 cellmaps_ppi_embedding-0.1.0a3/tests/
--rw-r--r--   0 churas     (504) staff       (20)       77 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1897 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/tests/test_cellmaps_network_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     2804 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/tests/test_cellmapsnetworkembeddingrunner.py
--rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/tests/test_integration_cellmaps_network_embedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.765277 cellmaps_ppi_embedding-0.1.0a4/
+-rw-r--r--   0 churas     (504) staff       (20)      192 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a4/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3707 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a4/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-22 19:40:12.765393 cellmaps_ppi_embedding-0.1.0a4/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3743 2023-05-15 16:46:17.000000 cellmaps_ppi_embedding-0.1.0a4/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.758388 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/
+-rw-r--r--   0 churas     (504) staff       (20)      296 2023-05-22 19:36:45.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     4915 2023-05-20 00:05:39.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      139 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    10746 2023-05-22 19:36:34.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.760033 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)      981 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       23 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.764219 cellmaps_ppi_embedding-0.1.0a4/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      623 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/Makefile
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/authors.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6093 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a4/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      290 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      972 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1238 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      470 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      820 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       81 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4400 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      792 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      725 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      405 2023-05-22 19:40:12.765815 cellmaps_ppi_embedding-0.1.0a4/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1860 2023-05-15 16:48:06.000000 cellmaps_ppi_embedding-0.1.0a4/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.765100 cellmaps_ppi_embedding-0.1.0a4/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       77 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1897 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/tests/test_cellmaps_network_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     2804 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/tests/test_cellmapsnetworkembeddingrunner.py
+-rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/tests/test_integration_cellmaps_network_embedding.py
```

### Comparing `cellmaps_ppi_embedding-0.1.0a3/CONTRIBUTING.rst` & `cellmaps_ppi_embedding-0.1.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/LICENSE` & `cellmaps_ppi_embedding-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/PKG-INFO` & `cellmaps_ppi_embedding-0.1.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_ppi_embedding
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A tool to generate embeddings from networks for CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_ppi_embedding
 Author: Mayank Jain
 Author-email: maj014@ucsd.edu
 License: MIT license
 Description: ==========================
         cellmaps_ppi_embedding
```

### Comparing `cellmaps_ppi_embedding-0.1.0a3/README.rst` & `cellmaps_ppi_embedding-0.1.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py` & `cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/runner.py` & `cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         """
         logger.debug('Getting id of input rocrate')
         input_dataset_id = self._provenance_utils.get_id_of_rocrate(self._inputdir)
 
         logger.debug('Registering computation with FAIRSCAPE')
         self._provenance_utils.register_computation(self._outdir,
                                                     name=cellmaps_ppi_embedding.__name__,
-                                                    run_by=str(os.getlogin()),
+                                                    run_by=str(self._provenance_utils.get_login()),
                                                     command=str(self._input_data_dict),
                                                     description='run of ' + cellmaps_ppi_embedding.__name__,
                                                     used_software=[self._softwareid],
                                                     used_dataset=[input_dataset_id],
                                                     generated=[self._embedding_file_id])
 
     def _register_embedding_file(self):
```

### Comparing `cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/PKG-INFO` & `cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-ppi-embedding
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A tool to generate embeddings from networks for CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_ppi_embedding
 Author: Mayank Jain
 Author-email: maj014@ucsd.edu
 License: MIT license
 Description: ==========================
         cellmaps_ppi_embedding
```

### Comparing `cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/SOURCES.txt` & `cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/Makefile` & `cellmaps_ppi_embedding-0.1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/conf.py` & `cellmaps_ppi_embedding-0.1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/index.rst` & `cellmaps_ppi_embedding-0.1.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/installation.rst` & `cellmaps_ppi_embedding-0.1.0a4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/make.bat` & `cellmaps_ppi_embedding-0.1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/newrelease.rst` & `cellmaps_ppi_embedding-0.1.0a4/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/pypircfile.rst` & `cellmaps_ppi_embedding-0.1.0a4/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/usage.rst` & `cellmaps_ppi_embedding-0.1.0a4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/docs/versioningscheme.rst` & `cellmaps_ppi_embedding-0.1.0a4/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/setup.py` & `cellmaps_ppi_embedding-0.1.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/tests/test_cellmaps_network_embeddingcmd.py` & `cellmaps_ppi_embedding-0.1.0a4/tests/test_cellmaps_network_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/tests/test_cellmapsnetworkembeddingrunner.py` & `cellmaps_ppi_embedding-0.1.0a4/tests/test_cellmapsnetworkembeddingrunner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a3/tests/test_integration_cellmaps_network_embedding.py` & `cellmaps_ppi_embedding-0.1.0a4/tests/test_integration_cellmaps_network_embedding.py`

 * *Files identical despite different names*

