# Comparing `tmp/superpowered-sdk-0.1.1.tar.gz` & `tmp/superpowered-sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.1.1.tar", last modified: Fri May 19 07:14:53 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.1.3.tar", last modified: Mon May 22 17:53:41 2023, max compression
```

## Comparing `superpowered-sdk-0.1.1.tar` & `superpowered-sdk-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-19 07:14:53.175529 superpowered-sdk-0.1.1/
--rw-r--r--   0 justinclark   (501) staff       (20)     6509 2023-05-19 07:14:53.174927 superpowered-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 justinclark   (501) staff       (20)     5009 2023-05-19 06:21:14.000000 superpowered-sdk-0.1.1/README.md
--rw-r--r--   0 justinclark   (501) staff       (20)       38 2023-05-19 07:14:53.175851 superpowered-sdk-0.1.1/setup.cfg
--rw-r--r--   0 justinclark   (501) staff       (20)     2040 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.1/setup.py
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-19 07:14:53.169304 superpowered-sdk-0.1.1/superpowered/
--rw-r--r--   0 justinclark   (501) staff       (20)      892 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.1/superpowered/__init__.py
--rw-r--r--   0 justinclark   (501) staff       (20)     1301 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.1/superpowered/exceptions.py
--rw-r--r--   0 justinclark   (501) staff       (20)    11202 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.1/superpowered/superpowered.py
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-19 07:14:53.174078 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/
--rw-r--r--   0 justinclark   (501) staff       (20)     6509 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 justinclark   (501) staff       (20)      298 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 justinclark   (501) staff       (20)        1 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 justinclark   (501) staff       (20)       17 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/requires.txt
--rw-r--r--   0 justinclark   (501) staff       (20)       13 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 17:53:41.824769 superpowered-sdk-0.1.3/
+-rw-r--r--   0 justinclark   (501) staff       (20)     6636 2023-05-22 17:53:41.824466 superpowered-sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 justinclark   (501) staff       (20)     5136 2023-05-19 14:21:49.000000 superpowered-sdk-0.1.3/README.md
+-rw-r--r--   0 justinclark   (501) staff       (20)       38 2023-05-22 17:53:41.824872 superpowered-sdk-0.1.3/setup.cfg
+-rw-r--r--   0 justinclark   (501) staff       (20)     2225 2023-05-22 17:50:06.000000 superpowered-sdk-0.1.3/setup.py
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 17:53:41.821669 superpowered-sdk-0.1.3/superpowered/
+-rw-r--r--   0 justinclark   (501) staff       (20)      892 2023-05-22 17:50:01.000000 superpowered-sdk-0.1.3/superpowered/__init__.py
+-rw-r--r--   0 justinclark   (501) staff       (20)     1301 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.3/superpowered/exceptions.py
+-rw-r--r--   0 justinclark   (501) staff       (20)    11202 2023-05-22 17:50:01.000000 superpowered-sdk-0.1.3/superpowered/superpowered.py
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 17:53:41.823996 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/
+-rw-r--r--   0 justinclark   (501) staff       (20)     6636 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 justinclark   (501) staff       (20)      298 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)        1 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)       17 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/requires.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)       13 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.1.1/PKG-INFO` & `superpowered-sdk-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.1
+Version: 0.1.3
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
@@ -34,14 +34,16 @@
 
 # This is the official Superpowered AI Python SDK
 
 ## Installation
 
 `pip install superpowered-sdk`
 
+_Note_: To create API keys, please login to the Superpowered AI dashboard and click the "Account" tab on the left navigation.
+
 
 ## Knowledge Base Operations
 
 **Create a knowledge base**
 
 ```python
 kb = superpowered.create_knowledge_base(
@@ -192,11 +194,11 @@
     query='What technological advancements do need to construct a dyson sphere?',
     passages=[
         '<web page content',
         '<text content>',
         '<etc.>'
     ],
     top_k=10,                       # OPTIONAL
-    max_chunk_length=400,           # OPTIONAL
+    max_chunk_length=500,           # OPTIONAL
     summarize_results=True          # OPTIONAL
 )
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.3 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Keywords: Superpowered AI Knowledge base as a service for LLM
 applications Classifier: Development Status :: 4 - Beta Classifier: Environment
@@ -15,15 +15,17 @@
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Topic :: Database Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6 Description-Content-Type: text/markdown # This is the
 official Superpowered AI Python SDK ## Installation `pip install superpowered-
