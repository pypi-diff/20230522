# Comparing `tmp/AdaptiveConsistency-0.0.1.tar.gz` & `tmp/AdaptiveConsistency-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdaptiveConsistency-0.0.1.tar", last modified: Mon May 22 18:13:16 2023, max compression
+gzip compressed data, was "AdaptiveConsistency-1.0.0.tar", last modified: Mon May 22 18:20:08 2023, max compression
```

## Comparing `AdaptiveConsistency-0.0.1.tar` & `AdaptiveConsistency-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hackear   (1000) hackear   (1000)        0 2023-05-22 18:13:16.493208 AdaptiveConsistency-0.0.1/
-drwxr-xr-x   0 hackear   (1000) hackear   (1000)        0 2023-05-22 18:13:16.493208 AdaptiveConsistency-0.0.1/AdaptiveConsistency.egg-info/
--rw-r--r--   0 hackear   (1000) hackear   (1000)     6160 2023-05-22 18:13:16.000000 AdaptiveConsistency-0.0.1/AdaptiveConsistency.egg-info/PKG-INFO
--rw-r--r--   0 hackear   (1000) hackear   (1000)      303 2023-05-22 18:13:16.000000 AdaptiveConsistency-0.0.1/AdaptiveConsistency.egg-info/SOURCES.txt
--rw-r--r--   0 hackear   (1000) hackear   (1000)        1 2023-05-22 18:13:16.000000 AdaptiveConsistency-0.0.1/AdaptiveConsistency.egg-info/dependency_links.txt
--rw-r--r--   0 hackear   (1000) hackear   (1000)       21 2023-05-22 18:13:16.000000 AdaptiveConsistency-0.0.1/AdaptiveConsistency.egg-info/top_level.txt
--rw-r--r--   0 hackear   (1000) hackear   (1000)     1073 2023-05-09 13:58:15.000000 AdaptiveConsistency-0.0.1/LICENSE
--rw-r--r--   0 hackear   (1000) hackear   (1000)     6160 2023-05-22 18:13:16.493208 AdaptiveConsistency-0.0.1/PKG-INFO
--rw-r--r--   0 hackear   (1000) hackear   (1000)     5928 2023-05-22 18:09:01.000000 AdaptiveConsistency-0.0.1/README.md
-drwxr-xr-x   0 hackear   (1000) hackear   (1000)        0 2023-05-22 18:13:16.493208 AdaptiveConsistency-0.0.1/adaptive_consistency/
--rw-r--r--   0 hackear   (1000) hackear   (1000)      336 2023-05-22 13:00:50.000000 AdaptiveConsistency-0.0.1/adaptive_consistency/__init__.py
--rw-r--r--   0 hackear   (1000) hackear   (1000)     4696 2023-05-22 12:42:35.000000 AdaptiveConsistency-0.0.1/adaptive_consistency/main.py
--rw-r--r--   0 hackear   (1000) hackear   (1000)     8403 2023-05-22 12:42:20.000000 AdaptiveConsistency-0.0.1/adaptive_consistency/stopping_criterias.py
--rw-r--r--   0 hackear   (1000) hackear   (1000)       38 2023-05-22 18:13:16.493208 AdaptiveConsistency-0.0.1/setup.cfg
--rw-r--r--   0 hackear   (1000) hackear   (1000)      477 2023-05-22 18:12:49.000000 AdaptiveConsistency-0.0.1/setup.py
+drwxr-xr-x   0 hackear   (1000) hackear   (1000)        0 2023-05-22 18:20:08.123208 AdaptiveConsistency-1.0.0/
+drwxr-xr-x   0 hackear   (1000) hackear   (1000)        0 2023-05-22 18:20:08.123208 AdaptiveConsistency-1.0.0/AdaptiveConsistency.egg-info/
+-rw-r--r--   0 hackear   (1000) hackear   (1000)     6157 2023-05-22 18:20:07.000000 AdaptiveConsistency-1.0.0/AdaptiveConsistency.egg-info/PKG-INFO
+-rw-r--r--   0 hackear   (1000) hackear   (1000)      303 2023-05-22 18:20:08.000000 AdaptiveConsistency-1.0.0/AdaptiveConsistency.egg-info/SOURCES.txt
+-rw-r--r--   0 hackear   (1000) hackear   (1000)        1 2023-05-22 18:20:07.000000 AdaptiveConsistency-1.0.0/AdaptiveConsistency.egg-info/dependency_links.txt
+-rw-r--r--   0 hackear   (1000) hackear   (1000)       21 2023-05-22 18:20:07.000000 AdaptiveConsistency-1.0.0/AdaptiveConsistency.egg-info/top_level.txt
+-rw-r--r--   0 hackear   (1000) hackear   (1000)     1073 2023-05-09 13:58:15.000000 AdaptiveConsistency-1.0.0/LICENSE
+-rw-r--r--   0 hackear   (1000) hackear   (1000)     6157 2023-05-22 18:20:08.123208 AdaptiveConsistency-1.0.0/PKG-INFO
+-rw-r--r--   0 hackear   (1000) hackear   (1000)     5925 2023-05-22 18:17:10.000000 AdaptiveConsistency-1.0.0/README.md
+drwxr-xr-x   0 hackear   (1000) hackear   (1000)        0 2023-05-22 18:20:08.123208 AdaptiveConsistency-1.0.0/adaptive_consistency/
+-rw-r--r--   0 hackear   (1000) hackear   (1000)      336 2023-05-22 13:00:50.000000 AdaptiveConsistency-1.0.0/adaptive_consistency/__init__.py
+-rw-r--r--   0 hackear   (1000) hackear   (1000)     4696 2023-05-22 12:42:35.000000 AdaptiveConsistency-1.0.0/adaptive_consistency/main.py
+-rw-r--r--   0 hackear   (1000) hackear   (1000)     8403 2023-05-22 12:42:20.000000 AdaptiveConsistency-1.0.0/adaptive_consistency/stopping_criterias.py
+-rw-r--r--   0 hackear   (1000) hackear   (1000)       38 2023-05-22 18:20:08.123208 AdaptiveConsistency-1.0.0/setup.cfg
+-rw-r--r--   0 hackear   (1000) hackear   (1000)      477 2023-05-22 18:18:04.000000 AdaptiveConsistency-1.0.0/setup.py
```

### Comparing `AdaptiveConsistency-0.0.1/AdaptiveConsistency.egg-info/PKG-INFO` & `AdaptiveConsistency-1.0.0/AdaptiveConsistency.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: AdaptiveConsistency
-Version: 0.0.1
+Version: 1.0.0
 Summary: Library for running AdapativeConsistency based Inference on large language models.
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Let's Sample Step by Step: Adaptive-Consistency for Efficient Reasoning with LLMs
 
 <p align="center">
   <a href="http://sample-step-by-step.info/">Website</a> •
   <a href="https://arxiv.org/abs/2305.11860">Paper</a> 
 </p>
 
 
 <p align="center">
