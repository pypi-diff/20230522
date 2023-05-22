# Comparing `tmp/cellmaps_coembedding-0.1.0a2.tar.gz` & `tmp/cellmaps_coembedding-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_coembedding-0.1.0a2.tar", last modified: Sat May 20 00:24:07 2023, max compression
+gzip compressed data, was "dist/cellmaps_coembedding-0.1.0a3.tar", last modified: Mon May 22 19:42:03 2023, max compression
```

## Comparing `cellmaps_coembedding-0.1.0a2.tar` & `cellmaps_coembedding-0.1.0a3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.275880 cellmaps_coembedding-0.1.0a2/
--rw-r--r--   0 churas     (504) staff       (20)      165 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3679 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 18:46:09.000000 cellmaps_coembedding-0.1.0a2/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6037 2023-05-20 00:24:07.276007 cellmaps_coembedding-0.1.0a2/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3941 2023-05-19 18:48:13.000000 cellmaps_coembedding-0.1.0a2/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.267329 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/
--rw-r--r--   0 churas     (504) staff       (20)      339 2023-05-20 00:18:02.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     7814 2023-05-19 20:52:55.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/cellmaps_coembeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      138 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/exceptions.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.270014 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/
--rw-r--r--   0 churas     (504) staff       (20)    13872 2023-05-18 21:57:55.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     3530 2023-05-03 00:16:38.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/architecture.py
--rw-r--r--   0 churas     (504) staff       (20)     3697 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/df_utils.py
--rw-r--r--   0 churas     (504) staff       (20)     1186 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/file_utils.py
--rw-r--r--   0 churas     (504) staff       (20)    11301 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/triplet_loss.py
--rw-r--r--   0 churas     (504) staff       (20)    18970 2023-05-20 00:21:44.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.268958 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6037 2023-05-20 00:24:07.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1372 2023-05-20 00:24:07.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-20 00:24:07.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-20 00:24:07.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       66 2023-05-20 00:24:07.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       21 2023-05-20 00:24:07.000000 cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.273909 cellmaps_coembedding-0.1.0a2/docs/
--rw-r--r--   0 churas     (504) staff       (20)      622 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.262502 cellmaps_coembedding-0.1.0a2/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.262691 cellmaps_coembedding-0.1.0a2/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.274526 cellmaps_coembedding-0.1.0a2/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a2/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a2/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a2/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1086 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a2/docs/cellmaps_coembedding.muse_sc.rst
--rw-r--r--   0 churas     (504) staff       (20)      877 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a2/docs/cellmaps_coembedding.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6062 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      288 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      955 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1216 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      460 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4376 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      790 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      709 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a2/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a2/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      403 2023-05-20 00:24:07.277012 cellmaps_coembedding-0.1.0a2/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2370 2023-05-19 18:48:26.000000 cellmaps_coembedding-0.1.0a2/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:24:07.275705 cellmaps_coembedding-0.1.0a2/tests/
--rw-r--r--   0 churas     (504) staff       (20)       75 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a2/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     2551 2023-05-09 23:51:08.000000 cellmaps_coembedding-0.1.0a2/tests/test_cellmaps_coembeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      911 2023-05-09 21:38:49.000000 cellmaps_coembedding-0.1.0a2/tests/test_cellmapscoembedder.py
--rw-r--r--   0 churas     (504) staff       (20)     2441 2023-05-09 23:46:41.000000 cellmaps_coembedding-0.1.0a2/tests/test_imagembeddingfilterandnametranslator.py
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 00:02:48.000000 cellmaps_coembedding-0.1.0a2/tests/test_integration_cellmaps_coembedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.176320 cellmaps_coembedding-0.1.0a3/
+-rw-r--r--   0 churas     (504) staff       (20)      165 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3679 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 18:46:09.000000 cellmaps_coembedding-0.1.0a3/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6037 2023-05-22 19:42:03.176449 cellmaps_coembedding-0.1.0a3/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3941 2023-05-19 18:48:13.000000 cellmaps_coembedding-0.1.0a3/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.166644 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/
+-rw-r--r--   0 churas     (504) staff       (20)      339 2023-05-22 19:37:29.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     7814 2023-05-19 20:52:55.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/cellmaps_coembeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      138 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/exceptions.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.169330 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/
+-rw-r--r--   0 churas     (504) staff       (20)    13872 2023-05-18 21:57:55.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     3530 2023-05-03 00:16:38.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/architecture.py
+-rw-r--r--   0 churas     (504) staff       (20)     3697 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/df_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)     1186 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/file_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)    11301 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/triplet_loss.py
+-rw-r--r--   0 churas     (504) staff       (20)    18991 2023-05-22 19:37:29.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.167964 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6037 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1372 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       66 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       21 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.174151 cellmaps_coembedding-0.1.0a3/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      622 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.163529 cellmaps_coembedding-0.1.0a3/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.163597 cellmaps_coembedding-0.1.0a3/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.174965 cellmaps_coembedding-0.1.0a3/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a3/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1086 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a3/docs/cellmaps_coembedding.muse_sc.rst
+-rw-r--r--   0 churas     (504) staff       (20)      877 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a3/docs/cellmaps_coembedding.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6062 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      288 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      955 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1216 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      460 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4376 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      790 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      709 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      403 2023-05-22 19:42:03.177497 cellmaps_coembedding-0.1.0a3/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2370 2023-05-19 18:48:26.000000 cellmaps_coembedding-0.1.0a3/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.176138 cellmaps_coembedding-0.1.0a3/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       75 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a3/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     2551 2023-05-09 23:51:08.000000 cellmaps_coembedding-0.1.0a3/tests/test_cellmaps_coembeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      911 2023-05-09 21:38:49.000000 cellmaps_coembedding-0.1.0a3/tests/test_cellmapscoembedder.py
+-rw-r--r--   0 churas     (504) staff       (20)     2441 2023-05-09 23:46:41.000000 cellmaps_coembedding-0.1.0a3/tests/test_imagembeddingfilterandnametranslator.py
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 00:02:48.000000 cellmaps_coembedding-0.1.0a3/tests/test_integration_cellmaps_coembedding.py
```

### Comparing `cellmaps_coembedding-0.1.0a2/CONTRIBUTING.rst` & `cellmaps_coembedding-0.1.0a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/LICENSE` & `cellmaps_coembedding-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/PKG-INFO` & `cellmaps_coembedding-0.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_coembedding
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A tool to generate coembeddings from IF image embeddings and PPI network embeddings
 Home-page: https://github.com/idekerlab/cellmaps_coembedding
 Author: Leah Schaffer
 Author-email: lvschaffer@health.ucsd.edu
 License: MIT license
 Description: ==================
         CM4AI CoEmbedding
