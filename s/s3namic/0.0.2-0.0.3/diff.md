# Comparing `tmp/s3namic-0.0.2.tar.gz` & `tmp/s3namic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3namic-0.0.2.tar", last modified: Mon May 22 05:23:38 2023, max compression
+gzip compressed data, was "s3namic-0.0.3.tar", last modified: Mon May 22 05:54:50 2023, max compression
```

## Comparing `s3namic-0.0.2.tar` & `s3namic-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 05:23:38.922896 s3namic-0.0.2/
--rw-rw-rw-   0        0        0    10806 2023-05-22 05:23:38.921892 s3namic-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10541 2023-05-22 05:13:42.000000 s3namic-0.0.2/README.md
--rw-rw-rw-   0        0        0     1346 2023-05-22 05:23:35.000000 s3namic-0.0.2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:23:38.908267 s3namic-0.0.2/core/
--rw-rw-rw-   0        0        0    28605 2023-05-22 05:20:59.000000 s3namic-0.0.2/core/s3namic.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:23:38.919890 s3namic-0.0.2/s3namic.egg-info/
--rw-rw-rw-   0        0        0    10806 2023-05-22 05:23:38.000000 s3namic-0.0.2/s3namic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-22 05:23:38.000000 s3namic-0.0.2/s3namic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 05:23:38.000000 s3namic-0.0.2/s3namic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-22 05:23:38.000000 s3namic-0.0.2/s3namic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-22 05:23:38.000000 s3namic-0.0.2/s3namic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 05:23:38.922896 s3namic-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 05:54:50.563327 s3namic-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-05-22 05:25:18.000000 s3namic-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    10829 2023-05-22 05:54:50.562322 s3namic-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10541 2023-05-22 05:13:42.000000 s3namic-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1392 2023-05-22 05:53:56.000000 s3namic-0.0.3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:54:50.559646 s3namic-0.0.3/s3namic.egg-info/
+-rw-rw-rw-   0        0        0    10829 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 05:54:50.563327 s3namic-0.0.3/setup.cfg
```

### Comparing `s3namic-0.0.2/PKG-INFO` & `s3namic-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: s3namic
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for managing AWS S3 bucket
 Home-page: https://github.com/hyoj0942/s3namic
 Author: Joey Kim
 Author-email: hyoj0942@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## Installation
 
 `pip install s3namic`
 
 ---
```

### Comparing `s3namic-0.0.2/README.md` & `s3namic-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `s3namic-0.0.2/__init__.py` & `s3namic-0.0.3/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 from _version import get_version
 
 __docformat__ = 'restructuredtext'
 
 _hard_dependencies=[
     'pandas', 
     'boto3', 
@@ -30,30 +30,31 @@
 __version__ = v.get("closest-tag", v["version"])
 
 del get_version, v
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
+from api import (
+    s3namic
+)
+
+__all__ = [
+    "s3namic",
+]
+
 setup(
     name='s3namic',
     version=__version__,
     description='A Python package for managing AWS S3 bucket',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
+    packages=find_packages(),
     author='Joey Kim',
     author_email='hyoj0942@gmail.com',
     url='https://github.com/hyoj0942/s3namic',
     install_requires=_hard_dependencies,
 )
 
 del _hard_dependencies, _dependency, _missing_dependencies
 
-from api import (
-    s3namic
-)
-
-__all__ = [
-    "s3namic",
-]
-
```

### Comparing `s3namic-0.0.2/s3namic.egg-info/PKG-INFO` & `s3namic-0.0.3/s3namic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: s3namic
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for managing AWS S3 bucket
 Home-page: https://github.com/hyoj0942/s3namic
 Author: Joey Kim
 Author-email: hyoj0942@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## Installation
 
 `pip install s3namic`
 
 ---
```

