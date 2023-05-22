# Comparing `tmp/aiextras-0.0.1.tar.gz` & `tmp/aiextras-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aiextras-0.0.1.tar", last modified: Mon May 22 03:54:15 2023, max compression
+gzip compressed data, was "dist\aiextras-0.0.2.tar", last modified: Mon May 22 04:06:31 2023, max compression
```

## Comparing `aiextras-0.0.1.tar` & `aiextras-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 03:54:15.000000 aiextras-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      338 2023-05-22 03:54:15.000000 aiextras-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 03:54:15.000000 aiextras-0.0.1/programs/
-drwxrwxrwx   0        0        0        0 2023-05-22 03:54:15.000000 aiextras-0.0.1/programs/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 03:54:15.000000 aiextras-0.0.1/programs/src/aiextras.egg-info/
--rw-rw-rw-   0        0        0      338 2023-05-22 03:54:15.000000 aiextras-0.0.1/programs/src/aiextras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-22 03:54:15.000000 aiextras-0.0.1/programs/src/aiextras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 03:54:15.000000 aiextras-0.0.1/programs/src/aiextras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 03:54:15.000000 aiextras-0.0.1/programs/src/aiextras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-22 03:54:15.000000 aiextras-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-05-22 03:47:06.000000 aiextras-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:06:31.000000 aiextras-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      338 2023-05-22 04:06:31.000000 aiextras-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 04:06:31.000000 aiextras-0.0.2/programs/
+drwxrwxrwx   0        0        0        0 2023-05-22 04:06:31.000000 aiextras-0.0.2/programs/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 04:06:31.000000 aiextras-0.0.2/programs/src/aiextras.egg-info/
+-rw-rw-rw-   0        0        0      338 2023-05-22 04:06:31.000000 aiextras-0.0.2/programs/src/aiextras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-22 04:06:31.000000 aiextras-0.0.2/programs/src/aiextras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 04:06:31.000000 aiextras-0.0.2/programs/src/aiextras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 04:06:31.000000 aiextras-0.0.2/programs/src/aiextras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-22 04:06:31.000000 aiextras-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2023-05-22 04:06:22.000000 aiextras-0.0.2/setup.py
```

### Comparing `aiextras-0.0.1/setup.py` & `aiextras-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiextras",                     # This is the name of the package
-    version="0.0.1",                        # The initial release version
+    version="0.0.2",                        # The initial release version
     author="AnupamKris",                     # Full name of the author
     description="AI2LAB Programs",
     # Long description read from the the readme file
     long_description=long_description,
     long_description_content_type="text/markdown",
     # List of all python modules to be installed
     packages=setuptools.find_packages(),
```

