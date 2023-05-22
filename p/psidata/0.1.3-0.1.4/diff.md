# Comparing `tmp/psidata-0.1.3.tar.gz` & `tmp/psidata-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psidata-0.1.3.tar", last modified: Mon May  8 16:11:15 2023, max compression
+gzip compressed data, was "psidata-0.1.4.tar", last modified: Mon May 22 21:43:29 2023, max compression
```

## Comparing `psidata-0.1.3.tar` & `psidata-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.317857 psidata-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.309857 psidata-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.313857 psidata-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-08 16:11:02.000000 psidata-0.1.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-08 16:11:02.000000 psidata-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 16:11:02.000000 psidata-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-08 16:11:15.317857 psidata-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 16:11:02.000000 psidata-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.313857 psidata-0.1.3/psidata/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/bcolz_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/legacy_bcolz_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/zarr_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.317857 psidata-0.1.3/psidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-08 16:11:02.000000 psidata-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:11:15.317857 psidata-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:43:29.214846 psidata-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:43:29.214846 psidata-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:43:29.214846 psidata-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-22 21:43:19.000000 psidata-0.1.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-22 21:43:19.000000 psidata-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-22 21:43:19.000000 psidata-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-22 21:43:29.214846 psidata-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-22 21:43:19.000000 psidata-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:43:29.214846 psidata-0.1.4/psidata/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-22 21:43:19.000000 psidata-0.1.4/psidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-22 21:43:19.000000 psidata-0.1.4/psidata/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-22 21:43:19.000000 psidata-0.1.4/psidata/bcolz_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-22 21:43:19.000000 psidata-0.1.4/psidata/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-22 21:43:19.000000 psidata-0.1.4/psidata/legacy_bcolz_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-22 21:43:19.000000 psidata-0.1.4/psidata/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-22 21:43:19.000000 psidata-0.1.4/psidata/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 21:43:29.000000 psidata-0.1.4/psidata/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-22 21:43:19.000000 psidata-0.1.4/psidata/zarr_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:43:29.214846 psidata-0.1.4/psidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-22 21:43:29.000000 psidata-0.1.4/psidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-22 21:43:29.000000 psidata-0.1.4/psidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:43:29.000000 psidata-0.1.4/psidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 21:43:29.000000 psidata-0.1.4/psidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 21:43:29.000000 psidata-0.1.4/psidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-22 21:43:19.000000 psidata-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 21:43:29.214846 psidata-0.1.4/setup.cfg
```

### Comparing `psidata-0.1.3/.github/workflows/publish-to-pypi.yml` & `psidata-0.1.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `psidata-0.1.3/.gitignore` & `psidata-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `psidata-0.1.3/LICENSE.txt` & `psidata-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psidata-0.1.3/PKG-INFO` & `psidata-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psidata
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lightweight wrapper for managing psiexperiment data
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2017-2022 psiepxeriment development team
```

### Comparing `psidata-0.1.3/psidata/bcolz_tools.py` & `psidata-0.1.4/psidata/bcolz_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         columns=columns, orient=orient)
     return df
 
 
 class BcolzSignal(Signal):
 
     def __init__(self, base_path):
+        super().__init__()
         self.base_path = base_path
 
     @property
     @functools.lru_cache()
     def array(self):
         return bcolz.carray(rootdir=self.base_path)
```

### Comparing `psidata-0.1.3/psidata/calibration.py` & `psidata-0.1.4/psidata/calibration.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.3/psidata/legacy_bcolz_tools.py` & `psidata-0.1.4/psidata/legacy_bcolz_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.3/psidata/recording.py` & `psidata-0.1.4/psidata/recording.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.3/psidata/signal.py` & `psidata-0.1.4/psidata/signal.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.3/psidata/zarr_tools.py` & `psidata-0.1.4/psidata/zarr_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.3/psidata.egg-info/PKG-INFO` & `psidata-0.1.4/psidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psidata
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lightweight wrapper for managing psiexperiment data
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2017-2022 psiepxeriment development team
```

### Comparing `psidata-0.1.3/pyproject.toml` & `psidata-0.1.4/pyproject.toml`

 * *Files identical despite different names*

