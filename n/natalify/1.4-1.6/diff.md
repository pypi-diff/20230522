# Comparing `tmp/natalify-1.4.tar.gz` & `tmp/natalify-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natalify-1.4.tar", last modified: Mon May 22 10:45:55 2023, max compression
+gzip compressed data, was "natalify-1.6.tar", last modified: Mon May 22 10:50:18 2023, max compression
```

## Comparing `natalify-1.4.tar` & `natalify-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:45:55.268817 natalify-1.4/
--rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-1.4/LICENSE
--rw-rw-rw-   0        0        0     1881 2023-05-22 10:45:55.268817 natalify-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1379 2023-05-22 10:45:00.000000 natalify-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 10:45:55.253192 natalify-1.4/natalify/
--rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-1.4/natalify/__init__.py
--rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-1.4/natalify/__main__.py
--rw-rw-rw-   0        0        0    63371 2023-05-22 10:12:00.000000 natalify-1.4/natalify/natalify.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:45:55.253192 natalify-1.4/natalify.egg-info/
--rw-rw-rw-   0        0        0     1881 2023-05-22 10:45:55.000000 natalify-1.4/natalify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-22 10:45:55.000000 natalify-1.4/natalify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:45:55.000000 natalify-1.4/natalify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-22 10:45:55.000000 natalify-1.4/natalify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 10:45:55.000000 natalify-1.4/natalify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:45:55.268817 natalify-1.4/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-05-22 10:45:46.000000 natalify-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:50:18.682714 natalify-1.6/
+-rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-1.6/LICENSE
+-rw-rw-rw-   0        0        0     1882 2023-05-22 10:50:18.682714 natalify-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-05-22 10:46:57.000000 natalify-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 10:50:18.667087 natalify-1.6/natalify/
+-rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-1.6/natalify/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-1.6/natalify/__main__.py
+-rw-rw-rw-   0        0        0    63371 2023-05-22 10:12:00.000000 natalify-1.6/natalify/natalify.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:50:18.682714 natalify-1.6/natalify.egg-info/
+-rw-rw-rw-   0        0        0     1882 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 10:50:18.000000 natalify-1.6/natalify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:50:18.682714 natalify-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-05-22 10:47:36.000000 natalify-1.6/setup.py
```

### Comparing `natalify-1.4/LICENSE` & `natalify-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `natalify-1.4/PKG-INFO` & `natalify-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 1.4
+Version: 1.6
 Summary: An automation software made for my friend Natalie
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -38,15 +38,15 @@
 To get started with Natalify, import the library and use the start method:
 
 ```python
 import natalify
 
 natalify.start()
 
-``
+```
 
 License
 Natalify is released under the GNU General Public License v3.0 (GPL-3.0).
 
 Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
```

### Comparing `natalify-1.4/README.md` & `natalify-1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 To get started with Natalify, import the library and use the start method:
 
 ```python
 import natalify
 
 natalify.start()
 
-``
+```
 
 License
 Natalify is released under the GNU General Public License v3.0 (GPL-3.0).
 
 Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
```

### Comparing `natalify-1.4/natalify/natalify.py` & `natalify-1.6/natalify/natalify.py`

 * *Files identical despite different names*

### Comparing `natalify-1.4/natalify.egg-info/PKG-INFO` & `natalify-1.6/natalify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 1.4
+Version: 1.6
 Summary: An automation software made for my friend Natalie
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -38,15 +38,15 @@
 To get started with Natalify, import the library and use the start method:
 
 ```python
 import natalify
 
 natalify.start()
 
-``
+```
 
 License
 Natalify is released under the GNU General Public License v3.0 (GPL-3.0).
 
 Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
```

### Comparing `natalify-1.4/setup.py` & `natalify-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='natalify',
-    version='1.4',
+    version='1.6',
     packages=setuptools.find_packages(),
     license='GPL-3.0',
     author='jack',
     author_email='kinginjack@gmail.com',
     description='An automation software made for my friend Natalie',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

