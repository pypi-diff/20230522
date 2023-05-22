# Comparing `tmp/HomoglyphsCJK-0.0.5.tar.gz` & `tmp/HomoglyphsCJK-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.0.5.tar", last modified: Mon May 22 03:33:46 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.0.6.tar", last modified: Mon May 22 03:38:39 2023, max compression
```

## Comparing `HomoglyphsCJK-0.0.5.tar` & `HomoglyphsCJK-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:33:46.548572 HomoglyphsCJK-0.0.5/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:33:46.547425 HomoglyphsCJK-0.0.5/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:33:46.548271 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 03:33:46.000000 HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3158 2023-05-22 03:33:46.548436 HomoglyphsCJK-0.0.5/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2614 2023-05-22 02:38:12.000000 HomoglyphsCJK-0.0.5/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 03:33:46.548613 HomoglyphsCJK-0.0.5/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-22 03:33:01.000000 HomoglyphsCJK-0.0.5/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:38:39.335941 HomoglyphsCJK-0.0.6/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:38:39.334741 HomoglyphsCJK-0.0.6/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.0.6/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.6/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.6/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 03:38:39.335606 HomoglyphsCJK-0.0.6/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3160 2023-05-22 03:38:39.000000 HomoglyphsCJK-0.0.6/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 03:38:39.000000 HomoglyphsCJK-0.0.6/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 03:38:39.000000 HomoglyphsCJK-0.0.6/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 03:38:39.000000 HomoglyphsCJK-0.0.6/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 03:38:39.000000 HomoglyphsCJK-0.0.6/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3160 2023-05-22 03:38:39.335803 HomoglyphsCJK-0.0.6/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2616 2023-05-22 03:38:21.000000 HomoglyphsCJK-0.0.6/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 03:38:39.335984 HomoglyphsCJK-0.0.6/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-22 03:38:04.000000 HomoglyphsCJK-0.0.6/setup.py
```

### Comparing `HomoglyphsCJK-0.0.5/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.0.6/HomoglyphsCJK/hg_functions.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.5/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.0.6/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.5/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.0.6/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,26 +13,26 @@
 HomoglyphsCJK
 =====
 
 An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
 
 ## Installation
 ```
-pip install HomoglyphsCJK==0.0.3
+pip install HomoglyphsCJK
 ```
 
 ## Usage
 There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
 
 When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write.
 
 + Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. Mac users probably want to use Python version == 3.7 for multiprocessing.
 
 ```python
-    from homo import homoglyph_distance,homoglyph_merge,download_dict
+    from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
     import pandas as pd
     df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['ocred_text'])
     df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给']),columns=['truth_text'])
 
     # merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
     ## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
     dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'ocred_text','truth_text',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
```

### Comparing `HomoglyphsCJK-0.0.5/PKG-INFO` & `HomoglyphsCJK-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,26 +13,26 @@
 HomoglyphsCJK
 =====
 
 An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
 
 ## Installation
 ```
-pip install HomoglyphsCJK==0.0.3
+pip install HomoglyphsCJK
 ```
 
 ## Usage
 There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
 
 When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write.
 
 + Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. Mac users probably want to use Python version == 3.7 for multiprocessing.
 
 ```python
-    from homo import homoglyph_distance,homoglyph_merge,download_dict
+    from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
     import pandas as pd
     df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['ocred_text'])
     df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给']),columns=['truth_text'])
 
     # merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
     ## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
     dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'ocred_text','truth_text',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
```

### Comparing `HomoglyphsCJK-0.0.5/README.md` & `HomoglyphsCJK-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 HomoglyphsCJK
 =====
 
 An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, particular useful for OCRed text record linkage.
 
 ## Installation
 ```
-pip install HomoglyphsCJK==0.0.3
+pip install HomoglyphsCJK
 ```
 
 ## Usage
 There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
 
 When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write.
 
 + Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. Mac users probably want to use Python version == 3.7 for multiprocessing.
 
 ```python
-    from homo import homoglyph_distance,homoglyph_merge,download_dict
+    from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
     import pandas as pd
     df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['ocred_text'])
     df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给']),columns=['truth_text'])
 
     # merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
     ## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
     dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'ocred_text','truth_text',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
```

### Comparing `HomoglyphsCJK-0.0.5/setup.py` & `HomoglyphsCJK-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
     packages=["HomoglyphsCJK"],
-    version="0.0.5",
+    version="0.0.6",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

