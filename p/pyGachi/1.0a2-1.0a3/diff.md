# Comparing `tmp/pyGachi-1.0a2.tar.gz` & `tmp/pyGachi-1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGachi-1.0a2.tar", last modified: Mon May 22 14:27:58 2023, max compression
+gzip compressed data, was "pyGachi-1.0a3.tar", last modified: Mon May 22 14:49:06 2023, max compression
```

## Comparing `pyGachi-1.0a2.tar` & `pyGachi-1.0a3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:27:58.165027 pyGachi-1.0a2/
--rw-rw-rw-   0        0        0     1031 2023-05-22 14:27:58.165027 pyGachi-1.0a2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 14:27:58.148026 pyGachi-1.0a2/pyGachi/
--rw-rw-rw-   0        0        0      452 2023-05-22 14:13:59.000000 pyGachi-1.0a2/pyGachi/__init__.py
--rw-rw-rw-   0        0        0     3654 2023-05-22 14:02:51.000000 pyGachi-1.0a2/pyGachi/bd1.py
--rw-rw-rw-   0        0        0     3347 2023-05-22 14:02:53.000000 pyGachi-1.0a2/pyGachi/bd2.py
--rw-rw-rw-   0        0        0     3058 2023-05-22 14:02:53.000000 pyGachi-1.0a2/pyGachi/oop1.py
--rw-rw-rw-   0        0        0     2639 2023-05-22 14:02:54.000000 pyGachi-1.0a2/pyGachi/oop2.py
--rw-rw-rw-   0        0        0      723 2023-05-22 14:02:55.000000 pyGachi-1.0a2/pyGachi/prog1.py
--rw-rw-rw-   0        0        0     1042 2023-05-22 14:02:55.000000 pyGachi-1.0a2/pyGachi/prog2.py
--rw-rw-rw-   0        0        0      333 2023-05-22 14:02:58.000000 pyGachi-1.0a2/pyGachi/prog3.py
--rw-rw-rw-   0        0        0      490 2023-05-22 14:02:59.000000 pyGachi-1.0a2/pyGachi/prog4.py
--rw-rw-rw-   0        0        0     2257 2023-05-22 14:03:00.000000 pyGachi-1.0a2/pyGachi/prog5.py
--rw-rw-rw-   0        0        0      809 2023-05-22 14:03:00.000000 pyGachi-1.0a2/pyGachi/siaod1.py
--rw-rw-rw-   0        0        0     3002 2023-05-22 14:03:01.000000 pyGachi-1.0a2/pyGachi/siaod2.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:27:58.164026 pyGachi-1.0a2/pyGachi.egg-info/
--rw-rw-rw-   0        0        0     1031 2023-05-22 14:27:57.000000 pyGachi-1.0a2/pyGachi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-22 14:27:58.000000 pyGachi-1.0a2/pyGachi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:27:57.000000 pyGachi-1.0a2/pyGachi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 14:27:57.000000 pyGachi-1.0a2/pyGachi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 14:27:57.000000 pyGachi-1.0a2/pyGachi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 14:27:58.166027 pyGachi-1.0a2/setup.cfg
--rw-rw-rw-   0        0        0     1313 2023-05-22 14:27:43.000000 pyGachi-1.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:49:06.773199 pyGachi-1.0a3/
+-rw-rw-rw-   0        0        0     1031 2023-05-22 14:49:06.773199 pyGachi-1.0a3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 14:49:06.754198 pyGachi-1.0a3/pyGachi/
+-rw-rw-rw-   0        0        0      452 2023-05-22 14:48:55.000000 pyGachi-1.0a3/pyGachi/__init__.py
+-rw-rw-rw-   0        0        0     3654 2023-05-22 14:02:51.000000 pyGachi-1.0a3/pyGachi/bd1.py
+-rw-rw-rw-   0        0        0     3347 2023-05-22 14:02:53.000000 pyGachi-1.0a3/pyGachi/bd2.py
+-rw-rw-rw-   0        0        0     3058 2023-05-22 14:02:53.000000 pyGachi-1.0a3/pyGachi/oop1.py
+-rw-rw-rw-   0        0        0     2639 2023-05-22 14:02:54.000000 pyGachi-1.0a3/pyGachi/oop2.py
+-rw-rw-rw-   0        0        0      723 2023-05-22 14:02:55.000000 pyGachi-1.0a3/pyGachi/prog1.py
+-rw-rw-rw-   0        0        0     1042 2023-05-22 14:02:55.000000 pyGachi-1.0a3/pyGachi/prog2.py
+-rw-rw-rw-   0        0        0      333 2023-05-22 14:02:58.000000 pyGachi-1.0a3/pyGachi/prog3.py
+-rw-rw-rw-   0        0        0      490 2023-05-22 14:02:59.000000 pyGachi-1.0a3/pyGachi/prog4.py
+-rw-rw-rw-   0        0        0     2257 2023-05-22 14:03:00.000000 pyGachi-1.0a3/pyGachi/prog5.py
+-rw-rw-rw-   0        0        0      809 2023-05-22 14:03:00.000000 pyGachi-1.0a3/pyGachi/siaod1.py
+-rw-rw-rw-   0        0        0     3002 2023-05-22 14:03:01.000000 pyGachi-1.0a3/pyGachi/siaod2.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:49:06.772199 pyGachi-1.0a3/pyGachi.egg-info/
+-rw-rw-rw-   0        0        0     1031 2023-05-22 14:49:06.000000 pyGachi-1.0a3/pyGachi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-05-22 14:49:06.000000 pyGachi-1.0a3/pyGachi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:49:06.000000 pyGachi-1.0a3/pyGachi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-22 14:49:06.000000 pyGachi-1.0a3/pyGachi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 14:49:06.000000 pyGachi-1.0a3/pyGachi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 14:49:06.777200 pyGachi-1.0a3/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2023-05-22 14:48:55.000000 pyGachi-1.0a3/setup.py
```

### Comparing `pyGachi-1.0a2/PKG-INFO` & `pyGachi-1.0a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyGachi
-Version: 1.0a2
+Version: 1.0a3
 Summary: Brat ne trogai, eto tibe ne nado
 Home-page: https://github.com/DANILYH/pyGachi
-Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.0a2.zip
+Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.0a3.zip
 Author: GachiParty
 Author-email: fetom30268@cutefier.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyGachi-1.0a2/pyGachi/bd1.py` & `pyGachi-1.0a3/pyGachi/bd1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi/bd2.py` & `pyGachi-1.0a3/pyGachi/bd2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi/oop1.py` & `pyGachi-1.0a3/pyGachi/oop1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi/oop2.py` & `pyGachi-1.0a3/pyGachi/oop2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi/prog1.py` & `pyGachi-1.0a3/pyGachi/prog1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi/prog2.py` & `pyGachi-1.0a3/pyGachi/prog2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi/prog5.py` & `pyGachi-1.0a3/pyGachi/prog5.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi/siaod1.py` & `pyGachi-1.0a3/pyGachi/siaod1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi/siaod2.py` & `pyGachi-1.0a3/pyGachi/siaod2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a2/pyGachi.egg-info/PKG-INFO` & `pyGachi-1.0a3/pyGachi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyGachi
-Version: 1.0a2
+Version: 1.0a3
 Summary: Brat ne trogai, eto tibe ne nado
 Home-page: https://github.com/DANILYH/pyGachi
-Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.0a2.zip
+Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.0a3.zip
 Author: GachiParty
 Author-email: fetom30268@cutefier.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyGachi-1.0a2/setup.py` & `pyGachi-1.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from io import open
 from setuptools import setup
 
-version = '1.0a2'
+version = '1.0a3'
 
 setup(
     name='pyGachi',
     author='GachiParty',
 
     version=version,
     author_email='fetom30268@cutefier.com',
```

