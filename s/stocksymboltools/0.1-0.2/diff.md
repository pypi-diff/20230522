# Comparing `tmp/stocksymboltools-0.1.tar.gz` & `tmp/stocksymboltools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocksymboltools-0.1.tar", last modified: Mon May 22 10:04:25 2023, max compression
+gzip compressed data, was "stocksymboltools-0.2.tar", last modified: Mon May 22 10:09:21 2023, max compression
```

## Comparing `stocksymboltools-0.1.tar` & `stocksymboltools-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:04:25.196838 stocksymboltools-0.1/
--rw-rw-rw-   0        0        0     1101 2023-05-22 09:54:03.000000 stocksymboltools-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      719 2023-05-22 10:04:25.195838 stocksymboltools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-05-22 09:55:32.000000 stocksymboltools-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 10:04:25.196838 stocksymboltools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-05-22 10:04:04.000000 stocksymboltools-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:04:25.156837 stocksymboltools-0.1/stocks/
--rw-rw-rw-   0        0        0        0 2023-05-22 09:46:48.000000 stocksymboltools-0.1/stocks/__init__.py
--rw-rw-rw-   0        0        0      323 2023-05-22 09:48:06.000000 stocksymboltools-0.1/stocks/mymodule.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:04:25.193843 stocksymboltools-0.1/stocksymboltools.egg-info/
--rw-rw-rw-   0        0        0      719 2023-05-22 10:04:25.000000 stocksymboltools-0.1/stocksymboltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-22 10:04:25.000000 stocksymboltools-0.1/stocksymboltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:04:25.000000 stocksymboltools-0.1/stocksymboltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 10:04:25.000000 stocksymboltools-0.1/stocksymboltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 10:04:25.000000 stocksymboltools-0.1/stocksymboltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 10:09:21.443560 stocksymboltools-0.2/
+-rw-rw-rw-   0        0        0     1101 2023-05-22 09:54:03.000000 stocksymboltools-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      748 2023-05-22 10:09:21.442561 stocksymboltools-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-22 10:06:44.000000 stocksymboltools-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:09:21.444566 stocksymboltools-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-05-22 10:08:50.000000 stocksymboltools-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:09:21.425562 stocksymboltools-0.2/stocks/
+-rw-rw-rw-   0        0        0        0 2023-05-22 09:46:48.000000 stocksymboltools-0.2/stocks/__init__.py
+-rw-rw-rw-   0        0        0      323 2023-05-22 09:48:06.000000 stocksymboltools-0.2/stocks/mymodule.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:09:21.441561 stocksymboltools-0.2/stocksymboltools.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-05-22 10:09:21.000000 stocksymboltools-0.2/stocksymboltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-22 10:09:21.000000 stocksymboltools-0.2/stocksymboltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:09:21.000000 stocksymboltools-0.2/stocksymboltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 10:09:21.000000 stocksymboltools-0.2/stocksymboltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 10:09:21.000000 stocksymboltools-0.2/stocksymboltools.egg-info/top_level.txt
```

### Comparing `stocksymboltools-0.1/LICENSE.txt` & `stocksymboltools-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stocksymboltools-0.1/PKG-INFO` & `stocksymboltools-0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stocksymboltools
-Version: 0.1
+Version: 0.2
 Summary: A library to get stock symbols
 Home-page: https://github.com/pavan-krishna123/stocks
 Author: Pavan krishna
 Author-email: narne.pavankrishna1@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# myLibrary
+# stocksymboltools
 
-myLibrary is a Python library for retrieving stock symbols from CSV files.
+stocksymboltools is a Python library for retrieving stock symbols from CSV files.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install myLibrary.
 
 ```bash
-pip install stocks
+pip install stocksymboltools==0.1
```

### Comparing `stocksymboltools-0.1/setup.py` & `stocksymboltools-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="stocksymboltools",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     description="A library to get stock symbols",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Pavan krishna",
     author_email="narne.pavankrishna1@gmail.com",
     url="https://github.com/pavan-krishna123/stocks",
@@ -16,7 +16,9 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=[
         'pandas',
     ],
 )
+
+
```

### Comparing `stocksymboltools-0.1/stocksymboltools.egg-info/PKG-INFO` & `stocksymboltools-0.2/stocksymboltools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stocksymboltools
-Version: 0.1
+Version: 0.2
 Summary: A library to get stock symbols
 Home-page: https://github.com/pavan-krishna123/stocks
 Author: Pavan krishna
 Author-email: narne.pavankrishna1@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# myLibrary
+# stocksymboltools
 
-myLibrary is a Python library for retrieving stock symbols from CSV files.
+stocksymboltools is a Python library for retrieving stock symbols from CSV files.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install myLibrary.
 
 ```bash
-pip install stocks
+pip install stocksymboltools==0.1
```

