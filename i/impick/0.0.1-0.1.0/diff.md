# Comparing `tmp/impick-0.0.1.tar.gz` & `tmp/impick-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impick-0.0.1.tar", last modified: Mon May 22 09:03:58 2023, max compression
+gzip compressed data, was "impick-0.1.0.tar", last modified: Mon May 22 15:48:01 2023, max compression
```

## Comparing `impick-0.0.1.tar` & `impick-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 09:03:58.040635 impick-0.0.1/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1088 2023-05-22 08:32:04.000000 impick-0.0.1/LICENSE
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2023-05-22 08:28:27.000000 impick-0.0.1/MANIFEST.in
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      540 2023-05-22 09:03:58.040635 impick-0.0.1/PKG-INFO
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       10 2023-05-22 08:31:04.000000 impick-0.0.1/README.md
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 09:03:58.040635 impick-0.0.1/impick/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 08:24:44.000000 impick-0.0.1/impick/__init__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 09:03:57.000000 impick-0.0.1/impick/__init__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       22 2023-05-22 09:03:19.000000 impick-0.0.1/impick/__version__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 09:03:57.000000 impick-0.0.1/impick/__version__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      225 2023-05-22 08:24:44.000000 impick-0.0.1/impick/py.typed
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      905 2023-05-22 08:41:57.000000 impick-0.0.1/impick/server.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       86 2023-05-22 09:03:57.000000 impick-0.0.1/impick/server.pyi
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 09:03:58.040635 impick-0.0.1/impick.egg-info/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      540 2023-05-22 09:03:57.000000 impick-0.0.1/impick.egg-info/PKG-INFO
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      401 2023-05-22 09:03:58.000000 impick-0.0.1/impick.egg-info/SOURCES.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-22 09:03:57.000000 impick-0.0.1/impick.egg-info/dependency_links.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       61 2023-05-22 09:03:57.000000 impick-0.0.1/impick.egg-info/entry_points.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-22 08:33:58.000000 impick-0.0.1/impick.egg-info/not-zip-safe
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       35 2023-05-22 09:03:57.000000 impick-0.0.1/impick.egg-info/requires.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        7 2023-05-22 09:03:57.000000 impick-0.0.1/impick.egg-info/top_level.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       35 2023-05-22 08:40:30.000000 impick-0.0.1/requirements.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       38 2023-05-22 09:03:58.040635 impick-0.0.1/setup.cfg
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1445 2023-05-22 08:35:44.000000 impick-0.0.1/setup.py
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:01.373058 impick-0.1.0/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1088 2023-05-22 08:32:04.000000 impick-0.1.0/LICENSE
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2023-05-22 08:28:27.000000 impick-0.1.0/MANIFEST.in
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2927 2023-05-22 15:48:01.373058 impick-0.1.0/PKG-INFO
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2399 2023-05-22 15:47:05.000000 impick-0.1.0/README.md
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:01.373058 impick-0.1.0/impick/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 08:24:44.000000 impick-0.1.0/impick/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:00.000000 impick-0.1.0/impick/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       22 2023-05-22 15:47:29.000000 impick-0.1.0/impick/__version__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:00.000000 impick-0.1.0/impick/__version__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      225 2023-05-22 08:24:44.000000 impick-0.1.0/impick/py.typed
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     5386 2023-05-22 15:21:34.000000 impick-0.1.0/impick/server.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      639 2023-05-22 15:48:00.000000 impick-0.1.0/impick/server.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:01.373058 impick-0.1.0/impick.egg-info/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2927 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/PKG-INFO
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      401 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/SOURCES.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/dependency_links.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       61 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/entry_points.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-22 08:33:58.000000 impick-0.1.0/impick.egg-info/not-zip-safe
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       66 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/requires.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        7 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/top_level.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       66 2023-05-22 14:43:47.000000 impick-0.1.0/requirements.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       38 2023-05-22 15:48:01.373058 impick-0.1.0/setup.cfg
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1443 2023-05-22 15:25:51.000000 impick-0.1.0/setup.py
```

### Comparing `impick-0.0.1/LICENSE` & `impick-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `impick-0.0.1/setup.py` & `impick-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NAME = "impick"
 DESCRIPTION = "ImPick - view and select a single image from a group using the web-GUI"
 LICENSE = "MIT"
 AUTHOR = "Vladislav A. Proskurov"
 AUTHOR_EMAIL = "rilshok@pm.me"
 URL = "https://github.com/rilshok/impick"
 CLASSIFIERS = [
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.7",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 1 - Planning",
 ]
 
 VERSION_PATH = str(Path(__file__).resolve().parent / NAME / "__version__.py")
 VERSION = runpy.run_path(VERSION_PATH)["__version__"]
@@ -38,14 +38,14 @@
     version=VERSION,
     url=URL,
     packages=find_packages(include=(NAME,)),
     include_package_data=True,
     zip_safe=False,
     install_requires=REQUIREMENTS,
     classifiers=CLASSIFIERS,
-    python_requires=">=3.11",
+    python_requires=">=3.7",
     entry_points={
         "console_scripts": [
             "impick_server=impick.server:start_server",
         ]
     },
 )
```

