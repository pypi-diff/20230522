# Comparing `tmp/linkero-0.9.8.tar.gz` & `tmp/linkero-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\linkero-0.9.8.tar", last modified: Fri Jun  1 15:43:37 2018, max compression
+gzip compressed data, was "dist\linkero-0.9.9.tar", last modified: Sat Jun  2 10:17:09 2018, max compression
```

## Comparing `linkero-0.9.8.tar` & `linkero-0.9.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2018-06-01 15:43:37.000000 linkero-0.9.8/
--rw-rw-rw-   0        0        0     7816 2018-06-01 15:33:15.000000 linkero-0.9.8/LICENSE
-drwxrwxrwx   0        0        0        0 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero/
-drwxrwxrwx   0        0        0        0 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero/config/
--rw-rw-rw-   0        0        0      861 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/config/config.json
-drwxrwxrwx   0        0        0        0 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero/core/
--rw-rw-rw-   0        0        0      330 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/core/ascii.py
--rw-rw-rw-   0        0        0     4340 2018-06-01 15:33:15.000000 linkero-0.9.8/linkero/core/common.py
-drwxrwxrwx   0        0        0        0 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero/core/gateway/
--rw-rw-rw-   0        0        0     1163 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/core/gateway/gevent_service.py
--rw-rw-rw-   0        0        0      405 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/core/gateway/waitress_service.py
--rw-rw-rw-   0        0        0        0 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/core/gateway/__init__.py
--rw-rw-rw-   0        0        0     6351 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/core/linkero.py
--rw-rw-rw-   0        0        0        0 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/core/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero/tools/
--rw-rw-rw-   0        0        0      645 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/tools/passwordHashGenerator.py
--rw-rw-rw-   0        0        0        0 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/tools/__init__.py
--rw-rw-rw-   0        0        0        0 2018-06-01 15:15:49.000000 linkero-0.9.8/linkero/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero.egg-info/
--rw-rw-rw-   0        0        0        1 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2115 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero.egg-info/requires.txt
--rw-rw-rw-   0        0        0      518 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2018-06-01 15:43:37.000000 linkero-0.9.8/linkero.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       32 2018-06-01 15:15:49.000000 linkero-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2115 2018-06-01 15:43:37.000000 linkero-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0      170 2018-06-01 15:15:49.000000 linkero-0.9.8/requirements.txt
--rw-rw-rw-   0        0        0       64 2018-06-01 15:43:37.000000 linkero-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     2577 2018-06-01 15:33:15.000000 linkero-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2018-06-02 10:17:09.000000 linkero-0.9.9/
+-rw-rw-rw-   0        0        0     7816 2018-06-02 09:54:04.000000 linkero-0.9.9/LICENSE
+drwxrwxrwx   0        0        0        0 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero/
+drwxrwxrwx   0        0        0        0 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero/config/
+-rw-rw-rw-   0        0        0      861 2018-01-29 21:38:32.000000 linkero-0.9.9/linkero/config/config.json
+drwxrwxrwx   0        0        0        0 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero/core/
+-rw-rw-rw-   0        0        0      330 2017-09-25 14:11:04.000000 linkero-0.9.9/linkero/core/ascii.py
+-rw-rw-rw-   0        0        0     4340 2018-06-02 10:12:35.000000 linkero-0.9.9/linkero/core/common.py
+drwxrwxrwx   0        0        0        0 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero/core/gateway/
+-rw-rw-rw-   0        0        0     1163 2017-11-14 17:58:27.000000 linkero-0.9.9/linkero/core/gateway/gevent_service.py
+-rw-rw-rw-   0        0        0      405 2017-11-14 17:58:27.000000 linkero-0.9.9/linkero/core/gateway/waitress_service.py
+-rw-rw-rw-   0        0        0        0 2017-09-25 14:11:04.000000 linkero-0.9.9/linkero/core/gateway/__init__.py
+-rw-rw-rw-   0        0        0     6351 2018-01-29 21:38:32.000000 linkero-0.9.9/linkero/core/linkero.py
+-rw-rw-rw-   0        0        0        0 2017-09-25 14:11:04.000000 linkero-0.9.9/linkero/core/__init__.py
+drwxrwxrwx   0        0        0        0 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero/tools/
+-rw-rw-rw-   0        0        0      645 2017-09-25 14:11:04.000000 linkero-0.9.9/linkero/tools/passwordHashGenerator.py
+-rw-rw-rw-   0        0        0        0 2017-09-25 14:11:04.000000 linkero-0.9.9/linkero/tools/__init__.py
+-rw-rw-rw-   0        0        0        0 2017-09-25 14:11:04.000000 linkero-0.9.9/linkero/__init__.py
+drwxrwxrwx   0        0        0        0 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2115 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      518 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2018-06-02 10:17:09.000000 linkero-0.9.9/linkero.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       32 2017-09-26 08:59:10.000000 linkero-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2115 2018-06-02 10:17:09.000000 linkero-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2018-06-02 10:12:35.000000 linkero-0.9.9/requirements.txt
+-rw-rw-rw-   0        0        0       64 2018-06-02 10:17:09.000000 linkero-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     2577 2018-06-02 09:54:04.000000 linkero-0.9.9/setup.py
```

### Comparing `linkero-0.9.8/LICENSE` & `linkero-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linkero-0.9.8/linkero/config/config.json` & `linkero-0.9.9/linkero/config/config.json`

 * *Files identical despite different names*

### Comparing `linkero-0.9.8/linkero/core/common.py` & `linkero-0.9.9/linkero/core/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 from shutil import copyfile
 from .ascii import ascii_warning
 
 
 class Metadata:
     def __init__(self):
