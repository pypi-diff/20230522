# Comparing `tmp/HomoglyphsCJK-0.0.3.tar.gz` & `tmp/HomoglyphsCJK-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.0.3.tar", last modified: Mon May 22 02:35:53 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.0.4.tar", last modified: Mon May 22 03:26:05 2023, max compression
```

## Comparing `HomoglyphsCJK-0.0.3.tar` & `HomoglyphsCJK-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:35:53.825710 HomoglyphsCJK-0.0.3/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:35:53.823758 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      257 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        5 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 02:35:53.825502 HomoglyphsCJK-0.0.3/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2614 2023-05-22 02:35:38.000000 HomoglyphsCJK-0.0.3/README.md
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:35:53.824983 HomoglyphsCJK-0.0.3/homo/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       80 2023-05-13 13:35:00.000000 HomoglyphsCJK-0.0.3/homo/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.3/homo/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.3/homo/test_run.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 02:35:53.825784 HomoglyphsCJK-0.0.3/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      918 2023-05-22 02:35:45.000000 HomoglyphsCJK-0.0.3/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:26:05.580017 HomoglyphsCJK-0.0.4/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:26:05.578907 HomoglyphsCJK-0.0.4/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       80 2023-05-13 13:35:00.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:26:05.579734 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 03:26:05.579893 HomoglyphsCJK-0.0.4/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2614 2023-05-22 02:38:12.000000 HomoglyphsCJK-0.0.4/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 03:26:05.580054 HomoglyphsCJK-0.0.4/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      918 2023-05-22 03:25:57.000000 HomoglyphsCJK-0.0.4/setup.py
```

### Comparing `HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.3
+Version: 0.0.4
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HomoglyphsCJK-0.0.3/PKG-INFO` & `HomoglyphsCJK-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.3
+Version: 0.0.4
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HomoglyphsCJK-0.0.3/README.md` & `HomoglyphsCJK-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.3/homo/hg_functions.py` & `HomoglyphsCJK-0.0.4/HomoglyphsCJK/hg_functions.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.3/homo/test_run.py` & `HomoglyphsCJK-0.0.4/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.3/setup.py` & `HomoglyphsCJK-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
-    version="0.0.3",
+    version="0.0.4",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

