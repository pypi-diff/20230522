# Comparing `tmp/HomoglyphsCJK-0.0.2.tar.gz` & `tmp/HomoglyphsCJK-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.0.2.tar", last modified: Mon May 22 02:32:54 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.0.3.tar", last modified: Mon May 22 02:35:53 2023, max compression
```

## Comparing `HomoglyphsCJK-0.0.2.tar` & `HomoglyphsCJK-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:32:54.660719 HomoglyphsCJK-0.0.2/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:32:54.658931 HomoglyphsCJK-0.0.2/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3190 2023-05-22 02:32:54.000000 HomoglyphsCJK-0.0.2/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      257 2023-05-22 02:32:54.000000 HomoglyphsCJK-0.0.2/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 02:32:54.000000 HomoglyphsCJK-0.0.2/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 02:32:54.000000 HomoglyphsCJK-0.0.2/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        5 2023-05-22 02:32:54.000000 HomoglyphsCJK-0.0.2/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3190 2023-05-22 02:32:54.660512 HomoglyphsCJK-0.0.2/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2646 2023-05-22 02:32:14.000000 HomoglyphsCJK-0.0.2/README.md
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:32:54.660020 HomoglyphsCJK-0.0.2/homo/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       80 2023-05-13 13:35:00.000000 HomoglyphsCJK-0.0.2/homo/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.2/homo/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.2/homo/test_run.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 02:32:54.660781 HomoglyphsCJK-0.0.2/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      918 2023-05-22 02:32:41.000000 HomoglyphsCJK-0.0.2/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:35:53.825710 HomoglyphsCJK-0.0.3/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:35:53.823758 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      257 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        5 2023-05-22 02:35:53.000000 HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 02:35:53.825502 HomoglyphsCJK-0.0.3/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2614 2023-05-22 02:35:38.000000 HomoglyphsCJK-0.0.3/README.md
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 02:35:53.824983 HomoglyphsCJK-0.0.3/homo/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       80 2023-05-13 13:35:00.000000 HomoglyphsCJK-0.0.3/homo/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.3/homo/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.3/homo/test_run.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 02:35:53.825784 HomoglyphsCJK-0.0.3/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      918 2023-05-22 02:35:45.000000 HomoglyphsCJK-0.0.3/setup.py
```

### Comparing `HomoglyphsCJK-0.0.2/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.0.3/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 HomoglyphsCJK
 =====
 
 An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
 
 ## Installation
 ```
-pip install -i https://test.pypi.org/simple/ homoglyphs-testpypi
+pip install HomoglyphsCJK==0.0.3
 ```
 
 ## Usage
 There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
 
 When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write.
```

### Comparing `HomoglyphsCJK-0.0.2/PKG-INFO` & `HomoglyphsCJK-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 HomoglyphsCJK
 =====
 
 An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
 
 ## Installation
 ```
-pip install -i https://test.pypi.org/simple/ homoglyphs-testpypi
+pip install HomoglyphsCJK==0.0.3
 ```
 
 ## Usage
 There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
 
 When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write.
```

### Comparing `HomoglyphsCJK-0.0.2/README.md` & `HomoglyphsCJK-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 HomoglyphsCJK
 =====
 
 An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
 
 ## Installation
 ```
-pip install -i https://test.pypi.org/simple/ homoglyphs-testpypi
+pip install HomoglyphsCJK==0.0.3
 ```
 
 ## Usage
 There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
 
 When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write.
```

### Comparing `HomoglyphsCJK-0.0.2/homo/hg_functions.py` & `HomoglyphsCJK-0.0.3/homo/hg_functions.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.2/homo/test_run.py` & `HomoglyphsCJK-0.0.3/homo/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.2/setup.py` & `HomoglyphsCJK-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
-    version="0.0.2",
+    version="0.0.3",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

