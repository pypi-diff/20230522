# Comparing `tmp/tldrwl-0.0.1.tar.gz` & `tmp/tldrwl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-0.0.1.tar", last modified: Mon May 22 01:23:24 2023, max compression
+gzip compressed data, was "tldrwl-0.0.2.tar", last modified: Mon May 22 01:36:02 2023, max compression
```

## Comparing `tldrwl-0.0.1.tar` & `tldrwl-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 01:23:24.477104 tldrwl-0.0.1/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      372 2023-05-22 01:23:24.477104 tldrwl-0.0.1/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       82 2023-05-21 23:46:41.000000 tldrwl-0.0.1/README.md
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 01:23:24.477104 tldrwl-0.0.1/setup.cfg
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      617 2023-05-22 01:22:27.000000 tldrwl-0.0.1/setup.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 01:23:24.477104 tldrwl-0.0.1/tldrwl/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.1/tldrwl/__init__.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      206 2023-05-22 01:07:09.000000 tldrwl-0.0.1/tldrwl/ai_interface.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      771 2023-05-22 01:05:47.000000 tldrwl-0.0.1/tldrwl/exception.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1048 2023-05-22 01:06:46.000000 tldrwl-0.0.1/tldrwl/register.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1491 2023-05-22 01:10:40.000000 tldrwl-0.0.1/tldrwl/summarize_text.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 01:23:24.477104 tldrwl-0.0.1/tldrwl.egg-info/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      372 2023-05-22 01:23:24.000000 tldrwl-0.0.1/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      273 2023-05-22 01:23:24.000000 tldrwl-0.0.1/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 01:23:24.000000 tldrwl-0.0.1/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       23 2023-05-22 01:23:24.000000 tldrwl-0.0.1/tldrwl.egg-info/requires.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 01:23:24.000000 tldrwl-0.0.1/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 01:36:02.336900 tldrwl-0.0.2/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.2/MANIFEST.in
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      372 2023-05-22 01:36:02.336900 tldrwl-0.0.2/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       82 2023-05-22 01:25:52.000000 tldrwl-0.0.2/README.md
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       23 2023-05-22 00:08:16.000000 tldrwl-0.0.2/requirements.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 01:36:02.336900 tldrwl-0.0.2/setup.cfg
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 01:35:23.000000 tldrwl-0.0.2/setup.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 01:36:02.336900 tldrwl-0.0.2/tldrwl/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.2/tldrwl/__init__.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      206 2023-05-22 01:07:09.000000 tldrwl-0.0.2/tldrwl/ai_interface.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      771 2023-05-22 01:05:47.000000 tldrwl-0.0.2/tldrwl/exception.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1048 2023-05-22 01:06:46.000000 tldrwl-0.0.2/tldrwl/register.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1491 2023-05-22 01:10:40.000000 tldrwl-0.0.2/tldrwl/summarize_text.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 01:36:02.336900 tldrwl-0.0.2/tldrwl.egg-info/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      372 2023-05-22 01:36:02.000000 tldrwl-0.0.2/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      302 2023-05-22 01:36:02.000000 tldrwl-0.0.2/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 01:36:02.000000 tldrwl-0.0.2/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       23 2023-05-22 01:36:02.000000 tldrwl-0.0.2/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 01:36:02.000000 tldrwl-0.0.2/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-0.0.1/tldrwl/exception.py` & `tldrwl-0.0.2/tldrwl/exception.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.1/tldrwl/register.py` & `tldrwl-0.0.2/tldrwl/register.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.1/tldrwl/summarize_text.py` & `tldrwl-0.0.2/tldrwl/summarize_text.py`

 * *Files identical despite different names*

