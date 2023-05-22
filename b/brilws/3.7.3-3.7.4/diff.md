# Comparing `tmp/brilws-3.7.3.tar.gz` & `tmp/brilws-3.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brilws-3.7.3.tar", last modified: Wed May  3 17:57:18 2023, max compression
+gzip compressed data, was "dist/brilws-3.7.4.tar", last modified: Mon May 22 14:00:47 2023, max compression
```

## Comparing `brilws-3.7.3.tar` & `brilws-3.7.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/
--rw-r--r--   0 xiezhen    (501) staff       (20)       86 2023-04-28 15:39:36.000000 brilws-3.7.3/MANIFEST.in
--rw-r--r--   0 xiezhen    (501) staff       (20)      875 2023-05-03 17:57:18.000000 brilws-3.7.3/PKG-INFO
--rw-r--r--   0 xiezhen    (501) staff       (20)      442 2023-04-28 15:39:36.000000 brilws-3.7.3/README.md
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws/
--rw-r--r--   0 xiezhen    (501) staff       (20)      430 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/RegexValidator.py
--rw-r--r--   0 xiezhen    (501) staff       (20)       34 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/__init__.py
--rw-r--r--   0 xiezhen    (501) staff       (20)       22 2023-05-03 17:51:23.000000 brilws-3.7.3/brilws/_version.py
--rw-r--r--   0 xiezhen    (501) staff       (20)    73253 2023-05-03 17:42:14.000000 brilws-3.7.3/brilws/api.py
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws/cli/
--rw-r--r--   0 xiezhen    (501) staff       (20)      219 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/__init__.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1695 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilcalc_beam.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     3407 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilcalc_lumi.py
--rw-r--r--   0 xiezhen    (501) staff       (20)    59077 2023-04-28 15:45:47.000000 brilws-3.7.3/brilws/cli/brilcalc_main.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1286 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilcalc_trg.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      870 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_create.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1576 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_loaddata.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1462 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_loadmap.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1413 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_loadresult.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     8529 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_main.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      745 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_insertdata.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      670 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_insertiov.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      626 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_listdata.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      918 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_listiov.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     7448 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_main.py
--rw-r--r--   0 xiezhen    (501) staff       (20)    17731 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/clicommonargs.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     8554 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/corrector.py
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws/data/
--rw-r--r--   0 xiezhen    (501) staff       (20)        0 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/data/__init__.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1407 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/data/bcm1fv1.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)     1129 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/data/readdb3.ini
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws/dbschema/
--rw-r--r--   0 xiezhen    (501) staff       (20)        0 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/dbschema/__init__.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1322 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/dbschema/schema_fixed.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)      390 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/dbschema/schema_iov.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)     4581 2023-04-28 15:41:04.000000 brilws-3.7.3/brilws/dbschema/schema_sharded.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)     1562 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/dbschema/schema_trg.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)     4131 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/display.py
--rw-r--r--   0 xiezhen    (501) staff       (20)    15804 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/fileapi.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     5929 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/formatter.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     2197 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/lumiParameters.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1864 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/params.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1267 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/timeconvert.py
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws.egg-info/
--rw-r--r--   0 xiezhen    (501) staff       (20)      875 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/PKG-INFO
--rw-r--r--   0 xiezhen    (501) staff       (20)     1125 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/SOURCES.txt
--rw-r--r--   0 xiezhen    (501) staff       (20)        1 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/dependency_links.txt
--rw-r--r--   0 xiezhen    (501) staff       (20)      172 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/entry_points.txt
--rw-r--r--   0 xiezhen    (501) staff       (20)        7 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/top_level.txt
--rw-r--r--   0 xiezhen    (501) staff       (20)       79 2023-05-03 17:57:18.000000 brilws-3.7.3/setup.cfg
--rwxr-xr-x   0 xiezhen    (501) staff       (20)     1040 2023-04-28 15:39:36.000000 brilws-3.7.3/setup.py
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-22 14:00:47.000000 brilws-3.7.4/
+-rw-r--r--   0 xiezhen    (501) staff       (20)       86 2023-04-28 15:39:36.000000 brilws-3.7.4/MANIFEST.in
+-rw-r--r--   0 xiezhen    (501) staff       (20)      875 2023-05-22 14:00:47.000000 brilws-3.7.4/PKG-INFO
+-rw-r--r--   0 xiezhen    (501) staff       (20)      442 2023-04-28 15:39:36.000000 brilws-3.7.4/README.md
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-22 14:00:47.000000 brilws-3.7.4/brilws/
+-rw-r--r--   0 xiezhen    (501) staff       (20)      430 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/RegexValidator.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)       34 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/__init__.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)       22 2023-05-22 13:57:52.000000 brilws-3.7.4/brilws/_version.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)    73264 2023-05-22 13:43:09.000000 brilws-3.7.4/brilws/api.py
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-22 14:00:47.000000 brilws-3.7.4/brilws/cli/
+-rw-r--r--   0 xiezhen    (501) staff       (20)      219 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/__init__.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1695 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/brilcalc_beam.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     3407 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/brilcalc_lumi.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)    59077 2023-05-22 13:42:59.000000 brilws-3.7.4/brilws/cli/brilcalc_main.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1286 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/brilcalc_trg.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      870 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/brilschema_create.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1576 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/brilschema_loaddata.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1462 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/brilschema_loadmap.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1413 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/brilschema_loadresult.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     8529 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/brilschema_main.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      745 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/briltag_insertdata.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      670 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/briltag_insertiov.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      626 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/briltag_listdata.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      918 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/briltag_listiov.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     7448 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/briltag_main.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)    17731 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/cli/clicommonargs.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     8554 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/corrector.py
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-22 14:00:47.000000 brilws-3.7.4/brilws/data/
+-rw-r--r--   0 xiezhen    (501) staff       (20)        0 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/data/__init__.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1407 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/data/bcm1fv1.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1129 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/data/readdb3.ini
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-22 14:00:47.000000 brilws-3.7.4/brilws/dbschema/
+-rw-r--r--   0 xiezhen    (501) staff       (20)        0 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/dbschema/__init__.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1322 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/dbschema/schema_fixed.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)      390 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/dbschema/schema_iov.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)     4581 2023-04-28 15:41:04.000000 brilws-3.7.4/brilws/dbschema/schema_sharded.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1562 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/dbschema/schema_trg.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)     4131 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/display.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)    15804 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/fileapi.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     5929 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/formatter.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     2197 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/lumiParameters.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1864 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/params.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1267 2023-04-28 15:39:36.000000 brilws-3.7.4/brilws/timeconvert.py
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-22 14:00:47.000000 brilws-3.7.4/brilws.egg-info/
+-rw-r--r--   0 xiezhen    (501) staff       (20)      875 2023-05-22 14:00:46.000000 brilws-3.7.4/brilws.egg-info/PKG-INFO
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1125 2023-05-22 14:00:46.000000 brilws-3.7.4/brilws.egg-info/SOURCES.txt
+-rw-r--r--   0 xiezhen    (501) staff       (20)        1 2023-05-22 14:00:46.000000 brilws-3.7.4/brilws.egg-info/dependency_links.txt
+-rw-r--r--   0 xiezhen    (501) staff       (20)      172 2023-05-22 14:00:46.000000 brilws-3.7.4/brilws.egg-info/entry_points.txt
+-rw-r--r--   0 xiezhen    (501) staff       (20)        7 2023-05-22 14:00:46.000000 brilws-3.7.4/brilws.egg-info/top_level.txt
+-rw-r--r--   0 xiezhen    (501) staff       (20)       79 2023-05-22 14:00:47.000000 brilws-3.7.4/setup.cfg
+-rwxr-xr-x   0 xiezhen    (501) staff       (20)     1040 2023-04-28 15:39:36.000000 brilws-3.7.4/setup.py
```

### Comparing `brilws-3.7.3/PKG-INFO` & `brilws-3.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: brilws
-Version: 3.7.3
+Version: 3.7.4
 Summary: bril worksuite
 Home-page: https://github.com/xiezhen/brilws
 Author: Zhen Xie
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/xiezhen/brilws/tarball/3.7.3
+Download-URL: https://github.com/xiezhen/brilws/tarball/3.7.4
 Description: ### BRIL Work Suite
         python package for working with BRIL data 
         
         #### Install
         
         #### into brilconda virtual environment
         pip install brilws
