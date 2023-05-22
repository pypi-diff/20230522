# Comparing `tmp/HomoglyphsCJK-0.0.7.tar.gz` & `tmp/HomoglyphsCJK-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.0.7.tar", last modified: Mon May 22 14:52:03 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.0.8.tar", last modified: Mon May 22 14:53:50 2023, max compression
```

## Comparing `HomoglyphsCJK-0.0.7.tar` & `HomoglyphsCJK-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:52:03.190775 HomoglyphsCJK-0.0.7/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:52:03.189115 HomoglyphsCJK-0.0.7/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.0.7/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.7/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.7/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:52:03.190288 HomoglyphsCJK-0.0.7/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3351 2023-05-22 14:52:03.000000 HomoglyphsCJK-0.0.7/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 14:52:03.000000 HomoglyphsCJK-0.0.7/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 14:52:03.000000 HomoglyphsCJK-0.0.7/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 14:52:03.000000 HomoglyphsCJK-0.0.7/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 14:52:03.000000 HomoglyphsCJK-0.0.7/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3351 2023-05-22 14:52:03.190583 HomoglyphsCJK-0.0.7/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2807 2023-05-22 14:51:52.000000 HomoglyphsCJK-0.0.7/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 14:52:03.190838 HomoglyphsCJK-0.0.7/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-22 14:50:54.000000 HomoglyphsCJK-0.0.7/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:53:50.820201 HomoglyphsCJK-0.0.8/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:53:50.818604 HomoglyphsCJK-0.0.8/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 14:53:50.819698 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3406 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 14:53:50.000000 HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3406 2023-05-22 14:53:50.819982 HomoglyphsCJK-0.0.8/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2862 2023-05-22 14:53:38.000000 HomoglyphsCJK-0.0.8/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 14:53:50.820266 HomoglyphsCJK-0.0.8/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-22 14:53:43.000000 HomoglyphsCJK-0.0.8/setup.py
```

### Comparing `HomoglyphsCJK-0.0.7/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.0.8/HomoglyphsCJK/hg_functions.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.7/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.0.8/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.7/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.0.8/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.7
+Version: 0.0.8
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -55,17 +55,18 @@
 | ---------- | ----------------------- | --------- |
 | 苏萃乡      | 小苏莽乡                 | 1.88      | 
 | 办雄        | 协雄                    | 0.15      |
 | 虐格给      | 唐格给                   | 0.87      |
 | 雪拉普岗    | 雪拉普岗日                | 1.0       | 
 
 + Homoglyph distance between two strings. The default weight on substitution, insertion, deletion is 1.
++ download_dict and homoglyph_merge will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
 
 ```python
-    # download_dict will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the dict.
+    
     download_dict('zhs')
     homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
     # 1.88
 ```
 
 ## Citation
```

### Comparing `HomoglyphsCJK-0.0.7/PKG-INFO` & `HomoglyphsCJK-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.7
+Version: 0.0.8
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -55,17 +55,18 @@
 | ---------- | ----------------------- | --------- |
 | 苏萃乡      | 小苏莽乡                 | 1.88      | 
 | 办雄        | 协雄                    | 0.15      |
 | 虐格给      | 唐格给                   | 0.87      |
 | 雪拉普岗    | 雪拉普岗日                | 1.0       | 
 
 + Homoglyph distance between two strings. The default weight on substitution, insertion, deletion is 1.
++ download_dict and homoglyph_merge will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
 
 ```python
-    # download_dict will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the dict.
+    
     download_dict('zhs')
     homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
     # 1.88
 ```
 
 ## Citation
```

### Comparing `HomoglyphsCJK-0.0.7/README.md` & `HomoglyphsCJK-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,18 @@
 | ---------- | ----------------------- | --------- |
 | 苏萃乡      | 小苏莽乡                 | 1.88      | 
 | 办雄        | 协雄                    | 0.15      |
 | 虐格给      | 唐格给                   | 0.87      |
 | 雪拉普岗    | 雪拉普岗日                | 1.0       | 
 
 + Homoglyph distance between two strings. The default weight on substitution, insertion, deletion is 1.
++ download_dict and homoglyph_merge will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
 
 ```python
-    # download_dict will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the dict.
+    
     download_dict('zhs')
     homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
     # 1.88
 ```
 
 ## Citation
```

### Comparing `HomoglyphsCJK-0.0.7/setup.py` & `HomoglyphsCJK-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
     packages=["HomoglyphsCJK"],
-    version="0.0.7",
+    version="0.0.8",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

