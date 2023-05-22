# Comparing `tmp/metabeaver-0.1.6.tar.gz` & `tmp/metabeaver-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.1.6.tar", last modified: Thu May  4 18:05:13 2023, max compression
+gzip compressed data, was "metabeaver-0.1.7.tar", last modified: Mon May 22 17:01:42 2023, max compression
```

## Comparing `metabeaver-0.1.6.tar` & `metabeaver-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.355059 metabeaver-0.1.6/
--rw-rw-rw-   0        0        0      221 2023-05-04 18:05:13.354060 metabeaver-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.326463 metabeaver-0.1.6/metabeaver/
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.342538 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.347543 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/
--rw-rw-rw-   0        0        0     3142 2023-05-04 17:59:02.000000 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-02 11:50:11.000000 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/testingTables.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.349538 metabeaver-0.1.6/metabeaver/InstallationScripts/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/InstallationScripts/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.1.6/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.350535 metabeaver-0.1.6/metabeaver/MetaProgramming/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/MetaProgramming/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.353079 metabeaver-0.1.6/metabeaver/Testing/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/Testing/__init__.py
--rw-rw-rw-   0        0        0     1804 2023-04-26 12:07:06.000000 metabeaver-0.1.6/metabeaver/Testing/concatenateDataXLSX.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.341531 metabeaver-0.1.6/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      221 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 18:05:13.355059 metabeaver-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-05-04 18:05:02.000000 metabeaver-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:01:42.869386 metabeaver-0.1.7/
+-rw-rw-rw-   0        0        0      221 2023-05-22 17:01:42.867381 metabeaver-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 17:01:42.829209 metabeaver-0.1.7/metabeaver/
+drwxrwxrwx   0        0        0        0 2023-05-22 17:01:42.844301 metabeaver-0.1.7/metabeaver/GoogleCloudPlatform/
+drwxrwxrwx   0        0        0        0 2023-05-22 17:01:42.852839 metabeaver-0.1.7/metabeaver/GoogleCloudPlatform/BigQuery/
+-rw-rw-rw-   0        0        0     5059 2023-05-22 15:42:45.000000 metabeaver-0.1.7/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.7/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 11:50:11.000000 metabeaver-0.1.7/metabeaver/GoogleCloudPlatform/BigQuery/testingTables.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.7/metabeaver/GoogleCloudPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:01:42.858846 metabeaver-0.1.7/metabeaver/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.7/metabeaver/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.1.7/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:01:42.861846 metabeaver-0.1.7/metabeaver/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.7/metabeaver/MetaProgramming/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:01:42.864393 metabeaver-0.1.7/metabeaver/Testing/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.7/metabeaver/Testing/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.7/metabeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:01:42.842283 metabeaver-0.1.7/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-05-22 17:01:42.000000 metabeaver-0.1.7/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-05-22 17:01:42.000000 metabeaver-0.1.7/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 17:01:42.000000 metabeaver-0.1.7/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-22 17:01:42.000000 metabeaver-0.1.7/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 17:01:42.000000 metabeaver-0.1.7/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 17:01:42.869386 metabeaver-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-05-22 17:01:36.000000 metabeaver-0.1.7/setup.py
```

### Comparing `metabeaver-0.1.6/metabeaver/InstallationScripts/autoGenerateRequirementsText.py` & `metabeaver-0.1.7/metabeaver/InstallationScripts/autoGenerateRequirementsText.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.1.6/metabeaver.egg-info/SOURCES.txt` & `metabeaver-0.1.7/metabeaver.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 metabeaver/GoogleCloudPlatform/__init__.py
 metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
 metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
 metabeaver/GoogleCloudPlatform/BigQuery/testingTables.py
 metabeaver/InstallationScripts/__init__.py
 metabeaver/InstallationScripts/autoGenerateRequirementsText.py
 metabeaver/MetaProgramming/__init__.py
-metabeaver/Testing/__init__.py
-metabeaver/Testing/concatenateDataXLSX.py
+metabeaver/Testing/__init__.py
```

### Comparing `metabeaver-0.1.6/setup.py` & `metabeaver-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.1.6', # Major, minor, patch
+    version='0.1.7', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'numpy',
         'pandas',
         'google-cloud-core',
         'google-cloud-bigquery',
     ],
```

