# Comparing `tmp/bgstools-0.1.1.tar.gz` & `tmp/bgstools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgstools-0.1.1.tar", max compression
+gzip compressed data, was "bgstools-0.1.2.tar", max compression
```

## Comparing `bgstools-0.1.1.tar` & `bgstools-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0       33 2023-05-03 11:54:58.568286 bgstools-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.1/bgstools/__init__.py
--rw-r--r--   0        0        0      298 2023-05-19 11:22:49.081592 bgstools-0.1.1/bgstools/bgstools.py
--rw-r--r--   0        0        0        0 2023-05-19 11:22:49.081592 bgstools-0.1.1/bgstools/datastorage/__init__.py
--rw-r--r--   0        0        0     4950 2023-05-19 11:22:49.081592 bgstools-0.1.1/bgstools/datastorage/datastorage.py
--rw-r--r--   0        0        0        0 2023-05-03 11:53:10.602842 bgstools-0.1.1/bgstools/io/__init__.py
--rw-r--r--   0        0        0      769 2023-05-03 11:53:10.602842 bgstools-0.1.1/bgstools/io/io.py
--rw-r--r--   0        0        0        0 2023-05-03 11:53:10.542842 bgstools-0.1.1/bgstools/spatial/__init__.py
--rw-r--r--   0        0        0     2654 2023-05-03 11:53:10.542842 bgstools-0.1.1/bgstools/spatial/spatial.py
--rw-r--r--   0        0        0        0 2023-05-03 11:53:10.492843 bgstools-0.1.1/bgstools/utils/__init__.py
--rw-r--r--   0        0        0      972 2023-05-03 11:53:10.492843 bgstools-0.1.1/bgstools/utils/utils.py
--rw-r--r--   0        0        0      351 2023-05-22 08:13:52.337270 bgstools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 bgstools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-05-22 09:38:31.760561 bgstools-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.2/bgstools/__init__.py
+-rw-r--r--   0        0        0      339 2023-05-22 15:45:26.380252 bgstools-0.1.2/bgstools/bgstools.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:22:49.081592 bgstools-0.1.2/bgstools/datastorage/__init__.py
+-rw-r--r--   0        0        0     4950 2023-05-19 11:22:49.081592 bgstools-0.1.2/bgstools/datastorage/datastorage.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:53:10.602842 bgstools-0.1.2/bgstools/io/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-22 15:44:57.697847 bgstools-0.1.2/bgstools/io/io.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:53:10.542842 bgstools-0.1.2/bgstools/spatial/__init__.py
+-rw-r--r--   0        0        0     2654 2023-05-03 11:53:10.542842 bgstools-0.1.2/bgstools/spatial/spatial.py
+-rw-r--r--   0        0        0        0 2023-05-22 15:59:56.616803 bgstools-0.1.2/bgstools/stt/__init__.py
+-rw-r--r--   0        0        0     2180 2023-05-22 16:11:53.523910 bgstools-0.1.2/bgstools/stt/stt.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:53:10.492843 bgstools-0.1.2/bgstools/utils/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-03 11:53:10.492843 bgstools-0.1.2/bgstools/utils/utils.py
+-rw-r--r--   0        0        0      373 2023-05-22 16:23:18.612932 bgstools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bgstools-0.1.2/PKG-INFO
```

### Comparing `bgstools-0.1.1/bgstools/datastorage/datastorage.py` & `bgstools-0.1.2/bgstools/datastorage/datastorage.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.1/bgstools/spatial/spatial.py` & `bgstools-0.1.2/bgstools/spatial/spatial.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.1/bgstools/utils/utils.py` & `bgstools-0.1.2/bgstools/utils/utils.py`

 * *Files identical despite different names*

