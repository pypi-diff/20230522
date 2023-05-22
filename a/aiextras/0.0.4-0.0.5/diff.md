# Comparing `tmp/aiextras-0.0.4.tar.gz` & `tmp/aiextras-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aiextras-0.0.4.tar", last modified: Mon May 22 04:12:09 2023, max compression
+gzip compressed data, was "dist\aiextras-0.0.5.tar", last modified: Mon May 22 04:13:30 2023, max compression
```

## Comparing `aiextras-0.0.4.tar` & `aiextras-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 04:12:09.000000 aiextras-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      338 2023-05-22 04:12:09.000000 aiextras-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 04:12:09.000000 aiextras-0.0.4/programs/
-drwxrwxrwx   0        0        0        0 2023-05-22 04:12:09.000000 aiextras-0.0.4/programs/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 04:12:09.000000 aiextras-0.0.4/programs/src/aiextras.egg-info/
--rw-rw-rw-   0        0        0      338 2023-05-22 04:12:09.000000 aiextras-0.0.4/programs/src/aiextras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-22 04:12:09.000000 aiextras-0.0.4/programs/src/aiextras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 04:12:09.000000 aiextras-0.0.4/programs/src/aiextras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 04:12:09.000000 aiextras-0.0.4/programs/src/aiextras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-22 04:12:09.000000 aiextras-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-05-22 04:12:00.000000 aiextras-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:13:30.000000 aiextras-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      338 2023-05-22 04:13:30.000000 aiextras-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 04:13:30.000000 aiextras-0.0.5/programs/
+drwxrwxrwx   0        0        0        0 2023-05-22 04:13:30.000000 aiextras-0.0.5/programs/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 04:13:30.000000 aiextras-0.0.5/programs/src/aiextras.egg-info/
+-rw-rw-rw-   0        0        0      338 2023-05-22 04:13:30.000000 aiextras-0.0.5/programs/src/aiextras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-22 04:13:30.000000 aiextras-0.0.5/programs/src/aiextras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 04:13:30.000000 aiextras-0.0.5/programs/src/aiextras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 04:13:30.000000 aiextras-0.0.5/programs/src/aiextras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-22 04:13:30.000000 aiextras-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2023-05-22 04:13:11.000000 aiextras-0.0.5/setup.py
```

### Comparing `aiextras-0.0.4/setup.py` & `aiextras-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiextras",                     # This is the name of the package
-    version="0.0.4",                        # The initial release version
+    version="0.0.5",                        # The initial release version
     author="AnupamKris",                     # Full name of the author
     description="AI2LAB Programs",
     # Long description read from the the readme file
     long_description=long_description,
     long_description_content_type="text/markdown",
     # List of all python modules to be installed
     packages=setuptools.find_packages(),
```

