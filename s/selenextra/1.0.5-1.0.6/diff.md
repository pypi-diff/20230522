# Comparing `tmp/selenextra-1.0.5.tar.gz` & `tmp/selenextra-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-1.0.5.tar", last modified: Mon May 22 06:05:06 2023, max compression
+gzip compressed data, was "selenextra-1.0.6.tar", last modified: Mon May 22 06:12:45 2023, max compression
```

## Comparing `selenextra-1.0.5.tar` & `selenextra-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 06:05:06.458127 selenextra-1.0.5/
--rw-rw-rw-   0        0        0    35823 2023-05-22 04:32:59.000000 selenextra-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      539 2023-05-22 06:05:06.458127 selenextra-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-22 04:32:59.000000 selenextra-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 06:05:06.453140 selenextra-1.0.5/selenextra/
--rw-rw-rw-   0        0        0     3967 2023-05-22 05:56:55.000000 selenextra-1.0.5/selenextra/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-22 05:56:18.000000 selenextra-1.0.5/selenextra/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:05:06.457130 selenextra-1.0.5/selenextra.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       74 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 06:05:06.458127 selenextra-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-05-22 06:04:51.000000 selenextra-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:12:45.741560 selenextra-1.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-05-22 06:11:20.000000 selenextra-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      539 2023-05-22 06:12:45.740563 selenextra-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-22 06:11:20.000000 selenextra-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 06:12:45.732584 selenextra-1.0.6/selenextra/
+-rw-rw-rw-   0        0        0     3967 2023-05-22 06:11:20.000000 selenextra-1.0.6/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-22 06:11:20.000000 selenextra-1.0.6/selenextra/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:12:45.739565 selenextra-1.0.6/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-22 06:12:45.000000 selenextra-1.0.6/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-22 06:12:45.000000 selenextra-1.0.6/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      102 2023-05-22 06:12:45.000000 selenextra-1.0.6/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 06:12:45.000000 selenextra-1.0.6/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 06:12:45.000000 selenextra-1.0.6/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:12:45.742557 selenextra-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      840 2023-05-22 06:11:56.000000 selenextra-1.0.6/setup.py
```

### Comparing `selenextra-1.0.5/LICENSE` & `selenextra-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-1.0.5/PKG-INFO` & `selenextra-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenextra
-Version: 1.0.5
+Version: 1.0.6
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `selenextra-1.0.5/selenextra/__init__.py` & `selenextra-1.0.6/selenextra/__init__.py`

 * *Files identical despite different names*

### Comparing `selenextra-1.0.5/selenextra.egg-info/PKG-INFO` & `selenextra-1.0.6/selenextra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenextra
-Version: 1.0.5
+Version: 1.0.6
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `selenextra-1.0.5/setup.py` & `selenextra-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='1.0.5',
+    version='1.0.6',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
         'selenium-wire'
     ],
     dependency_links=[
-        'git+https://github.com/nguyenvantat1182002/undetected-chromedriver@master'
+        'git+https://github.com/nguyenvantat1182002/undetected-chromedriver@master#egg=undetected-chromedriver'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

