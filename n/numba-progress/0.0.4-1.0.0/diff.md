# Comparing `tmp/numba-progress-0.0.4.tar.gz` & `tmp/numba-progress-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba-progress-0.0.4.tar", last modified: Thu Nov 10 09:23:02 2022, max compression
+gzip compressed data, was "numba-progress-1.0.0.tar", last modified: Mon May 22 07:34:46 2023, max compression
```

## Comparing `numba-progress-0.0.4.tar` & `numba-progress-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 09:23:02.857493 numba-progress-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-11-10 09:22:45.000000 numba-progress-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 09:22:45.000000 numba-progress-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-11-10 09:23:02.857493 numba-progress-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-11-10 09:22:45.000000 numba-progress-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 09:23:02.857493 numba-progress-0.0.4/numba_progress/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-10 09:22:45.000000 numba-progress-0.0.4/numba_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-10 09:22:45.000000 numba-progress-0.0.4/numba_progress/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6156 2022-11-10 09:22:45.000000 numba-progress-0.0.4/numba_progress/numba_atomic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6466 2022-11-10 09:22:45.000000 numba-progress-0.0.4/numba_progress/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 09:23:02.857493 numba-progress-0.0.4/numba_progress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-11-10 09:23:02.000000 numba-progress-0.0.4/numba_progress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-10 09:23:02.000000 numba-progress-0.0.4/numba_progress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 09:23:02.000000 numba-progress-0.0.4/numba_progress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-10 09:23:02.000000 numba-progress-0.0.4/numba_progress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 09:23:02.000000 numba-progress-0.0.4/numba_progress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 09:23:02.000000 numba-progress-0.0.4/numba_progress.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-10 09:22:45.000000 numba-progress-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 09:23:02.857493 numba-progress-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-11-10 09:22:45.000000 numba-progress-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:46.779036 numba-progress-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 07:34:26.000000 numba-progress-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 07:34:26.000000 numba-progress-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-22 07:34:46.779036 numba-progress-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-22 07:34:26.000000 numba-progress-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:46.779036 numba-progress-1.0.0/numba_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 07:34:26.000000 numba-progress-1.0.0/numba_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 07:34:26.000000 numba-progress-1.0.0/numba_progress/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-22 07:34:26.000000 numba-progress-1.0.0/numba_progress/numba_atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-22 07:34:26.000000 numba-progress-1.0.0/numba_progress/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:46.779036 numba-progress-1.0.0/numba_progress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-22 07:34:46.000000 numba-progress-1.0.0/numba_progress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 07:34:46.000000 numba-progress-1.0.0/numba_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:34:46.000000 numba-progress-1.0.0/numba_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 07:34:46.000000 numba-progress-1.0.0/numba_progress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 07:34:46.000000 numba-progress-1.0.0/numba_progress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:34:46.000000 numba-progress-1.0.0/numba_progress.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 07:34:26.000000 numba-progress-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:34:46.779036 numba-progress-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-22 07:34:26.000000 numba-progress-1.0.0/setup.py
```

### Comparing `numba-progress-0.0.4/LICENSE` & `numba-progress-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numba-progress-0.0.4/PKG-INFO` & `numba-progress-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-progress
-Version: 0.0.4
+Version: 1.0.0
 Summary: A progress bar implementation for numba functions using tqdm
 Home-page: https://github.com/mortacious/numba-progress
 Author: Felix Igelbrink
 Author-email: felix.igelbrink@uni-osnabrueck.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/numba-progress/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `numba-progress-0.0.4/README.md` & `numba-progress-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `numba-progress-0.0.4/numba_progress/numba_atomic.py` & `numba-progress-1.0.0/numba_progress/numba_atomic.py`

 * *Files identical despite different names*

### Comparing `numba-progress-0.0.4/numba_progress/progress.py` & `numba-progress-1.0.0/numba_progress/progress.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from numba.extending import overload_method, typeof_impl, as_numba_type, models, register_model, \
     make_attribute_wrapper, overload_attribute, unbox, NativeValue, box
 from .numba_atomic import atomic_add
 from numba import types
 from numba.core import cgutils
 from numba.core.boxing import unbox_array
 
