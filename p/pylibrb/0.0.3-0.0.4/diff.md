# Comparing `tmp/pylibrb-0.0.3.tar.gz` & `tmp/pylibrb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibrb-0.0.3.tar", last modified: Mon May 22 14:28:52 2023, max compression
+gzip compressed data, was "pylibrb-0.0.4.tar", last modified: Mon May 22 17:41:52 2023, max compression
```

## Comparing `pylibrb-0.0.3.tar` & `pylibrb-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.854421 pylibrb-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-22 14:28:36.000000 pylibrb-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 14:28:36.000000 pylibrb-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 14:28:52.854421 pylibrb-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-22 14:28:36.000000 pylibrb-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 14:28:36.000000 pylibrb-0.0.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 14:28:36.000000 pylibrb-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 14:28:52.854421 pylibrb-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 14:28:36.000000 pylibrb-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.850421 pylibrb-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.854421 pylibrb-0.0.3/src/pylibrb/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 14:28:36.000000 pylibrb-0.0.3/src/pylibrb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36255 2023-05-22 14:28:36.000000 pylibrb-0.0.3/src/pylibrb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:36.000000 pylibrb-0.0.3/src/pylibrb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.854421 pylibrb-0.0.3/src/pylibrb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.854421 pylibrb-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-22 14:28:36.000000 pylibrb-0.0.3/tests/test_stretcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-22 17:41:38.000000 pylibrb-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 17:41:38.000000 pylibrb-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 17:41:52.297926 pylibrb-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-22 17:41:38.000000 pylibrb-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 17:41:38.000000 pylibrb-0.0.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 17:41:38.000000 pylibrb-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 17:41:52.297926 pylibrb-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 17:41:38.000000 pylibrb-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/src/pylibrb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-22 17:41:38.000000 pylibrb-0.0.4/src/pylibrb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:38.000000 pylibrb-0.0.4/src/pylibrb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36163 2023-05-22 17:41:38.000000 pylibrb-0.0.4/src/pylibrb/pylibrb_ext.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/src/pylibrb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-22 17:41:38.000000 pylibrb-0.0.4/tests/test_stretcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-22 17:41:38.000000 pylibrb-0.0.4/tests/test_utils.py
```

### Comparing `pylibrb-0.0.3/LICENSE` & `pylibrb-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.3/PKG-INFO` & `pylibrb-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `pylibrb-0.0.3/README.md` & `pylibrb-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.3/setup.cfg` & `pylibrb-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.3/src/pylibrb/__init__.pyi` & `pylibrb-0.0.4/src/pylibrb/pylibrb_ext.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from enum import Flag
 
 import numpy as np
 
-import pylibrb.pylibrb_ext
-
 MIN_SAMPLE_RATE: int
 '''Minimum sample rate an audio can have.'''
 
 MAX_SAMPLE_RATE: int
 '''Maximum sample rate an audio can have.'''
 
 MAX_CHANNELS_NUM: int
@@ -18,17 +16,14 @@
 
 SAMPLES_AXIS: int
 '''Axis of samples in an audio array.'''
 
 DTYPE_NAME: str
 '''Name of the audio type in NumPy's format.'''
 
-DType: np.dtype
-'''The data type used internally for audio.'''
-
 AUTO_FORMANT_SCALE: float
 '''Default value of `formant_scale`, which causes the scale to be calculated automatically.
 
 See the documentation of `RubberBandStretcher.formant_scale` for more details.
 '''
```

### Comparing `pylibrb-0.0.3/src/pylibrb.egg-info/PKG-INFO` & `pylibrb-0.0.4/src/pylibrb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `pylibrb-0.0.3/tests/test_stretcher.py` & `pylibrb-0.0.4/tests/test_stretcher.py`

 * *Files identical despite different names*

