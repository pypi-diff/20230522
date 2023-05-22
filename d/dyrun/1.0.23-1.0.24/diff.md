# Comparing `tmp/dyrun-1.0.23.tar.gz` & `tmp/dyrun-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyrun-1.0.23.tar", last modified: Mon May 22 10:25:21 2023, max compression
+gzip compressed data, was "dyrun-1.0.24.tar", last modified: Mon May 22 12:06:17 2023, max compression
```

## Comparing `dyrun-1.0.23.tar` & `dyrun-1.0.24.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.979932 dyrun-1.0.23/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       25 2023-05-22 08:23:25.000000 dyrun-1.0.23/MANIFEST.in
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1745 2023-05-22 10:25:21.979932 dyrun-1.0.23/PKG-INFO
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     2281 2023-05-22 07:00:51.000000 dyrun-1.0.23/README.md
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.955931 dyrun-1.0.23/dyrun/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:46.000000 dyrun-1.0.23/dyrun/__init__.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.959931 dyrun-1.0.23/dyrun/blocks/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      379 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/blocks/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:54.000000 dyrun-1.0.23/dyrun/blocks/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7286 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/blocks/comp_neuro_blocks.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     8524 2023-05-22 06:56:27.000000 dyrun-1.0.23/dyrun/blocks/general_blocks.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      696 2023-05-22 10:21:41.000000 dyrun-1.0.23/dyrun/cli.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.963931 dyrun-1.0.23/dyrun/core/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      613 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:00.000000 dyrun-1.0.23/dyrun/core/__init__.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.963931 dyrun-1.0.23/dyrun/core/caller/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:06:24.000000 dyrun-1.0.23/dyrun/core/caller/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    32865 2023-05-22 06:57:20.000000 dyrun-1.0.23/dyrun/core/caller/dynamic_engine.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    22507 2023-05-22 06:57:56.000000 dyrun-1.0.23/dyrun/core/caller/scope_engine.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.967931 dyrun-1.0.23/dyrun/core/lib/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/__init__.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    41730 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/core_library.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.975932 dyrun-1.0.23/dyrun/core/lib/eclib/
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     4108 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/README.md
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      183 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/__init__.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1957 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/dyn_elgamal.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     7406 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/elgamal.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)    13247 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/gsw.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1856 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/gsw_lwe.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      592 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/modutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      722 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/numutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9140 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/paillier.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      913 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/primeutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      531 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/randutils.py
--rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9298 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/core/lib/eclib/regev.py
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    13761 2023-05-22 07:47:03.000000 dyrun-1.0.23/dyrun/core/lib/required_libraries.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.975932 dyrun-1.0.23/dyrun/data/
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.975932 dyrun-1.0.23/dyrun/data/inputs/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      323 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/data/inputs/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)   495021 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/data/logo.png
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.975932 dyrun-1.0.23/dyrun/data/outputs/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      256 2023-05-21 19:36:38.000000 dyrun-1.0.23/dyrun/data/outputs/README.md
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    10907 2023-05-21 19:38:34.000000 dyrun-1.0.23/dyrun/dyrun.ipynb
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7219 2023-05-21 19:38:20.000000 dyrun-1.0.23/dyrun/dyrun.py
-drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 10:25:21.959931 dyrun-1.0.23/dyrun.egg-info/
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1745 2023-05-22 10:25:21.000000 dyrun-1.0.23/dyrun.egg-info/PKG-INFO
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1089 2023-05-22 10:25:21.000000 dyrun-1.0.23/dyrun.egg-info/SOURCES.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        1 2023-05-22 10:25:21.000000 dyrun-1.0.23/dyrun.egg-info/dependency_links.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       47 2023-05-22 10:25:21.000000 dyrun-1.0.23/dyrun.egg-info/entry_points.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       58 2023-05-22 10:25:21.000000 dyrun-1.0.23/dyrun.egg-info/requires.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        6 2023-05-22 10:25:21.000000 dyrun-1.0.23/dyrun.egg-info/top_level.txt
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       38 2023-05-22 10:25:21.979932 dyrun-1.0.23/setup.cfg
--rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1099 2023-05-22 10:25:11.000000 dyrun-1.0.23/setup.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.954318 dyrun-1.0.24/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       25 2023-05-22 08:23:25.000000 dyrun-1.0.24/MANIFEST.in
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     3440 2023-05-22 12:06:17.954318 dyrun-1.0.24/PKG-INFO
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     2439 2023-05-22 10:39:18.000000 dyrun-1.0.24/README.md
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.942318 dyrun-1.0.24/dyrun/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:46.000000 dyrun-1.0.24/dyrun/__init__.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.946318 dyrun-1.0.24/dyrun/blocks/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      379 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/blocks/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:54.000000 dyrun-1.0.24/dyrun/blocks/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7286 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/blocks/comp_neuro_blocks.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     8524 2023-05-22 06:56:27.000000 dyrun-1.0.24/dyrun/blocks/general_blocks.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      696 2023-05-22 10:21:41.000000 dyrun-1.0.24/dyrun/cli.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.946318 dyrun-1.0.24/dyrun/core/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      613 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:07:00.000000 dyrun-1.0.24/dyrun/core/__init__.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.946318 dyrun-1.0.24/dyrun/core/caller/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-22 08:06:24.000000 dyrun-1.0.24/dyrun/core/caller/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    32865 2023-05-22 06:57:20.000000 dyrun-1.0.24/dyrun/core/caller/dynamic_engine.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    22507 2023-05-22 06:57:56.000000 dyrun-1.0.24/dyrun/core/caller/scope_engine.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.946318 dyrun-1.0.24/dyrun/core/lib/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      279 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/__init__.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    41730 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/core_library.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.950318 dyrun-1.0.24/dyrun/core/lib/eclib/
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     4108 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/README.md
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      183 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/__init__.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1957 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/dyn_elgamal.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     7406 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/elgamal.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)    13247 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/gsw.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     1856 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/gsw_lwe.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      592 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/modutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      722 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/numutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9140 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/paillier.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      913 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/primeutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)      531 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/randutils.py
+-rwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)     9298 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/core/lib/eclib/regev.py
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    13761 2023-05-22 07:47:03.000000 dyrun-1.0.24/dyrun/core/lib/required_libraries.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.950318 dyrun-1.0.24/dyrun/data/
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.950318 dyrun-1.0.24/dyrun/data/inputs/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      323 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/data/inputs/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)   495021 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/data/logo.png
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.954318 dyrun-1.0.24/dyrun/data/outputs/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      256 2023-05-21 19:36:38.000000 dyrun-1.0.24/dyrun/data/outputs/README.md
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)    10913 2023-05-22 10:39:46.000000 dyrun-1.0.24/dyrun/dyrun.ipynb
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     7225 2023-05-22 10:39:57.000000 dyrun-1.0.24/dyrun/dyrun.py
+drwxrwxr-x   0 abolfazl  (1000) abolfazl  (1000)        0 2023-05-22 12:06:17.946318 dyrun-1.0.24/dyrun.egg-info/
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     3440 2023-05-22 12:06:17.000000 dyrun-1.0.24/dyrun.egg-info/PKG-INFO
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)     1089 2023-05-22 12:06:17.000000 dyrun-1.0.24/dyrun.egg-info/SOURCES.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        1 2023-05-22 12:06:17.000000 dyrun-1.0.24/dyrun.egg-info/dependency_links.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       47 2023-05-22 12:06:17.000000 dyrun-1.0.24/dyrun.egg-info/entry_points.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       58 2023-05-22 12:06:17.000000 dyrun-1.0.24/dyrun.egg-info/requires.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)        6 2023-05-22 12:06:17.000000 dyrun-1.0.24/dyrun.egg-info/top_level.txt
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)       38 2023-05-22 12:06:17.954318 dyrun-1.0.24/setup.cfg
+-rw-rw-r--   0 abolfazl  (1000) abolfazl  (1000)      993 2023-05-22 12:05:12.000000 dyrun-1.0.24/setup.py
```

### Comparing `dyrun-1.0.23/README.md` & `dyrun-1.0.24/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="https://github.com/abolfazldelavar/dyrun/blob/main/data/logo.png?raw=true" align="right" width="300" alt="header pic"/>
+<img src="https://github.com/abolfazldelavar/dyrun/blob/main/dyrun/data/logo.png?raw=true" align="right" width="300" alt="header pic"/>
 
 # Dynamic Runner (DYRUN)
 
 This Python-based basement environment is designed for simulating dynamical systems, including differential equations, and visualizing their results, which can be particularly useful for academic research and paper presentations. `dyrun` is a simple tool that facilitates simulations expeditiously and effortlessly, using invaluable instruments for modeling linear and nonlinear dynamic systems. This formidable instrument is capable of executing **differential mathematical equations** [1] and is advantageous for
 
 * **Control engineering**,
 * **Estimation** [2, 3],
