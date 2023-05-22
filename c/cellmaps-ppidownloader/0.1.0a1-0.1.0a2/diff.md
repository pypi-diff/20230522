# Comparing `tmp/cellmaps_ppidownloader-0.1.0a1.tar.gz` & `tmp/cellmaps_ppidownloader-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_ppidownloader-0.1.0a1.tar", last modified: Mon May 15 16:39:18 2023, max compression
+gzip compressed data, was "dist/cellmaps_ppidownloader-0.1.0a2.tar", last modified: Mon May 22 18:11:37 2023, max compression
```

## Comparing `cellmaps_ppidownloader-0.1.0a1.tar` & `cellmaps_ppidownloader-0.1.0a2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:39:18.789044 cellmaps_ppidownloader-0.1.0a1/
--rw-r--r--   0 churas     (504) staff       (20)      150 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3707 2023-05-05 23:27:01.000000 cellmaps_ppidownloader-0.1.0a1/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-15 16:37:52.000000 cellmaps_ppidownloader-0.1.0a1/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     4933 2023-05-15 16:39:18.789216 cellmaps_ppidownloader-0.1.0a1/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3068 2023-05-15 16:36:17.000000 cellmaps_ppidownloader-0.1.0a1/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:39:18.776610 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader/
--rw-r--r--   0 churas     (504) staff       (20)      298 2023-05-15 16:36:17.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     6214 2023-05-05 23:36:15.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader/cellmaps_ppidownloadercmd.py
--rw-r--r--   0 churas     (504) staff       (20)      141 2023-05-05 22:59:00.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    10646 2023-05-08 16:57:53.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader/gene.py
--rw-r--r--   0 churas     (504) staff       (20)    15012 2023-05-12 21:42:34.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:39:18.778351 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     4933 2023-05-15 16:39:18.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1075 2023-05-15 16:39:18.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-15 16:39:18.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-15 16:39:18.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       50 2023-05-15 16:39:18.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       23 2023-05-15 16:39:18.000000 cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:39:18.786154 cellmaps_ppidownloader-0.1.0a1/docs/
--rw-r--r--   0 churas     (504) staff       (20)      625 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/Makefile
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1029 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/cellmaps_downloader.rst
--rw-r--r--   0 churas     (504) staff       (20)     1027 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/cellmaps_imagedownloader.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6091 2023-05-05 22:59:00.000000 cellmaps_ppidownloader-0.1.0a1/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      292 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      939 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1254 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      472 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       83 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4424 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      739 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a1/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      405 2023-05-15 16:39:18.789781 cellmaps_ppidownloader-0.1.0a1/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1918 2023-05-05 23:27:01.000000 cellmaps_ppidownloader-0.1.0a1/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:39:18.788620 cellmaps_ppidownloader-0.1.0a1/tests/
--rw-r--r--   0 churas     (504) staff       (20)       77 2023-05-05 22:59:00.000000 cellmaps_ppidownloader-0.1.0a1/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1417 2023-05-05 23:17:40.000000 cellmaps_ppidownloader-0.1.0a1/tests/test_cellmaps_ppidownloadercmd.py
--rw-r--r--   0 churas     (504) staff       (20)     2237 2023-05-05 23:17:09.000000 cellmaps_ppidownloader-0.1.0a1/tests/test_genenodegenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     2232 2023-05-05 23:27:01.000000 cellmaps_ppidownloader-0.1.0a1/tests/test_genequery.py
--rw-r--r--   0 churas     (504) staff       (20)      805 2023-05-05 23:27:01.000000 cellmaps_ppidownloader-0.1.0a1/tests/test_integration_cellmaps_downloader.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 18:11:37.579732 cellmaps_ppidownloader-0.1.0a2/
+-rw-r--r--   0 churas     (504) staff       (20)      150 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3707 2023-05-05 23:27:01.000000 cellmaps_ppidownloader-0.1.0a2/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-15 16:37:52.000000 cellmaps_ppidownloader-0.1.0a2/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5367 2023-05-22 18:11:37.579897 cellmaps_ppidownloader-0.1.0a2/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3446 2023-05-16 21:00:25.000000 cellmaps_ppidownloader-0.1.0a2/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 18:11:37.572700 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader/
+-rw-r--r--   0 churas     (504) staff       (20)      298 2023-05-15 18:23:05.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     8317 2023-05-15 18:28:29.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader/cellmaps_ppidownloadercmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      141 2023-05-05 22:59:00.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    11128 2023-05-15 18:29:45.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader/gene.py
+-rw-r--r--   0 churas     (504) staff       (20)    15012 2023-05-12 21:42:34.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 18:11:37.574068 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5367 2023-05-22 18:11:37.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1075 2023-05-22 18:11:37.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 18:11:37.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 18:11:37.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       50 2023-05-22 18:11:37.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       23 2023-05-22 18:11:37.000000 cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 18:11:37.578005 cellmaps_ppidownloader-0.1.0a2/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      625 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/Makefile
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1029 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/cellmaps_downloader.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1027 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/cellmaps_imagedownloader.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6091 2023-05-05 22:59:00.000000 cellmaps_ppidownloader-0.1.0a2/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      292 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      939 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1254 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      472 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       83 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4424 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      739 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-05 22:53:45.000000 cellmaps_ppidownloader-0.1.0a2/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      405 2023-05-22 18:11:37.580745 cellmaps_ppidownloader-0.1.0a2/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1918 2023-05-05 23:27:01.000000 cellmaps_ppidownloader-0.1.0a2/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 18:11:37.579544 cellmaps_ppidownloader-0.1.0a2/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       77 2023-05-05 22:59:00.000000 cellmaps_ppidownloader-0.1.0a2/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1417 2023-05-05 23:17:40.000000 cellmaps_ppidownloader-0.1.0a2/tests/test_cellmaps_ppidownloadercmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     2237 2023-05-05 23:17:09.000000 cellmaps_ppidownloader-0.1.0a2/tests/test_genenodegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     2232 2023-05-05 23:27:01.000000 cellmaps_ppidownloader-0.1.0a2/tests/test_genequery.py
+-rw-r--r--   0 churas     (504) staff       (20)      805 2023-05-05 23:27:01.000000 cellmaps_ppidownloader-0.1.0a2/tests/test_integration_cellmaps_downloader.py
```

### Comparing `cellmaps_ppidownloader-0.1.0a1/CONTRIBUTING.rst` & `cellmaps_ppidownloader-0.1.0a2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/LICENSE` & `cellmaps_ppidownloader-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/PKG-INFO` & `cellmaps_ppidownloader-0.1.0a2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_ppidownloader
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Downloads APMS edgelist data for CM4AI MuSIC pipeline
 Home-page: https://github.com/idekerlab/cellmaps_ppidownloader
 Author: Gege Qian
 Author-email: geqian@ucsd.edu
 License: MIT license
 Description: =========================
         cellmaps_ppidownloader
