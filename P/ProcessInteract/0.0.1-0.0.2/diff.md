# Comparing `tmp/ProcessInteract-0.0.1.tar.gz` & `tmp/ProcessInteract-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcessInteract-0.0.1.tar", last modified: Mon May 22 08:11:33 2023, max compression
+gzip compressed data, was "ProcessInteract-0.0.2.tar", last modified: Mon May 22 08:18:29 2023, max compression
```

## Comparing `ProcessInteract-0.0.1.tar` & `ProcessInteract-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 weirdoo   (1000) weirdoo   (1000)        0 2023-05-22 08:11:33.416058 ProcessInteract-0.0.1/
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      204 2023-05-22 08:11:33.416058 ProcessInteract-0.0.1/PKG-INFO
-drwxr-xr-x   0 weirdoo   (1000) weirdoo   (1000)        0 2023-05-22 08:11:33.416058 ProcessInteract-0.0.1/ProcessInteract.egg-info/
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      204 2023-05-22 08:11:33.000000 ProcessInteract-0.0.1/ProcessInteract.egg-info/PKG-INFO
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      216 2023-05-22 08:11:33.000000 ProcessInteract-0.0.1/ProcessInteract.egg-info/SOURCES.txt
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)        1 2023-05-22 08:11:33.000000 ProcessInteract-0.0.1/ProcessInteract.egg-info/dependency_links.txt
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)       16 2023-05-22 08:11:33.000000 ProcessInteract-0.0.1/ProcessInteract.egg-info/top_level.txt
-drwxr-xr-x   0 weirdoo   (1000) weirdoo   (1000)        0 2023-05-22 08:11:33.416058 ProcessInteract-0.0.1/processinteract/
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)        0 2023-05-22 07:56:58.000000 ProcessInteract-0.0.1/processinteract/__init__.py
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      425 2023-05-22 07:55:20.000000 ProcessInteract-0.0.1/processinteract/main.py
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)       38 2023-05-22 08:11:33.416058 ProcessInteract-0.0.1/setup.cfg
--rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      332 2023-05-22 08:11:11.000000 ProcessInteract-0.0.1/setup.py
+drwxr-xr-x   0 weirdoo   (1000) weirdoo   (1000)        0 2023-05-22 08:18:29.472738 ProcessInteract-0.0.2/
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      204 2023-05-22 08:18:29.472738 ProcessInteract-0.0.2/PKG-INFO
+drwxr-xr-x   0 weirdoo   (1000) weirdoo   (1000)        0 2023-05-22 08:18:29.472738 ProcessInteract-0.0.2/ProcessInteract.egg-info/
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      204 2023-05-22 08:18:29.000000 ProcessInteract-0.0.2/ProcessInteract.egg-info/PKG-INFO
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      216 2023-05-22 08:18:29.000000 ProcessInteract-0.0.2/ProcessInteract.egg-info/SOURCES.txt
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)        1 2023-05-22 08:18:29.000000 ProcessInteract-0.0.2/ProcessInteract.egg-info/dependency_links.txt
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)       16 2023-05-22 08:18:29.000000 ProcessInteract-0.0.2/ProcessInteract.egg-info/top_level.txt
+drwxr-xr-x   0 weirdoo   (1000) weirdoo   (1000)        0 2023-05-22 08:18:29.472738 ProcessInteract-0.0.2/processinteract/
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)       18 2023-05-22 08:17:01.000000 ProcessInteract-0.0.2/processinteract/__init__.py
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      555 2023-05-22 08:17:01.000000 ProcessInteract-0.0.2/processinteract/main.py
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)       38 2023-05-22 08:18:29.472738 ProcessInteract-0.0.2/setup.cfg
+-rw-r--r--   0 weirdoo   (1000) weirdoo   (1000)      332 2023-05-22 08:17:57.000000 ProcessInteract-0.0.2/setup.py
```

