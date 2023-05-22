# Comparing `tmp/aiextras-0.0.6.tar.gz` & `tmp/aiextras-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aiextras-0.0.6.tar", last modified: Mon May 22 04:21:39 2023, max compression
+gzip compressed data, was "dist\aiextras-0.0.7.tar", last modified: Mon May 22 04:23:59 2023, max compression
```

## Comparing `aiextras-0.0.6.tar` & `aiextras-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 04:21:39.000000 aiextras-0.0.6/
--rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      338 2023-05-22 04:21:39.000000 aiextras-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 04:21:39.000000 aiextras-0.0.6/programs/
-drwxrwxrwx   0        0        0        0 2023-05-22 04:21:39.000000 aiextras-0.0.6/programs/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 04:21:39.000000 aiextras-0.0.6/programs/src/aiextras.egg-info/
--rw-rw-rw-   0        0        0      338 2023-05-22 04:21:39.000000 aiextras-0.0.6/programs/src/aiextras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-22 04:21:39.000000 aiextras-0.0.6/programs/src/aiextras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 04:21:39.000000 aiextras-0.0.6/programs/src/aiextras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 04:21:39.000000 aiextras-0.0.6/programs/src/aiextras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-22 04:21:39.000000 aiextras-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-05-22 04:21:14.000000 aiextras-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:23:59.000000 aiextras-0.0.7/
+-rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      338 2023-05-22 04:23:59.000000 aiextras-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 04:23:59.000000 aiextras-0.0.7/programs/
+drwxrwxrwx   0        0        0        0 2023-05-22 04:23:59.000000 aiextras-0.0.7/programs/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 04:23:59.000000 aiextras-0.0.7/programs/src/aiextras.egg-info/
+-rw-rw-rw-   0        0        0      338 2023-05-22 04:23:59.000000 aiextras-0.0.7/programs/src/aiextras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-22 04:23:59.000000 aiextras-0.0.7/programs/src/aiextras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 04:23:59.000000 aiextras-0.0.7/programs/src/aiextras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 04:23:59.000000 aiextras-0.0.7/programs/src/aiextras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-22 04:23:59.000000 aiextras-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2023-05-22 04:23:56.000000 aiextras-0.0.7/setup.py
```

### Comparing `aiextras-0.0.6/setup.py` & `aiextras-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiextras",                     # This is the name of the package
-    version="0.0.6",                        # The initial release version
+    version="0.0.7",                        # The initial release version
     author="AnupamKris",                     # Full name of the author
     description="AI2LAB Programs",
     # Long description read from the the readme file
     long_description=long_description,
     long_description_content_type="text/markdown",
     # List of all python modules to be installed
     packages=setuptools.find_packages(),
```

