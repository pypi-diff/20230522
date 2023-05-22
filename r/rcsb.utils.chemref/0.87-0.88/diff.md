# Comparing `tmp/rcsb.utils.chemref-0.87.tar.gz` & `tmp/rcsb.utils.chemref-0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.chemref-0.87.tar", last modified: Wed Apr 19 15:16:43 2023, max compression
+gzip compressed data, was "rcsb.utils.chemref-0.88.tar", last modified: Mon May 22 13:46:14 2023, max compression
```

## Comparing `rcsb.utils.chemref-0.87.tar` & `rcsb.utils.chemref-0.88.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.929126 rcsb.utils.chemref-0.87/
--rw-r--r--   0 vsts      (1001) docker     (122)     5519 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-04-19 15:16:43.929126 rcsb.utils.chemref-0.87/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1034 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.925126 rcsb.utils.chemref-0.87/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.925126 rcsb.utils.chemref-0.87/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.929126 rcsb.utils.chemref-0.87/rcsb/utils/chemref/
--rw-r--r--   0 vsts      (1001) docker     (122)    10179 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/AtcProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6623 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/BirdProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/CARDProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4726 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/CODProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12549 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChEMBLProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7747 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChemCompModelProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9066 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChemCompProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16161 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugBankProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9477 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugBankReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugCentralProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PharosProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2509 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PharosReadSqlDump.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7494 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PsiModProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4060 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PubChemProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    54562 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PubChemUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6478 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/RcsbLigandScoreProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6669 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ResidProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1586 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ResidReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.925126 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-19 15:09:29.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      197 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-19 15:16:43.929126 rcsb.utils.chemref-0.87/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2227 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.064298 rcsb.utils.chemref-0.88/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5567 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-05-22 13:46:14.064298 rcsb.utils.chemref-0.88/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1034 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.060297 rcsb.utils.chemref-0.88/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.060297 rcsb.utils.chemref-0.88/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.064298 rcsb.utils.chemref-0.88/rcsb/utils/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10179 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/AtcProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6625 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/BirdProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/CARDProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4726 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/CODProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12549 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChEMBLProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7749 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChemCompModelProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9068 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChemCompProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16161 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugBankProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9477 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugBankReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugCentralProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PharosProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2509 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PharosReadSqlDump.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7494 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PsiModProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4060 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PubChemProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    54562 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PubChemUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6478 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/RcsbLigandScoreProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6669 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ResidProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1586 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ResidReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.060297 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:37:28.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      197 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-05-22 13:36:41.000000 rcsb.utils.chemref-0.88/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-22 13:46:14.064298 rcsb.utils.chemref-0.88/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2227 2023-05-22 13:36:41.000000 rcsb.utils.chemref-0.88/setup.py
```

### Comparing `rcsb.utils.chemref-0.87/HISTORY.txt` & `rcsb.utils.chemref-0.88/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -73,7 +73,8 @@
   3-Jan-2022  - V0.81 Update AtcProvider data loading methods to address recent changes in source NCBO ATC files
  28-Mar-2022  - V0.82 Fix pylint issue with "Iterated dict modified inside for loop body" in testChemCompProvider
  25-Jul-2022  - V0.83 Revert last change to AtcProvider - source NCBO ATC files were updated again to restore previous format
  27-Jul-2022  - V0.84 Adapt to multiple possible naming schemes for ATC class IDs
   9-Jan-2023  - V0.85 Configuration changes to support tox 4
  22-Mar-2023  - V0.86 Update references to py-rcsb_exdb_assets master branch
  19-Apr-2023  - V0.87 Update file path in ATCProvider
+ 19-May-2023  - V0.88 Update DNS to PDB archive
```

### Comparing `rcsb.utils.chemref-0.87/LICENSE` & `rcsb.utils.chemref-0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/PKG-INFO` & `rcsb.utils.chemref-0.88/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chemref
-Version: 0.87
+Version: 0.88
 Summary: RCSB Python Chemical Reference Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chemref
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chemref-0.87/README.md` & `rcsb.utils.chemref-0.88/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/AtcProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/AtcProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/BirdProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/BirdProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def __init__(self, **kwargs):
         dirName = "bird"
         cachePath = kwargs.get("cachePath", ".")
         super(BirdProvider, self).__init__(cachePath, [dirName])
 
         # Default source target locators
         self.__birdUrlTarget = kwargs.get("birdUrlTarget", None)
