# Comparing `tmp/genbase-0.3.1.tar.gz` & `tmp/genbase-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genbase-0.3.1.tar", last modified: Mon May 22 09:36:31 2023, max compression
+gzip compressed data, was "genbase-0.3.2.tar", last modified: Mon May 22 09:43:04 2023, max compression
```

## Comparing `genbase-0.3.1.tar` & `genbase-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.572032 genbase-0.3.1/
--rw-r--r--   0 marcelr    (502) staff       (20)      284 2022-03-04 11:29:53.000000 genbase-0.3.1/.flake8
--rw-r--r--   0 marcelr    (502) staff       (20)     2099 2021-11-18 11:01:25.000000 genbase-0.3.1/.gitignore
--rw-r--r--   0 marcelr    (502) staff       (20)      475 2022-06-01 11:19:34.000000 genbase-0.3.1/.gitlab-ci.yml
--rw-r--r--   0 marcelr    (502) staff       (20)     8253 2023-05-22 09:35:35.000000 genbase-0.3.1/CHANGELOG.md
--rw-r--r--   0 marcelr    (502) staff       (20)     7651 2021-11-18 11:00:43.000000 genbase-0.3.1/LICENSE
--rw-r--r--   0 marcelr    (502) staff       (20)       40 2022-03-04 14:42:50.000000 genbase-0.3.1/MANIFEST.in
--rw-r--r--   0 marcelr    (502) staff       (20)      264 2022-06-01 09:21:57.000000 genbase-0.3.1/Makefile
--rw-r--r--   0 marcelr    (502) staff       (20)    13008 2023-05-22 09:36:31.571528 genbase-0.3.1/PKG-INFO
--rw-r--r--   0 marcelr    (502) staff       (20)    12452 2023-01-30 09:01:57.000000 genbase-0.3.1/README.md
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.550149 genbase-0.3.1/genbase/
--rw-r--r--   0 marcelr    (502) staff       (20)     7541 2023-02-22 14:23:45.000000 genbase-0.3.1/genbase/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)       86 2023-05-22 09:34:57.000000 genbase-0.3.1/genbase/_version.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.555686 genbase-0.3.1/genbase/data/
--rw-r--r--   0 marcelr    (502) staff       (20)    10546 2023-05-22 09:34:38.000000 genbase-0.3.1/genbase/data/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)     1755 2022-06-01 09:25:31.000000 genbase-0.3.1/genbase/decorator.py
--rw-r--r--   0 marcelr    (502) staff       (20)     2341 2022-03-21 10:23:10.000000 genbase-0.3.1/genbase/internationalization.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.562061 genbase-0.3.1/genbase/locale/
--rw-r--r--   0 marcelr    (502) staff       (20)       87 2021-11-27 18:49:35.000000 genbase-0.3.1/genbase/locale/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)      356 2021-11-27 19:00:44.000000 genbase-0.3.1/genbase/locale/en.json
--rw-r--r--   0 marcelr    (502) staff       (20)      363 2021-10-02 13:07:17.000000 genbase-0.3.1/genbase/locale/nl.json
--rw-r--r--   0 marcelr    (502) staff       (20)     2763 2022-06-01 09:24:24.000000 genbase-0.3.1/genbase/mixin.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.562571 genbase-0.3.1/genbase/model/
--rw-r--r--   0 marcelr    (502) staff       (20)     6979 2022-06-01 11:19:21.000000 genbase-0.3.1/genbase/model/__init__.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.563242 genbase-0.3.1/genbase/test/
--rw-r--r--   0 marcelr    (502) staff       (20)      910 2022-06-01 11:19:21.000000 genbase-0.3.1/genbase/test/test_internationalization.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.565819 genbase-0.3.1/genbase/ui/
--rw-r--r--   0 marcelr    (502) staff       (20)     2188 2023-01-29 11:31:51.000000 genbase-0.3.1/genbase/ui/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)    22248 2023-01-28 12:50:57.000000 genbase-0.3.1/genbase/ui/notebook.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.566631 genbase-0.3.1/genbase/ui/plot/
--rw-r--r--   0 marcelr    (502) staff       (20)     2158 2023-02-23 12:17:06.000000 genbase-0.3.1/genbase/ui/plot/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)      664 2021-12-05 12:25:32.000000 genbase-0.3.1/genbase/ui/svg.py
--rw-r--r--   0 marcelr    (502) staff       (20)     8810 2023-01-28 11:01:33.000000 genbase-0.3.1/genbase/utils.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.554968 genbase-0.3.1/genbase.egg-info/
--rw-r--r--   0 marcelr    (502) staff       (20)    13008 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/PKG-INFO
--rw-r--r--   0 marcelr    (502) staff       (20)      660 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/SOURCES.txt
--rw-r--r--   0 marcelr    (502) staff       (20)        1 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/dependency_links.txt
--rw-r--r--   0 marcelr    (502) staff       (20)      240 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/requires.txt
--rw-r--r--   0 marcelr    (502) staff       (20)        8 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/top_level.txt
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.570845 genbase-0.3.1/img/
--rw-r--r--   0 marcelr    (502) staff       (20)      612 2021-11-18 11:32:43.000000 genbase-0.3.1/img/gb.png
--rw-r--r--   0 marcelr    (502) staff       (20)     2915 2021-11-18 11:34:55.000000 genbase-0.3.1/img/genbase.png
--rw-r--r--   0 marcelr    (502) staff       (20)       38 2023-05-22 09:36:31.572119 genbase-0.3.1/setup.cfg
--rw-r--r--   0 marcelr    (502) staff       (20)     1504 2023-01-26 16:10:20.000000 genbase-0.3.1/setup.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.256175 genbase-0.3.2/
+-rw-r--r--   0 marcelr    (502) staff       (20)      284 2022-03-04 11:29:53.000000 genbase-0.3.2/.flake8
+-rw-r--r--   0 marcelr    (502) staff       (20)     2099 2021-11-18 11:01:25.000000 genbase-0.3.2/.gitignore
+-rw-r--r--   0 marcelr    (502) staff       (20)      475 2022-06-01 11:19:34.000000 genbase-0.3.2/.gitlab-ci.yml
+-rw-r--r--   0 marcelr    (502) staff       (20)     8253 2023-05-22 09:35:35.000000 genbase-0.3.2/CHANGELOG.md
+-rw-r--r--   0 marcelr    (502) staff       (20)     7651 2021-11-18 11:00:43.000000 genbase-0.3.2/LICENSE
+-rw-r--r--   0 marcelr    (502) staff       (20)       40 2022-03-04 14:42:50.000000 genbase-0.3.2/MANIFEST.in
+-rw-r--r--   0 marcelr    (502) staff       (20)      264 2022-06-01 09:21:57.000000 genbase-0.3.2/Makefile
+-rw-r--r--   0 marcelr    (502) staff       (20)    13008 2023-05-22 09:43:04.255849 genbase-0.3.2/PKG-INFO
+-rw-r--r--   0 marcelr    (502) staff       (20)    12452 2023-01-30 09:01:57.000000 genbase-0.3.2/README.md
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.238274 genbase-0.3.2/genbase/
+-rw-r--r--   0 marcelr    (502) staff       (20)     7541 2023-02-22 14:23:45.000000 genbase-0.3.2/genbase/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)       86 2023-05-22 09:42:58.000000 genbase-0.3.2/genbase/_version.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.247337 genbase-0.3.2/genbase/data/
+-rw-r--r--   0 marcelr    (502) staff       (20)    10617 2023-05-22 09:42:38.000000 genbase-0.3.2/genbase/data/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)     1755 2022-06-01 09:25:31.000000 genbase-0.3.2/genbase/decorator.py
+-rw-r--r--   0 marcelr    (502) staff       (20)     2341 2022-03-21 10:23:10.000000 genbase-0.3.2/genbase/internationalization.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.249334 genbase-0.3.2/genbase/locale/
+-rw-r--r--   0 marcelr    (502) staff       (20)       87 2021-11-27 18:49:35.000000 genbase-0.3.2/genbase/locale/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)      356 2021-11-27 19:00:44.000000 genbase-0.3.2/genbase/locale/en.json
+-rw-r--r--   0 marcelr    (502) staff       (20)      363 2021-10-02 13:07:17.000000 genbase-0.3.2/genbase/locale/nl.json
+-rw-r--r--   0 marcelr    (502) staff       (20)     2763 2022-06-01 09:24:24.000000 genbase-0.3.2/genbase/mixin.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.249948 genbase-0.3.2/genbase/model/
+-rw-r--r--   0 marcelr    (502) staff       (20)     6979 2022-06-01 11:19:21.000000 genbase-0.3.2/genbase/model/__init__.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.250560 genbase-0.3.2/genbase/test/
+-rw-r--r--   0 marcelr    (502) staff       (20)      910 2022-06-01 11:19:21.000000 genbase-0.3.2/genbase/test/test_internationalization.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.253024 genbase-0.3.2/genbase/ui/
+-rw-r--r--   0 marcelr    (502) staff       (20)     2188 2023-01-29 11:31:51.000000 genbase-0.3.2/genbase/ui/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)    22248 2023-01-28 12:50:57.000000 genbase-0.3.2/genbase/ui/notebook.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.253666 genbase-0.3.2/genbase/ui/plot/
+-rw-r--r--   0 marcelr    (502) staff       (20)     2158 2023-02-23 12:17:06.000000 genbase-0.3.2/genbase/ui/plot/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)      664 2021-12-05 12:25:32.000000 genbase-0.3.2/genbase/ui/svg.py
+-rw-r--r--   0 marcelr    (502) staff       (20)     8810 2023-01-28 11:01:33.000000 genbase-0.3.2/genbase/utils.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.245396 genbase-0.3.2/genbase.egg-info/
+-rw-r--r--   0 marcelr    (502) staff       (20)    13008 2023-05-22 09:43:04.000000 genbase-0.3.2/genbase.egg-info/PKG-INFO
+-rw-r--r--   0 marcelr    (502) staff       (20)      660 2023-05-22 09:43:04.000000 genbase-0.3.2/genbase.egg-info/SOURCES.txt
+-rw-r--r--   0 marcelr    (502) staff       (20)        1 2023-05-22 09:43:04.000000 genbase-0.3.2/genbase.egg-info/dependency_links.txt
+-rw-r--r--   0 marcelr    (502) staff       (20)      240 2023-05-22 09:43:04.000000 genbase-0.3.2/genbase.egg-info/requires.txt
+-rw-r--r--   0 marcelr    (502) staff       (20)        8 2023-05-22 09:43:04.000000 genbase-0.3.2/genbase.egg-info/top_level.txt
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:43:04.255200 genbase-0.3.2/img/
+-rw-r--r--   0 marcelr    (502) staff       (20)      612 2021-11-18 11:32:43.000000 genbase-0.3.2/img/gb.png
+-rw-r--r--   0 marcelr    (502) staff       (20)     2915 2021-11-18 11:34:55.000000 genbase-0.3.2/img/genbase.png
+-rw-r--r--   0 marcelr    (502) staff       (20)       38 2023-05-22 09:43:04.256245 genbase-0.3.2/setup.cfg
+-rw-r--r--   0 marcelr    (502) staff       (20)     1504 2023-01-26 16:10:20.000000 genbase-0.3.2/setup.py
```

### Comparing `genbase-0.3.1/.gitignore` & `genbase-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/CHANGELOG.md` & `genbase-0.3.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/LICENSE` & `genbase-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/PKG-INFO` & `genbase-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genbase
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generation base dependency
 Home-page: https://git.science.uu.nl/m.j.robeer/genbase
 Author: Marcel Robeer
 Author-email: m.j.robeer@uu.nl
 License: GNU LGPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: genbase Version: 0.3.1 Summary: Generation base
