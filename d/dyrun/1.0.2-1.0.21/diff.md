# Comparing `tmp/dyrun-1.0.2.tar.gz` & `tmp/dyrun-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyrun-1.0.2.tar", last modified: Mon May 22 08:34:35 2023, max compression
+gzip compressed data, was "dyrun-1.0.21.tar", last modified: Mon May 22 08:49:02 2023, max compression
```

## Comparing `dyrun-1.0.2.tar` & `dyrun-1.0.21.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.207407 dyrun-1.0.2/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       25 2023-05-22 08:23:25.000000 dyrun-1.0.2/MANIFEST.in
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1744 2023-05-22 08:34:35.207407 dyrun-1.0.2/PKG-INFO
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     2281 2023-05-22 07:00:51.000000 dyrun-1.0.2/README.md
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.187406 dyrun-1.0.2/dyrun/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:46.000000 dyrun-1.0.2/dyrun/__init__.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.191407 dyrun-1.0.2/dyrun/blocks/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      379 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/blocks/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:54.000000 dyrun-1.0.2/dyrun/blocks/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7286 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/blocks/comp_neuro_blocks.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     8524 2023-05-22 06:56:27.000000 dyrun-1.0.2/dyrun/blocks/general_blocks.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.191407 dyrun-1.0.2/dyrun/core/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      613 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:00.000000 dyrun-1.0.2/dyrun/core/__init__.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.195407 dyrun-1.0.2/dyrun/core/caller/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:06:24.000000 dyrun-1.0.2/dyrun/core/caller/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    32865 2023-05-22 06:57:20.000000 dyrun-1.0.2/dyrun/core/caller/dynamic_engine.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    22507 2023-05-22 06:57:56.000000 dyrun-1.0.2/dyrun/core/caller/scope_engine.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.195407 dyrun-1.0.2/dyrun/core/lib/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    41730 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/core_library.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.199406 dyrun-1.0.2/dyrun/core/lib/eclib/
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     4108 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/README.md
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      183 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/__init__.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1957 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/dyn_elgamal.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     7406 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/elgamal.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)    13247 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/gsw.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1856 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/gsw_lwe.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      592 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/modutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      722 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/numutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9140 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/paillier.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      913 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/primeutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      531 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/randutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9298 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/core/lib/eclib/regev.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    13761 2023-05-22 07:47:03.000000 dyrun-1.0.2/dyrun/core/lib/required_libraries.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.203407 dyrun-1.0.2/dyrun/data/
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.203407 dyrun-1.0.2/dyrun/data/inputs/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      323 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/data/inputs/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)   495021 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/data/logo.png
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.203407 dyrun-1.0.2/dyrun/data/outputs/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      256 2023-05-21 19:36:38.000000 dyrun-1.0.2/dyrun/data/outputs/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    10907 2023-05-21 19:38:34.000000 dyrun-1.0.2/dyrun/dyrun.ipynb
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7219 2023-05-21 19:38:20.000000 dyrun-1.0.2/dyrun/dyrun.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:34:35.191407 dyrun-1.0.2/dyrun.egg-info/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1744 2023-05-22 08:34:35.000000 dyrun-1.0.2/dyrun.egg-info/PKG-INFO
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1044 2023-05-22 08:34:35.000000 dyrun-1.0.2/dyrun.egg-info/SOURCES.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        1 2023-05-22 08:34:35.000000 dyrun-1.0.2/dyrun.egg-info/dependency_links.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       42 2023-05-22 08:34:35.000000 dyrun-1.0.2/dyrun.egg-info/requires.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        6 2023-05-22 08:34:35.000000 dyrun-1.0.2/dyrun.egg-info/top_level.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       38 2023-05-22 08:34:35.207407 dyrun-1.0.2/setup.cfg
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1306 2023-05-22 08:34:22.000000 dyrun-1.0.2/setup.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.212793 dyrun-1.0.21/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       25 2023-05-22 08:23:25.000000 dyrun-1.0.21/MANIFEST.in
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1745 2023-05-22 08:49:02.212793 dyrun-1.0.21/PKG-INFO
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     2281 2023-05-22 07:00:51.000000 dyrun-1.0.21/README.md
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.200793 dyrun-1.0.21/dyrun/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:46.000000 dyrun-1.0.21/dyrun/__init__.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.200793 dyrun-1.0.21/dyrun/blocks/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      379 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/blocks/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:54.000000 dyrun-1.0.21/dyrun/blocks/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7286 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/blocks/comp_neuro_blocks.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     8524 2023-05-22 06:56:27.000000 dyrun-1.0.21/dyrun/blocks/general_blocks.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.204794 dyrun-1.0.21/dyrun/core/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      613 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:00.000000 dyrun-1.0.21/dyrun/core/__init__.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.204794 dyrun-1.0.21/dyrun/core/caller/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:06:24.000000 dyrun-1.0.21/dyrun/core/caller/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    32865 2023-05-22 06:57:20.000000 dyrun-1.0.21/dyrun/core/caller/dynamic_engine.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    22507 2023-05-22 06:57:56.000000 dyrun-1.0.21/dyrun/core/caller/scope_engine.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.204794 dyrun-1.0.21/dyrun/core/lib/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    41730 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/core_library.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.208793 dyrun-1.0.21/dyrun/core/lib/eclib/
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     4108 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/README.md
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      183 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/__init__.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1957 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/dyn_elgamal.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     7406 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/elgamal.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)    13247 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/gsw.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1856 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/gsw_lwe.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      592 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/modutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      722 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/numutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9140 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/paillier.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      913 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/primeutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      531 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/randutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9298 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/core/lib/eclib/regev.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    13761 2023-05-22 07:47:03.000000 dyrun-1.0.21/dyrun/core/lib/required_libraries.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.208793 dyrun-1.0.21/dyrun/data/
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.212793 dyrun-1.0.21/dyrun/data/inputs/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      323 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/data/inputs/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)   495021 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/data/logo.png
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.212793 dyrun-1.0.21/dyrun/data/outputs/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      256 2023-05-21 19:36:38.000000 dyrun-1.0.21/dyrun/data/outputs/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    10907 2023-05-21 19:38:34.000000 dyrun-1.0.21/dyrun/dyrun.ipynb
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7219 2023-05-21 19:38:20.000000 dyrun-1.0.21/dyrun/dyrun.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 08:49:02.200793 dyrun-1.0.21/dyrun.egg-info/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1745 2023-05-22 08:49:02.000000 dyrun-1.0.21/dyrun.egg-info/PKG-INFO
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1044 2023-05-22 08:49:02.000000 dyrun-1.0.21/dyrun.egg-info/SOURCES.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        1 2023-05-22 08:49:02.000000 dyrun-1.0.21/dyrun.egg-info/dependency_links.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       52 2023-05-22 08:49:02.000000 dyrun-1.0.21/dyrun.egg-info/requires.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        6 2023-05-22 08:49:02.000000 dyrun-1.0.21/dyrun.egg-info/top_level.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       38 2023-05-22 08:49:02.212793 dyrun-1.0.21/setup.cfg
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      983 2023-05-22 08:48:51.000000 dyrun-1.0.21/setup.py
```

### Comparing `dyrun-1.0.2/PKG-INFO` & `dyrun-1.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyrun
-Version: 1.0.2
+Version: 1.0.21
 Summary: Easy way to simulation
 Home-page: https://github.com/abolfazldelavar/dyrun
 Author: Abolfazl Delavar
 Author-email: faryadell@gmail.com
 License: MIT License
 
 Copyright (c) 2023, Abolfazl Delavar, all rights reserved.
