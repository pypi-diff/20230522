# Comparing `tmp/rcsb.utils.repository-0.39.tar.gz` & `tmp/rcsb.utils.repository-0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.repository-0.39.tar", last modified: Wed Mar 22 20:10:07 2023, max compression
+gzip compressed data, was "rcsb.utils.repository-0.40.tar", last modified: Mon May 22 13:48:37 2023, max compression
```

## Comparing `rcsb.utils.repository-0.39.tar` & `rcsb.utils.repository-0.40.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:10:07.136918 rcsb.utils.repository-0.39/
--rw-r--r--   0 vsts      (1001) docker     (122)     3033 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      114 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-03-22 20:10:07.136918 rcsb.utils.repository-0.39/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1242 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:10:07.132918 rcsb.utils.repository-0.39/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:10:07.136918 rcsb.utils.repository-0.39/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:10:07.136918 rcsb.utils.repository-0.39/rcsb/utils/repository/
--rw-r--r--   0 vsts      (1001) docker     (122)    14686 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/utils/repository/CurrentHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15454 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/utils/repository/RemovedHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    64927 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/utils/repository/RepositoryProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19042 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/utils/repository/ScanRepoUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5416 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/utils/repository/UnreleasedHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4109 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/utils/repository/UpdateHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/rcsb/utils/repository/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:10:07.136918 rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-03-22 20:10:07.000000 rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      699 2023-03-22 20:10:07.000000 rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 20:10:07.000000 rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 20:10:05.000000 rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-03-22 20:10:07.000000 rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-03-22 20:10:07.000000 rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-03-22 20:10:07.136918 rcsb.utils.repository-0.39/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2236 2023-03-22 20:02:28.000000 rcsb.utils.repository-0.39/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.645387 rcsb.utils.repository-0.40/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3079 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      114 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-05-22 13:48:37.645387 rcsb.utils.repository-0.40/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1242 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.641387 rcsb.utils.repository-0.40/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.641387 rcsb.utils.repository-0.40/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.645387 rcsb.utils.repository-0.40/rcsb/utils/repository/
+-rw-r--r--   0 vsts      (1001) docker     (122)    14690 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/CurrentHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15458 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/RemovedHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    64933 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/RepositoryProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19042 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/ScanRepoUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5420 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/UnreleasedHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/UpdateHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.641387 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      699 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:48:36.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-22 13:48:37.645387 rcsb.utils.repository-0.40/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2236 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/setup.py
```

### Comparing `rcsb.utils.repository-0.39/HISTORY.txt` & `rcsb.utils.repository-0.40/HISTORY.txt`

 * *Files 3% similar despite different names*

```diff
@@ -29,7 +29,8 @@
 13-Apr-2022 - V0.34 Update RepositoryProvider methods for obtaining list of computed-model files;
                     Update getSupersededBy method to recursively return all superseded entries
 20-Apr-2022 - V0.35 Fix issue in RepositoryProvider for mapping source and internal computed-model IDs
 03-Aug-2022 - V0.36 Enable retrieval of specific model files with input
 23-Dec-2022 - V0.37 Configuration changes to support tox 4
 14-Feb-2023 - V0.38 Add support for requesting specific inputIdCodeList/idCodeList for CSMs
 22-Mar-2023 - V0.39 Update references to py-rcsb_exdb_assets master branch
+19-May-2023 - V0.40 Update DNS to PDB archive
```

### Comparing `rcsb.utils.repository-0.39/LICENSE` & `rcsb.utils.repository-0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.39/PKG-INFO` & `rcsb.utils.repository-0.40/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.repository
-Version: 0.39
+Version: 0.40
 Summary: RCSB Python Repository Data Management Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_repository
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.repository-0.39/README.md` & `rcsb.utils.repository-0.40/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.39/rcsb/utils/repository/CurrentHoldingsProvider.py` & `rcsb.utils.repository-0.40/rcsb/utils/repository/CurrentHoldingsProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     def __init__(self, cachePath, useCache, **kwargs):
         self.__cachePath = cachePath
         self.__dirPath = os.path.join(cachePath, "holdings")
         #
         edMapsLocator = kwargs.get("edmapsLocator", "https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/fall_back/edmaps.json")
         #