+Metadata-Version: 2.1 Name: genbase Version: 0.3.2 Summary: Generation base
 dependency Home-page: https://git.science.uu.nl/m.j.robeer/genbase Author:
 Marcel Robeer Author-email: m.j.robeer@uu.nl License: GNU LGPL v3 Classifier:
 Development Status :: 3 - Alpha Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or
 later (LGPLv3+) Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE *
```

### Comparing `genbase-0.3.1/README.md` & `genbase-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/__init__.py` & `genbase-0.3.2/genbase/__init__.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/data/__init__.py` & `genbase-0.3.2/genbase/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,22 @@
     elif compression == 'xz':
         from pandas.compat import get_lzma_file
         return get_lzma_file()(handle, mode=mode)
     elif compression == 'zip':
         from pandas.io.common import _BytesZipFile
 
         handle = _BytesZipFile(handle, mode)
+        handle = handle.buffer if hasattr(handle, 'buffer') else handle
         if handle.mode == "r":
             zip_names = handle.namelist()
 
             if len(zip_names) == 0:
                 raise ValueError(f'Empty ZIP file "{ioargs.filepath_or_buffer}"')
             return [handle.open(name) for name in zip_names]
-    raise NotImplementedError(f'Unable to process "{handle}" with compressiong method "{compression}"!')
+    raise NotImplementedError(f'Unable to process "{handle}" with compression method "{compression}"!')
 
 
 def pandas_to_instancelib(dataset, data_cols, label_cols, label_map=None):
     env = il.pandas_to_env(dataset, data_cols, label_cols)
     if label_map is not None:
         if isinstance(label_map, dict):
             label_map = {str(k): v for k, v in label_map.items()}
