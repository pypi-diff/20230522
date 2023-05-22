# Comparing `tmp/vector_vault-0.2.7.tar.gz` & `tmp/vector_vault-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.2.7.tar", last modified: Mon May 22 19:22:32 2023, max compression
+gzip compressed data, was "vector_vault-0.2.8.tar", last modified: Mon May 22 19:51:41 2023, max compression
```

## Comparing `vector_vault-0.2.7.tar` & `vector_vault-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:22:32.563318 vector_vault-0.2.7/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 19:22:32.563189 vector_vault-0.2.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-22 19:22:32.563356 vector_vault-0.2.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-22 19:22:03.000000 vector_vault-0.2.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:22:32.561941 vector_vault-0.2.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 19:22:32.000000 vector_vault-0.2.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      390 2023-05-22 19:22:32.000000 vector_vault-0.2.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-22 19:22:32.000000 vector_vault-0.2.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-22 19:22:32.000000 vector_vault-0.2.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-22 19:22:32.000000 vector_vault-0.2.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:22:32.563025 vector_vault-0.2.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2.7/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3380 2023-05-22 19:00:54.000000 vector_vault-0.2.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1824 2023-05-22 19:13:17.000000 vector_vault-0.2.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-0.2.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17297 2023-05-22 19:20:13.000000 vector_vault-0.2.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:51:41.308486 vector_vault-0.2.8/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.8/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 19:51:41.308290 vector_vault-0.2.8/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.8/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-22 19:51:41.308529 vector_vault-0.2.8/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-22 19:49:44.000000 vector_vault-0.2.8/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:51:41.306506 vector_vault-0.2.8/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      384 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:51:41.308075 vector_vault-0.2.8/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.8/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5165 2023-05-22 19:44:52.000000 vector_vault-0.2.8/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3380 2023-05-22 19:00:54.000000 vector_vault-0.2.8/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1824 2023-05-22 19:13:17.000000 vector_vault-0.2.8/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.8/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-0.2.8/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-22 19:49:38.000000 vector_vault-0.2.8/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.8/vectorvault/wrap.py
```

### Comparing `vector_vault-0.2.7/LICENSE` & `vector_vault-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.7/PKG-INFO` & `vector_vault-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.2.7
+Version: 0.2.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2.7/README.md` & `vector_vault-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.7/setup.py` & `vector_vault-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.2.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.2.8/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.2.7
+Version: 0.2.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2.7/vectorvault/__init__.py` & `vector_vault-0.2.8/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.7/vectorvault/cloudmanager.py` & `vector_vault-0.2.8/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.7/vectorvault/creds.py` & `vector_vault-0.2.8/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.7/vectorvault/download.py` & `vector_vault-0.2.8/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.7/vectorvault/itemize.py` & `vector_vault-0.2.8/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.7/vectorvault/vault.py` & `vector_vault-0.2.8/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 import time
 import json
 import re
 import openai
 from concurrent.futures import ThreadPoolExecutor
 from .cloudmanager import CloudManager