-    <a href="https://github.com/Pranjal2041/Adaptive-Consistency/blob/master/LICENSE">
-            <img src="https://img.shields.io/github/license/Pranjal2041/Adaptive-Consistency.svg"
+    <a href="https://github.com/Pranjal2041/AdaptiveConsistency/blob/master/LICENSE">
+            <img src="https://img.shields.io/github/license/Pranjal2041/AdaptiveConsistency.svg"
                 alt="GitHub license">
     </a>
-    <a href="https://twitter.com/intent/tweet?text=Check%20out%20Adaptive-Consistency%3A%20https%3A%2F%2Fgithub.com%2Fpranjal2041%2FAdaptiveeConsistency">
+    <a href="https://twitter.com/intent/tweet?text=Check%20out%20AdaptiveConsistency%3A%20https%3A%2F%2Fgithub.com%2Fpranjal2041%2FAdaptiveeConsistency">
     <img src="https://img.shields.io/twitter/url/https/github.com/Pranjal2041/AdaptiveConsistency.svg?style=social" alt="Twitter">
     </a>      
 </p>
 
 
 
 <!-- <br> -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AdaptiveConsistency Version: 0.0.1 Summary: Library
+Metadata-Version: 2.1 Name: AdaptiveConsistency Version: 1.0.0 Summary: Library
 for running AdapativeConsistency based Inference on large language models.
 License: MIT Description-Content-Type: text/markdown License-File: LICENSE #
 Let's Sample Step by Step: Adaptive-Consistency for Efficient Reasoning with
 LLMs
                                Website â¢ Paper
                           [GitHub_license] [Twitter]
  [Pranjal Aggarwal](https://github.com/Pranjal2041), [Aman Madaan](https://
```

### Comparing `AdaptiveConsistency-0.0.1/LICENSE` & `AdaptiveConsistency-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AdaptiveConsistency-0.0.1/PKG-INFO` & `AdaptiveConsistency-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: AdaptiveConsistency
-Version: 0.0.1
+Version: 1.0.0
 Summary: Library for running AdapativeConsistency based Inference on large language models.
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Let's Sample Step by Step: Adaptive-Consistency for Efficient Reasoning with LLMs
 
 <p align="center">
   <a href="http://sample-step-by-step.info/">Website</a> •
   <a href="https://arxiv.org/abs/2305.11860">Paper</a> 
 </p>
 
 
 <p align="center">
-    <a href="https://github.com/Pranjal2041/Adaptive-Consistency/blob/master/LICENSE">
-            <img src="https://img.shields.io/github/license/Pranjal2041/Adaptive-Consistency.svg"
+    <a href="https://github.com/Pranjal2041/AdaptiveConsistency/blob/master/LICENSE">
+            <img src="https://img.shields.io/github/license/Pranjal2041/AdaptiveConsistency.svg"
                 alt="GitHub license">
     </a>
-    <a href="https://twitter.com/intent/tweet?text=Check%20out%20Adaptive-Consistency%3A%20https%3A%2F%2Fgithub.com%2Fpranjal2041%2FAdaptiveeConsistency">
+    <a href="https://twitter.com/intent/tweet?text=Check%20out%20AdaptiveConsistency%3A%20https%3A%2F%2Fgithub.com%2Fpranjal2041%2FAdaptiveeConsistency">
     <img src="https://img.shields.io/twitter/url/https/github.com/Pranjal2041/AdaptiveConsistency.svg?style=social" alt="Twitter">
     </a>      
 </p>
 
 
 
 <!-- <br> -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AdaptiveConsistency Version: 0.0.1 Summary: Library
+Metadata-Version: 2.1 Name: AdaptiveConsistency Version: 1.0.0 Summary: Library
 for running AdapativeConsistency based Inference on large language models.
 License: MIT Description-Content-Type: text/markdown License-File: LICENSE #
 Let's Sample Step by Step: Adaptive-Consistency for Efficient Reasoning with
 LLMs
                                Website â¢ Paper
                           [GitHub_license] [Twitter]
  [Pranjal Aggarwal](https://github.com/Pranjal2041), [Aman Madaan](https://
```

### Comparing `AdaptiveConsistency-0.0.1/README.md` & `AdaptiveConsistency-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 <p align="center">
   <a href="http://sample-step-by-step.info/">Website</a> •
   <a href="https://arxiv.org/abs/2305.11860">Paper</a> 
 </p>
 
 
 <p align="center">
-    <a href="https://github.com/Pranjal2041/Adaptive-Consistency/blob/master/LICENSE">
-            <img src="https://img.shields.io/github/license/Pranjal2041/Adaptive-Consistency.svg"
+    <a href="https://github.com/Pranjal2041/AdaptiveConsistency/blob/master/LICENSE">
+            <img src="https://img.shields.io/github/license/Pranjal2041/AdaptiveConsistency.svg"
                 alt="GitHub license">
     </a>
-    <a href="https://twitter.com/intent/tweet?text=Check%20out%20Adaptive-Consistency%3A%20https%3A%2F%2Fgithub.com%2Fpranjal2041%2FAdaptiveeConsistency">
+    <a href="https://twitter.com/intent/tweet?text=Check%20out%20AdaptiveConsistency%3A%20https%3A%2F%2Fgithub.com%2Fpranjal2041%2FAdaptiveeConsistency">
     <img src="https://img.shields.io/twitter/url/https/github.com/Pranjal2041/AdaptiveConsistency.svg?style=social" alt="Twitter">
     </a>      
 </p>
 
 
 
 <!-- <br> -->
```

### Comparing `AdaptiveConsistency-0.0.1/adaptive_consistency/main.py` & `AdaptiveConsistency-1.0.0/adaptive_consistency/main.py`

 * *Files identical despite different names*

### Comparing `AdaptiveConsistency-0.0.1/adaptive_consistency/stopping_criterias.py` & `AdaptiveConsistency-1.0.0/adaptive_consistency/stopping_criterias.py`

 * *Files identical despite different names*