```

### Comparing `brilws-3.7.3/brilws/api.py` & `brilws-3.7.4/brilws/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1418,30 +1418,31 @@
 
 def is_hltpath_in_dataset(engine,hltconfigidhltpathidpairs,datasetname,schemaname=''):
     '''
     hltconfigidhltpathidpairs : [(hltconfigid,hltpathid)]
     '''
     datasettablename = dname = 'datasethltpathmap'
     hlttablename = hname = 'hltpathl1seedmap'
+    connection = engine.connect()
     if schemaname:
         datasethltpathmap = '.'.join([schemaname,dname])
         hltpathl1seedmap = '.'.join([schemaname,hname])
     for (hltconfigid,hltpathid) in hltconfigidhltpathidpairs:
       q = "select count(*) from {datasethltpathmap} d, {hltpathl1seedmap} h where h.hltconfigid=d.hltconfigid and d.hltconfigid=:hltconfigid and d.datasetpathname=:datasetname and h.hltpathid=:hltpathid".format(datasethltpathmap=datasethltpathmap,hltpathl1seedmap=hltpathl1seedmap)
       binddict = {}
       binddict['hltpathid'] = hltpathid
       binddict['datasetname'] = datasetname
       binddict['hltconfigid'] = hltconfigid
       log.debug(q+','+str(binddict))