-from .closedai import ClosedAI
+from .ai import AI
 from .itemize import itemize, name, name_vecs, get_item, build_return, get_vectors
 
 
 class Vault:
     def __init__(self, user: str, api_key: str, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
@@ -36,15 +36,15 @@
         self.x_checked = False
         self.verbose = verbose
         self.items = []
         self.last_time = None
         self.last_chat_time = None
         self.first_run = True
         self.needed_sleep_time = None
-        self.closedai = ClosedAI()
+        self.ai = AI()
 
 
     def check_index(self):
         start_time = time.time()
         if self.cloud_manager.vault_exists(name_vecs(self.vault)):
             self.load_vectors()
             num_existing_items = self.vectors.get_n_items()
@@ -102,15 +102,15 @@
 
         if self.verbose:
             print("save vectors time --- %s seconds ---" % (time.time() - start_time))
 
 
     def delete(self):
         if self.verbose == True:
-                print('Deleting started. Note: this can take a while for large datasets')
+            print('Deleting started. Note: this can take a while for large datasets')
         # Clear the local vector data
         self.vectors = get_vectors(self.dims)
         self.items.clear()
         self.x = 0
         self.cloud_manager.delete()
         print('Vault deleted')
     
@@ -193,19 +193,19 @@
 
         self.items.append(itemize(self.vault, self.x, meta, text, name))
         self.x += 1
 
 
     def add(self, text: str, meta: dict = None, name: str = None):
         """
-            If your text length lenght is greater than 15000 characters, Vault.split_text(your_text)  
+            If your text length lenght is greater than 4000 tokens, Vault.split_text(your_text)  
             will automatically be added
         """
 
-        if len(text) > 14000:
+        if self.ai.get_tokens(text) > 4000:
             if self.verbose == True:
                 print('Text length too long. Using the built-in "split_text()" function to get a list of text segments') 
             texts = self.split_text(text) # returns list of text segments
         else:
             texts = [text]
 
         for text in texts:
@@ -264,15 +264,15 @@
         
         time.sleep(self.needed_sleep_time)
         
         texts = []
         text_len = 0
         for item in self.items:
             text = item['text']
-            text_len += self.closedai.get_tokens(text)
+            text_len += self.ai.get_tokens(text)
             texts.append(text)
         num_batches = int(np.ceil(len(texts) / batch_size))
 
         # Prepare the text chunks for all batches
         batches_text_chunks = [
             texts[i * batch_size:min((i + 1) * batch_size, len(texts))]
             for i in range(num_batches)
@@ -288,15 +288,15 @@
                 print(f'Projected Tokens per min:{projected_tokens_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {text_len}')
             # 1 min divided by the cap per min and the total we are sending now and factor in the last trip time
             self.needed_sleep_time = 60 / (350000 / text_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
 
             if self.verbose == True:
-                print(f'Time calc to sleep: {self.needed_sleep_time}')
+                print(f"Time calc'd to sleep: {self.needed_sleep_time}")
             if req_min > 3500:
                 time.sleep(1)
 
         # Process the batches in parallel using ThreadPoolExecutor
         with ThreadPoolExecutor() as executor:
             process_batch_with_params = lambda batch_text_chunks: self.process_batch(batch_text_chunks, never_stop, loop_timeout)
             batch_embeddings_list = list(executor.map(process_batch_with_params, batches_text_chunks))
@@ -365,62 +365,61 @@
             self.needed_sleep_time = 0
         
         if not history:
             history = ''
         
         time.sleep(self.needed_sleep_time)
 
-        if self.closedai.get_tokens(text) > 4000:
+        if self.ai.get_tokens(text) > 4000:
             if summary:
                 inputs = self.split_text(text, 14500)
             else:
                 inputs = self.split_text(text)
         else:
             inputs = [text]
         response = ''
         for segment in inputs:
             start_time = time.time()
-            seg_len = self.closedai.get_tokens(segment)
+            seg_len = self.ai.get_tokens(segment)
             # max 90,000 tokens per minute | max requests per minute = 3500
             trip_time = float(start_time - self.last_chat_time)
             req_min = 60 / trip_time # 1 min (60) / time between requests (trip_time)
             projected_tokens_per_min = req_min * seg_len
             rate_ratio = projected_tokens_per_min / 90000
             if self.verbose == True:
                 print(f'Projected Tokens per min:{projected_tokens_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {seg_len}')
             # 1 min divided by the cap per min and the total we are sending now and factor in the last trip time
             self.needed_sleep_time = 60 / (90000 / seg_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
             if self.verbose == True:
-                print(f'Time calc to sleep: {self.needed_sleep_time}')
+                print(f"Time calc'd to sleep: {self.needed_sleep_time}")
 
             if expansion:
                 iq = f"be direct and short. Question: {segment} \n The intent of this question is to: "
-                intent_expansion = self.closedai.llm(iq)
+                intent_expansion = self.ai.llm(iq)
                 kq = f"be general, direct, and short. Don't give an answer, only topics this question falls under to this question: {segment}"
-                knowledge_expansion = self.closedai.llm(kq)
+                knowledge_expansion = self.ai.llm(kq)
                 segment = f'question_intent: {intent_expansion} | {knowledge_expansion}\n\
                 Question: {segment}'
-                print(segment)
 
             while True:
                 try:
                     if summary and not get_context:
-                        response += self.closedai.summarize(segment, model=model)
+                        response += self.ai.summarize(segment, model=model)
                     elif get_context and not summary:
                         user_input = segment + history if history_search else segment
-                        if self.closedai.get_tokens(user_input) > 4000:
+                        if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
-                        if self.closedai.get_tokens(user_input) > 4000:
+                        if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         context = self.get_similar(user_input, n=n_context)
-                        response = self.closedai.llm_w_context(segment, context, history, model=model)
+                        response = self.ai.llm_w_context(segment, context, history, model=model)
                     else:
-                        response = self.closedai.llm(segment, history, model=model)
+                        response = self.ai.llm(segment, history, model=model)
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 15 seconds")
                     time.sleep(15)
                     
             self.last_chat_time = start_time
```

### Comparing `vector_vault-0.2.7/vectorvault/wrap.py` & `vector_vault-0.2.8/vectorvault/wrap.py`

 * *Files identical despite different names*