-sdk` ## Knowledge Base Operations **Create a knowledge base** ```python kb =
+sdk` _Note_: To create API keys, please login to the Superpowered AI dashboard
+and click the "Account" tab on the left navigation. ## Knowledge Base
+Operations **Create a knowledge base** ```python kb =
 superpowered.create_knowledge_base( title='research-biology',
 description='Papers, podcasts, and articles about biology.', # OPTIONAL
 supp_id='' # OPTIONAL ) # use kb['id'] when uploading documents for this
 knowledge base ``` **Get knowledge base(s)** ```python # list all knowledge
 bases kbs = superpowered.list_knowledge_bases() # returns list of kb objects #
 list knowledge bases that meet criteria kbs = superpowered.list_knowledge_bases
 (supp_id='') # OR kbs = superpowered.list_knowledge_bases
@@ -69,9 +71,9 @@
 without having to create a knowledge base** This functionality is perfect for
 web search applications like Google Chrome extensions. ```python # if passages
 are longer than `max_chunk_length`, we will chunk the passages to # make them
 more easily parsable by our model result = superpowered.query_passages
 ( query='What technological advancements do need to construct a dyson sphere?',
 passages=[ '
 , '', '
->' ], top_k=10, # OPTIONAL max_chunk_length=400, # OPTIONAL
+>' ], top_k=10, # OPTIONAL max_chunk_length=500, # OPTIONAL
 summarize_results=True # OPTIONAL ) ```
```

### Comparing `superpowered-sdk-0.1.1/README.md` & `superpowered-sdk-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This is the official Superpowered AI Python SDK
 
 ## Installation
 
 `pip install superpowered-sdk`
 
+_Note_: To create API keys, please login to the Superpowered AI dashboard and click the "Account" tab on the left navigation.
+
 
 ## Knowledge Base Operations
 
 **Create a knowledge base**
 
 ```python
 kb = superpowered.create_knowledge_base(
@@ -158,11 +160,11 @@
     query='What technological advancements do need to construct a dyson sphere?',
     passages=[
         '<web page content',
         '<text content>',
         '<etc.>'
     ],
     top_k=10,                       # OPTIONAL
-    max_chunk_length=400,           # OPTIONAL
+    max_chunk_length=500,           # OPTIONAL
     summarize_results=True          # OPTIONAL
 )
 ```
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
 # This is the official Superpowered AI Python SDK ## Installation `pip install
-superpowered-sdk` ## Knowledge Base Operations **Create a knowledge base**
-```python kb = superpowered.create_knowledge_base( title='research-biology',
+superpowered-sdk` _Note_: To create API keys, please login to the Superpowered
+AI dashboard and click the "Account" tab on the left navigation. ## Knowledge
+Base Operations **Create a knowledge base** ```python kb =
+superpowered.create_knowledge_base( title='research-biology',
 description='Papers, podcasts, and articles about biology.', # OPTIONAL
 supp_id='' # OPTIONAL ) # use kb['id'] when uploading documents for this
 knowledge base ``` **Get knowledge base(s)** ```python # list all knowledge
 bases kbs = superpowered.list_knowledge_bases() # returns list of kb objects #
 list knowledge bases that meet criteria kbs = superpowered.list_knowledge_bases
 (supp_id='') # OR kbs = superpowered.list_knowledge_bases
 (title_begins_with='research-') # get single knowledge base kb =
@@ -49,9 +51,9 @@
 without having to create a knowledge base** This functionality is perfect for
 web search applications like Google Chrome extensions. ```python # if passages
 are longer than `max_chunk_length`, we will chunk the passages to # make them
 more easily parsable by our model result = superpowered.query_passages
 ( query='What technological advancements do need to construct a dyson sphere?',
 passages=[ '
 , '', '
->' ], top_k=10, # OPTIONAL max_chunk_length=400, # OPTIONAL
+>' ], top_k=10, # OPTIONAL max_chunk_length=500, # OPTIONAL
 summarize_results=True # OPTIONAL ) ```
```

### Comparing `superpowered-sdk-0.1.1/setup.py` & `superpowered-sdk-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import os
 import setuptools
+import shutil
+
 
 long_desc = """# Superpowered AI
 Knowledge base as a service for LLM applications
 """
 
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname), "r", encoding="utf-8") as fh:
         return fh.read()
 
 
+# copy errors.json to the package directory
+DIR = os.path.dirname(os.path.abspath(__file__))
+shutil.copy(f'{DIR}/../../errors.json', f'{DIR}/superpowered/errors.json')
+
+
 setuptools.setup(
     name="superpowered-sdk",
     version=read("VERSION"),
     description="Superpowered AI SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

### Comparing `superpowered-sdk-0.1.1/superpowered/__init__.py` & `superpowered-sdk-0.1.3/superpowered/__init__.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.1/superpowered/exceptions.py` & `superpowered-sdk-0.1.3/superpowered/exceptions.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.1/superpowered/superpowered.py` & `superpowered-sdk-0.1.3/superpowered/superpowered.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.1/superpowered_sdk.egg-info/PKG-INFO` & `superpowered-sdk-0.1.3/superpowered_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.1
+Version: 0.1.3
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
@@ -34,14 +34,16 @@
 
 # This is the official Superpowered AI Python SDK
 
 ## Installation
 
 `pip install superpowered-sdk`
 
+_Note_: To create API keys, please login to the Superpowered AI dashboard and click the "Account" tab on the left navigation.
+
 
 ## Knowledge Base Operations
 
 **Create a knowledge base**
 
 ```python
 kb = superpowered.create_knowledge_base(
@@ -192,11 +194,11 @@
     query='What technological advancements do need to construct a dyson sphere?',
     passages=[
         '<web page content',
         '<text content>',
         '<etc.>'
     ],
     top_k=10,                       # OPTIONAL
-    max_chunk_length=400,           # OPTIONAL
+    max_chunk_length=500,           # OPTIONAL
     summarize_results=True          # OPTIONAL
 )
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.3 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Keywords: Superpowered AI Knowledge base as a service for LLM
 applications Classifier: Development Status :: 4 - Beta Classifier: Environment
@@ -15,15 +15,17 @@
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Topic :: Database Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6 Description-Content-Type: text/markdown # This is the
 official Superpowered AI Python SDK ## Installation `pip install superpowered-
-sdk` ## Knowledge Base Operations **Create a knowledge base** ```python kb =
+sdk` _Note_: To create API keys, please login to the Superpowered AI dashboard
+and click the "Account" tab on the left navigation. ## Knowledge Base
+Operations **Create a knowledge base** ```python kb =
 superpowered.create_knowledge_base( title='research-biology',
 description='Papers, podcasts, and articles about biology.', # OPTIONAL
 supp_id='' # OPTIONAL ) # use kb['id'] when uploading documents for this
 knowledge base ``` **Get knowledge base(s)** ```python # list all knowledge
 bases kbs = superpowered.list_knowledge_bases() # returns list of kb objects #
 list knowledge bases that meet criteria kbs = superpowered.list_knowledge_bases
 (supp_id='') # OR kbs = superpowered.list_knowledge_bases
@@ -69,9 +71,9 @@
 without having to create a knowledge base** This functionality is perfect for
 web search applications like Google Chrome extensions. ```python # if passages
 are longer than `max_chunk_length`, we will chunk the passages to # make them
 more easily parsable by our model result = superpowered.query_passages
 ( query='What technological advancements do need to construct a dyson sphere?',
 passages=[ '
 , '', '
->' ], top_k=10, # OPTIONAL max_chunk_length=400, # OPTIONAL
+>' ], top_k=10, # OPTIONAL max_chunk_length=500, # OPTIONAL
 summarize_results=True # OPTIONAL ) ```
```

