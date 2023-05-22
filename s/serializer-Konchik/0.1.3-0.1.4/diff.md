# Comparing `tmp/serializer_Konchik-0.1.3.tar.gz` & `tmp/serializer_Konchik-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_Konchik-0.1.3.tar", last modified: Mon May 22 16:59:40 2023, max compression
+gzip compressed data, was "serializer_Konchik-0.1.4.tar", last modified: Mon May 22 17:06:16 2023, max compression
```

## Comparing `serializer_Konchik-0.1.3.tar` & `serializer_Konchik-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.432658 serializer_Konchik-0.1.3/
--rw-rw-rw-   0        0        0      262 2023-05-22 16:59:40.432658 serializer_Konchik-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.421095 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/
--rw-rw-rw-   0        0        0      262 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:59:40.432658 serializer_Konchik-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-05-22 16:58:58.000000 serializer_Konchik-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.423509 serializer_Konchik-0.1.3/src/
--rw-rw-rw-   0        0        0      131 2023-05-22 14:43:23.000000 serializer_Konchik-0.1.3/src/__init__.py
--rw-rw-rw-   0        0        0     2698 2023-05-20 13:25:33.000000 serializer_Konchik-0.1.3/src/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.424650 serializer_Konchik-0.1.3/src/packer/
--rw-rw-rw-   0        0        0       80 2023-05-15 16:52:51.000000 serializer_Konchik-0.1.3/src/packer/__init__.py
--rw-rw-rw-   0        0        0     5256 2023-05-20 20:31:34.000000 serializer_Konchik-0.1.3/src/packer/packer.py
--rw-rw-rw-   0        0        0     5364 2023-05-20 20:11:55.000000 serializer_Konchik-0.1.3/src/packer/unpacker.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.432658 serializer_Konchik-0.1.3/src/serializer/
--rw-rw-rw-   0        0        0      181 2023-05-21 18:46:42.000000 serializer_Konchik-0.1.3/src/serializer/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.3/src/serializer/base_serializer.py
--rw-rw-rw-   0        0        0     3301 2023-05-22 16:06:02.000000 serializer_Konchik-0.1.3/src/serializer/json_serializer.py
--rw-rw-rw-   0        0        0      702 2023-05-22 16:06:59.000000 serializer_Konchik-0.1.3/src/serializer/serializer_factory.py
--rw-rw-rw-   0        0        0     3854 2023-05-22 16:05:46.000000 serializer_Konchik-0.1.3/src/serializer/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:06:16.016859 serializer_Konchik-0.1.4/
+-rw-rw-rw-   0        0        0      262 2023-05-22 17:06:16.016859 serializer_Konchik-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 17:06:15.990535 serializer_Konchik-0.1.4/serializer_Konchik/
+-rw-rw-rw-   0        0        0      176 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/__init__.py
+-rw-rw-rw-   0        0        0     2698 2023-05-20 13:25:33.000000 serializer_Konchik-0.1.4/serializer_Konchik/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:06:16.009779 serializer_Konchik-0.1.4/serializer_Konchik/packer/
+-rw-rw-rw-   0        0        0      110 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/packer/__init__.py
+-rw-rw-rw-   0        0        0     5256 2023-05-20 20:31:34.000000 serializer_Konchik-0.1.4/serializer_Konchik/packer/packer.py
+-rw-rw-rw-   0        0        0     5364 2023-05-20 20:11:55.000000 serializer_Konchik-0.1.4/serializer_Konchik/packer/unpacker.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:06:16.015863 serializer_Konchik-0.1.4/serializer_Konchik/serializer/
+-rw-rw-rw-   0        0        0      226 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/base_serializer.py
+-rw-rw-rw-   0        0        0     3331 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/json_serializer.py
+-rw-rw-rw-   0        0        0      732 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/serializer_factory.py
+-rw-rw-rw-   0        0        0     3884 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:06:16.004712 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 17:06:16.016859 serializer_Konchik-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-05-22 17:05:22.000000 serializer_Konchik-0.1.4/setup.py
```

### Comparing `serializer_Konchik-0.1.3/setup.py` & `serializer_Konchik-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="serializer_Konchik",
-    version="0.1.3",
+    version="0.1.4",
     description="JSON / XML serializer",
     author="Denis Konchik",
     author_email="denis.pptx@gmail.com",
     license="MIT",
     classifiers=[
         "Programming Language :: Python",
         "Operating System :: OS Independent"
     ],
-    packages=["src", "src.packer", "src.serializer"],
-    package_dir={"serializer": "src",
-                 "serializer.packer": "src.packer",
-                 "serializer.serializer": "src.serializer"},
+    packages=["serializer_Konchik", "serializer_Konchik.packer", "serializer_Konchik.serializer"],
     include_package_data=True,
     install_requires=["regex"]
 )
```

### Comparing `serializer_Konchik-0.1.3/src/constants.py` & `serializer_Konchik-0.1.4/serializer_Konchik/constants.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.3/src/packer/packer.py` & `serializer_Konchik-0.1.4/serializer_Konchik/packer/packer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.3/src/packer/unpacker.py` & `serializer_Konchik-0.1.4/serializer_Konchik/packer/unpacker.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.3/src/serializer/base_serializer.py` & `serializer_Konchik-0.1.4/serializer_Konchik/serializer/base_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.3/src/serializer/json_serializer.py` & `serializer_Konchik-0.1.4/serializer_Konchik/serializer/json_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
-from src.serializer.base_serializer import BaseSerializer
-from src.packer import Packer, Unpacker
+from serializer_Konchik.serializer.base_serializer import BaseSerializer
+from serializer_Konchik.packer import Packer, Unpacker
 from ..constants import (PRIMITIVES,
                          JsonRegularExpression as Expression)
 import regex
 
 
 class JsonSerializer(BaseSerializer):
```

### Comparing `serializer_Konchik-0.1.3/src/serializer/serializer_factory.py` & `serializer_Konchik-0.1.4/serializer_Konchik/serializer/serializer_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.serializer.json_serializer import JsonSerializer
-from src.serializer.xml_serializer import XmlSerializer
+from serializer_Konchik.serializer.json_serializer import JsonSerializer
+from serializer_Konchik.serializer.xml_serializer import XmlSerializer
 from ..constants import JSON, XML
 
 
 class SerializerFactory:
 
     @staticmethod
     def create(name: str) -> JsonSerializer | XmlSerializer:
```

### Comparing `serializer_Konchik-0.1.3/src/serializer/xml_serializer.py` & `serializer_Konchik-0.1.4/serializer_Konchik/serializer/xml_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import regex
 import builtins
 from typing import Any
-from src.packer import Packer, Unpacker
-from src.serializer.base_serializer import BaseSerializer
+from serializer_Konchik.packer import Packer, Unpacker
+from serializer_Konchik.serializer.base_serializer import BaseSerializer
 from types import NoneType
 from ..constants import (PRIMITIVES, KEY, VALUE,
                          XmlRegularExpression as Expression)
 
 
 class XmlSerializer(BaseSerializer):
```

