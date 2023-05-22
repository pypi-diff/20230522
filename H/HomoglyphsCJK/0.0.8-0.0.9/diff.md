# Comparing `tmp/HomoglyphsCJK-0.0.8.tar.gz` & `tmp/HomoglyphsCJK-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.0.8.tar", last modified: Mon May 22 14:53:50 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.0.9.tar", last modified: Mon May 22 15:03:32 2023, max compression
```

## Comparing `HomoglyphsCJK-0.0.8.tar` & `HomoglyphsCJK-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:53:50.820201 HomoglyphsCJK-0.0.8/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:53:50.818604 HomoglyphsCJK-0.0.8/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:53:50.819698 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3406 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3406 2023-05-22 14:53:50.819982 HomoglyphsCJK-0.0.8/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2862 2023-05-22 14:53:38.000000 HomoglyphsCJK-0.0.8/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 14:53:50.820266 HomoglyphsCJK-0.0.8/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-22 14:53:43.000000 HomoglyphsCJK-0.0.8/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 15:03:32.219113 HomoglyphsCJK-0.0.9/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 15:03:32.217255 HomoglyphsCJK-0.0.9/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 15:03:32.218598 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3357 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3357 2023-05-22 15:03:32.218915 HomoglyphsCJK-0.0.9/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2813 2023-05-22 15:03:01.000000 HomoglyphsCJK-0.0.9/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 15:03:32.219177 HomoglyphsCJK-0.0.9/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-22 15:03:25.000000 HomoglyphsCJK-0.0.9/setup.py
```

### Comparing `HomoglyphsCJK-0.0.8/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.0.9/HomoglyphsCJK/hg_functions.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.8/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.0.9/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.8
+Version: 0.0.9
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 HomoglyphsCJK
 =====
 
-An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
+An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words.
 
 ## Installation
 ```
 pip install HomoglyphsCJK
 ```
 
 ## Usage
```

### Comparing `HomoglyphsCJK-0.0.8/PKG-INFO` & `HomoglyphsCJK-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.8
+Version: 0.0.9
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 HomoglyphsCJK
 =====
 
-An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
+An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words.
 
 ## Installation
 ```
 pip install HomoglyphsCJK
 ```
 
 ## Usage
```

### Comparing `HomoglyphsCJK-0.0.8/README.md` & `HomoglyphsCJK-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 HomoglyphsCJK
 =====
 
-An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
+An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words.
 
 ## Installation
 ```
 pip install HomoglyphsCJK
 ```
 
 ## Usage
```

### Comparing `HomoglyphsCJK-0.0.8/setup.py` & `HomoglyphsCJK-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
     packages=["HomoglyphsCJK"],
-    version="0.0.8",
+    version="0.0.9",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

