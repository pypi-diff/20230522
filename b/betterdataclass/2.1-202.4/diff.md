# Comparing `tmp/betterdataclass-2.1.tar.gz` & `tmp/betterdataclass-202.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterdataclass-2.1.tar", last modified: Sat May 20 08:27:50 2023, max compression
+gzip compressed data, was "betterdataclass-202.4.tar", last modified: Mon May 22 15:46:48 2023, max compression
```

## Comparing `betterdataclass-2.1.tar` & `betterdataclass-202.4.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:27:50.396816 betterdataclass-2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 08:27:37.000000 betterdataclass-2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-20 08:27:50.392816 betterdataclass-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-20 08:27:37.000000 betterdataclass-2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:27:50.392816 betterdataclass-2.1/betterdataclass/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-20 08:27:37.000000 betterdataclass-2.1/betterdataclass/StrictDictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-20 08:27:37.000000 betterdataclass-2.1/betterdataclass/StrictList.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-20 08:27:37.000000 betterdataclass-2.1/betterdataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:27:50.392816 betterdataclass-2.1/betterdataclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-20 08:27:50.000000 betterdataclass-2.1/betterdataclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-20 08:27:50.000000 betterdataclass-2.1/betterdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:27:50.000000 betterdataclass-2.1/betterdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 08:27:50.000000 betterdataclass-2.1/betterdataclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:27:50.396816 betterdataclass-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-20 08:27:37.000000 betterdataclass-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:48.981143 betterdataclass-202.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 15:46:37.000000 betterdataclass-202.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-22 15:46:48.977143 betterdataclass-202.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-22 15:46:37.000000 betterdataclass-202.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:48.977143 betterdataclass-202.4/betterdataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/StrictDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/StrictList.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:48.977143 betterdataclass-202.4/betterdataclass/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/helper/initiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/helper/to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/helper/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:48.977143 betterdataclass-202.4/betterdataclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-22 15:46:48.000000 betterdataclass-202.4/betterdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-22 15:46:48.000000 betterdataclass-202.4/betterdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:46:48.000000 betterdataclass-202.4/betterdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 15:46:48.000000 betterdataclass-202.4/betterdataclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 15:46:37.000000 betterdataclass-202.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:46:48.981143 betterdataclass-202.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-22 15:46:37.000000 betterdataclass-202.4/setup.py
```

### Comparing `betterdataclass-2.1/LICENSE` & `betterdataclass-202.4/LICENSE`

 * *Files identical despite different names*

### Comparing `betterdataclass-2.1/PKG-INFO` & `betterdataclass-202.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 2.1
+Version: 202.4
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
+Home-page: https://github.com/dvnasutosh/betterdataclasses
 Author: Asutosh Rath
 Author-email: dvnasutosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
 
-`betterdataclass` is a Python library that enhances the functionality of the existing `dataclass` system. It provides additional features and improvements to make working with data classes even better.
+Go to github.com/dvnasutosh/betterdataclasses
```

### Comparing `betterdataclass-2.1/README.md` & `betterdataclass-202.4/README.md`

 * *Files identical despite different names*

### Comparing `betterdataclass-2.1/betterdataclass/StrictDictionary.py` & `betterdataclass-202.4/betterdataclass/StrictDictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from typing import get_args, get_args, get_args, Final, Final, Final, Any,get_origin
 
 import json
-from betterdataclass.helper.to_dict import to_raw_dict
-from betterdataclass.helper.validate import validate
-from betterdataclass.helper.initiate import initialize
+from .helper.to_dict import to_raw_dict
+from .helper.validate import validate
+from .helper.initiate import initialize
 
 class Dictionary(object):
     """
     A class that can be used to create a dictionary-like object with arbitrary key-value pairs.
     """
     def __init__(self, **kwargs) -> None:
         """
```

### Comparing `betterdataclass-2.1/betterdataclass/StrictList.py` & `betterdataclass-202.4/betterdataclass/StrictList.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections.abc import Iterable
 from typing_extensions import SupportsIndex
-from betterdataclass.helper.validate import validate
 from typing import Any
 
+from .helper.validate import validate
+
 class StrictList(list):
     """
     """
     def __init__(self,*data) -> None:
         for each in data:
             if not self.restriction(each):
                 raise ValueError(f"Data does not follow restrictions set for {self.__class__}")
```

### Comparing `betterdataclass-2.1/betterdataclass.egg-info/PKG-INFO` & `betterdataclass-202.4/betterdataclass.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 2.1
+Version: 202.4
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
+Home-page: https://github.com/dvnasutosh/betterdataclasses
 Author: Asutosh Rath
 Author-email: dvnasutosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
 
-`betterdataclass` is a Python library that enhances the functionality of the existing `dataclass` system. It provides additional features and improvements to make working with data classes even better.
+Go to github.com/dvnasutosh/betterdataclasses
```

### Comparing `betterdataclass-2.1/setup.py` & `betterdataclass-202.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,40 @@
-from setuptools import setup
+from setuptools import find_packages, setup
+
 setup(
     name="betterdataclass",
-    version="2.01",
+    version="202.4",
     description="A multipurpose dataclass libarary used for validation and data structuring.",
-    long_description="`betterdataclass` is a Python library that enhances the functionality of the existing `dataclass` system. It provides additional features and improvements to make working with data classes even better.",
+    long_description="Go to github.com/dvnasutosh/betterdataclasses",
+    url='https://github.com/dvnasutosh/betterdataclasses',
+    
     author="Asutosh Rath",
     author_email="dvnasutosh@gmail.com",
-    packages=['betterdataclass'],
+    packages=find_packages(),
+    
+    
         classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)'
     ]
-)
+)
+
+'''
+My directory setup
+betterdataclasses(projectfolder)
+--betterdataclass(libraryfolder)
+----StrictDictionary.py
+----StrictList.py
+----__init__.py
+----helper
+------initiate.py
+------validate.py
+------to_dictr.py
+'''
```

