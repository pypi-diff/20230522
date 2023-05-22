# Comparing `tmp/betterdataclass-2.0.tar.gz` & `tmp/betterdataclass-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterdataclass-2.0.tar", last modified: Mon May 22 14:03:33 2023, max compression
+gzip compressed data, was "betterdataclass-2.1.tar", last modified: Sat May 20 08:27:50 2023, max compression
```

## Comparing `betterdataclass-2.0.tar` & `betterdataclass-2.1.tar`

### file list

```diff
@@ -1,19 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:03:33.072818 betterdataclass-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 14:03:22.000000 betterdataclass-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-22 14:03:33.072818 betterdataclass-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-22 14:03:22.000000 betterdataclass-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:03:33.068818 betterdataclass-2.0/betterdataclass/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-22 14:03:22.000000 betterdataclass-2.0/betterdataclass/StrictDictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-22 14:03:22.000000 betterdataclass-2.0/betterdataclass/StrictList.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 14:03:22.000000 betterdataclass-2.0/betterdataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:03:33.072818 betterdataclass-2.0/betterdataclass/helper/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 14:03:22.000000 betterdataclass-2.0/betterdataclass/helper/initiate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-22 14:03:22.000000 betterdataclass-2.0/betterdataclass/helper/to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 14:03:22.000000 betterdataclass-2.0/betterdataclass/helper/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:03:33.072818 betterdataclass-2.0/betterdataclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-22 14:03:33.000000 betterdataclass-2.0/betterdataclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 14:03:33.000000 betterdataclass-2.0/betterdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:03:33.000000 betterdataclass-2.0/betterdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 14:03:33.000000 betterdataclass-2.0/betterdataclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:03:33.072818 betterdataclass-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 14:03:22.000000 betterdataclass-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:27:50.396816 betterdataclass-2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 08:27:37.000000 betterdataclass-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-20 08:27:50.392816 betterdataclass-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-20 08:27:37.000000 betterdataclass-2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:27:50.392816 betterdataclass-2.1/betterdataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-20 08:27:37.000000 betterdataclass-2.1/betterdataclass/StrictDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-20 08:27:37.000000 betterdataclass-2.1/betterdataclass/StrictList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-20 08:27:37.000000 betterdataclass-2.1/betterdataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:27:50.392816 betterdataclass-2.1/betterdataclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-20 08:27:50.000000 betterdataclass-2.1/betterdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-20 08:27:50.000000 betterdataclass-2.1/betterdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:27:50.000000 betterdataclass-2.1/betterdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 08:27:50.000000 betterdataclass-2.1/betterdataclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:27:50.396816 betterdataclass-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-20 08:27:37.000000 betterdataclass-2.1/setup.py
```

### Comparing `betterdataclass-2.0/LICENSE` & `betterdataclass-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betterdataclass-2.0/PKG-INFO` & `betterdataclass-2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 2.0
+Version: 2.1
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
-Home-page: https://github.com/dvnasutosh/betterdataclasses
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
 
-Go to github.com/dvnasutosh/betterdataclasses
+`betterdataclass` is a Python library that enhances the functionality of the existing `dataclass` system. It provides additional features and improvements to make working with data classes even better.
```

### Comparing `betterdataclass-2.0/README.md` & `betterdataclass-2.1/README.md`

 * *Files identical despite different names*

### Comparing `betterdataclass-2.0/betterdataclass/StrictDictionary.py` & `betterdataclass-2.1/betterdataclass/StrictDictionary.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-2.0/betterdataclass/StrictList.py` & `betterdataclass-2.1/betterdataclass/StrictList.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-2.0/betterdataclass.egg-info/PKG-INFO` & `betterdataclass-2.1/betterdataclass.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 2.0
+Version: 2.1
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
-Home-page: https://github.com/dvnasutosh/betterdataclasses
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
 
-Go to github.com/dvnasutosh/betterdataclasses
+`betterdataclass` is a Python library that enhances the functionality of the existing `dataclass` system. It provides additional features and improvements to make working with data classes even better.
```

### Comparing `betterdataclass-2.0/setup.py` & `betterdataclass-2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from setuptools import setup
-
 setup(
     name="betterdataclass",
-    version="2.0",
+    version="2.01",
     description="A multipurpose dataclass libarary used for validation and data structuring.",
-    long_description="Go to github.com/dvnasutosh/betterdataclasses",
-    url='https://github.com/dvnasutosh/betterdataclasses',
-    
+    long_description="`betterdataclass` is a Python library that enhances the functionality of the existing `dataclass` system. It provides additional features and improvements to make working with data classes even better.",
     author="Asutosh Rath",
     author_email="dvnasutosh@gmail.com",
-    packages=['betterdataclass','betterdataclass.helper'],
+    packages=['betterdataclass'],
         classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