```

### Comparing `genbase-0.3.1/genbase/decorator.py` & `genbase-0.3.2/genbase/decorator.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/internationalization.py` & `genbase-0.3.2/genbase/internationalization.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/mixin.py` & `genbase-0.3.2/genbase/mixin.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/model/__init__.py` & `genbase-0.3.2/genbase/model/__init__.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/test/test_internationalization.py` & `genbase-0.3.2/genbase/test/test_internationalization.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/ui/__init__.py` & `genbase-0.3.2/genbase/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/ui/notebook.py` & `genbase-0.3.2/genbase/ui/notebook.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/ui/plot/__init__.py` & `genbase-0.3.2/genbase/ui/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/ui/svg.py` & `genbase-0.3.2/genbase/ui/svg.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase/utils.py` & `genbase-0.3.2/genbase/utils.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/genbase.egg-info/PKG-INFO` & `genbase-0.3.2/genbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genbase
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generation base dependency
 Home-page: https://git.science.uu.nl/m.j.robeer/genbase
 Author: Marcel Robeer
 Author-email: m.j.robeer@uu.nl
 License: GNU LGPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: genbase Version: 0.3.1 Summary: Generation base
+Metadata-Version: 2.1 Name: genbase Version: 0.3.2 Summary: Generation base
 dependency Home-page: https://git.science.uu.nl/m.j.robeer/genbase Author:
 Marcel Robeer Author-email: m.j.robeer@uu.nl License: GNU LGPL v3 Classifier:
 Development Status :: 3 - Alpha Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or
 later (LGPLv3+) Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE *
```

### Comparing `genbase-0.3.1/genbase.egg-info/SOURCES.txt` & `genbase-0.3.2/genbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/img/gb.png` & `genbase-0.3.2/img/gb.png`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/img/genbase.png` & `genbase-0.3.2/img/genbase.png`

 * *Files identical despite different names*

### Comparing `genbase-0.3.1/setup.py` & `genbase-0.3.2/setup.py`

 * *Files identical despite different names*