-        self.__version__ = '0.9.8'
+        self.__version__ = '0.9.9'
         self.__author__ = 'Rubén de Celis Hernández'
 
     def get_version(self):
         return self.__version__
     def get_author(self):
         return self.__author__
```

### Comparing `linkero-0.9.8/linkero/core/gateway/gevent_service.py` & `linkero-0.9.9/linkero/core/gateway/gevent_service.py`

 * *Files identical despite different names*

### Comparing `linkero-0.9.8/linkero/core/linkero.py` & `linkero-0.9.9/linkero/core/linkero.py`

 * *Files identical despite different names*

### Comparing `linkero-0.9.8/linkero/tools/passwordHashGenerator.py` & `linkero-0.9.9/linkero/tools/passwordHashGenerator.py`

 * *Files identical despite different names*

### Comparing `linkero-0.9.8/linkero.egg-info/PKG-INFO` & `linkero-0.9.9/linkero.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: linkero
-Version: 0.9.8
+Version: 0.9.9
 Summary: Restful API for external requests
 Home-page: https://github.com/ingran/linkero
 Author: Rubén de Celis Hernández
 Author-email: contact@rdch106.hol.es
 License: LGPL v3
-Download-URL: https://github.com/ingran/linkero/archive/v0.9.8.tar.gz
+Download-URL: https://github.com/ingran/linkero/archive/v0.9.9.tar.gz
 Description: 
         Linkero is compatible with **Python-2** and **Python-3**.
         
         ************************************
         What can I do with Linkero?
         ************************************
```

### Comparing `linkero-0.9.8/linkero.egg-info/SOURCES.txt` & `linkero-0.9.9/linkero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkero-0.9.8/PKG-INFO` & `linkero-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: linkero
-Version: 0.9.8
+Version: 0.9.9
 Summary: Restful API for external requests
 Home-page: https://github.com/ingran/linkero
 Author: Rubén de Celis Hernández
 Author-email: contact@rdch106.hol.es
 License: LGPL v3
-Download-URL: https://github.com/ingran/linkero/archive/v0.9.8.tar.gz
+Download-URL: https://github.com/ingran/linkero/archive/v0.9.9.tar.gz
 Description: 
         Linkero is compatible with **Python-2** and **Python-3**.
         
         ************************************
         What can I do with Linkero?
         ************************************
```

### Comparing `linkero-0.9.8/setup.py` & `linkero-0.9.9/setup.py`

 * *Files identical despite different names*

