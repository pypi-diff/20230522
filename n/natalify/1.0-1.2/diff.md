# Comparing `tmp/natalify-1.0.tar.gz` & `tmp/natalify-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natalify-1.0.tar", last modified: Mon May 22 10:18:51 2023, max compression
+gzip compressed data, was "natalify-1.2.tar", last modified: Mon May 22 10:33:29 2023, max compression
```

## Comparing `natalify-1.0.tar` & `natalify-1.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:18:51.555838 natalify-1.0/
--rw-rw-rw-   0        0        0      749 2023-05-22 10:18:51.555838 natalify-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 10:18:51.540233 natalify-1.0/natalify/
--rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-1.0/natalify/__init__.py
--rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-1.0/natalify/__main__.py
--rw-rw-rw-   0        0        0    63371 2023-05-22 10:12:00.000000 natalify-1.0/natalify/natalify.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:18:51.555838 natalify-1.0/natalify.egg-info/
--rw-rw-rw-   0        0        0      749 2023-05-22 10:18:49.000000 natalify-1.0/natalify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-22 10:18:51.000000 natalify-1.0/natalify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:18:49.000000 natalify-1.0/natalify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-22 10:18:50.000000 natalify-1.0/natalify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 10:18:50.000000 natalify-1.0/natalify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:18:51.555838 natalify-1.0/setup.cfg
--rw-rw-rw-   0        0        0      990 2023-05-22 10:18:29.000000 natalify-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:33:29.499461 natalify-1.2/
+-rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-1.2/LICENSE
+-rw-rw-rw-   0        0        0     1859 2023-05-22 10:33:29.499461 natalify-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-05-22 10:31:58.000000 natalify-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 10:33:29.483831 natalify-1.2/natalify/
+-rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-1.2/natalify/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-1.2/natalify/__main__.py
+-rw-rw-rw-   0        0        0    63371 2023-05-22 10:12:00.000000 natalify-1.2/natalify/natalify.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:33:29.499461 natalify-1.2/natalify.egg-info/
+-rw-rw-rw-   0        0        0     1859 2023-05-22 10:33:29.000000 natalify-1.2/natalify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-22 10:33:29.000000 natalify-1.2/natalify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:33:29.000000 natalify-1.2/natalify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-22 10:33:29.000000 natalify-1.2/natalify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 10:33:29.000000 natalify-1.2/natalify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:33:29.499461 natalify-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-05-22 10:32:41.000000 natalify-1.2/setup.py
```

### Comparing `natalify-1.0/natalify/natalify.py` & `natalify-1.2/natalify/natalify.py`

 * *Files identical despite different names*

