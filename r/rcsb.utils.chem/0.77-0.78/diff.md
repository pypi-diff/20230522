# Comparing `tmp/rcsb.utils.chem-0.77.tar.gz` & `tmp/rcsb.utils.chem-0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.chem-0.77.tar", last modified: Tue Jan 10 15:45:14 2023, max compression
+gzip compressed data, was "rcsb.utils.chem-0.78.tar", last modified: Mon May 22 13:49:05 2023, max compression
```

## Comparing `rcsb.utils.chem-0.77.tar` & `rcsb.utils.chem-0.78.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:45:14.266231 rcsb.utils.chem-0.77/
--rw-r--r--   0 vsts      (1001) docker     (122)     5410 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1982 2023-01-10 15:45:14.266231 rcsb.utils.chem-0.77/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1307 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:45:14.262231 rcsb.utils.chem-0.77/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:45:14.262231 rcsb.utils.chem-0.77/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:45:14.266231 rcsb.utils.chem-0.77/rcsb/utils/chem/
--rw-r--r--   0 vsts      (1001) docker     (122)     9130 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/BatchChemSearch.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5041 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/CactvsMoleculeFactory.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10127 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/ChemAxonDescriptorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13794 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompDepictWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13168 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompIndexProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7905 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompMoleculeProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16533 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompSearchIndexProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    27265 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompSearchWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    96737 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/FailList.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5204 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/IoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2721 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/MolecularFormula.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13176 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/MoleculeAnnotationsCompare.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5106 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/ObMoleculeFactory.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22814 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeAlignUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15861 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeChemCompUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3861 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeCommonUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9851 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeDepict.py
--rw-r--r--   0 vsts      (1001) docker     (122)    49180 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeDepictAlign.py
--rw-r--r--   0 vsts      (1001) docker     (122)    31812 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    50250 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeMoleculeFactory.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10831 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeMoleculeProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11322 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeSearchMoleculeProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12387 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/OeSubStructSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15773 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/PdbxChemComp.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1959 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/PdbxChemCompConstants.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6738 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/RdMoleculeFactory.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3964 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/rcsb/utils/chem/cactvsAnnotateMol.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:45:14.262231 rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1982 2023-01-10 15:45:14.000000 rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1460 2023-01-10 15:45:14.000000 rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-10 15:45:14.000000 rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       79 2023-01-10 15:45:14.000000 rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-10 15:45:11.000000 rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-01-10 15:45:14.000000 rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-01-10 15:45:14.000000 rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      185 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-01-10 15:45:14.266231 rcsb.utils.chem-0.77/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2397 2023-01-10 15:32:56.000000 rcsb.utils.chem-0.77/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:49:05.396345 rcsb.utils.chem-0.78/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5456 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1982 2023-05-22 13:49:05.396345 rcsb.utils.chem-0.78/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1307 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:49:05.392345 rcsb.utils.chem-0.78/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:49:05.392345 rcsb.utils.chem-0.78/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:49:05.396345 rcsb.utils.chem-0.78/rcsb/utils/chem/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9130 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/BatchChemSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5041 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/CactvsMoleculeFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10127 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/ChemAxonDescriptorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13794 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompDepictWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13168 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompIndexProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7909 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompMoleculeProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16533 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompSearchIndexProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    27265 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompSearchWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    96737 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/FailList.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5204 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/IoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2721 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/MolecularFormula.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13176 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/MoleculeAnnotationsCompare.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5106 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/ObMoleculeFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22814 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeAlignUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15861 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeChemCompUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3861 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeCommonUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9851 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    49180 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeDepictAlign.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    31812 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    50250 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeMoleculeFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10831 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeMoleculeProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11322 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeSearchMoleculeProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12387 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/OeSubStructSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15773 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/PdbxChemComp.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1959 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/PdbxChemCompConstants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6738 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/RdMoleculeFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3964 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/rcsb/utils/chem/cactvsAnnotateMol.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:49:05.392345 rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1982 2023-05-22 13:49:05.000000 rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1460 2023-05-22 13:49:05.000000 rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:49:05.000000 rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       79 2023-05-22 13:49:05.000000 rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:49:04.000000 rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-05-22 13:49:05.000000 rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-22 13:49:05.000000 rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      185 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-22 13:49:05.396345 rcsb.utils.chem-0.78/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2397 2023-05-22 13:37:07.000000 rcsb.utils.chem-0.78/setup.py
```

### Comparing `rcsb.utils.chem-0.77/HISTORY.txt` & `rcsb.utils.chem-0.78/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,8 +61,9 @@
 13-Mar-2021 - V0.70 Change to multi-process timeout decorator with variable timeout settings.
  5-May-2021 - V0.71 Update dependencies
  9-Jun-2021 - V0.72 Update installation tools and add diagnostic output for fingerprint score results
  9-Jun-2021 - V0.73 Update manifest files
 22-Aug-2021 - V0.74 Add ChemAxonDescriptorProvider and associated tests.  Add ChemAxon smiles to search index build.
 26-Aug-2021 - V0.75 Add filter for obsolete definitions in ChemCompMoleculeProvider and ChemCompSearchIndexProvider modules
 23-Sep-2021 - V0.76 Set default for skipObsolete to True
