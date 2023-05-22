# Comparing `tmp/relativedate-0.1.0.tar.gz` & `tmp/relativedate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relativedate-0.1.0.tar", last modified: Mon May 22 15:30:32 2023, max compression
+gzip compressed data, was "relativedate-0.1.2.tar", last modified: Mon May 22 16:57:32 2023, max compression
```

## Comparing `relativedate-0.1.0.tar` & `relativedate-0.1.2.tar`

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
+drwxrwxrwx   0        0        0        0 2023-05-22 16:57:32.157441 relativedate-0.1.2/
+-rw-rw-rw-   0        0        0     1353 2023-05-22 16:57:32.155445 relativedate-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-05-22 16:36:21.000000 relativedate-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 16:57:32.136496 relativedate-0.1.2/relativedate/
+-rw-rw-rw-   0        0        0     1115 2023-05-22 15:26:47.000000 relativedate-0.1.2/relativedate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:57:32.154450 relativedate-0.1.2/relativedate.egg-info/
+-rw-rw-rw-   0        0        0     1353 2023-05-22 16:57:31.000000 relativedate-0.1.2/relativedate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-05-22 16:57:32.000000 relativedate-0.1.2/relativedate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:57:31.000000 relativedate-0.1.2/relativedate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-22 16:57:31.000000 relativedate-0.1.2/relativedate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:57:32.158443 relativedate-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-05-22 16:57:26.000000 relativedate-0.1.2/setup.py
```

### Comparing `relativedate-0.1.0/relativedate/__init__.py` & `relativedate-0.1.2/relativedate/__init__.py`

 * *Files identical despite different names*

