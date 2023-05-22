# Comparing `tmp/s3namic-0.0.4.tar.gz` & `tmp/s3namic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3namic-0.0.4.tar", last modified: Mon May 22 06:02:21 2023, max compression
+gzip compressed data, was "s3namic-0.0.5.tar", last modified: Mon May 22 07:14:04 2023, max compression
```

## Comparing `s3namic-0.0.4.tar` & `s3namic-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 06:02:21.803730 s3namic-0.0.4/
--rw-rw-rw-   0        0        0     1086 2023-05-22 05:25:18.000000 s3namic-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    10865 2023-05-22 06:02:21.802726 s3namic-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    10541 2023-05-22 05:13:42.000000 s3namic-0.0.4/README.md
--rw-rw-rw-   0        0        0     1438 2023-05-22 06:01:49.000000 s3namic-0.0.4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:02:21.789866 s3namic-0.0.4/core/
--rw-rw-rw-   0        0        0    28605 2023-05-22 05:20:59.000000 s3namic-0.0.4/core/s3namic.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:02:21.799726 s3namic-0.0.4/s3namic.egg-info/
--rw-rw-rw-   0        0        0    10865 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 06:02:21.804727 s3namic-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 07:14:04.100276 s3namic-0.0.5/
+-rw-rw-rw-   0        0        0     1086 2023-05-22 05:25:18.000000 s3namic-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    10865 2023-05-22 07:14:04.099275 s3namic-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10541 2023-05-22 05:13:42.000000 s3namic-0.0.5/README.md
+-rw-rw-rw-   0        0        0      708 2023-05-22 07:11:06.000000 s3namic-0.0.5/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:14:04.086275 s3namic-0.0.5/s3namic/
+-rw-rw-rw-   0        0        0       25 2023-05-22 06:24:22.000000 s3namic-0.0.5/s3namic/__init__.py
+-rw-rw-rw-   0        0        0    28605 2023-05-22 05:20:59.000000 s3namic-0.0.5/s3namic/core.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:14:04.096274 s3namic-0.0.5/s3namic.egg-info/
+-rw-rw-rw-   0        0        0    10865 2023-05-22 07:14:03.000000 s3namic-0.0.5/s3namic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-05-22 07:14:03.000000 s3namic-0.0.5/s3namic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 07:14:03.000000 s3namic-0.0.5/s3namic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-22 07:14:03.000000 s3namic-0.0.5/s3namic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 07:14:03.000000 s3namic-0.0.5/s3namic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 07:14:04.100276 s3namic-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      871 2023-05-22 07:11:34.000000 s3namic-0.0.5/setup.py
```

### Comparing `s3namic-0.0.4/LICENSE` & `s3namic-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `s3namic-0.0.4/PKG-INFO` & `s3namic-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3namic
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for managing AWS S3 bucket
 Home-page: https://github.com/hyoj0942/s3namic
 Author: Joey Kim
 Author-email: hyoj0942@gmail.com
 License: MIT
 Keywords: aws,s3,bucket,management
 Description-Content-Type: text/markdown
```

### Comparing `s3namic-0.0.4/README.md` & `s3namic-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `s3namic-0.0.4/__init__.py` & `s3namic-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,35 @@
 from setuptools import setup, find_packages
 from _version import get_version
+from api import s3namic
 
-__docformat__ = 'restructuredtext'
-
-_hard_dependencies=[
-    'pandas', 
-    'boto3', 
-    'botocore',
-    'pyarrow',
-]
-
-# _soft_dependencies=[
-#     'pyarrow',
-# ]
-
-_missing_dependencies = []
-for _dependency in _hard_dependencies:
-    try:
-        __import__(_dependency)
-    except ImportError as _e:
-        _missing_dependencies.append(f"{_dependency}: ({_e})")
-        
-if _missing_dependencies:
-    raise ImportError(
-        f"Required packages not installed. Please install the following packages:\n" + "\n".join(_missing_dependencies)
-    )
-    
 v = get_version()
 __version__ = v.get("closest-tag", v["version"])
 
 del get_version, v
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
-
-from api import (
-    s3namic
-)
-
-__all__ = [
-    "s3namic",
+    
+_hard_dependencies=[
+    'pandas', 
+    'boto3', 
+    'botocore',
+    'pyarrow',
 ]
 
 setup(
     name='s3namic',
     version=__version__,
     description='A Python package for managing AWS S3 bucket',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
-    packages=['core'],
+    packages=['s3namic'],
     author='Joey Kim',
     author_email='hyoj0942@gmail.com',
     url='https://github.com/hyoj0942/s3namic',
     install_requires=_hard_dependencies,
     keywords=['aws', 's3', 'bucket', 'management'],
 )
 
-del _hard_dependencies, _dependency, _missing_dependencies
-
+del _hard_dependencies
```

### Comparing `s3namic-0.0.4/core/s3namic.py` & `s3namic-0.0.5/s3namic/core.py`

 * *Files identical despite different names*

### Comparing `s3namic-0.0.4/s3namic.egg-info/PKG-INFO` & `s3namic-0.0.5/s3namic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3namic
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for managing AWS S3 bucket
 Home-page: https://github.com/hyoj0942/s3namic
 Author: Joey Kim
 Author-email: hyoj0942@gmail.com
 License: MIT
 Keywords: aws,s3,bucket,management
 Description-Content-Type: text/markdown
```

