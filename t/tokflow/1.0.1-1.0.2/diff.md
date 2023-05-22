# Comparing `tmp/TokFlow-1.0.1.tar.gz` & `tmp/tokflow-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TokFlow-1.0.1.tar", last modified: Fri May 19 05:22:15 2023, max compression
+gzip compressed data, was "tokflow-1.0.2.tar", last modified: Mon May 22 02:52:46 2023, max compression
```

## Comparing `TokFlow-1.0.1.tar` & `tokflow-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 05:22:15.362028 TokFlow-1.0.1/
--rw-rw-rw-   0        0        0    11364 2023-05-19 04:51:42.000000 TokFlow-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4054 2023-05-19 05:22:15.351859 TokFlow-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3332 2023-05-19 05:20:51.000000 TokFlow-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 05:22:15.347845 TokFlow-1.0.1/TokFlow.egg-info/
--rw-rw-rw-   0        0        0     4054 2023-05-19 05:22:15.000000 TokFlow-1.0.1/TokFlow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-19 05:22:15.000000 TokFlow-1.0.1/TokFlow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 05:22:15.000000 TokFlow-1.0.1/TokFlow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 05:22:15.000000 TokFlow-1.0.1/TokFlow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 05:22:15.362028 TokFlow-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      896 2023-05-19 05:21:10.000000 TokFlow-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:22:15.350848 TokFlow-1.0.1/tokflow/
--rw-rw-rw-   0        0        0       72 2023-05-19 05:04:54.000000 TokFlow-1.0.1/tokflow/__init__.py
--rw-rw-rw-   0        0        0     9784 2023-05-19 04:51:42.000000 TokFlow-1.0.1/tokflow/tok_flow.py
--rw-rw-rw-   0        0        0     9059 2023-05-19 04:51:42.000000 TokFlow-1.0.1/tokflow/tok_flow_worker.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:52:46.328494 tokflow-1.0.2/
+-rw-rw-rw-   0        0        0    11364 2023-05-19 04:51:42.000000 tokflow-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4054 2023-05-22 02:52:46.328494 tokflow-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3332 2023-05-19 05:20:51.000000 tokflow-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 02:52:46.312326 tokflow-1.0.2/TokFlow.egg-info/
+-rw-rw-rw-   0        0        0     4054 2023-05-22 02:52:46.000000 tokflow-1.0.2/TokFlow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-22 02:52:46.000000 tokflow-1.0.2/TokFlow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 02:52:46.000000 tokflow-1.0.2/TokFlow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 02:52:46.000000 tokflow-1.0.2/TokFlow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 02:52:46.328494 tokflow-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-05-22 02:51:38.000000 tokflow-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:52:46.327494 tokflow-1.0.2/tokflow/
+-rw-rw-rw-   0        0        0       72 2023-05-19 05:04:54.000000 tokflow-1.0.2/tokflow/__init__.py
+-rw-rw-rw-   0        0        0     9784 2023-05-19 04:51:42.000000 tokflow-1.0.2/tokflow/tok_flow.py
+-rw-rw-rw-   0        0        0     9059 2023-05-19 04:51:42.000000 tokflow-1.0.2/tokflow/tok_flow_worker.py
```

### Comparing `TokFlow-1.0.1/LICENSE` & `tokflow-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TokFlow-1.0.1/PKG-INFO` & `tokflow-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TokFlow
-Version: 1.0.1
+Name: tokflow
+Version: 1.0.2
 Summary: LLM utility of streaming token realtime replacement processing
 Home-page: https://github.com/riversun/TokFlow
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TokFlow-1.0.1/README.md` & `tokflow-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `TokFlow-1.0.1/TokFlow.egg-info/PKG-INFO` & `tokflow-1.0.2/TokFlow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TokFlow
-Version: 1.0.1
+Name: tokflow
+Version: 1.0.2
 Summary: LLM utility of streaming token realtime replacement processing
 Home-page: https://github.com/riversun/TokFlow
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TokFlow-1.0.1/setup.py` & `tokflow-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="TokFlow",
-    version="1.0.1",
+    name="tokflow",
+    version="1.0.2",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="LLM utility of streaming token realtime replacement processing",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/TokFlow",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
-    tests_require=["pytest","httpx"],
+    tests_require=["pytest"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `TokFlow-1.0.1/tokflow/tok_flow.py` & `tokflow-1.0.2/tokflow/tok_flow.py`

 * *Files identical despite different names*

### Comparing `TokFlow-1.0.1/tokflow/tok_flow_worker.py` & `tokflow-1.0.2/tokflow/tok_flow_worker.py`

 * *Files identical despite different names*

