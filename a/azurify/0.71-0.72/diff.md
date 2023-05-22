# Comparing `tmp/azurify-0.71.tar.gz` & `tmp/azurify-0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurify-0.71.tar", last modified: Mon May 22 12:50:01 2023, max compression
+gzip compressed data, was "azurify-0.72.tar", last modified: Mon May 22 12:50:23 2023, max compression
```

## Comparing `azurify-0.71.tar` & `azurify-0.72.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-22 12:50:01.606178 azurify-0.71/
--rw-r--r--   0 deniz      (501) staff       (20)     1067 2023-05-15 16:05:12.000000 azurify-0.71/LICENSE
--rw-r--r--   0 deniz      (501) staff       (20)     2993 2023-05-22 12:50:01.599038 azurify-0.71/PKG-INFO
-drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-22 12:50:01.594106 azurify-0.71/azurify/
--rw-r--r--   0 deniz      (501) staff       (20)      121 2023-05-22 12:49:11.000000 azurify-0.71/azurify/__init__.py
--rw-r--r--   0 deniz      (501) staff       (20)     1627 2023-05-15 16:05:12.000000 azurify-0.71/azurify/azconverter.py
--rw-r--r--   0 deniz      (501) staff       (20)      593 2023-05-21 11:18:15.000000 azurify-0.71/azurify/azenv.py
--rw-r--r--   0 deniz      (501) staff       (20)     5146 2023-05-22 12:47:42.000000 azurify-0.71/azurify/azkeyvault.py
--rw-r--r--   0 deniz      (501) staff       (20)     3542 2023-05-17 11:43:21.000000 azurify-0.71/azurify/azsecrets.py
--rw-r--r--   0 deniz      (501) staff       (20)     3014 2023-05-15 16:05:12.000000 azurify-0.71/azurify/azstorage.py
--rw-r--r--   0 deniz      (501) staff       (20)      547 2023-05-15 16:05:12.000000 azurify-0.71/azurify/test_azconverter.py
--rw-r--r--   0 deniz      (501) staff       (20)     2113 2023-05-17 16:34:50.000000 azurify-0.71/azurify/test_azkeyvault.py
--rw-r--r--   0 deniz      (501) staff       (20)     3507 2023-05-17 17:55:01.000000 azurify-0.71/azurify/test_azsecrets.py
--rw-r--r--   0 deniz      (501) staff       (20)        0 2023-05-15 16:05:12.000000 azurify-0.71/azurify/test_azstorage.py
-drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-22 12:50:01.598359 azurify-0.71/azurify.egg-info/
--rw-r--r--   0 deniz      (501) staff       (20)     2993 2023-05-22 12:50:01.000000 azurify-0.71/azurify.egg-info/PKG-INFO
--rw-r--r--   0 deniz      (501) staff       (20)      431 2023-05-22 12:50:01.000000 azurify-0.71/azurify.egg-info/SOURCES.txt
--rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-22 12:50:01.000000 azurify-0.71/azurify.egg-info/dependency_links.txt
--rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-16 09:30:41.000000 azurify-0.71/azurify.egg-info/not-zip-safe
--rw-r--r--   0 deniz      (501) staff       (20)      133 2023-05-22 12:50:01.000000 azurify-0.71/azurify.egg-info/requires.txt
--rw-r--r--   0 deniz      (501) staff       (20)        8 2023-05-22 12:50:01.000000 azurify-0.71/azurify.egg-info/top_level.txt
--rw-r--r--   0 deniz      (501) staff       (20)       38 2023-05-22 12:50:01.606349 azurify-0.71/setup.cfg
--rw-r--r--   0 deniz      (501) staff       (20)      998 2023-05-17 18:17:42.000000 azurify-0.71/setup.py
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-22 12:50:23.073174 azurify-0.72/
+-rw-r--r--   0 deniz      (501) staff       (20)     1067 2023-05-15 16:05:12.000000 azurify-0.72/LICENSE
+-rw-r--r--   0 deniz      (501) staff       (20)     2993 2023-05-22 12:50:23.072489 azurify-0.72/PKG-INFO
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-22 12:50:23.067813 azurify-0.72/azurify/
+-rw-r--r--   0 deniz      (501) staff       (20)      121 2023-05-22 12:49:11.000000 azurify-0.72/azurify/__init__.py
+-rw-r--r--   0 deniz      (501) staff       (20)     1627 2023-05-15 16:05:12.000000 azurify-0.72/azurify/azconverter.py
+-rw-r--r--   0 deniz      (501) staff       (20)      593 2023-05-21 11:18:15.000000 azurify-0.72/azurify/azenv.py
+-rw-r--r--   0 deniz      (501) staff       (20)     5146 2023-05-22 12:47:42.000000 azurify-0.72/azurify/azkeyvault.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3542 2023-05-17 11:43:21.000000 azurify-0.72/azurify/azsecrets.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3014 2023-05-15 16:05:12.000000 azurify-0.72/azurify/azstorage.py
+-rw-r--r--   0 deniz      (501) staff       (20)      547 2023-05-15 16:05:12.000000 azurify-0.72/azurify/test_azconverter.py
+-rw-r--r--   0 deniz      (501) staff       (20)     2113 2023-05-17 16:34:50.000000 azurify-0.72/azurify/test_azkeyvault.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3507 2023-05-17 17:55:01.000000 azurify-0.72/azurify/test_azsecrets.py
+-rw-r--r--   0 deniz      (501) staff       (20)        0 2023-05-15 16:05:12.000000 azurify-0.72/azurify/test_azstorage.py
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-22 12:50:23.071607 azurify-0.72/azurify.egg-info/
+-rw-r--r--   0 deniz      (501) staff       (20)     2993 2023-05-22 12:50:22.000000 azurify-0.72/azurify.egg-info/PKG-INFO
+-rw-r--r--   0 deniz      (501) staff       (20)      431 2023-05-22 12:50:22.000000 azurify-0.72/azurify.egg-info/SOURCES.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-22 12:50:22.000000 azurify-0.72/azurify.egg-info/dependency_links.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-16 09:30:41.000000 azurify-0.72/azurify.egg-info/not-zip-safe
+-rw-r--r--   0 deniz      (501) staff       (20)      133 2023-05-22 12:50:22.000000 azurify-0.72/azurify.egg-info/requires.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        8 2023-05-22 12:50:22.000000 azurify-0.72/azurify.egg-info/top_level.txt
+-rw-r--r--   0 deniz      (501) staff       (20)       38 2023-05-22 12:50:23.073373 azurify-0.72/setup.cfg
+-rw-r--r--   0 deniz      (501) staff       (20)      998 2023-05-22 12:50:18.000000 azurify-0.72/setup.py
```

### Comparing `azurify-0.71/LICENSE` & `azurify-0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `azurify-0.71/PKG-INFO` & `azurify-0.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurify
-Version: 0.71
+Version: 0.72
 Summary: Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.
 Home-page: https://github.com/zinyosrim/azurify
 Author: Zin Yosrim
 Author-email: zinyosrim@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `azurify-0.71/azurify/azconverter.py` & `azurify-0.72/azurify/azconverter.py`

 * *Files identical despite different names*

### Comparing `azurify-0.71/azurify/azenv.py` & `azurify-0.72/azurify/azenv.py`

 * *Files identical despite different names*

### Comparing `azurify-0.71/azurify/azkeyvault.py` & `azurify-0.72/azurify/azkeyvault.py`

 * *Files identical despite different names*

### Comparing `azurify-0.71/azurify/azsecrets.py` & `azurify-0.72/azurify/azsecrets.py`

 * *Files identical despite different names*

### Comparing `azurify-0.71/azurify/azstorage.py` & `azurify-0.72/azurify/azstorage.py`

 * *Files identical despite different names*

### Comparing `azurify-0.71/azurify/test_azconverter.py` & `azurify-0.72/azurify/test_azconverter.py`

 * *Files identical despite different names*

### Comparing `azurify-0.71/azurify/test_azkeyvault.py` & `azurify-0.72/azurify/test_azkeyvault.py`

 * *Files identical despite different names*

### Comparing `azurify-0.71/azurify/test_azsecrets.py` & `azurify-0.72/azurify/test_azsecrets.py`

 * *Files identical despite different names*

### Comparing `azurify-0.71/azurify.egg-info/PKG-INFO` & `azurify-0.72/azurify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurify
-Version: 0.71
+Version: 0.72
 Summary: Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.
 Home-page: https://github.com/zinyosrim/azurify
 Author: Zin Yosrim
 Author-email: zinyosrim@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `azurify-0.71/setup.py` & `azurify-0.72/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="azurify",
-    version="0.71",
+    version="0.72",
     description="Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zinyosrim/azurify",
     author="Zin Yosrim",
     author_email="zinyosrim@gmail.com",
     license="MIT",
```