@@ -96,15 +96,22 @@
         
         **Example usage**
         
         **TODO:** Add information about example usage
         
         .. code-block::
         
-           cellmaps_ppidownloadercmd.py # TODO Add other needed arguments here
+            # Download bioplex 1.0 interaction list and baitlist
+            # curl commands below do just that, but if not installed download
+            # the files from https://bioplex.hms.harvard.edu/interactions.php
+            # via a browser
+            curl -O https://bioplex.hms.harvard.edu/data/BioPlex_interactionList_v2.tsv
+            curl -O https://bioplex.hms.harvard.edu/data/BioPlex_1p0_293T_baitList.tsv
+        
+            cellmaps_ppidownloadercmd.py # TODO Add other needed arguments here
         
         
         Via Docker
         ~~~~~~~~~~~~~~~~~~~~~~
         
         **Example usage**
```

### Comparing `cellmaps_ppidownloader-0.1.0a1/README.rst` & `cellmaps_ppidownloader-0.1.0a2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -88,15 +88,22 @@
 
 **Example usage**
 
 **TODO:** Add information about example usage
 
 .. code-block::
 
-   cellmaps_ppidownloadercmd.py # TODO Add other needed arguments here
+    # Download bioplex 1.0 interaction list and baitlist
+    # curl commands below do just that, but if not installed download
+    # the files from https://bioplex.hms.harvard.edu/interactions.php
+    # via a browser
+    curl -O https://bioplex.hms.harvard.edu/data/BioPlex_interactionList_v2.tsv
+    curl -O https://bioplex.hms.harvard.edu/data/BioPlex_1p0_293T_baitList.tsv
+
+    cellmaps_ppidownloadercmd.py # TODO Add other needed arguments here
 
 
 Via Docker
 ~~~~~~~~~~~~~~~~~~~~~~
 
 **Example usage**
```

### Comparing `cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader/gene.py` & `cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader/gene.py`

 * *Files 5% similar despite different names*

```diff
@@ -158,15 +158,19 @@
         """
         super().__init__()
         self._apms_edgelist = apms_edgelist
         self._apms_baitlist = apms_baitlist
         self._genequery = genequery
 
     @staticmethod
-    def get_apms_edgelist_from_tsvfile(tsvfile=None):
+    def get_apms_edgelist_from_tsvfile(tsvfile=None,
+                                       geneid_one_col='GeneID1',
+                                       symbol_one_col='Symbol1',
+                                       geneid_two_col='GeneID2',
+                                       symbol_two_col='Symbol2'):
         """
         Generates list of dicts by parsing TSV file specified
         by **tsvfile** with the
         format header column and corresponding values:
 
         .. code-block::
 