-        baseUrl = kwargs.get("holdingsTargetUrl", "https://ftp.wwpdb.org/pub/pdb/holdings")
-        fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://ftp.wwpdb.org/pub/pdb/holdings")
+        baseUrl = kwargs.get("holdingsTargetUrl", "https://files.wwpdb.org/pub/pdb/holdings")
+        fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://files.wwpdb.org/pub/pdb/holdings")
         #
         entryUrlContent = os.path.join(baseUrl, "current_file_holdings.json.gz")
         entryUrlFallbackContent = os.path.join(fallbackUrl, "current_file_holdings.json.gz")
         entryUrlIds = os.path.join(baseUrl, "released_structures_last_modified_dates.json.gz")
         entryUrlFallbackIds = os.path.join(fallbackUrl, "released_structures_last_modified_dates.json.gz")
         #
         refdataUrlIds = os.path.join(baseUrl, "refdata_id_list.json.gz")
```

### Comparing `rcsb.utils.repository-0.39/rcsb/utils/repository/RemovedHoldingsProvider.py` & `rcsb.utils.repository-0.40/rcsb/utils/repository/RemovedHoldingsProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     """Provide an inventory of removed repository content."""
 
     def __init__(self, cachePath, useCache, **kwargs):
         self.__cachePath = cachePath
         self.__dirPath = os.path.join(self.__cachePath, "holdings")
         self.__filterType = kwargs.get("filterType", "")
         self.__assignDates = "assign-dates" in self.__filterType
-        baseUrl = kwargs.get("holdingsTargetUrl", "https://ftp.wwpdb.org/pub/pdb/holdings")
-        fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://ftp.wwpdb.org/pub/pdb/holdings")
+        baseUrl = kwargs.get("holdingsTargetUrl", "https://files.wwpdb.org/pub/pdb/holdings")
+        fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://files.wwpdb.org/pub/pdb/holdings")
         #
         urlTarget = os.path.join(baseUrl, "all_removed_entries.json.gz")
         urlFallbackTarget = os.path.join(fallbackUrl, "all_removed_entries.json.gz")
         #
         self.__mU = MarshalUtil(workPath=self.__dirPath)
         self.__invD = self.__reload(urlTarget, urlFallbackTarget, self.__dirPath, useCache=useCache)
```

### Comparing `rcsb.utils.repository-0.39/rcsb/utils/repository/RepositoryProvider.py` & `rcsb.utils.repository-0.40/rcsb/utils/repository/RepositoryProvider.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         self.__fileLimit = fileLimit
         self.__numProc = numProc
         self.__verbose = verbose
         self.__cfgOb = cfgOb
         self.__configName = self.__cfgOb.getDefaultSectionName()
         #
         self.__discoveryMode = discoveryMode if discoveryMode else self.__cfgOb.get("DISCOVERY_MODE", sectionName=self.__configName, default="local")
