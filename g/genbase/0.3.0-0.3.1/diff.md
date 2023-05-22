# Comparing `tmp/genbase-0.3.0.tar.gz` & `tmp/genbase-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genbase-0.3.0.tar", last modified: Wed Feb 22 17:49:05 2023, max compression
+gzip compressed data, was "genbase-0.3.1.tar", last modified: Mon May 22 09:36:31 2023, max compression
```

## Comparing `genbase-0.3.0.tar` & `genbase-0.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.607981 genbase-0.3.0/
--rw-r--r--   0 marcelr    (502) staff       (20)      284 2022-03-04 11:29:53.000000 genbase-0.3.0/.flake8
--rw-r--r--   0 marcelr    (502) staff       (20)     2099 2021-11-18 11:01:25.000000 genbase-0.3.0/.gitignore
--rw-r--r--   0 marcelr    (502) staff       (20)      475 2022-06-01 11:19:34.000000 genbase-0.3.0/.gitlab-ci.yml
--rw-r--r--   0 marcelr    (502) staff       (20)     8139 2023-02-22 17:48:30.000000 genbase-0.3.0/CHANGELOG.md
--rw-r--r--   0 marcelr    (502) staff       (20)     7651 2021-11-18 11:00:43.000000 genbase-0.3.0/LICENSE
--rw-r--r--   0 marcelr    (502) staff       (20)       40 2022-03-04 14:42:50.000000 genbase-0.3.0/MANIFEST.in
--rw-r--r--   0 marcelr    (502) staff       (20)      264 2022-06-01 09:21:57.000000 genbase-0.3.0/Makefile
--rw-r--r--   0 marcelr    (502) staff       (20)    13028 2023-02-22 17:49:05.607416 genbase-0.3.0/PKG-INFO
--rw-r--r--   0 marcelr    (502) staff       (20)    12452 2023-01-30 09:01:57.000000 genbase-0.3.0/README.md
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.584009 genbase-0.3.0/genbase/
--rw-r--r--   0 marcelr    (502) staff       (20)     7541 2023-02-22 14:23:45.000000 genbase-0.3.0/genbase/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)       86 2023-02-22 17:48:45.000000 genbase-0.3.0/genbase/_version.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.591501 genbase-0.3.0/genbase/data/
--rw-r--r--   0 marcelr    (502) staff       (20)    10423 2023-01-26 15:45:01.000000 genbase-0.3.0/genbase/data/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)     1755 2022-06-01 09:25:31.000000 genbase-0.3.0/genbase/decorator.py
--rw-r--r--   0 marcelr    (502) staff       (20)     2341 2022-03-21 10:23:10.000000 genbase-0.3.0/genbase/internationalization.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.592652 genbase-0.3.0/genbase/locale/
--rw-r--r--   0 marcelr    (502) staff       (20)       87 2021-11-27 18:49:35.000000 genbase-0.3.0/genbase/locale/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)      356 2021-11-27 19:00:44.000000 genbase-0.3.0/genbase/locale/en.json
--rw-r--r--   0 marcelr    (502) staff       (20)      363 2021-10-02 13:07:17.000000 genbase-0.3.0/genbase/locale/nl.json
--rw-r--r--   0 marcelr    (502) staff       (20)     2763 2022-06-01 09:24:24.000000 genbase-0.3.0/genbase/mixin.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.593050 genbase-0.3.0/genbase/model/
--rw-r--r--   0 marcelr    (502) staff       (20)     6979 2022-06-01 11:19:21.000000 genbase-0.3.0/genbase/model/__init__.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.593448 genbase-0.3.0/genbase/test/
--rw-r--r--   0 marcelr    (502) staff       (20)      910 2022-06-01 11:19:21.000000 genbase-0.3.0/genbase/test/test_internationalization.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.594717 genbase-0.3.0/genbase/ui/
--rw-r--r--   0 marcelr    (502) staff       (20)     2188 2023-01-29 11:31:51.000000 genbase-0.3.0/genbase/ui/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)    22248 2023-01-28 12:50:57.000000 genbase-0.3.0/genbase/ui/notebook.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.595125 genbase-0.3.0/genbase/ui/plot/
--rw-r--r--   0 marcelr    (502) staff       (20)     2089 2023-02-22 17:45:52.000000 genbase-0.3.0/genbase/ui/plot/__init__.py
--rw-r--r--   0 marcelr    (502) staff       (20)      664 2021-12-05 12:25:32.000000 genbase-0.3.0/genbase/ui/svg.py
--rw-r--r--   0 marcelr    (502) staff       (20)     8810 2023-01-28 11:01:33.000000 genbase-0.3.0/genbase/utils.py
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.591119 genbase-0.3.0/genbase.egg-info/
--rw-r--r--   0 marcelr    (502) staff       (20)    13028 2023-02-22 17:49:05.000000 genbase-0.3.0/genbase.egg-info/PKG-INFO
--rw-r--r--   0 marcelr    (502) staff       (20)      660 2023-02-22 17:49:05.000000 genbase-0.3.0/genbase.egg-info/SOURCES.txt
--rw-r--r--   0 marcelr    (502) staff       (20)        1 2023-02-22 17:49:05.000000 genbase-0.3.0/genbase.egg-info/dependency_links.txt
--rw-r--r--   0 marcelr    (502) staff       (20)      240 2023-02-22 17:49:05.000000 genbase-0.3.0/genbase.egg-info/requires.txt
--rw-r--r--   0 marcelr    (502) staff       (20)        8 2023-02-22 17:49:05.000000 genbase-0.3.0/genbase.egg-info/top_level.txt
-drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-02-22 17:49:05.606814 genbase-0.3.0/img/
--rw-r--r--   0 marcelr    (502) staff       (20)      612 2021-11-18 11:32:43.000000 genbase-0.3.0/img/gb.png
--rw-r--r--   0 marcelr    (502) staff       (20)     2915 2021-11-18 11:34:55.000000 genbase-0.3.0/img/genbase.png
--rw-r--r--   0 marcelr    (502) staff       (20)       38 2023-02-22 17:49:05.608129 genbase-0.3.0/setup.cfg
--rw-r--r--   0 marcelr    (502) staff       (20)     1504 2023-01-26 16:10:20.000000 genbase-0.3.0/setup.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.572032 genbase-0.3.1/
+-rw-r--r--   0 marcelr    (502) staff       (20)      284 2022-03-04 11:29:53.000000 genbase-0.3.1/.flake8
+-rw-r--r--   0 marcelr    (502) staff       (20)     2099 2021-11-18 11:01:25.000000 genbase-0.3.1/.gitignore
+-rw-r--r--   0 marcelr    (502) staff       (20)      475 2022-06-01 11:19:34.000000 genbase-0.3.1/.gitlab-ci.yml
+-rw-r--r--   0 marcelr    (502) staff       (20)     8253 2023-05-22 09:35:35.000000 genbase-0.3.1/CHANGELOG.md
+-rw-r--r--   0 marcelr    (502) staff       (20)     7651 2021-11-18 11:00:43.000000 genbase-0.3.1/LICENSE
+-rw-r--r--   0 marcelr    (502) staff       (20)       40 2022-03-04 14:42:50.000000 genbase-0.3.1/MANIFEST.in
+-rw-r--r--   0 marcelr    (502) staff       (20)      264 2022-06-01 09:21:57.000000 genbase-0.3.1/Makefile
+-rw-r--r--   0 marcelr    (502) staff       (20)    13008 2023-05-22 09:36:31.571528 genbase-0.3.1/PKG-INFO
+-rw-r--r--   0 marcelr    (502) staff       (20)    12452 2023-01-30 09:01:57.000000 genbase-0.3.1/README.md
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.550149 genbase-0.3.1/genbase/
+-rw-r--r--   0 marcelr    (502) staff       (20)     7541 2023-02-22 14:23:45.000000 genbase-0.3.1/genbase/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)       86 2023-05-22 09:34:57.000000 genbase-0.3.1/genbase/_version.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.555686 genbase-0.3.1/genbase/data/
+-rw-r--r--   0 marcelr    (502) staff       (20)    10546 2023-05-22 09:34:38.000000 genbase-0.3.1/genbase/data/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)     1755 2022-06-01 09:25:31.000000 genbase-0.3.1/genbase/decorator.py
+-rw-r--r--   0 marcelr    (502) staff       (20)     2341 2022-03-21 10:23:10.000000 genbase-0.3.1/genbase/internationalization.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.562061 genbase-0.3.1/genbase/locale/
+-rw-r--r--   0 marcelr    (502) staff       (20)       87 2021-11-27 18:49:35.000000 genbase-0.3.1/genbase/locale/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)      356 2021-11-27 19:00:44.000000 genbase-0.3.1/genbase/locale/en.json
+-rw-r--r--   0 marcelr    (502) staff       (20)      363 2021-10-02 13:07:17.000000 genbase-0.3.1/genbase/locale/nl.json
+-rw-r--r--   0 marcelr    (502) staff       (20)     2763 2022-06-01 09:24:24.000000 genbase-0.3.1/genbase/mixin.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.562571 genbase-0.3.1/genbase/model/
+-rw-r--r--   0 marcelr    (502) staff       (20)     6979 2022-06-01 11:19:21.000000 genbase-0.3.1/genbase/model/__init__.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.563242 genbase-0.3.1/genbase/test/
+-rw-r--r--   0 marcelr    (502) staff       (20)      910 2022-06-01 11:19:21.000000 genbase-0.3.1/genbase/test/test_internationalization.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.565819 genbase-0.3.1/genbase/ui/
+-rw-r--r--   0 marcelr    (502) staff       (20)     2188 2023-01-29 11:31:51.000000 genbase-0.3.1/genbase/ui/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)    22248 2023-01-28 12:50:57.000000 genbase-0.3.1/genbase/ui/notebook.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.566631 genbase-0.3.1/genbase/ui/plot/
+-rw-r--r--   0 marcelr    (502) staff       (20)     2158 2023-02-23 12:17:06.000000 genbase-0.3.1/genbase/ui/plot/__init__.py
+-rw-r--r--   0 marcelr    (502) staff       (20)      664 2021-12-05 12:25:32.000000 genbase-0.3.1/genbase/ui/svg.py
+-rw-r--r--   0 marcelr    (502) staff       (20)     8810 2023-01-28 11:01:33.000000 genbase-0.3.1/genbase/utils.py
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.554968 genbase-0.3.1/genbase.egg-info/
+-rw-r--r--   0 marcelr    (502) staff       (20)    13008 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/PKG-INFO
+-rw-r--r--   0 marcelr    (502) staff       (20)      660 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/SOURCES.txt
+-rw-r--r--   0 marcelr    (502) staff       (20)        1 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/dependency_links.txt
+-rw-r--r--   0 marcelr    (502) staff       (20)      240 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/requires.txt
+-rw-r--r--   0 marcelr    (502) staff       (20)        8 2023-05-22 09:36:31.000000 genbase-0.3.1/genbase.egg-info/top_level.txt
+drwxr-xr-x   0 marcelr    (502) staff       (20)        0 2023-05-22 09:36:31.570845 genbase-0.3.1/img/
+-rw-r--r--   0 marcelr    (502) staff       (20)      612 2021-11-18 11:32:43.000000 genbase-0.3.1/img/gb.png
+-rw-r--r--   0 marcelr    (502) staff       (20)     2915 2021-11-18 11:34:55.000000 genbase-0.3.1/img/genbase.png
+-rw-r--r--   0 marcelr    (502) staff       (20)       38 2023-05-22 09:36:31.572119 genbase-0.3.1/setup.cfg
+-rw-r--r--   0 marcelr    (502) staff       (20)     1504 2023-01-26 16:10:20.000000 genbase-0.3.1/setup.py
```

### Comparing `genbase-0.3.0/.gitignore` & `genbase-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/CHANGELOG.md` & `genbase-0.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to `genbase` will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.1] - 2023-05-22
+### Fixed
+- Support for `pandas==1.5.3`
+
 ## [0.3.0] - 2023-02-22
 ### Added
 - Ability to adjust visualization of `plotly` plots with `update_layout()` and `update_traces()`
 
 ## [0.2.20] - 2023-01-29
 ### Fixed
 - Hotfix for Google Colab rendering
