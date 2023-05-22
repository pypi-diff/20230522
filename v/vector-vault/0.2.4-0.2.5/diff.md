# Comparing `tmp/vector_vault-0.2.4.tar.gz` & `tmp/vector_vault-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.2.4.tar", last modified: Mon May 22 02:11:10 2023, max compression
+gzip compressed data, was "vector_vault-0.2.5.tar", last modified: Mon May 22 17:55:16 2023, max compression
```

## Comparing `vector_vault-0.2.4.tar` & `vector_vault-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 02:11:10.383853 vector_vault-0.2.4/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.4/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 02:11:10.383690 vector_vault-0.2.4/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.4/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-22 02:11:10.383890 vector_vault-0.2.4/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-22 02:10:43.000000 vector_vault-0.2.4/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 02:11:10.381257 vector_vault-0.2.4/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-22 02:11:10.000000 vector_vault-0.2.4/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 02:11:10.383252 vector_vault-0.2.4/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.4/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2.4/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2.4/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2.4/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.4/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18863 2023-05-22 02:10:39.000000 vector_vault-0.2.4/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.4/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 17:55:16.538791 vector_vault-0.2.5/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.5/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 17:55:16.538629 vector_vault-0.2.5/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.5/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-22 17:55:16.538826 vector_vault-0.2.5/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-22 17:55:04.000000 vector_vault-0.2.5/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 17:55:16.537111 vector_vault-0.2.5/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 17:55:16.000000 vector_vault-0.2.5/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      390 2023-05-22 17:55:16.000000 vector_vault-0.2.5/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-22 17:55:16.000000 vector_vault-0.2.5/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-22 17:55:16.000000 vector_vault-0.2.5/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-22 17:55:16.000000 vector_vault-0.2.5/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 17:55:16.538430 vector_vault-0.2.5/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.5/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2.5/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2.5/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2.5/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.5/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1466 2023-05-22 17:46:51.000000 vector_vault-0.2.5/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17347 2023-05-22 17:49:36.000000 vector_vault-0.2.5/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.5/vectorvault/wrap.py
```

### Comparing `vector_vault-0.2.4/LICENSE` & `vector_vault-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.4/PKG-INFO` & `vector_vault-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.2.4
+Version: 0.2.5
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2.4/README.md` & `vector_vault-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.4/setup.py` & `vector_vault-0.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.2.4/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.2.5/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.2.4
+Version: 0.2.5
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2.4/vectorvault/__init__.py` & `vector_vault-0.2.5/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.4/vectorvault/closedai.py` & `vector_vault-0.2.5/vectorvault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.4/vectorvault/cloudmanager.py` & `vector_vault-0.2.5/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.4/vectorvault/creds.py` & `vector_vault-0.2.5/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.4/vectorvault/download.py` & `vector_vault-0.2.5/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.4/vectorvault/vault.py` & `vector_vault-0.2.5/vectorvault/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import json
 import re
 import openai
 from annoy import AnnoyIndex
 from concurrent.futures import ThreadPoolExecutor
 from .cloudmanager import CloudManager
 from .closedai import ClosedAI