-        self.__birdUrlTarget = self.__birdUrlTarget if self.__birdUrlTarget else "http://ftp.wwpdb.org/pub/pdb/data/bird/prd/prd-all.cif.gz"
+        self.__birdUrlTarget = self.__birdUrlTarget if self.__birdUrlTarget else "http://files.wwpdb.org/pub/pdb/data/bird/prd/prd-all.cif.gz"
         #
         dirPath = os.path.join(cachePath, dirName)
         useCache = kwargs.get("useCache", True)
         molLimit = kwargs.get("molLimit", 0)
         #
         self.__mU = MarshalUtil(workPath=dirPath)
         self.__birdD = self.__reload(self.__birdUrlTarget, dirPath, useCache=useCache, molLimit=molLimit)
```

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/CARDProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/CARDProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/CODProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/CODProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChEMBLProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChEMBLProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChemCompModelProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChemCompModelProvider.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
 
     def __init__(self, **kwargs):
         dirName = "chem_comp_model"
         cachePath = kwargs.get("cachePath", ".")
         super(ChemCompModelProvider, self).__init__(cachePath, [dirName])
 
-        urlTarget = kwargs.get("urlTarget", "http://ftp.wwpdb.org/pub/pdb/data/component-models/complete/chem_comp_model.cif.gz")
+        urlTarget = kwargs.get("urlTarget", "http://files.wwpdb.org/pub/pdb/data/component-models/complete/chem_comp_model.cif.gz")
         dirPath = os.path.join(cachePath, dirName)
         useCache = kwargs.get("useCache", True)
         mappingFileName = kwargs.get("mappingFileName", "ccdc_pdb_mapping.json")
         auditFileName = kwargs.get("mappingFileName", "ccdc_model_audit.json")
         #
         self.__mU = MarshalUtil(workPath=dirPath)
         self.__mappingD, self.__auditD = self.__reload(urlTarget, dirPath, mappingFileName, auditFileName, useCache=useCache)
```

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChemCompProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChemCompProvider.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """Utilities to provide essential data items for chemical component definitions."""
 
     def __init__(self, **kwargs):
         dirName = "chem_comp"
         cachePath = kwargs.get("cachePath", ".")
         super(ChemCompProvider, self).__init__(cachePath, [dirName])
         #
-        urlTarget = kwargs.get("ccUrlTarget", "http://ftp.wwpdb.org/pub/pdb/data/monomers/components.cif.gz")
+        urlTarget = kwargs.get("ccUrlTarget", "http://files.wwpdb.org/pub/pdb/data/monomers/components.cif.gz")
         # self.__birdUrlTarget = kwargs.get("birdUrlTarget", "ftp://ftp.wwpdb.org/pub/pdb/data/bird/prd/prdcc-all.cif.gz")
         #
         dirPath = os.path.join(cachePath, dirName)
         useCache = kwargs.get("useCache", True)
         ccdFileName = kwargs.get("ccdFileName", "ccd_abbridged_definitions.json")
         #
         self.__mU = MarshalUtil(workPath=dirPath)
```

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugBankProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugBankProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugBankReader.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugBankReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugCentralProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugCentralProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PharosProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PharosProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PharosReadSqlDump.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PharosReadSqlDump.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PsiModProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PsiModProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PubChemProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PubChemProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PubChemUtils.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PubChemUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/RcsbLigandScoreProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/RcsbLigandScoreProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ResidProvider.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ResidProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ResidReader.py` & `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ResidReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/PKG-INFO` & `rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chemref
-Version: 0.87
+Version: 0.88
 Summary: RCSB Python Chemical Reference Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chemref
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/SOURCES.txt` & `rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.87/setup.py` & `rcsb.utils.chemref-0.88/setup.py`

 * *Files identical despite different names*