- 9-Jan-2023 - V0.77 Configuration changes to support tox 4
+ 9-Jan-2023 - V0.77 Configuration changes to support tox 4
+19-May-2023 - V0.78 Update DNS to PDB archive
```

### Comparing `rcsb.utils.chem-0.77/LICENSE` & `rcsb.utils.chem-0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/PKG-INFO` & `rcsb.utils.chem-0.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chem
-Version: 0.77
+Version: 0.78
 Summary: RCSB Python Chemical Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chem
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chem-0.77/README.md` & `rcsb.utils.chem-0.78/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/BatchChemSearch.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/BatchChemSearch.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/CactvsMoleculeFactory.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/CactvsMoleculeFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/ChemAxonDescriptorProvider.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/ChemAxonDescriptorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompDepictWrapper.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompDepictWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompIndexProvider.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompIndexProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompMoleculeProvider.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompMoleculeProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 class ChemCompMoleculeProvider(object):
     """Utilities to read and serialize the dictionary of PDBx/mmCIF chemical component definitions."""
 
     def __init__(self, **kwargs):
         # Default source target locators
         self.__ccUrlTarget = kwargs.get("ccUrlTarget", None)
-        self.__ccUrlTarget = self.__ccUrlTarget if self.__ccUrlTarget else "http://ftp.wwpdb.org/pub/pdb/data/monomers/components.cif.gz"
+        self.__ccUrlTarget = self.__ccUrlTarget if self.__ccUrlTarget else "http://files.wwpdb.org/pub/pdb/data/monomers/components.cif.gz"
         self.__birdUrlTarget = kwargs.get("birdUrlTarget", None)
-        self.__birdUrlTarget = self.__birdUrlTarget if self.__birdUrlTarget else "http://ftp.wwpdb.org/pub/pdb/data/bird/prd/prdcc-all.cif.gz"
+        self.__birdUrlTarget = self.__birdUrlTarget if self.__birdUrlTarget else "http://files.wwpdb.org/pub/pdb/data/bird/prd/prdcc-all.cif.gz"
         #
         ccFileNamePrefix = kwargs.get("ccFileNamePrefix", "cc")
         cachePath = kwargs.get("cachePath", ".")
         dirPath = os.path.join(cachePath, "chem_comp")
         useCache = kwargs.get("useCache", True)
         molLimit = kwargs.get("molLimit", 0)
         skipObsolete = kwargs.get("skipObsolete", True)
```

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompSearchIndexProvider.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompSearchIndexProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/ChemCompSearchWrapper.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/ChemCompSearchWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/FailList.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/FailList.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/IoUtils.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/IoUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/MolecularFormula.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/MolecularFormula.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/MoleculeAnnotationsCompare.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/MoleculeAnnotationsCompare.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/ObMoleculeFactory.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/ObMoleculeFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeAlignUtils.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeAlignUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeChemCompUtils.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeChemCompUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeCommonUtils.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeCommonUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeDepict.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeDepict.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeDepictAlign.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeDepictAlign.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeIoUtils.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeIoUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeMoleculeFactory.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeMoleculeFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeMoleculeProvider.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeMoleculeProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeSearchMoleculeProvider.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeSearchMoleculeProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeSearchUtils.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeSearchUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/OeSubStructSearchUtils.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/OeSubStructSearchUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/PdbxChemComp.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/PdbxChemComp.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/PdbxChemCompConstants.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/PdbxChemCompConstants.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/RdMoleculeFactory.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/RdMoleculeFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb/utils/chem/cactvsAnnotateMol.py` & `rcsb.utils.chem-0.78/rcsb/utils/chem/cactvsAnnotateMol.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/PKG-INFO` & `rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chem
-Version: 0.77
+Version: 0.78
 Summary: RCSB Python Chemical Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chem
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chem-0.77/rcsb.utils.chem.egg-info/SOURCES.txt` & `rcsb.utils.chem-0.78/rcsb.utils.chem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.77/setup.py` & `rcsb.utils.chem-0.78/setup.py`

 * *Files identical despite different names*

