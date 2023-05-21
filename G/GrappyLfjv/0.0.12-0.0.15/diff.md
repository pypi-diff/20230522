# Comparing `tmp/GrappyLfjv-0.0.12.tar.gz` & `tmp/GrappyLfjv-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GrappyLfjv-0.0.12.tar", last modified: Sun May 14 21:44:52 2023, max compression
+gzip compressed data, was "GrappyLfjv-0.0.15.tar", last modified: Sun May 21 23:41:03 2023, max compression
```

## Comparing `GrappyLfjv-0.0.12.tar` & `GrappyLfjv-0.0.15.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-14 21:44:52.584895 GrappyLfjv-0.0.12/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-14 21:26:18.000000 GrappyLfjv-0.0.12/LICENSE
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      270 2023-05-14 21:44:52.584435 GrappyLfjv-0.0.12/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        0 2023-05-14 21:36:57.000000 GrappyLfjv-0.0.12/README.md
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-14 21:44:52.585069 GrappyLfjv-0.0.12/setup.cfg
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      416 2023-05-14 21:41:59.000000 GrappyLfjv-0.0.12/setup.py
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-14 21:44:52.580703 GrappyLfjv-0.0.12/src/
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-14 21:44:52.583714 GrappyLfjv-0.0.12/src/GrappyLfjv.egg-info/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      270 2023-05-14 21:44:52.000000 GrappyLfjv-0.0.12/src/GrappyLfjv.egg-info/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-14 21:44:52.000000 GrappyLfjv-0.0.12/src/GrappyLfjv.egg-info/SOURCES.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-14 21:44:52.000000 GrappyLfjv-0.0.12/src/GrappyLfjv.egg-info/dependency_links.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-14 21:44:52.000000 GrappyLfjv-0.0.12/src/GrappyLfjv.egg-info/requires.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-14 21:44:52.000000 GrappyLfjv-0.0.12/src/GrappyLfjv.egg-info/top_level.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      394 2023-05-14 20:37:24.000000 GrappyLfjv-0.0.12/src/grappy.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-21 23:41:03.311720 GrappyLfjv-0.0.15/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.15/LICENSE
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      270 2023-05-21 23:41:03.311170 GrappyLfjv-0.0.15/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      264 2023-05-21 23:32:04.000000 GrappyLfjv-0.0.15/README.md
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-21 23:41:03.311870 GrappyLfjv-0.0.15/setup.cfg
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      416 2023-05-21 23:33:54.000000 GrappyLfjv-0.0.15/setup.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-21 23:41:03.308126 GrappyLfjv-0.0.15/src/
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-21 23:41:03.310585 GrappyLfjv-0.0.15/src/GrappyLfjv.egg-info/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      270 2023-05-21 23:41:03.000000 GrappyLfjv-0.0.15/src/GrappyLfjv.egg-info/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-21 23:41:03.000000 GrappyLfjv-0.0.15/src/GrappyLfjv.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-21 23:41:03.000000 GrappyLfjv-0.0.15/src/GrappyLfjv.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-21 23:41:03.000000 GrappyLfjv-0.0.15/src/GrappyLfjv.egg-info/requires.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-21 23:41:03.000000 GrappyLfjv-0.0.15/src/GrappyLfjv.egg-info/top_level.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     4086 2023-05-21 23:35:12.000000 GrappyLfjv-0.0.15/src/grappy.py
```

### Comparing `GrappyLfjv-0.0.12/LICENSE` & `GrappyLfjv-0.0.15/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Benjamin Trécian
+Copyright (c) 2023 Benjamin Trévian
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

