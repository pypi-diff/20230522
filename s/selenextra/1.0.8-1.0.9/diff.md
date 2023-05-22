# Comparing `tmp/selenextra-1.0.8.tar.gz` & `tmp/selenextra-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-1.0.8.tar", last modified: Mon May 22 06:54:59 2023, max compression
+gzip compressed data, was "selenextra-1.0.9.tar", last modified: Mon May 22 06:56:51 2023, max compression
```

## Comparing `selenextra-1.0.8.tar` & `selenextra-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 06:54:59.914064 selenextra-1.0.8/
--rw-rw-rw-   0        0        0    35823 2023-05-22 06:11:20.000000 selenextra-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      539 2023-05-22 06:54:59.913065 selenextra-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-22 06:11:20.000000 selenextra-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 06:54:59.907081 selenextra-1.0.8/selenextra/
--rw-rw-rw-   0        0        0     3967 2023-05-22 06:11:20.000000 selenextra-1.0.8/selenextra/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-22 06:11:20.000000 selenextra-1.0.8/selenextra/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:54:59.912068 selenextra-1.0.8/selenextra.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-22 06:54:59.000000 selenextra-1.0.8/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-22 06:54:59.000000 selenextra-1.0.8/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 06:54:59.000000 selenextra-1.0.8/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-05-22 06:54:59.000000 selenextra-1.0.8/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 06:54:59.000000 selenextra-1.0.8/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 06:54:59.914064 selenextra-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-05-22 06:54:29.000000 selenextra-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:56:51.165518 selenextra-1.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-05-22 06:11:20.000000 selenextra-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      539 2023-05-22 06:56:51.165518 selenextra-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-22 06:11:20.000000 selenextra-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 06:56:51.159536 selenextra-1.0.9/selenextra/
+-rw-rw-rw-   0        0        0     3967 2023-05-22 06:11:20.000000 selenextra-1.0.9/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-22 06:11:20.000000 selenextra-1.0.9/selenextra/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:56:51.164520 selenextra-1.0.9/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-22 06:56:51.000000 selenextra-1.0.9/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-22 06:56:51.000000 selenextra-1.0.9/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      110 2023-05-22 06:56:51.000000 selenextra-1.0.9/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 06:56:51.000000 selenextra-1.0.9/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 06:56:51.000000 selenextra-1.0.9/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:56:51.165518 selenextra-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      848 2023-05-22 06:56:50.000000 selenextra-1.0.9/setup.py
```

### Comparing `selenextra-1.0.8/LICENSE` & `selenextra-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-1.0.8/PKG-INFO` & `selenextra-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenextra
-Version: 1.0.8
+Version: 1.0.9
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `selenextra-1.0.8/selenextra/__init__.py` & `selenextra-1.0.9/selenextra/__init__.py`

 * *Files identical despite different names*

### Comparing `selenextra-1.0.8/selenextra.egg-info/PKG-INFO` & `selenextra-1.0.9/selenextra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenextra
-Version: 1.0.8
+Version: 1.0.9
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `selenextra-1.0.8/setup.py` & `selenextra-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='1.0.8',
+    version='1.0.9',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
-        'undetected_chromedriver @ git+https://github.com/nguyenvantat1182002/undetected-chromedriver@master',
         'selenium-wire'
     ],
+    dependency_links=[
+        'https://github.com/nguyenvantat1182002/undetected-chromedriver/archive/master.zip#egg=undetected_chromedriver'
+    ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
```

