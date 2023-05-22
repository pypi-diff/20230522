# Comparing `tmp/oba-0.0.7.tar.gz` & `tmp/oba-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oba-0.0.7.tar", last modified: Thu May 11 10:18:50 2023, max compression
+gzip compressed data, was "oba-0.0.8.tar", last modified: Mon May 22 10:57:07 2023, max compression
```

## Comparing `oba-0.0.7.tar` & `oba-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-11 10:18:50.680847 oba-0.0.7/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1068 2022-11-07 04:42:30.000000 oba-0.0.7/LICENSE
--rw-r--r--   0 jyonnliu   (501) staff       (20)      798 2023-05-11 10:18:50.680743 oba-0.0.7/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      491 2022-11-07 04:37:13.000000 oba-0.0.7/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-11 10:18:50.680043 oba-0.0.7/oba/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       59 2022-10-21 09:44:26.000000 oba-0.0.7/oba/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     2320 2023-05-11 10:00:56.000000 oba-0.0.7/oba/oba.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-11 10:18:50.680588 oba-0.0.7/oba.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      798 2023-05-11 10:18:50.000000 oba-0.0.7/oba.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      161 2023-05-11 10:18:50.000000 oba-0.0.7/oba.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-05-11 10:18:50.000000 oba-0.0.7/oba.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        4 2023-05-11 10:18:50.000000 oba-0.0.7/oba.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-05-11 10:18:50.680884 oba-0.0.7/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      609 2023-05-11 10:18:39.000000 oba-0.0.7/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-22 10:57:07.001253 oba-0.0.8/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1068 2022-11-07 04:42:30.000000 oba-0.0.8/LICENSE
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      798 2023-05-22 10:57:07.001129 oba-0.0.8/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      491 2022-11-07 04:37:13.000000 oba-0.0.8/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-22 10:57:07.000432 oba-0.0.8/oba/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       59 2022-10-21 09:44:26.000000 oba-0.0.8/oba/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     2349 2023-05-22 10:56:38.000000 oba-0.0.8/oba/oba.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-22 10:57:07.000951 oba-0.0.8/oba.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      798 2023-05-22 10:57:06.000000 oba-0.0.8/oba.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      161 2023-05-22 10:57:06.000000 oba-0.0.8/oba.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-05-22 10:57:06.000000 oba-0.0.8/oba.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        4 2023-05-22 10:57:06.000000 oba-0.0.8/oba.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-05-22 10:57:07.001285 oba-0.0.8/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      609 2023-05-22 10:57:02.000000 oba-0.0.8/setup.py
```

### Comparing `oba-0.0.7/LICENSE` & `oba-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oba-0.0.7/PKG-INFO` & `oba-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oba
-Version: 0.0.7
+Version: 0.0.8
 Summary: make iter object easy to access (item to attr)
 Home-page: https://github.com/Jyonn/Oba
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: dict,object
 Platform: any
```

### Comparing `oba-0.0.7/oba/oba.py` & `oba-0.0.8/oba/oba.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def __str__(self):
         raise ValueError(f'Path {NoneObj.raw(self)} not exists')
     
     
 class Obj:
     @staticmethod
     def iterable(obj):
-        return isinstance(obj, Iterable)
+        return isinstance(obj, Iterable) and not isinstance(obj, str)
 
     @staticmethod
     def raw(o: 'Obj'):
         if isinstance(o, Obj):
             return object.__getattribute__(o, '__obj')
         return o
```

### Comparing `oba-0.0.7/oba.egg-info/PKG-INFO` & `oba-0.0.8/oba.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oba
-Version: 0.0.7
+Version: 0.0.8
 Summary: make iter object easy to access (item to attr)
 Home-page: https://github.com/Jyonn/Oba
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: dict,object
 Platform: any
```

### Comparing `oba-0.0.7/setup.py` & `oba-0.0.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='oba',
-    version='0.0.7',
+    version='0.0.8',
     keywords=['dict', 'object'],
     description='make iter object easy to access (item to attr)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/Oba',
     author='Jyonn Liu',
```

