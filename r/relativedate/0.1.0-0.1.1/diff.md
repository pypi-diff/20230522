# Comparing `tmp/relativedate-0.1.0.tar.gz` & `tmp/relativedate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relativedate-0.1.0.tar", last modified: Mon May 22 15:30:32 2023, max compression
+gzip compressed data, was "relativedate-0.1.1.tar", last modified: Mon May 22 16:39:43 2023, max compression
```

## Comparing `relativedate-0.1.0.tar` & `relativedate-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 15:30:32.249988 relativedate-0.1.0/
--rw-rw-rw-   0        0        0      178 2023-05-22 15:30:32.248990 relativedate-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 15:30:32.226055 relativedate-0.1.0/relativedate/
--rw-rw-rw-   0        0        0     1115 2023-05-22 15:26:47.000000 relativedate-0.1.0/relativedate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:30:32.247993 relativedate-0.1.0/relativedate.egg-info/
--rw-rw-rw-   0        0        0      178 2023-05-22 15:30:31.000000 relativedate-0.1.0/relativedate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-22 15:30:32.000000 relativedate-0.1.0/relativedate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 15:30:31.000000 relativedate-0.1.0/relativedate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-22 15:30:31.000000 relativedate-0.1.0/relativedate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 15:30:32.250985 relativedate-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      278 2023-05-22 15:28:45.000000 relativedate-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:39:43.327487 relativedate-0.1.1/
+-rw-rw-rw-   0        0        0      178 2023-05-22 16:39:43.327487 relativedate-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-05-22 16:36:21.000000 relativedate-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 16:39:43.322500 relativedate-0.1.1/relativedate/
+-rw-rw-rw-   0        0        0     1115 2023-05-22 15:26:47.000000 relativedate-0.1.1/relativedate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:39:43.326497 relativedate-0.1.1/relativedate.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-05-22 16:39:43.000000 relativedate-0.1.1/relativedate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-05-22 16:39:43.000000 relativedate-0.1.1/relativedate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:39:43.000000 relativedate-0.1.1/relativedate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-22 16:39:43.000000 relativedate-0.1.1/relativedate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:39:43.327487 relativedate-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      278 2023-05-22 16:39:38.000000 relativedate-0.1.1/setup.py
```

### Comparing `relativedate-0.1.0/relativedate/__init__.py` & `relativedate-0.1.1/relativedate/__init__.py`

 * *Files identical despite different names*

