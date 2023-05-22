# Comparing `tmp/dyrun-1.1.1.tar.gz` & `tmp/dyrun-1.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyrun-1.1.1.tar", last modified: Mon May 22 16:32:43 2023, max compression
+gzip compressed data, was "dyrun-1.1.11.tar", last modified: Mon May 22 16:37:50 2023, max compression
```

## Comparing `dyrun-1.1.1.tar` & `dyrun-1.1.11.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.523192 dyrun-1.1.1/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       25 2023-05-22 08:23:25.000000 dyrun-1.1.1/MANIFEST.in
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    19444 2023-05-22 16:32:43.523192 dyrun-1.1.1/PKG-INFO
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    16588 2023-05-22 16:32:01.000000 dyrun-1.1.1/README.md
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.503192 dyrun-1.1.1/dyrun/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:46.000000 dyrun-1.1.1/dyrun/__init__.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.507192 dyrun-1.1.1/dyrun/blocks/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      379 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/blocks/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:54.000000 dyrun-1.1.1/dyrun/blocks/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7286 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/blocks/comp_neuro_blocks.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     8524 2023-05-22 06:56:27.000000 dyrun-1.1.1/dyrun/blocks/general_blocks.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      696 2023-05-22 10:21:41.000000 dyrun-1.1.1/dyrun/cli.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.507192 dyrun-1.1.1/dyrun/core/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      613 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:00.000000 dyrun-1.1.1/dyrun/core/__init__.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.511192 dyrun-1.1.1/dyrun/core/caller/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:06:24.000000 dyrun-1.1.1/dyrun/core/caller/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    32865 2023-05-22 06:57:20.000000 dyrun-1.1.1/dyrun/core/caller/dynamic_engine.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    22507 2023-05-22 06:57:56.000000 dyrun-1.1.1/dyrun/core/caller/scope_engine.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.511192 dyrun-1.1.1/dyrun/core/lib/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    41720 2023-05-22 14:00:06.000000 dyrun-1.1.1/dyrun/core/lib/core_library.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.519192 dyrun-1.1.1/dyrun/core/lib/eclib/
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     4108 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/README.md
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      183 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/__init__.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1957 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/dyn_elgamal.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     7406 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/elgamal.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)    13247 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/gsw.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1908 2023-05-22 15:30:26.000000 dyrun-1.1.1/dyrun/core/lib/eclib/gsw_lwe.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      592 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/modutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      722 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/numutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9140 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/paillier.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      913 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/primeutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      531 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/core/lib/eclib/randutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9334 2023-05-22 15:29:03.000000 dyrun-1.1.1/dyrun/core/lib/eclib/regev.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    13761 2023-05-22 07:47:03.000000 dyrun-1.1.1/dyrun/core/lib/required_libraries.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.519192 dyrun-1.1.1/dyrun/data/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      181 2023-05-22 16:18:45.000000 dyrun-1.1.1/dyrun/data/README.md
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.523192 dyrun-1.1.1/dyrun/data/inputs/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      323 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/data/inputs/README.md
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.523192 dyrun-1.1.1/dyrun/data/outputs/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      256 2023-05-21 19:36:38.000000 dyrun-1.1.1/dyrun/data/outputs/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    10905 2023-05-22 15:49:16.000000 dyrun-1.1.1/dyrun/dyrun.ipynb
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7214 2023-05-22 12:30:30.000000 dyrun-1.1.1/dyrun/dyrun.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:32:43.507192 dyrun-1.1.1/dyrun.egg-info/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    19444 2023-05-22 16:32:43.000000 dyrun-1.1.1/dyrun.egg-info/PKG-INFO
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1090 2023-05-22 16:32:43.000000 dyrun-1.1.1/dyrun.egg-info/SOURCES.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        1 2023-05-22 16:32:43.000000 dyrun-1.1.1/dyrun.egg-info/dependency_links.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       51 2023-05-22 16:32:43.000000 dyrun-1.1.1/dyrun.egg-info/entry_points.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       58 2023-05-22 16:32:43.000000 dyrun-1.1.1/dyrun.egg-info/requires.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        6 2023-05-22 16:32:43.000000 dyrun-1.1.1/dyrun.egg-info/top_level.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       38 2023-05-22 16:32:43.523192 dyrun-1.1.1/setup.cfg
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      997 2023-05-22 16:31:40.000000 dyrun-1.1.1/setup.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.122364 dyrun-1.1.11/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       25 2023-05-22 08:23:25.000000 dyrun-1.1.11/MANIFEST.in
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    19441 2023-05-22 16:37:50.122364 dyrun-1.1.11/PKG-INFO
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    16584 2023-05-22 16:36:46.000000 dyrun-1.1.11/README.md
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.114364 dyrun-1.1.11/dyrun/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:46.000000 dyrun-1.1.11/dyrun/__init__.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.114364 dyrun-1.1.11/dyrun/blocks/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      379 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/blocks/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:54.000000 dyrun-1.1.11/dyrun/blocks/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7286 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/blocks/comp_neuro_blocks.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     8524 2023-05-22 06:56:27.000000 dyrun-1.1.11/dyrun/blocks/general_blocks.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      696 2023-05-22 10:21:41.000000 dyrun-1.1.11/dyrun/cli.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.114364 dyrun-1.1.11/dyrun/core/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      613 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:00.000000 dyrun-1.1.11/dyrun/core/__init__.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.114364 dyrun-1.1.11/dyrun/core/caller/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:06:24.000000 dyrun-1.1.11/dyrun/core/caller/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    32865 2023-05-22 06:57:20.000000 dyrun-1.1.11/dyrun/core/caller/dynamic_engine.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    22507 2023-05-22 06:57:56.000000 dyrun-1.1.11/dyrun/core/caller/scope_engine.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.118364 dyrun-1.1.11/dyrun/core/lib/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    41720 2023-05-22 14:00:06.000000 dyrun-1.1.11/dyrun/core/lib/core_library.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.118364 dyrun-1.1.11/dyrun/core/lib/eclib/
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     4108 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/README.md
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      183 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/__init__.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1957 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/dyn_elgamal.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     7406 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/elgamal.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)    13247 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/gsw.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1908 2023-05-22 15:30:26.000000 dyrun-1.1.11/dyrun/core/lib/eclib/gsw_lwe.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      592 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/modutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      722 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/numutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9140 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/paillier.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      913 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/primeutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      531 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/core/lib/eclib/randutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9334 2023-05-22 15:29:03.000000 dyrun-1.1.11/dyrun/core/lib/eclib/regev.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    13761 2023-05-22 07:47:03.000000 dyrun-1.1.11/dyrun/core/lib/required_libraries.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.118364 dyrun-1.1.11/dyrun/data/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      181 2023-05-22 16:18:45.000000 dyrun-1.1.11/dyrun/data/README.md
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.118364 dyrun-1.1.11/dyrun/data/inputs/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      323 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/data/inputs/README.md
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.118364 dyrun-1.1.11/dyrun/data/outputs/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      256 2023-05-21 19:36:38.000000 dyrun-1.1.11/dyrun/data/outputs/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    10905 2023-05-22 15:49:16.000000 dyrun-1.1.11/dyrun/dyrun.ipynb
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7214 2023-05-22 12:30:30.000000 dyrun-1.1.11/dyrun/dyrun.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 16:37:50.114364 dyrun-1.1.11/dyrun.egg-info/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    19441 2023-05-22 16:37:49.000000 dyrun-1.1.11/dyrun.egg-info/PKG-INFO
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1090 2023-05-22 16:37:50.000000 dyrun-1.1.11/dyrun.egg-info/SOURCES.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        1 2023-05-22 16:37:49.000000 dyrun-1.1.11/dyrun.egg-info/dependency_links.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       47 2023-05-22 16:37:49.000000 dyrun-1.1.11/dyrun.egg-info/entry_points.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       58 2023-05-22 16:37:49.000000 dyrun-1.1.11/dyrun.egg-info/requires.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        6 2023-05-22 16:37:49.000000 dyrun-1.1.11/dyrun.egg-info/top_level.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       38 2023-05-22 16:37:50.122364 dyrun-1.1.11/setup.cfg
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      993 2023-05-22 16:36:19.000000 dyrun-1.1.11/setup.py
```

### Comparing `dyrun-1.1.1/PKG-INFO` & `dyrun-1.1.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyrun
-Version: 1.1.1
+Version: 1.1.11
 Summary: Easy way to simulation
 Home-page: https://github.com/abolfazldelavar/dyrun
 Author: Abolfazl Delavar
 Author-email: faryadell@gmail.com
 License: MIT
 Description: <img src="https://github.com/abolfazldelavar/dyrun/blob/main/logo.png?raw=true" align="right" width="300" alt="header pic"/>
         