+from .itemize import itemize, name, name_vecs, get_item, build_return
 
 
 class Vault:
     def __init__(self, user: str, api_key: str, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = AnnoyIndex(dims, 'angular')
         self.dims = dims
@@ -42,16 +43,15 @@
         self.first_run = True
         self.needed_sleep_time = None
         self.closedai = ClosedAI()
 
 
     def check_index(self):
         start_time = time.time()
-        if self.cloud_manager.vault_exists(f'{self.vault}.ann'):
-            print('vault exists')
+        if self.cloud_manager.vault_exists(name_vecs(self.vault)):
             self.load_vectors()
             num_existing_items = self.vectors.get_n_items()
             new_index = AnnoyIndex(self.dims, 'angular')
             for i in range(num_existing_items):
                 vector = self.vectors.get_item_vector(i)
                 new_index.add_item(i, vector)
                 self.x = i
@@ -63,44 +63,44 @@
         if self.verbose == True:
             print("initialize index --- %s seconds ---" % (time.time() - start_time))
         
 
     def load_vectors(self):
         start_time = time.time()
         # Download the .ann file from google cloud storage to a temporary file
-        temp_file_path = self.cloud_manager.download_to_temp_file(f'{self.vault}.ann')
+        temp_file_path = self.cloud_manager.download_to_temp_file(name_vecs(self.vault))
 
         # Load the AnnoyIndex object from the temporary file, then delete the temp file
         self.vectors.load(temp_file_path)
         os.remove(temp_file_path)
         if self.verbose:
             print("get load vectors --- %s seconds ---" % (time.time() - start_time))
 
     
     def get_vaults(self, vault: str = None):
         vault = self.vault if vault is None else vault
-        return self.cloud_manager.get_vaults(vault=f'{vault}')
+        return self.cloud_manager.get_vaults(vault)
 
 
     def get_total_vectors(self):
         return self.vectors.get_n_items()
     
 
     def save(self, trees=16):
         start_time = time.time()
         self.vectors.build(trees)
 
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             self.vectors.save(temp_file.name)
-            self.cloud_manager.upload_temp_file(temp_file.name, f'{self.vault}.ann')
+            self.cloud_manager.upload_temp_file(temp_file.name, name_vecs(self.vault))
 
         total_saved_items = 0
         for item in self.items:
-            item_id = item["meta"]["item_id"]
-            self.cloud_manager.upload(item_id, item["text"], item["meta"])
+            item_text, item_id, item_meta = get_item(item)
+            self.cloud_manager.upload(item_id, item_text, item_meta)
             total_saved_items += 1
 
         self.items.clear()
         self.x_checked = False
 
         if self.verbose:
             print("save vectors time --- %s seconds ---" % (time.time() - start_time))
@@ -153,34 +153,23 @@
         return segments
 
 
     def get_items_by_vector(self, vector, n: int = 4):
         self.load_vectors()
         start_time = time.time()
 
-        # Create an empty list to store the results
         results = []
-        indexes = self.vectors.get_nns_by_vector(vector, n)
-        print(indexes)
-        for index in indexes:
+        vecs = self.vectors.get_nns_by_vector(vector, n)
+        for vec in vecs:
             # Retrieve the item
-            item_data = self.cloud_manager.download_text_from_cloud(f'{self.vault}/{index}/item')
-
+            item_data = self.cloud_manager.download_text_from_cloud(name(self.vault, vec, item=True))
             # Retrieve the metadata
-            meta_data = self.cloud_manager.download_text_from_cloud(f'{self.vault}/{index}/meta')
+            meta_data = self.cloud_manager.download_text_from_cloud(name(self.vault, vec, meta=True))
             meta = json.loads(meta_data)
-
-            # Create a dictionary with data and metadata
-            result = {
-                "data": item_data,
-                "metadata": meta
-            }
-
-            # Append the result to the list
-            results.append(result)
+            build_return(results, item_data, meta)
 
         # Create a return dictionary
         return_dict = {
             "results": results
         }
 
         if self.verbose == True:
@@ -199,37 +188,16 @@
             If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         if self.x_checked == False:
             self.check_index()
         else: 
             pass
-        
-        # set value if none exist
-        meta = {} if meta is None else meta
-
-        if 'name' not in meta and name is None:
-            name = f'{self.vault}-{self.x}'
-        elif name is not None:
-            name = name
-        meta['name'] = name
-        meta['item_id'] = self.x  # Store the item index in the metadata
-
-        if 'created_at' not in meta:
-            meta['created_at'] = datetime.datetime.utcnow().isoformat()
-        if 'updated_at' not in meta:
-            meta['updated_at'] = datetime.datetime.utcnow().isoformat()
-
-        # Add item and its metadata to the items list
-        item = {
-            "text": text,
-            "meta": meta
-        }
-        self.items.append(item)
 
+        self.items.append(itemize(self.vault, self.x, meta, text, name))
         self.x += 1
 
 
     def add(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 15000 characters, Vault.split_text(your_text)  
             will automatically be added
@@ -256,38 +224,17 @@
         else: 
             pass
         start_time = time.time()
 
         if len(text) > 36000:
             raise 'Text length too long. Use the "split_text() function to get a list of text segments'
 
-        # set value if none exist
-        meta = {} if meta is None else meta
-
-        if 'name' not in meta and name is None:
-            name = f'{self.vault}-{self.x}'
-        elif name is not None:
-            name = name
-        meta['name'] = name
-        meta['item_id'] = self.x  # Store the item index in the metadata
-
-        if 'created_at' not in meta:
-            meta['created_at'] = datetime.datetime.utcnow().isoformat()
-        if 'updated_at' not in meta:
-            meta['updated_at'] = datetime.datetime.utcnow().isoformat()
-
         # Add vector to vectorspace
         self.vectors.add_item(self.x, vector)
-
-        # Add item and its metadata to the items list
-        item = {
-            "text": text,
-            "meta": meta
-        }
-        self.items.append(item)
+        self.items.append(itemize(self.vault, self.x, meta, text, name))
 
         self.x += 1
 
         if self.verbose == True:
             print("add item time --- %s seconds ---" % (time.time() - start_time))
```

### Comparing `vector_vault-0.2.4/vectorvault/wrap.py` & `vector_vault-0.2.5/vectorvault/wrap.py`

 * *Files identical despite different names*

