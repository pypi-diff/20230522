# Comparing `tmp/tree-of-thoughts-0.1.2.tar.gz` & `tmp/tree-of-thoughts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.1.2.tar", last modified: Mon May 22 02:08:33 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.1.3.tar", last modified: Mon May 22 12:13:22 2023, max compression
```

## Comparing `tree-of-thoughts-0.1.2.tar` & `tree-of-thoughts-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:08:33.365486 tree-of-thoughts-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 02:08:20.000000 tree-of-thoughts-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 02:08:33.365486 tree-of-thoughts-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-05-22 02:08:20.000000 tree-of-thoughts-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:08:33.365486 tree-of-thoughts-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-22 02:08:20.000000 tree-of-thoughts-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:08:33.365486 tree-of-thoughts-0.1.2/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 02:08:20.000000 tree-of-thoughts-0.1.2/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-05-22 02:08:20.000000 tree-of-thoughts-0.1.2/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:08:33.365486 tree-of-thoughts-0.1.2/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 02:08:33.000000 tree-of-thoughts-0.1.2/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 02:08:33.000000 tree-of-thoughts-0.1.2/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:08:33.000000 tree-of-thoughts-0.1.2/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 02:08:33.000000 tree-of-thoughts-0.1.2/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 02:08:33.000000 tree-of-thoughts-0.1.2/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-05-22 12:13:07.000000 tree-of-thoughts-0.1.3/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:13:22.749392 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 12:13:22.000000 tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.1.2/LICENSE` & `tree-of-thoughts-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.1.2/PKG-INFO` & `tree-of-thoughts-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.1.2/README.md` & `tree-of-thoughts-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 This implementation of Tree of Thoughts is brought to you by Agora, Agora advances Humanity with open source SOTA Multi-Modality AI research! We plan on combating Humanity's grandest root problems like food insecurity, planetary insecurity, and disease, and hopefully death itself.
 
 [Join our Discord and contribute to this project](https://discord.gg/qUtxnK2NMf)
 
 ## Getting started
 Clone this repository with ```git clone https://github.com/kyegomez/tree-of-thoughts```
 
+or:
+
+```pip install tree-of-thoughts ```
+
+
 Navigate to the repository folder: ``` cd tree-of-thoughts```
 
 ```pip install openai```
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
```

### Comparing `tree-of-thoughts-0.1.2/setup.py` & `tree-of-thoughts-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.1.2',
+  version = '0.1.3',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.1.2/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.1.3/tree_of_thoughts/treeofthoughts.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.1.2/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.1.3/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