@@ -255,14 +259,15 @@
 - `CHANGELOG.md`
 - `git` setup
 - Moved mixins from `text_sensitivity` to `genbase`
 - Moved machine learning model imports from `text_explainability` to `genbase`
 - Moved data wrappers from `text_explainability` to `genbase`
 
 [Unreleased]: https://git.science.uu.nl/m.j.robeer/genbase
+[0.3.1]: https://pypi.org/project/genbase/0.3.1/
 [0.3.0]: https://pypi.org/project/genbase/0.3.0/
 [0.2.20]: https://pypi.org/project/genbase/0.2.20/
 [0.2.15]: https://pypi.org/project/genbase/0.2.15/
 [0.2.14]: https://pypi.org/project/genbase/0.2.14/
 [0.2.13]: https://pypi.org/project/genbase/0.2.13/
 [0.2.12]: https://pypi.org/project/genbase/0.2.12/
 [0.2.11]: https://pypi.org/project/genbase/0.2.11/
```

### Comparing `genbase-0.3.0/LICENSE` & `genbase-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/PKG-INFO` & `genbase-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: genbase
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generation base dependency
 Home-page: https://git.science.uu.nl/m.j.robeer/genbase
 Author: Marcel Robeer
 Author-email: m.j.robeer@uu.nl
 License: GNU LGPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -314,9 +313,7 @@
 ...         return type.replace(' ').title() if 'explanation' in type else type
 
 >>> from genbase import MetaInfo
 >>> NiceCls(MetaInfo):
 ...     def __init__(self, **kwargs):
 ...         super().__init__(renderer=CustomRenderer, **kwargs)
 ```
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: genbase Version: 0.3.0 Summary: Generation base
+Metadata-Version: 2.1 Name: genbase Version: 0.3.1 Summary: Generation base
 dependency Home-page: https://git.science.uu.nl/m.j.robeer/genbase Author:
-Marcel Robeer Author-email: m.j.robeer@uu.nl License: GNU LGPL v3 Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Programming
-Language :: Python Classifier: License :: OSI Approved :: GNU Lesser General
-Public License v3 or later (LGPLv3+) Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE *
+Marcel Robeer Author-email: m.j.robeer@uu.nl License: GNU LGPL v3 Classifier:
+Development Status :: 3 - Alpha Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or
+later (LGPLv3+) Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE *
                                 [genbase logo]*
 **
                     **** Generation base dependency** ****
 [![PyPI](https://img.shields.io/pypi/v/genbase)](https://pypi.org/project/
 genbase/) [![Python_version](https://img.shields.io/badge/python-
 3.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/genbase/) [!
 [Build_passing](https://img.shields.io/badge/build-passing-brightgreen)](https:
```