```

### Comparing `dyrun-1.0.2/README.md` & `dyrun-1.0.21/README.md`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/blocks/comp_neuro_blocks.py` & `dyrun-1.0.21/dyrun/blocks/comp_neuro_blocks.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/blocks/general_blocks.py` & `dyrun-1.0.21/dyrun/blocks/general_blocks.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/README.md` & `dyrun-1.0.21/dyrun/core/README.md`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/caller/dynamic_engine.py` & `dyrun-1.0.21/dyrun/core/caller/dynamic_engine.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/caller/scope_engine.py` & `dyrun-1.0.21/dyrun/core/caller/scope_engine.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/core_library.py` & `dyrun-1.0.21/dyrun/core/lib/core_library.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/README.md` & `dyrun-1.0.21/dyrun/core/lib/eclib/README.md`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/dyn_elgamal.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/dyn_elgamal.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/elgamal.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/elgamal.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/gsw.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/gsw.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/gsw_lwe.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/gsw_lwe.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/modutils.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/modutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/numutils.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/numutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/paillier.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/paillier.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/primeutils.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/primeutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/randutils.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/randutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/eclib/regev.py` & `dyrun-1.0.21/dyrun/core/lib/eclib/regev.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/core/lib/required_libraries.py` & `dyrun-1.0.21/dyrun/core/lib/required_libraries.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/data/logo.png` & `dyrun-1.0.21/dyrun/data/logo.png`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/dyrun.ipynb` & `dyrun-1.0.21/dyrun/dyrun.ipynb`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun/dyrun.py` & `dyrun-1.0.21/dyrun/dyrun.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.2/dyrun.egg-info/PKG-INFO` & `dyrun-1.0.21/dyrun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyrun
-Version: 1.0.2
+Version: 1.0.21
 Summary: Easy way to simulation
 Home-page: https://github.com/abolfazldelavar/dyrun
 Author: Abolfazl Delavar
 Author-email: faryadell@gmail.com
 License: MIT License
 
 Copyright (c) 2023, Abolfazl Delavar, all rights reserved.
```

### Comparing `dyrun-1.0.2/dyrun.egg-info/SOURCES.txt` & `dyrun-1.0.21/dyrun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