```

### Comparing `cellmaps_coembedding-0.1.0a2/README.rst` & `cellmaps_coembedding-0.1.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/cellmaps_coembeddingcmd.py` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/cellmaps_coembeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/__init__.py` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/__init__.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/architecture.py` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/architecture.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/df_utils.py` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/df_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/file_utils.py` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/file_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/muse_sc/triplet_loss.py` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding/runner.py` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,15 +429,15 @@
         """
         logger.debug('Getting id of input rocrate')
         used_dataset = []
         for entry in self._inputdirs:
             used_dataset.append(self._provenance_utils.get_id_of_rocrate(entry))
         self._provenance_utils.register_computation(self._outdir,
                                                     name=cellmaps_coembedding.__name__ + ' computation',
-                                                    run_by=str(os.getlogin()),
+                                                    run_by=str(self._provenance_utils.get_login()),
                                                     command=str(self._input_data_dict),
                                                     description='run of ' + cellmaps_coembedding.__name__,
                                                     used_software=[self._softwareid],
                                                     used_dataset=used_dataset,
                                                     generated=[self._coembedding_id])
 
     def _register_image_coembedding_file(self):
```

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/PKG-INFO` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-coembedding
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A tool to generate coembeddings from IF image embeddings and PPI network embeddings
 Home-page: https://github.com/idekerlab/cellmaps_coembedding
 Author: Leah Schaffer
 Author-email: lvschaffer@health.ucsd.edu
 License: MIT license
 Description: ==================
         CM4AI CoEmbedding
```

### Comparing `cellmaps_coembedding-0.1.0a2/cellmaps_coembedding.egg-info/SOURCES.txt` & `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/Makefile` & `cellmaps_coembedding-0.1.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/cellmaps_coembedding.muse_sc.rst` & `cellmaps_coembedding-0.1.0a3/docs/cellmaps_coembedding.muse_sc.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/cellmaps_coembedding.rst` & `cellmaps_coembedding-0.1.0a3/docs/cellmaps_coembedding.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/conf.py` & `cellmaps_coembedding-0.1.0a3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/index.rst` & `cellmaps_coembedding-0.1.0a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/installation.rst` & `cellmaps_coembedding-0.1.0a3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/make.bat` & `cellmaps_coembedding-0.1.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/newrelease.rst` & `cellmaps_coembedding-0.1.0a3/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/pypircfile.rst` & `cellmaps_coembedding-0.1.0a3/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/usage.rst` & `cellmaps_coembedding-0.1.0a3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/docs/versioningscheme.rst` & `cellmaps_coembedding-0.1.0a3/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/setup.py` & `cellmaps_coembedding-0.1.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/tests/test_cellmaps_coembeddingcmd.py` & `cellmaps_coembedding-0.1.0a3/tests/test_cellmaps_coembeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/tests/test_cellmapscoembedder.py` & `cellmaps_coembedding-0.1.0a3/tests/test_cellmapscoembedder.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/tests/test_imagembeddingfilterandnametranslator.py` & `cellmaps_coembedding-0.1.0a3/tests/test_imagembeddingfilterandnametranslator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a2/tests/test_integration_cellmaps_coembedding.py` & `cellmaps_coembedding-0.1.0a3/tests/test_integration_cellmaps_coembedding.py`

 * *Files identical despite different names*

