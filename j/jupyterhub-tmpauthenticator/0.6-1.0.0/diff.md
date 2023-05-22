# Comparing `tmp/jupyterhub-tmpauthenticator-0.6.tar.gz` & `tmp/jupyterhub-tmpauthenticator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterhub-tmpauthenticator-0.6.tar", last modified: Sat May 18 22:31:38 2019, max compression
+gzip compressed data, was "jupyterhub-tmpauthenticator-1.0.0.tar", last modified: Mon May 22 14:06:27 2023, max compression
```

## Comparing `jupyterhub-tmpauthenticator-0.6.tar` & `jupyterhub-tmpauthenticator-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxr-x   0 yuvipanda  (1000) yuvipanda  (1000)        0 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/
--rw-rw-r--   0 yuvipanda  (1000) yuvipanda  (1000)     1528 2019-05-18 22:26:52.000000 jupyterhub-tmpauthenticator-0.6/LICENSE
--rw-rw-r--   0 yuvipanda  (1000) yuvipanda  (1000)       34 2019-05-18 22:26:52.000000 jupyterhub-tmpauthenticator-0.6/MANIFEST.in
--rw-rw-r--   0 yuvipanda  (1000) yuvipanda  (1000)      322 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/PKG-INFO
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)      735 2017-05-04 22:34:38.000000 jupyterhub-tmpauthenticator-0.6/README.md
-drwxrwxr-x   0 yuvipanda  (1000) yuvipanda  (1000)        0 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/jupyterhub_tmpauthenticator.egg-info/
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)      322 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/jupyterhub_tmpauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)      271 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/jupyterhub_tmpauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)        1 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/jupyterhub_tmpauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)       17 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/jupyterhub_tmpauthenticator.egg-info/top_level.txt
--rw-rw-r--   0 yuvipanda  (1000) yuvipanda  (1000)       38 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/setup.cfg
--rw-rw-r--   0 yuvipanda  (1000) yuvipanda  (1000)      383 2019-05-18 22:30:47.000000 jupyterhub-tmpauthenticator-0.6/setup.py
-drwxrwxr-x   0 yuvipanda  (1000) yuvipanda  (1000)        0 2019-05-18 22:31:38.000000 jupyterhub-tmpauthenticator-0.6/tmpauthenticator/
--rw-rw-r--   0 yuvipanda  (1000) yuvipanda  (1000)     2776 2019-05-18 22:30:31.000000 jupyterhub-tmpauthenticator-0.6/tmpauthenticator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:27.465742 jupyterhub-tmpauthenticator-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-22 14:06:13.000000 jupyterhub-tmpauthenticator-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 14:06:13.000000 jupyterhub-tmpauthenticator-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-22 14:06:27.465742 jupyterhub-tmpauthenticator-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-22 14:06:13.000000 jupyterhub-tmpauthenticator-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:27.461742 jupyterhub-tmpauthenticator-1.0.0/jupyterhub_tmpauthenticator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-22 14:06:27.000000 jupyterhub-tmpauthenticator-1.0.0/jupyterhub_tmpauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-22 14:06:27.000000 jupyterhub-tmpauthenticator-1.0.0/jupyterhub_tmpauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:06:27.000000 jupyterhub-tmpauthenticator-1.0.0/jupyterhub_tmpauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 14:06:27.000000 jupyterhub-tmpauthenticator-1.0.0/jupyterhub_tmpauthenticator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 14:06:27.000000 jupyterhub-tmpauthenticator-1.0.0/jupyterhub_tmpauthenticator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 14:06:27.000000 jupyterhub-tmpauthenticator-1.0.0/jupyterhub_tmpauthenticator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-22 14:06:13.000000 jupyterhub-tmpauthenticator-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:06:27.465742 jupyterhub-tmpauthenticator-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 14:06:13.000000 jupyterhub-tmpauthenticator-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:27.465742 jupyterhub-tmpauthenticator-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-22 14:06:13.000000 jupyterhub-tmpauthenticator-1.0.0/tests/test_tmpauthenticator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:27.465742 jupyterhub-tmpauthenticator-1.0.0/tmpauthenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-22 14:06:13.000000 jupyterhub-tmpauthenticator-1.0.0/tmpauthenticator/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jupyterhub-tmpauthenticator-0.6/LICENSE` & `jupyterhub-tmpauthenticator-1.0.0/LICENSE`

 * *Files identical despite different names*

