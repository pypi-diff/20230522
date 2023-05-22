# Comparing `tmp/HomoglyphsCJK-0.0.4.tar.gz` & `tmp/HomoglyphsCJK-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.0.4.tar", last modified: Mon May 22 03:26:05 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.0.5.tar", last modified: Mon May 22 03:33:46 2023, max compression
```

## Comparing `HomoglyphsCJK-0.0.4.tar` & `HomoglyphsCJK-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:26:05.580017 HomoglyphsCJK-0.0.4/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:26:05.578907 HomoglyphsCJK-0.0.4/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       80 2023-05-13 13:35:00.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:26:05.579734 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 03:26:05.000000 HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 03:26:05.579893 HomoglyphsCJK-0.0.4/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2614 2023-05-22 02:38:12.000000 HomoglyphsCJK-0.0.4/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 03:26:05.580054 HomoglyphsCJK-0.0.4/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      918 2023-05-22 03:25:57.000000 HomoglyphsCJK-0.0.4/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:33:46.548572 HomoglyphsCJK-0.0.5/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:33:46.547425 HomoglyphsCJK-0.0.5/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:33:46.548271 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 03:33:46.548436 HomoglyphsCJK-0.0.5/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2614 2023-05-22 02:38:12.000000 HomoglyphsCJK-0.0.5/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 03:33:46.548613 HomoglyphsCJK-0.0.5/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-22 03:33:01.000000 HomoglyphsCJK-0.0.5/setup.py
```

### Comparing `HomoglyphsCJK-0.0.4/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.0.5/HomoglyphsCJK/hg_functions.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.4/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.0.5/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.4/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.4
+Version: 0.0.5
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HomoglyphsCJK-0.0.4/PKG-INFO` & `HomoglyphsCJK-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.4
+Version: 0.0.5
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HomoglyphsCJK-0.0.4/README.md` & `HomoglyphsCJK-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.4/setup.py` & `HomoglyphsCJK-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from setuptools import find_packages, setup
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
-    version="0.0.4",
+    packages=["HomoglyphsCJK"],
+    version="0.0.5",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

