# Comparing `tmp/jwtools-0.1.5.tar.gz` & `tmp/jwtools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtools-0.1.5.tar", last modified: Thu May 18 03:37:30 2023, max compression
+gzip compressed data, was "jwtools-0.1.6.tar", last modified: Mon May 22 05:30:25 2023, max compression
```

## Comparing `jwtools-0.1.5.tar` & `jwtools-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 03:37:30.626638 jwtools-0.1.5/
--rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1324 2023-05-18 03:37:30.625639 jwtools-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      771 2023-05-18 02:30:45.000000 jwtools-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 03:37:30.620637 jwtools-0.1.5/jwtools/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.5/jwtools/__init__.py
--rw-rw-rw-   0        0        0     1312 2023-05-18 03:36:42.000000 jwtools-0.1.5/jwtools/func.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:37:30.623639 jwtools-0.1.5/jwtools.egg-info/
--rw-rw-rw-   0        0        0     1324 2023-05-18 03:37:30.000000 jwtools-0.1.5/jwtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-18 03:37:30.000000 jwtools-0.1.5/jwtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 03:37:30.000000 jwtools-0.1.5/jwtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-18 03:37:30.000000 jwtools-0.1.5/jwtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 03:37:30.626638 jwtools-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-18 03:37:26.000000 jwtools-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:37:30.624638 jwtools-0.1.5/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0      209 2023-05-18 03:36:21.000000 jwtools-0.1.5/tests/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:30:25.662289 jwtools-0.1.6/
+-rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1324 2023-05-22 05:30:25.661289 jwtools-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      771 2023-05-18 02:30:45.000000 jwtools-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 05:30:25.654283 jwtools-0.1.6/jwtools/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.6/jwtools/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-05-19 10:02:42.000000 jwtools-0.1.6/jwtools/dt.py
+-rw-rw-rw-   0        0        0     1568 2023-05-22 05:29:30.000000 jwtools-0.1.6/jwtools/func.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:30:25.658285 jwtools-0.1.6/jwtools.egg-info/
+-rw-rw-rw-   0        0        0     1324 2023-05-22 05:30:25.000000 jwtools-0.1.6/jwtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-22 05:30:25.000000 jwtools-0.1.6/jwtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:30:25.000000 jwtools-0.1.6/jwtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 05:30:25.000000 jwtools-0.1.6/jwtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 05:30:25.662289 jwtools-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-05-22 05:29:30.000000 jwtools-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:30:25.660291 jwtools-0.1.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-05-18 03:36:21.000000 jwtools-0.1.6/tests/test1.py
```

### Comparing `jwtools-0.1.5/LICENSE` & `jwtools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.5/PKG-INFO` & `jwtools-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtools
-Version: 0.1.5
+Version: 0.1.6
 Summary: It is a micro-toolbox that includes various common operations and will continue to be improved in the future.
 Home-page: https://github.com/jinghewang/python-jwtools.git
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jwtools-0.1.5/README.md` & `jwtools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.5/jwtools/func.py` & `jwtools-0.1.6/jwtools/func.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,7 +46,22 @@
     :param filename：要读取的文件名。
     :param encoding：文件的编码方式，默认为utf-8。
     :return: 从文件中读取到的文本内容。
     """
     with open(filename, "r", encoding=encoding) as file:
         text = file.read()
     return text
+
+
+def print_vf(*args):
+    """
+    print var or function
+    :author wjh
+    :date 2023-05-22
+    :param args:
+    :return:
+    """
+    for arg in args:
+        if callable(arg):
+            print(arg())
+        else:
+            print(arg)
```

### Comparing `jwtools-0.1.5/jwtools.egg-info/PKG-INFO` & `jwtools-0.1.6/jwtools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtools
-Version: 0.1.5
+Version: 0.1.6
 Summary: It is a micro-toolbox that includes various common operations and will continue to be improved in the future.
 Home-page: https://github.com/jinghewang/python-jwtools.git
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jwtools-0.1.5/setup.py` & `jwtools-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jwtools',
-    version='0.1.5',
+    version='0.1.6',
     description="It is a micro-toolbox that includes various common operations and will continue to be improved in the future.",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     author='jinghewang',
     author_email='jinghewang@163.com',
     license='MIT License',
```

