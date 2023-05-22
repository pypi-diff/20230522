# Comparing `tmp/htutil-3.1.0.tar.gz` & `tmp/htutil-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/htutil/htutil/dist/.tmp-5oj0ya71/htutil-3.1.0.tar", last modified: Sun May 21 03:04:20 2023, max compression
+gzip compressed data, was "/home/runner/work/htutil/htutil/dist/.tmp-cgj6lu8x/htutil-3.2.0.tar", last modified: Mon May 22 15:21:23 2023, max compression
```

## Comparing `htutil-3.1.0.tar` & `htutil-3.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:04:20.000000 htutil-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-21 03:04:08.000000 htutil-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-21 03:04:20.000000 htutil-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-21 03:04:08.000000 htutil-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 03:04:08.000000 htutil-3.1.0/htutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-21 03:04:08.000000 htutil-3.1.0/htutil/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-21 03:04:08.000000 htutil-3.1.0/htutil/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-21 03:04:08.000000 htutil-3.1.0/htutil/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 03:04:20.000000 htutil-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-21 03:04:08.000000 htutil-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:23.000000 htutil-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-22 15:21:15.000000 htutil-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-22 15:21:23.000000 htutil-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-22 15:21:15.000000 htutil-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:23.000000 htutil-3.2.0/htutil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:15.000000 htutil-3.2.0/htutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-22 15:21:15.000000 htutil-3.2.0/htutil/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 15:21:15.000000 htutil-3.2.0/htutil/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-22 15:21:15.000000 htutil-3.2.0/htutil/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:23.000000 htutil-3.2.0/htutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-22 15:21:23.000000 htutil-3.2.0/htutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-22 15:21:23.000000 htutil-3.2.0/htutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:21:23.000000 htutil-3.2.0/htutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 15:21:23.000000 htutil-3.2.0/htutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 15:21:23.000000 htutil-3.2.0/htutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:21:23.000000 htutil-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-22 15:21:15.000000 htutil-3.2.0/setup.py
```

### Comparing `htutil-3.1.0/LICENSE` & `htutil-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htutil-3.1.0/PKG-INFO` & `htutil-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htutil
-Version: 3.1.0
+Version: 3.2.0
 Summary: HaoTian's Python Util
 Home-page: https://github.com/117503445/htutil
 Author: 117503445
 Author-email: t117503445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `htutil-3.1.0/README.md` & `htutil-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `htutil-3.1.0/htutil/cache.py` & `htutil-3.2.0/htutil/cache.py`

 * *Files identical despite different names*

### Comparing `htutil-3.1.0/htutil/file.py` & `htutil-3.2.0/htutil/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import pickle as pkl
 from pathlib import Path
 import json
+import yaml
 
 
 def read_text(path: str| Path) -> str:
     with open(path, 'r', encoding='utf-8', errors='ignore') as f:
         lines = f.readlines()
         text = ''.join(lines)
         return text
@@ -96,14 +97,19 @@
 def write_json(path: str| Path, content, indent=4) -> None:
     write_text(path, json.dumps(content, indent=indent, ensure_ascii=False, default=lambda x: x.__dict__))
 
 
 def read_json(path: str| Path):
     return json.loads(read_text(path))
 
+def write_yaml(path: str| Path, content, indent=4) -> None:
+    write_text(path, yaml.dump(content, allow_unicode=True, indent=indent))
+
+def read_yaml(path: str| Path):
+    return yaml.load(read_text(path), Loader=yaml.FullLoader)
 
 def main():
     s = 'hello'
     write_text('1.txt', s)
     # hello in 1.txt
     append_text('1.txt', 'world')
     # helloworld in 1.txt
@@ -114,12 +120,19 @@
     write_lines('1.txt', s)
     # hello\nworld in 1.txt
     append_lines('1.txt', ['\npython'])
     # hello\nworld\npython in 1.txt
     s = read_lines('1.txt')
     print(s)  # ['hello', 'world', 'python']
 
+    s = {'a': 1, 'b': [1, 2, 3]}
+    write_yaml('1.yaml', s)
+
+    s = read_yaml('1.yaml')
+    print(s) # {'a': 1, 'b': [1, 2, 3]}
+
     os.remove('1.txt')
+    os.remove('1.yaml')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `htutil-3.1.0/htutil.egg-info/PKG-INFO` & `htutil-3.2.0/htutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htutil
-Version: 3.1.0
+Version: 3.2.0
 Summary: HaoTian's Python Util
 Home-page: https://github.com/117503445/htutil
 Author: 117503445
 Author-email: t117503445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `htutil-3.1.0/setup.py` & `htutil-3.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="htutil",
-    version="3.1.0",
+    version="3.2.0",
     author="117503445",
     author_email="t117503445@gmail.com",
     description="HaoTian's Python Util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/117503445/htutil",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
-    ]
+    ],   
+    install_requires=['pyyaml']
 )
```

