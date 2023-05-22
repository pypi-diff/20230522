# Comparing `tmp/UComp-4.0.1.tar.gz` & `tmp/UComp-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-4.0.1.tar", last modified: Fri May 19 10:28:10 2023, max compression
+gzip compressed data, was "UComp-4.0.2.tar", last modified: Mon May 22 15:27:44 2023, max compression
```

## Comparing `UComp-4.0.1.tar` & `UComp-4.0.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 10:28:10.021241 UComp-4.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-19 10:28:10.009260 UComp-4.0.1/Cpp/
--rw-rw-rw-   0        0        0     5689 2022-10-14 09:00:45.000000 UComp-4.0.1/Cpp/pythonETS.cpp
--rw-rw-rw-   0        0        0    16433 2022-10-21 09:30:02.000000 UComp-4.0.1/Cpp/pythonUComp.cpp
--rw-rw-rw-   0        0        0      274 2023-05-19 10:28:10.022237 UComp-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-4.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 10:28:10.020240 UComp-4.0.1/UComp.egg-info/
--rw-rw-rw-   0        0        0      274 2023-05-19 10:28:09.000000 UComp-4.0.1/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-05-19 10:28:09.000000 UComp-4.0.1/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 10:28:09.000000 UComp-4.0.1/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 10:28:09.000000 UComp-4.0.1/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-05-19 10:28:10.024237 UComp-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-05-19 10:21:34.000000 UComp-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:27:44.590026 UComp-4.0.2/
+-rw-rw-rw-   0        0        0      303 2023-05-22 15:27:44.590026 UComp-4.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-4.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 15:27:44.590026 UComp-4.0.2/UComp.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-05-22 15:27:44.000000 UComp-4.0.2/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-22 15:27:44.000000 UComp-4.0.2/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 15:27:44.000000 UComp-4.0.2/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-22 15:27:44.000000 UComp-4.0.2/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 15:27:44.000000 UComp-4.0.2/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 15:27:44.590026 UComp-4.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      500 2023-05-22 15:27:27.000000 UComp-4.0.2/setup.py
```

