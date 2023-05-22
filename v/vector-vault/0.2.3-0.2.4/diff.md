# Comparing `tmp/vector_vault-0.2.3.tar.gz` & `tmp/vector_vault-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.2.3.tar", last modified: Sun May 21 18:37:17 2023, max compression
+gzip compressed data, was "vector_vault-0.2.4.tar", last modified: Mon May 22 02:11:10 2023, max compression
```

## Comparing `vector_vault-0.2.3.tar` & `vector_vault-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:37:17.107588 vector_vault-0.2.3/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 18:37:17.107430 vector_vault-0.2.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 18:37:17.107635 vector_vault-0.2.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-21 18:37:11.000000 vector_vault-0.2.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:37:17.106001 vector_vault-0.2.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:37:17.107249 vector_vault-0.2.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2.3/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18832 2023-05-21 18:36:59.000000 vector_vault-0.2.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 02:11:10.383853 vector_vault-0.2.4/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.4/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 02:11:10.383690 vector_vault-0.2.4/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.4/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-22 02:11:10.383890 vector_vault-0.2.4/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-22 02:10:43.000000 vector_vault-0.2.4/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 02:11:10.381257 vector_vault-0.2.4/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 02:11:10.383252 vector_vault-0.2.4/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.4/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2.4/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2.4/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2.4/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.4/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18863 2023-05-22 02:10:39.000000 vector_vault-0.2.4/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.4/vectorvault/wrap.py
```

### Comparing `vector_vault-0.2.3/LICENSE` & `vector_vault-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.3/PKG-INFO` & `vector_vault-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.2.3
+Version: 0.2.4
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2.3/README.md` & `vector_vault-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.3/setup.py` & `vector_vault-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.2.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.2.4/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.2.3
+Version: 0.2.4
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2.3/vectorvault/__init__.py` & `vector_vault-0.2.4/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.3/vectorvault/closedai.py` & `vector_vault-0.2.4/vectorvault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.3/vectorvault/cloudmanager.py` & `vector_vault-0.2.4/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.3/vectorvault/creds.py` & `vector_vault-0.2.4/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.3/vectorvault/download.py` & `vector_vault-0.2.4/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.3/vectorvault/vault.py` & `vector_vault-0.2.4/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         total_saved_items = 0
         for item in self.items:
             item_id = item["meta"]["item_id"]
             self.cloud_manager.upload(item_id, item["text"], item["meta"])
             total_saved_items += 1
 
         self.items.clear()
+        self.x_checked = False
 
         if self.verbose:
             print("save vectors time --- %s seconds ---" % (time.time() - start_time))
 
 
     def delete(self):
         if self.verbose == True:
```

### Comparing `vector_vault-0.2.3/vectorvault/wrap.py` & `vector_vault-0.2.4/vectorvault/wrap.py`

 * *Files identical despite different names*