-    connection = engine.connect()
-    resultProxy = connection.execute(q,binddict)
-    for row in resultProxy:
-      result = int(row[0])
-      if result>0:
-        return True
+      resultProxy = connection.execute(q,binddict)
+
+      for row in resultProxy:
+        result = int(row[0])
+        if result>0:
+          return True
     return False
 
 def is_hltpathid_in_dataset(engine,hltpathid,datasetname,hltconfigid,schemaname=''):
     '''
     Check if a hltpathid and a dataset is in the same menu, no more relationship for now
     input :
        hltpathid : hltpathid
```

### Comparing `brilws-3.7.3/brilws/cli/brilcalc_beam.py` & `brilws-3.7.4/brilws/cli/brilcalc_beam.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/brilcalc_lumi.py` & `brilws-3.7.4/brilws/cli/brilcalc_lumi.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/brilcalc_main.py` & `brilws-3.7.4/brilws/cli/brilcalc_main.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/brilcalc_trg.py` & `brilws-3.7.4/brilws/cli/brilcalc_trg.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/brilschema_create.py` & `brilws-3.7.4/brilws/cli/brilschema_create.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/brilschema_loaddata.py` & `brilws-3.7.4/brilws/cli/brilschema_loaddata.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/brilschema_loadmap.py` & `brilws-3.7.4/brilws/cli/brilschema_loadmap.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/brilschema_loadresult.py` & `brilws-3.7.4/brilws/cli/brilschema_loadresult.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/brilschema_main.py` & `brilws-3.7.4/brilws/cli/brilschema_main.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/briltag_insertdata.py` & `brilws-3.7.4/brilws/cli/briltag_insertdata.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/briltag_insertiov.py` & `brilws-3.7.4/brilws/cli/briltag_insertiov.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/briltag_listdata.py` & `brilws-3.7.4/brilws/cli/briltag_listdata.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/briltag_listiov.py` & `brilws-3.7.4/brilws/cli/briltag_listiov.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/briltag_main.py` & `brilws-3.7.4/brilws/cli/briltag_main.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/cli/clicommonargs.py` & `brilws-3.7.4/brilws/cli/clicommonargs.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/corrector.py` & `brilws-3.7.4/brilws/corrector.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/data/bcm1fv1.yaml` & `brilws-3.7.4/brilws/data/bcm1fv1.yaml`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/data/readdb3.ini` & `brilws-3.7.4/brilws/data/readdb3.ini`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/dbschema/schema_fixed.yaml` & `brilws-3.7.4/brilws/dbschema/schema_fixed.yaml`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/dbschema/schema_sharded.yaml` & `brilws-3.7.4/brilws/dbschema/schema_sharded.yaml`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/dbschema/schema_trg.yaml` & `brilws-3.7.4/brilws/dbschema/schema_trg.yaml`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/display.py` & `brilws-3.7.4/brilws/display.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/fileapi.py` & `brilws-3.7.4/brilws/fileapi.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/formatter.py` & `brilws-3.7.4/brilws/formatter.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/lumiParameters.py` & `brilws-3.7.4/brilws/lumiParameters.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/params.py` & `brilws-3.7.4/brilws/params.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws/timeconvert.py` & `brilws-3.7.4/brilws/timeconvert.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/brilws.egg-info/PKG-INFO` & `brilws-3.7.4/brilws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: brilws
-Version: 3.7.3
+Version: 3.7.4
 Summary: bril worksuite
 Home-page: https://github.com/xiezhen/brilws
 Author: Zhen Xie
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/xiezhen/brilws/tarball/3.7.3
+Download-URL: https://github.com/xiezhen/brilws/tarball/3.7.4
 Description: ### BRIL Work Suite
         python package for working with BRIL data 
         
         #### Install
         
         #### into brilconda virtual environment
         pip install brilws
```

### Comparing `brilws-3.7.3/brilws.egg-info/SOURCES.txt` & `brilws-3.7.4/brilws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brilws-3.7.3/setup.py` & `brilws-3.7.4/setup.py`

 * *Files identical despite different names*

