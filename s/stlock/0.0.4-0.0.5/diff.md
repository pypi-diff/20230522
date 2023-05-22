# Comparing `tmp/stlock-0.0.4.tar.gz` & `tmp/stlock-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlock-0.0.4.tar", last modified: Mon May 22 19:06:00 2023, max compression
+gzip compressed data, was "stlock-0.0.5.tar", last modified: Mon May 22 19:44:39 2023, max compression
```

## Comparing `stlock-0.0.4.tar` & `stlock-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:06:00.166790 stlock-0.0.4/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      103 2023-05-22 19:06:00.166790 stlock-0.0.4/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-22 19:06:00.166790 stlock-0.0.4/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-22 19:05:58.000000 stlock-0.0.4/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:06:00.166790 stlock-0.0.4/stlock/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.4/stlock/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2149 2023-05-22 17:38:41.000000 stlock-0.0.4/stlock/stlock.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:06:00.166790 stlock-0.0.4/stlock.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      103 2023-05-22 19:06:00.000000 stlock-0.0.4/stlock.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      232 2023-05-22 19:06:00.000000 stlock-0.0.4/stlock.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 19:06:00.000000 stlock-0.0.4/stlock.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.4/stlock.egg-info/not-zip-safe
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-22 19:06:00.000000 stlock-0.0.4/stlock.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-22 19:06:00.000000 stlock-0.0.4/stlock.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:44:39.084804 stlock-0.0.5/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3238 2023-05-22 19:44:39.084804 stlock-0.0.5/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3093 2023-05-22 19:40:10.000000 stlock-0.0.5/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-22 19:44:39.084804 stlock-0.0.5/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      402 2023-05-22 19:44:34.000000 stlock-0.0.5/setup.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:44:39.084804 stlock-0.0.5/stlock/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.5/stlock/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2149 2023-05-22 17:38:41.000000 stlock-0.0.5/stlock/stlock.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:44:39.084804 stlock-0.0.5/stlock.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3238 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.5/stlock.egg-info/not-zip-safe
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/top_level.txt
```

### Comparing `stlock-0.0.4/stlock/stlock.py` & `stlock-0.0.5/stlock/stlock.py`

 * *Files identical despite different names*

