# Comparing `tmp/nmping-0.1.tar.gz` & `tmp/nmping-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmping-0.1.tar", last modified: Mon May 22 08:33:33 2023, max compression
+gzip compressed data, was "nmping-0.2.tar", last modified: Mon May 22 08:45:03 2023, max compression
```

## Comparing `nmping-0.1.tar` & `nmping-0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 08:33:33.382625 nmping-0.1/
--rw-rw-rw-   0        0        0      518 2023-05-22 08:33:33.381626 nmping-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-22 08:27:39.000000 nmping-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 08:33:33.380626 nmping-0.1/nmping.egg-info/
--rw-rw-rw-   0        0        0      518 2023-05-22 08:33:33.000000 nmping-0.1/nmping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-22 08:33:33.000000 nmping-0.1/nmping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 08:33:33.000000 nmping-0.1/nmping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 08:33:33.000000 nmping-0.1/nmping.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 08:33:33.000000 nmping-0.1/nmping.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 08:33:33.382625 nmping-0.1/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-05-22 08:26:35.000000 nmping-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:45:03.251327 nmping-0.2/
+-rw-rw-rw-   0        0        0      518 2023-05-22 08:45:03.250345 nmping-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-22 08:27:39.000000 nmping-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 08:45:03.249063 nmping-0.2/nmping.egg-info/
+-rw-rw-rw-   0        0        0      518 2023-05-22 08:45:03.000000 nmping-0.2/nmping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-05-22 08:45:03.000000 nmping-0.2/nmping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:45:03.000000 nmping-0.2/nmping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:45:03.000000 nmping-0.2/nmping.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 08:45:03.251327 nmping-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-05-22 08:42:41.000000 nmping-0.2/setup.py
```

### Comparing `nmping-0.1/PKG-INFO` & `nmping-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmping
-Version: 0.1
+Version: 0.2
 Summary: This is an Example Package
 Home-page: https://github.com/PierreGode/Nmping
 Author: Pierre Gode
 Author-email: pierre@gode.one
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nmping-0.1/nmping.egg-info/PKG-INFO` & `nmping-0.2/nmping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmping
-Version: 0.1
+Version: 0.2
 Summary: This is an Example Package
 Home-page: https://github.com/PierreGode/Nmping
 Author: Pierre Gode
 Author-email: pierre@gode.one
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nmping-0.1/setup.py` & `nmping-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="nmping",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
-        'tkinter',
+        # 'tkinter',
         # e.g., 'numpy >= 1.13.3'
     ],
     author="Pierre Gode",
     author_email="pierre@gode.one",
     description="This is an Example Package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