### Comparing `genbase-0.3.0/README.md` & `genbase-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/__init__.py` & `genbase-0.3.1/genbase/__init__.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/data/__init__.py` & `genbase-0.3.1/genbase/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,16 @@
         label_cols = [label_cols]
 
     file_type = get_file_type(dataset)
     path_like = isinstance(dataset, str)
 
     # Unpack archived file
     extensions = pd.io.common._compression_to_extension.values() if hasattr(pd.io.common, '_compression_to_extension') \
-        else pd.io.common.extension_to_compression.keys()
+        else (pd.io.common._extension_to_compression.keys() if hasattr(pd.io.common, '_extension_to_compression') else \
+              pd.io.common.extension_to_compression.keys())
     if file_type in extensions:
         ioargs = pd.io.common._get_filepath_or_buffer(dataset, compression=file_type.replace('.', ''))
         info(f'Unpacking file "{dataset}".')
         return import_from_key_values([(file.name, file) for file in get_compressed_files(ioargs)],
                                       data_cols=data_cols,
                                       label_cols=label_cols,
                                       label_map=label_map,
```

### Comparing `genbase-0.3.0/genbase/decorator.py` & `genbase-0.3.1/genbase/decorator.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/internationalization.py` & `genbase-0.3.1/genbase/internationalization.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/mixin.py` & `genbase-0.3.1/genbase/mixin.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/model/__init__.py` & `genbase-0.3.1/genbase/model/__init__.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/test/test_internationalization.py` & `genbase-0.3.1/genbase/test/test_internationalization.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/ui/__init__.py` & `genbase-0.3.1/genbase/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/ui/notebook.py` & `genbase-0.3.1/genbase/ui/notebook.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/ui/plot/__init__.py` & `genbase-0.3.1/genbase/ui/plot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     """
     import importlib.util
     return importlib.util.find_spec('plotly') is not None
 
 
 class ExpressPlot:
     def __init__(self, df: pd.DataFrame, px_fn: Callable, *args, **kwargs):
-        self.plot = px_fn(df, *args, **kwargs)
+        template = kwargs.pop('template', 'none')
+        self.plot = px_fn(df, *args, template=template, **kwargs)
 
     @property
     def static(self):
         return self.to_png()
 
     @property
     def interactive(self) -> str:
```

### Comparing `genbase-0.3.0/genbase/ui/svg.py` & `genbase-0.3.1/genbase/ui/svg.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase/utils.py` & `genbase-0.3.1/genbase/utils.py`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/genbase.egg-info/PKG-INFO` & `genbase-0.3.1/genbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: genbase
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generation base dependency
 Home-page: https://git.science.uu.nl/m.j.robeer/genbase
 Author: Marcel Robeer
 Author-email: m.j.robeer@uu.nl
 License: GNU LGPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -314,9 +313,7 @@
 ...         return type.replace(' ').title() if 'explanation' in type else type
 
 >>> from genbase import MetaInfo
 >>> NiceCls(MetaInfo):
 ...     def __init__(self, **kwargs):
 ...         super().__init__(renderer=CustomRenderer, **kwargs)
 ```
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: genbase Version: 0.3.0 Summary: Generation base
+Metadata-Version: 2.1 Name: genbase Version: 0.3.1 Summary: Generation base
 dependency Home-page: https://git.science.uu.nl/m.j.robeer/genbase Author:
-Marcel Robeer Author-email: m.j.robeer@uu.nl License: GNU LGPL v3 Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Programming
-Language :: Python Classifier: License :: OSI Approved :: GNU Lesser General
-Public License v3 or later (LGPLv3+) Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE *
+Marcel Robeer Author-email: m.j.robeer@uu.nl License: GNU LGPL v3 Classifier:
+Development Status :: 3 - Alpha Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or
+later (LGPLv3+) Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE *
                                 [genbase logo]*
 **
                     **** Generation base dependency** ****
 [![PyPI](https://img.shields.io/pypi/v/genbase)](https://pypi.org/project/
 genbase/) [![Python_version](https://img.shields.io/badge/python-
 3.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/genbase/) [!
 [Build_passing](https://img.shields.io/badge/build-passing-brightgreen)](https:
```

### Comparing `genbase-0.3.0/genbase.egg-info/SOURCES.txt` & `genbase-0.3.1/genbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/img/gb.png` & `genbase-0.3.1/img/gb.png`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/img/genbase.png` & `genbase-0.3.1/img/genbase.png`

 * *Files identical despite different names*

### Comparing `genbase-0.3.0/setup.py` & `genbase-0.3.1/setup.py`

 * *Files identical despite different names*