@@ -184,22 +188,25 @@
                        'Symbol2': VAL}
         :rtype: list
         """
         edgelist = []
         with open(tsvfile, 'r') as f:
             reader = csv.DictReader(f, delimiter='\t')
             for row in reader:
-                edgelist.append({'GeneID1': row['GeneID1'],
-                                 'Symbol1': row['Symbol1'],
-                                 'GeneID2': row['GeneID2'],
-                                 'Symbol2': row['Symbol2']})
+                edgelist.append({'GeneID1': row[geneid_one_col],
+                                 'Symbol1': row[symbol_one_col],
+                                 'GeneID2': row[geneid_two_col],
+                                 'Symbol2': row[symbol_two_col]})
         return edgelist
 
     @staticmethod
-    def get_apms_baitlist_from_tsvfile(tsvfile=None):
+    def get_apms_baitlist_from_tsvfile(tsvfile=None,
+                                       symbol_col='GeneSymbol',
+                                       geneid_col='GeneID',
+                                       numinteractors_col='# Interactors'):
         """
         Generates list of dicts by parsing TSV file specified
         by **tsvfile** with the
         format header column and corresponding values:
 
         .. code-block::
 
@@ -216,17 +223,17 @@
                         'NumIteractors': VAL }
         :rtype: list
         """
         edgelist = []
         with open(tsvfile, 'r') as f:
             reader = csv.DictReader(f, delimiter='\t')
             for row in reader:
-                edgelist.append({'GeneSymbol': row['GeneSymbol'],
-                                 'GeneID': row['GeneID'],
-                                 'NumInteractors': row['# Interactors']})
+                edgelist.append({'GeneSymbol': row[symbol_col],
+                                 'GeneID': row[geneid_col],
+                                 'NumInteractors': row[numinteractors_col]})
         return edgelist
 
     def get_apms_edgelist(self):
         """
         Gets apms edgelist passed in via constructor
 
         :return:
```

### Comparing `cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader/runner.py` & `cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader/runner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/PKG-INFO` & `cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-ppidownloader
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Downloads APMS edgelist data for CM4AI MuSIC pipeline
 Home-page: https://github.com/idekerlab/cellmaps_ppidownloader
 Author: Gege Qian
 Author-email: geqian@ucsd.edu
 License: MIT license
 Description: =========================
         cellmaps_ppidownloader
@@ -96,15 +96,22 @@
         
         **Example usage**
         
         **TODO:** Add information about example usage
         
         .. code-block::
         
-           cellmaps_ppidownloadercmd.py # TODO Add other needed arguments here
+            # Download bioplex 1.0 interaction list and baitlist
+            # curl commands below do just that, but if not installed download
+            # the files from https://bioplex.hms.harvard.edu/interactions.php
+            # via a browser
+            curl -O https://bioplex.hms.harvard.edu/data/BioPlex_interactionList_v2.tsv
+            curl -O https://bioplex.hms.harvard.edu/data/BioPlex_1p0_293T_baitList.tsv
+        
+            cellmaps_ppidownloadercmd.py # TODO Add other needed arguments here
         
         
         Via Docker
         ~~~~~~~~~~~~~~~~~~~~~~
         
         **Example usage**
```

### Comparing `cellmaps_ppidownloader-0.1.0a1/cellmaps_ppidownloader.egg-info/SOURCES.txt` & `cellmaps_ppidownloader-0.1.0a2/cellmaps_ppidownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/Makefile` & `cellmaps_ppidownloader-0.1.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/cellmaps_downloader.rst` & `cellmaps_ppidownloader-0.1.0a2/docs/cellmaps_downloader.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/cellmaps_imagedownloader.rst` & `cellmaps_ppidownloader-0.1.0a2/docs/cellmaps_imagedownloader.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/conf.py` & `cellmaps_ppidownloader-0.1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/index.rst` & `cellmaps_ppidownloader-0.1.0a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/installation.rst` & `cellmaps_ppidownloader-0.1.0a2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/make.bat` & `cellmaps_ppidownloader-0.1.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/newrelease.rst` & `cellmaps_ppidownloader-0.1.0a2/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/pypircfile.rst` & `cellmaps_ppidownloader-0.1.0a2/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/usage.rst` & `cellmaps_ppidownloader-0.1.0a2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/docs/versioningscheme.rst` & `cellmaps_ppidownloader-0.1.0a2/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/setup.py` & `cellmaps_ppidownloader-0.1.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/tests/test_cellmaps_ppidownloadercmd.py` & `cellmaps_ppidownloader-0.1.0a2/tests/test_cellmaps_ppidownloadercmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/tests/test_genenodegenerator.py` & `cellmaps_ppidownloader-0.1.0a2/tests/test_genenodegenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/tests/test_genequery.py` & `cellmaps_ppidownloader-0.1.0a2/tests/test_genequery.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppidownloader-0.1.0a1/tests/test_integration_cellmaps_downloader.py` & `cellmaps_ppidownloader-0.1.0a2/tests/test_integration_cellmaps_downloader.py`

 * *Files identical despite different names*