@@ -40,15 +40,15 @@
         ```
         pip install dyrun
         ```
         
         To build a new project, just run the following order:
         
         ```
-        dyrun new DIR_NAME
+        dyrun DIR_NAME
         ```
         
         If the package has been installed, you can update it by:
         
         ```
         pip install --upgrade dyrun
         ```
```

### Comparing `dyrun-1.1.1/README.md` & `dyrun-1.1.11/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ```
 pip install dyrun
 ```
 
 To build a new project, just run the following order:
 
 ```
-dyrun new DIR_NAME
+dyrun DIR_NAME
 ```
 
 If the package has been installed, you can update it by:
 
 ```
 pip install --upgrade dyrun
 ```
```

### Comparing `dyrun-1.1.1/dyrun/blocks/comp_neuro_blocks.py` & `dyrun-1.1.11/dyrun/blocks/comp_neuro_blocks.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/blocks/general_blocks.py` & `dyrun-1.1.11/dyrun/blocks/general_blocks.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/cli.py` & `dyrun-1.1.11/dyrun/cli.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/README.md` & `dyrun-1.1.11/dyrun/core/README.md`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/caller/dynamic_engine.py` & `dyrun-1.1.11/dyrun/core/caller/dynamic_engine.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/caller/scope_engine.py` & `dyrun-1.1.11/dyrun/core/caller/scope_engine.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/core_library.py` & `dyrun-1.1.11/dyrun/core/lib/core_library.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/README.md` & `dyrun-1.1.11/dyrun/core/lib/eclib/README.md`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/dyn_elgamal.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/dyn_elgamal.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/elgamal.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/elgamal.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/gsw.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/gsw.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/gsw_lwe.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/gsw_lwe.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/modutils.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/modutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/numutils.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/numutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/paillier.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/paillier.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/primeutils.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/primeutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/randutils.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/randutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/eclib/regev.py` & `dyrun-1.1.11/dyrun/core/lib/eclib/regev.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/core/lib/required_libraries.py` & `dyrun-1.1.11/dyrun/core/lib/required_libraries.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/dyrun.ipynb` & `dyrun-1.1.11/dyrun/dyrun.ipynb`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun/dyrun.py` & `dyrun-1.1.11/dyrun/dyrun.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/dyrun.egg-info/PKG-INFO` & `dyrun-1.1.11/dyrun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyrun
-Version: 1.1.1
+Version: 1.1.11
 Summary: Easy way to simulation
 Home-page: https://github.com/abolfazldelavar/dyrun
 Author: Abolfazl Delavar
 Author-email: faryadell@gmail.com
 License: MIT
 Description: <img src="https://github.com/abolfazldelavar/dyrun/blob/main/logo.png?raw=true" align="right" width="300" alt="header pic"/>
         
@@ -40,15 +40,15 @@
         ```
         pip install dyrun
         ```
         
         To build a new project, just run the following order:
         
         ```
-        dyrun new DIR_NAME
+        dyrun DIR_NAME
         ```
         
         If the package has been installed, you can update it by:
         
         ```
         pip install --upgrade dyrun
         ```
```

### Comparing `dyrun-1.1.1/dyrun.egg-info/SOURCES.txt` & `dyrun-1.1.11/dyrun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyrun-1.1.1/setup.py` & `dyrun-1.1.11/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'dyrun',
-    version = '1.1.01',
+    version = '1.1.11',
     author = 'Abolfazl Delavar',
     author_email = 'faryadell@gmail.com',
     description = 'Easy way to simulation',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/abolfazldelavar/dyrun',
     packages = find_packages(),
@@ -18,11 +18,11 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires = '>=3.6',
     include_package_data = True,
     entry_points = {
         'console_scripts': [
-            'dyrun new=dyrun.cli:build_cmd'
+            'dyrun=dyrun.cli:build_cmd'
         ]
     }
 )
```