-        self.__baseUrlPDB = self.__cfgOb.getPath("PDB_REPO_URL", sectionName=self.__configName, default="https://ftp.wwpdb.org/pub")
-        self.__fallbackUrlPDB = self.__cfgOb.getPath("PDB_REPO_FALLBACK_URL", sectionName=self.__configName, default="https://ftp.wwpdb.org/pub")
+        self.__baseUrlPDB = self.__cfgOb.getPath("PDB_REPO_URL", sectionName=self.__configName, default="https://files.wwpdb.org/pub")
+        self.__fallbackUrlPDB = self.__cfgOb.getPath("PDB_REPO_FALLBACK_URL", sectionName=self.__configName, default="https://files.wwpdb.org/pub")
         self.__baseUrlPDBDev = self.__cfgOb.getPath("PDBDEV_REPO_URL", sectionName=self.__configName, default="https://pdb-dev.wwpdb.org")
         self.__edMapUrl = self.__cfgOb.getPath("RCSB_EDMAP_LIST_PATH", sectionName=self.__configName, default=None)
         #
         self.__kwD = {
             "holdingsTargetUrl": os.path.join(self.__baseUrlPDB, "pdb", "holdings"),
             "holdingsFallbackUrl": os.path.join(self.__fallbackUrlPDB, "pdb", "holdings"),
             "edmapsLocator": self.__edMapUrl,
@@ -443,15 +443,15 @@
                 uri = os.path.join(self.__baseUrlPDB, "pdb", "refdata", "chem_comp", idCode[-1], idCode, idCode + ".cif")
             #
             elif contentType in ["pdbx", "pdbx_core"]:
                 # pdb/data/structures/divided/mmCIF
                 uri = os.path.join(self.__baseUrlPDB, "pdb", "data", "structures", "divided", "mmCIF", idCodel[1:3], idCodel + ".cif.gz")
             elif contentType in ["vrpt", "validation_report"]:
                 # /pdb/validation_reports/
-                # https://ftp.wwpdb.org/pub/pdb/validation_reports/00/100d/100d_validation.xml.gz
+                # https://files.wwpdb.org/pub/pdb/validation_reports/00/100d/100d_validation.xml.gz
                 uri = os.path.join(self.__baseUrlPDB, "pdb", "validation_reports", idCodel[1:3], idCodel, idCodel + "_validation.xml.gz")
                 # logger.info("uri %r", uri)
             #
             elif contentType in ["pdbx_obsolete"]:
                 # pdb/data/structures/obsolete/mmCIF/
                 uri = os.path.join(self.__baseUrlPDB, "pdb", "data", "structures", "obsolete", "mmCIF", idCodel[1:3], idCodel + ".cif.gz")
             elif contentType in ["bird_consolidated", "bird_chem_comp_core"]:
```

### Comparing `rcsb.utils.repository-0.39/rcsb/utils/repository/ScanRepoUtil.py` & `rcsb.utils.repository-0.40/rcsb/utils/repository/ScanRepoUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.39/rcsb/utils/repository/UnreleasedHoldingsProvider.py` & `rcsb.utils.repository-0.40/rcsb/utils/repository/UnreleasedHoldingsProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 class UnreleasedHoldingsProvider(object):
     """Provide an inventory of unreleased repository content."""
 
     def __init__(self, cachePath, useCache, **kwargs):
         self.__dirPath = os.path.join(cachePath, "holdings")
         self.__filterType = kwargs.get("filterType", "")
         self.__assignDates = "assign-dates" in self.__filterType
-        baseUrl = kwargs.get("holdingsTargetUrl", "https://ftp.wwpdb.org/pub/pdb/holdings")
-        fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://ftp.wwpdb.org/pub/pdb/holdings")
+        baseUrl = kwargs.get("holdingsTargetUrl", "https://files.wwpdb.org/pub/pdb/holdings")
+        fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://files.wwpdb.org/pub/pdb/holdings")
         #
         urlTarget = os.path.join(baseUrl, "unreleased_entries.json.gz")
         urlFallbackTarget = os.path.join(fallbackUrl, "unreleased_entries.json.gz")
         #
         self.__mU = MarshalUtil(workPath=self.__dirPath)
         self.__invD = self.__reload(urlTarget, urlFallbackTarget, self.__dirPath, useCache=useCache)
```

### Comparing `rcsb.utils.repository-0.39/rcsb/utils/repository/UpdateHoldingsProvider.py` & `rcsb.utils.repository-0.40/rcsb/utils/repository/UpdateHoldingsProvider.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 class UpdateHoldingsProvider(object):
     """Provide inventory of the current repository update."""
 
     def __init__(self, cachePath, useCache, **kwargs):
         self.__dirPath = os.path.join(cachePath, "holdings")
         #
-        baseUrl = kwargs.get("updateTargetUrl", "https://ftp.wwpdb.org/pub/pdb/data/status/latest")
-        fallbackUrl = kwargs.get("updateFallbackUrl", "https://ftp.wwpdb.org/pub/pdb/data/status/latest")
+        baseUrl = kwargs.get("updateTargetUrl", "https://files.wwpdb.org/pub/pdb/data/status/latest")
+        fallbackUrl = kwargs.get("updateFallbackUrl", "https://files.wwpdb.org/pub/pdb/data/status/latest")
         #
         self.__mU = MarshalUtil(workPath=self.__dirPath)
         self.__updD = self.__reloadUpdateLists(baseUrl, fallbackUrl, self.__dirPath, useCache=useCache)
 
     def testCache(self, minCount=100):
         logger.info("Length update updD (%d)", len(self.__updD) if self.__updD else 0)
         if self.__updD and len(self.__updD) > minCount:
```

### Comparing `rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/PKG-INFO` & `rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.repository
-Version: 0.39
+Version: 0.40
 Summary: RCSB Python Repository Data Management Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_repository
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.repository-0.39/rcsb.utils.repository.egg-info/SOURCES.txt` & `rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.39/setup.py` & `rcsb.utils.repository-0.40/setup.py`

 * *Files identical despite different names*