-__all__ = ['ProgressBar']
+__all__ = ['ProgressBar', 'ProgressBarType']
 
 def is_notebook():
     """Determine if we're running within an IPython kernel
 
     >>> is_notebook()
     False
     """
@@ -117,73 +117,74 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
 
 # Numba Native Implementation for the ProgressBar Class
 
-class ProgressBarType(types.Type):
+class ProgressBarTypeImpl(types.Type):
     def __init__(self):
         super().__init__(name='ProgressBar')
 
 
-progressbar_type = ProgressBarType()
+# This is the numba type representation of the ProgressBar class to be used in signatures
+ProgressBarType = ProgressBarTypeImpl()
 
 
 @typeof_impl.register(ProgressBar)
 def typeof_index(val, c):
-    return progressbar_type
+    return ProgressBarType
 
 
-as_numba_type.register(ProgressBar, progressbar_type)
+as_numba_type.register(ProgressBar, ProgressBarType)
 
 
-@register_model(ProgressBarType)
+@register_model(ProgressBarTypeImpl)
 class ProgressBarModel(models.StructModel):
     def __init__(self, dmm, fe_type):
         members = [
             ('hook', types.Array(types.uint64, 1, 'C')),
         ]
         models.StructModel.__init__(self, dmm, fe_type, members)
 
 
 # make the hook attribute accessible
-make_attribute_wrapper(ProgressBarType, 'hook', 'hook')
+make_attribute_wrapper(ProgressBarTypeImpl, 'hook', 'hook')
 
 
-@overload_attribute(ProgressBarType, 'value')
+@overload_attribute(ProgressBarTypeImpl, 'value')
 def get_value(progress_bar):
     def getter(progress_bar):
         return progress_bar.hook[0]
     return getter
 
 
-@unbox(ProgressBarType)
+@unbox(ProgressBarTypeImpl)
 def unbox_progressbar(typ, obj, c):
     """
     Convert a ProgressBar to it's native representation (proxy object)
     """
     hook_obj = c.pyapi.object_getattr_string(obj, 'hook')
     progress_bar = cgutils.create_struct_proxy(typ)(c.context, c.builder)
     progress_bar.hook = unbox_array(types.Array(types.uint64, 1, 'C'), hook_obj, c).value
     c.pyapi.decref(hook_obj)
     is_error = cgutils.is_not_null(c.builder, c.pyapi.err_occurred())
     return NativeValue(progress_bar._getvalue(), is_error=is_error)
 
 
-@box(ProgressBarType)
+@box(ProgressBarTypeImpl)
 def box_progressbar(typ, val, c):
     raise TypeError("Native representation of ProgressBar cannot be converted back to a python object "
                     "as it contains internal python state.")
 
 
-@overload_method(ProgressBarType, "update", jit_options={"nogil": True})
+@overload_method(ProgressBarTypeImpl, "update", jit_options={"nogil": True})
 def _ol_update(self, n=1):
     """
     Numpy implementation of the update method.
     """
-    if isinstance(self, ProgressBarType):
+    if isinstance(self, ProgressBarTypeImpl):
         def _update_impl(self, n=1):
             atomic_add(self.hook, 0, n)
         return _update_impl
```

### Comparing `numba-progress-0.0.4/numba_progress.egg-info/PKG-INFO` & `numba-progress-1.0.0/numba_progress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-progress
-Version: 0.0.4
+Version: 1.0.0
 Summary: A progress bar implementation for numba functions using tqdm
 Home-page: https://github.com/mortacious/numba-progress
 Author: Felix Igelbrink
 Author-email: felix.igelbrink@uni-osnabrueck.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/numba-progress/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `numba-progress-0.0.4/setup.py` & `numba-progress-1.0.0/setup.py`

 * *Files identical despite different names*