@@ -23,17 +23,23 @@
 
 "*Successful people are those who can build solid foundations with the bricks others throw at them.*"
 
 # Instructions
 
 ## Installation
 
-To download full package, run the below code:
+To install the full package, run the below code:
 
-`Comming soon ...`
+`pip install dyrun`
+
+To build a new project, just run the following order:
+
+`dyrun DIR_NAME`
+
+where the **DIR_NAME** denotes the folder you wish to create the project.
 
 ## First trying
 
 ...
 
 
 # References
```

### Comparing `dyrun-1.0.23/dyrun/blocks/comp_neuro_blocks.py` & `dyrun-1.0.24/dyrun/blocks/comp_neuro_blocks.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/blocks/general_blocks.py` & `dyrun-1.0.24/dyrun/blocks/general_blocks.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/cli.py` & `dyrun-1.0.24/dyrun/cli.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/README.md` & `dyrun-1.0.24/dyrun/core/README.md`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/caller/dynamic_engine.py` & `dyrun-1.0.24/dyrun/core/caller/dynamic_engine.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/caller/scope_engine.py` & `dyrun-1.0.24/dyrun/core/caller/scope_engine.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/core_library.py` & `dyrun-1.0.24/dyrun/core/lib/core_library.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/README.md` & `dyrun-1.0.24/dyrun/core/lib/eclib/README.md`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/dyn_elgamal.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/dyn_elgamal.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/elgamal.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/elgamal.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/gsw.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/gsw.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/gsw_lwe.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/gsw_lwe.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/modutils.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/modutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/numutils.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/numutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/paillier.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/paillier.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/primeutils.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/primeutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/randutils.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/randutils.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/eclib/regev.py` & `dyrun-1.0.24/dyrun/core/lib/eclib/regev.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/core/lib/required_libraries.py` & `dyrun-1.0.24/dyrun/core/lib/required_libraries.py`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/data/logo.png` & `dyrun-1.0.24/dyrun/data/logo.png`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/dyrun/dyrun.ipynb` & `dyrun-1.0.24/dyrun/dyrun.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998553240740741%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '<img "*

 * *            'src="https://github.com/abolfazldelavar/dyrun/blob/main/dyrun/data/logo.png?raw=true" '*

 * *            'align="right" width="250" alt="header pic"/>\\n\')], delete: [0]}}}'}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<img src=\"https://github.com/abolfazldelavar/dyrun/blob/main/data/logo.png?raw=true\" align=\"right\" width=\"250\" alt=\"header pic\"/>\n",
