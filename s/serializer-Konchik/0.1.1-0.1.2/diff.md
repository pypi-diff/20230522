# Comparing `tmp/serializer_Konchik-0.1.1.tar.gz` & `tmp/serializer_Konchik-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_Konchik-0.1.1.tar", last modified: Mon May 22 16:44:38 2023, max compression
+gzip compressed data, was "serializer_Konchik-0.1.2.tar", last modified: Mon May 22 16:54:53 2023, max compression
```

## Comparing `serializer_Konchik-0.1.1.tar` & `serializer_Konchik-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:44:38.814371 serializer_Konchik-0.1.1/
--rw-rw-rw-   0        0        0      262 2023-05-22 16:44:38.814371 serializer_Konchik-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 16:44:38.798775 serializer_Konchik-0.1.1/serializer_Konchik.egg-info/
--rw-rw-rw-   0        0        0      262 2023-05-22 16:44:38.000000 serializer_Konchik-0.1.1/serializer_Konchik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-22 16:44:38.000000 serializer_Konchik-0.1.1/serializer_Konchik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:44:38.000000 serializer_Konchik-0.1.1/serializer_Konchik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 16:44:38.000000 serializer_Konchik-0.1.1/serializer_Konchik.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-22 16:44:38.000000 serializer_Konchik-0.1.1/serializer_Konchik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:44:38.814371 serializer_Konchik-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      518 2023-05-22 16:44:24.000000 serializer_Konchik-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:44:38.814371 serializer_Konchik-0.1.1/src/
--rw-rw-rw-   0        0        0      131 2023-05-22 14:43:23.000000 serializer_Konchik-0.1.1/src/__init__.py
--rw-rw-rw-   0        0        0     2698 2023-05-20 13:25:33.000000 serializer_Konchik-0.1.1/src/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.741932 serializer_Konchik-0.1.2/
+-rw-rw-rw-   0        0        0      262 2023-05-22 16:54:53.741932 serializer_Konchik-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.695158 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:54:53.741932 serializer_Konchik-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      550 2023-05-22 16:54:33.000000 serializer_Konchik-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.695158 serializer_Konchik-0.1.2/src/
+-rw-rw-rw-   0        0        0      131 2023-05-22 14:43:23.000000 serializer_Konchik-0.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0     2698 2023-05-20 13:25:33.000000 serializer_Konchik-0.1.2/src/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.726317 serializer_Konchik-0.1.2/src/packer/
+-rw-rw-rw-   0        0        0       80 2023-05-15 16:52:51.000000 serializer_Konchik-0.1.2/src/packer/__init__.py
+-rw-rw-rw-   0        0        0     5256 2023-05-20 20:31:34.000000 serializer_Konchik-0.1.2/src/packer/packer.py
+-rw-rw-rw-   0        0        0     5364 2023-05-20 20:11:55.000000 serializer_Konchik-0.1.2/src/packer/unpacker.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.741932 serializer_Konchik-0.1.2/src/serializer/
+-rw-rw-rw-   0        0        0      181 2023-05-21 18:46:42.000000 serializer_Konchik-0.1.2/src/serializer/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.2/src/serializer/base_serializer.py
+-rw-rw-rw-   0        0        0     3301 2023-05-22 16:06:02.000000 serializer_Konchik-0.1.2/src/serializer/json_serializer.py
+-rw-rw-rw-   0        0        0      702 2023-05-22 16:06:59.000000 serializer_Konchik-0.1.2/src/serializer/serializer_factory.py
+-rw-rw-rw-   0        0        0     3854 2023-05-22 16:05:46.000000 serializer_Konchik-0.1.2/src/serializer/xml_serializer.py
```

### Comparing `serializer_Konchik-0.1.1/setup.py` & `serializer_Konchik-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="serializer_Konchik",
-    version="0.1.1",
+    version="0.1.2",
     description="JSON / XML serializer",
     author="Denis Konchik",
     author_email="denis.pptx@gmail.com",
     license="MIT",
     classifiers=[
         "Programming Language :: Python",
         "Operating System :: OS Independent"
     ],
-    packages=["src"],
+    packages=["src", "src.packer", "src.serializer"],
     include_package_data=True,
     install_requires=["regex"]
 )
```

### Comparing `serializer_Konchik-0.1.1/src/constants.py` & `serializer_Konchik-0.1.2/src/constants.py`

 * *Files identical despite different names*

