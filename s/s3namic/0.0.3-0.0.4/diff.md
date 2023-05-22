# Comparing `tmp/s3namic-0.0.3.tar.gz` & `tmp/s3namic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3namic-0.0.3.tar", last modified: Mon May 22 05:54:50 2023, max compression
+gzip compressed data, was "s3namic-0.0.4.tar", last modified: Mon May 22 06:02:21 2023, max compression
```

## Comparing `s3namic-0.0.3.tar` & `s3namic-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 05:54:50.563327 s3namic-0.0.3/
--rw-rw-rw-   0        0        0     1086 2023-05-22 05:25:18.000000 s3namic-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    10829 2023-05-22 05:54:50.562322 s3namic-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    10541 2023-05-22 05:13:42.000000 s3namic-0.0.3/README.md
--rw-rw-rw-   0        0        0     1392 2023-05-22 05:53:56.000000 s3namic-0.0.3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:54:50.559646 s3namic-0.0.3/s3namic.egg-info/
--rw-rw-rw-   0        0        0    10829 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 05:54:50.000000 s3namic-0.0.3/s3namic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 05:54:50.563327 s3namic-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 06:02:21.803730 s3namic-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-22 05:25:18.000000 s3namic-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    10865 2023-05-22 06:02:21.802726 s3namic-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10541 2023-05-22 05:13:42.000000 s3namic-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1438 2023-05-22 06:01:49.000000 s3namic-0.0.4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:02:21.789866 s3namic-0.0.4/core/
+-rw-rw-rw-   0        0        0    28605 2023-05-22 05:20:59.000000 s3namic-0.0.4/core/s3namic.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:02:21.799726 s3namic-0.0.4/s3namic.egg-info/
+-rw-rw-rw-   0        0        0    10865 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-22 06:02:21.000000 s3namic-0.0.4/s3namic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:02:21.804727 s3namic-0.0.4/setup.cfg
```

### Comparing `s3namic-0.0.3/LICENSE` & `s3namic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `s3namic-0.0.3/PKG-INFO` & `s3namic-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: s3namic
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for managing AWS S3 bucket
 Home-page: https://github.com/hyoj0942/s3namic
 Author: Joey Kim
 Author-email: hyoj0942@gmail.com
 License: MIT
+Keywords: aws,s3,bucket,management
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Installation
 
 `pip install s3namic`
```

### Comparing `s3namic-0.0.3/README.md` & `s3namic-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `s3namic-0.0.3/__init__.py` & `s3namic-0.0.4/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,16 +45,17 @@
 setup(
     name='s3namic',
     version=__version__,
     description='A Python package for managing AWS S3 bucket',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
-    packages=find_packages(),
+    packages=['core'],
     author='Joey Kim',
     author_email='hyoj0942@gmail.com',
     url='https://github.com/hyoj0942/s3namic',
     install_requires=_hard_dependencies,
+    keywords=['aws', 's3', 'bucket', 'management'],
 )
 
 del _hard_dependencies, _dependency, _missing_dependencies
```

### Comparing `s3namic-0.0.3/s3namic.egg-info/PKG-INFO` & `s3namic-0.0.4/s3namic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: s3namic
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for managing AWS S3 bucket
 Home-page: https://github.com/hyoj0942/s3namic
 Author: Joey Kim
 Author-email: hyoj0942@gmail.com
 License: MIT
+Keywords: aws,s3,bucket,management
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Installation
 
 `pip install s3namic`
```