+                "<img src=\"https://github.com/abolfazldelavar/dyrun/blob/main/dyrun/data/logo.png?raw=true\" align=\"right\" width=\"250\" alt=\"header pic\"/>\n",
                 "\n",
                 "# DYNAMIC RUNNER\n",
                 "**Dynamic Runner** or `dyrun` is a simple tool that facilitates simulations expeditiously and effortlessly, using invaluable instruments for modeling linear and nonlinear dynamic systems, irrespective of their time dependence or independence. This formidable instrument is capable of executing **dynamic mathematical models** and is advantageous for control engineering applications, estimation, and prediction. Moreover, it is applicable to Machine Learning and AI domains, including neural networks. Researchers who wish to delve into the realm of dynamic and control systems will find this package to be an invaluable resource. Enjoy!\n",
                 "\n",
                 "https://github.com/abolfazldelavar/dyrun\n",
                 "\n",
                 "\"*Successful people are those who can build solid foundations with the bricks others throw at them.*\"\n"
```

### Comparing `dyrun-1.0.23/dyrun/dyrun.py` & `dyrun-1.0.24/dyrun/dyrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/env python
 
 # %% [markdown]
-# <img src="https://github.com/abolfazldelavar/dyrun/blob/main/data/logo.png?raw=true" align="right" width="250" alt="header pic"/>
+# <img src="https://github.com/abolfazldelavar/dyrun/blob/main/dyrun/data/logo.png?raw=true" align="right" width="250" alt="header pic"/>
 # 
 # # DYNAMIC RUNNER
 # **Dynamic Runner** or `dyrun` is a simple tool that facilitates simulations expeditiously and effortlessly, using invaluable instruments for modeling linear and nonlinear dynamic systems, irrespective of their time dependence or independence. This formidable instrument is capable of executing **dynamic mathematical models** and is advantageous for control engineering applications, estimation, and prediction. Moreover, it is applicable to Machine Learning and AI domains, including neural networks. Researchers who wish to delve into the realm of dynamic and control systems will find this package to be an invaluable resource. Enjoy!
 # 
 # https://github.com/abolfazldelavar/dyrun
 # 
 # "*Successful people are those who can build solid foundations with the bricks others throw at them.*"
```

### Comparing `dyrun-1.0.23/dyrun.egg-info/SOURCES.txt` & `dyrun-1.0.24/dyrun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyrun-1.0.23/setup.py` & `dyrun-1.0.24/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'dyrun',
-    version = '1.0.23',
+    version = '1.0.24',
     author = 'Abolfazl Delavar',
     author_email = 'faryadell@gmail.com',
     description = 'Easy way to simulation',
-    long_description = 'DYRUN is a simple tool that facilitates dynamic simulations and illustration expeditiously and effortlessly.',
+    long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/abolfazldelavar/dyrun',
     packages = find_packages(),
-    license = open('LICENSE.md').read(),
+    license = 'MIT',
     install_requires = ['numpy', 'pandas', 'matplotlib', 'control', 'pyqt5', 'opencv-python', 'click'],
     keywords=['Control', 'Simulation', 'Academic', 'Mathematics', 'Differential', 'Closed-loop', 'Numberical calculation'],
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

