# Comparing `tmp/doppkit-esri-toolbox-0.1.1.tar.gz` & `tmp/doppkit-esri-toolbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-esri-toolbox-0.1.1.tar", last modified: Fri May 19 16:37:26 2023, max compression
+gzip compressed data, was "doppkit-esri-toolbox-0.1.2.tar", last modified: Mon May 22 16:13:15 2023, max compression
```

## Comparing `doppkit-esri-toolbox-0.1.1.tar` & `doppkit-esri-toolbox-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.734407 doppkit-esri-toolbox-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.734407 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/esri/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/esri/arcpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 16:13:15.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/esri/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:13:15.691635 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/esri/arcpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-22 16:13:02.000000 doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py
```

### Comparing `doppkit-esri-toolbox-0.1.1/LICENSE` & `doppkit-esri-toolbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.1/PKG-INFO` & `doppkit-esri-toolbox-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit-esri-toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-esri-toolbox-0.1.1/README.md` & `doppkit-esri-toolbox-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.1/pyproject.toml` & `doppkit-esri-toolbox-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/PKG-INFO` & `doppkit-esri-toolbox-0.1.2/src/doppkit_esri_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit-esri-toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py` & `doppkit-esri-toolbox-0.1.2/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py`

 * *Files identical despite different names*

