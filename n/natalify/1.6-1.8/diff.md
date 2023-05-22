# Comparing `tmp/natalify-1.6.tar.gz` & `tmp/natalify-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natalify-1.6.tar", last modified: Mon May 22 10:50:18 2023, max compression
+gzip compressed data, was "natalify-1.8.tar", last modified: Mon May 22 10:57:21 2023, max compression
```

## Comparing `natalify-1.6.tar` & `natalify-1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:50:18.682714 natalify-1.6/
--rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-1.6/LICENSE
--rw-rw-rw-   0        0        0     1882 2023-05-22 10:50:18.682714 natalify-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2023-05-22 10:46:57.000000 natalify-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 10:50:18.667087 natalify-1.6/natalify/
--rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-1.6/natalify/__init__.py
--rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-1.6/natalify/__main__.py
--rw-rw-rw-   0        0        0    63371 2023-05-22 10:12:00.000000 natalify-1.6/natalify/natalify.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:50:18.682714 natalify-1.6/natalify.egg-info/
--rw-rw-rw-   0        0        0     1882 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:50:18.682714 natalify-1.6/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-05-22 10:47:36.000000 natalify-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:57:21.252908 natalify-1.8/
+-rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-1.8/LICENSE
+-rw-rw-rw-   0        0        0     1879 2023-05-22 10:57:21.252908 natalify-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-05-22 10:46:57.000000 natalify-1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 10:57:21.237281 natalify-1.8/natalify/
+-rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-1.8/natalify/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-1.8/natalify/__main__.py
+-rw-rw-rw-   0        0        0    63371 2023-05-22 10:12:00.000000 natalify-1.8/natalify/natalify.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:57:21.252908 natalify-1.8/natalify.egg-info/
+-rw-rw-rw-   0        0        0     1879 2023-05-22 10:57:21.000000 natalify-1.8/natalify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-22 10:57:21.000000 natalify-1.8/natalify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:57:21.000000 natalify-1.8/natalify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-22 10:57:21.000000 natalify-1.8/natalify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 10:57:21.000000 natalify-1.8/natalify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:57:21.252908 natalify-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-22 10:57:13.000000 natalify-1.8/setup.py
```

### Comparing `natalify-1.6/LICENSE` & `natalify-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `natalify-1.6/PKG-INFO` & `natalify-1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 1.6
-Summary: An automation software made for my friend Natalie
+Version: 1.8
+Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `natalify-1.6/README.md` & `natalify-1.8/README.md`

 * *Files identical despite different names*

### Comparing `natalify-1.6/natalify/natalify.py` & `natalify-1.8/natalify/natalify.py`

 * *Files identical despite different names*

### Comparing `natalify-1.6/natalify.egg-info/PKG-INFO` & `natalify-1.8/natalify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 1.6
-Summary: An automation software made for my friend Natalie
+Version: 1.8
+Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `natalify-1.6/setup.py` & `natalify-1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='natalify',
-    version='1.6',
+    version='1.8',
     packages=setuptools.find_packages(),
     license='GPL-3.0',
     author='jack',
     author_email='kinginjack@gmail.com',
-    description='An automation software made for my friend Natalie',
+    description='A simple automation software for various tasks',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['selenium', 'colorama', 'datetime', 'cryptography', 'webdriver-manager', 'termcolor', 'tinydb'],
     python_requires='>=3.8',
+
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
+
 )
```

