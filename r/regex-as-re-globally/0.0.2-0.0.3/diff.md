# Comparing `tmp/regex-as-re-globally-0.0.2.tar.gz` & `tmp/regex-as-re-globally-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/regex-as-re-globally-0.0.2.tar", last modified: Wed Mar  2 19:42:31 2022, max compression
+gzip compressed data, was "dist/regex-as-re-globally-0.0.3.tar", last modified: Mon May 22 21:39:14 2023, max compression
```

## Comparing `regex-as-re-globally-0.0.2.tar` & `regex-as-re-globally-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/
--rw-r--r--   0 brondsem   (502) staff       (20)     1315 2022-03-01 23:14:13.000000 regex-as-re-globally-0.0.2/LICENSE.txt
--rw-r--r--   0 brondsem   (502) staff       (20)       51 2022-03-01 23:14:13.000000 regex-as-re-globally-0.0.2/MANIFEST.in
--rw-r--r--   0 brondsem   (502) staff       (20)     1851 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/PKG-INFO
--rw-r--r--   0 brondsem   (502) staff       (20)     1285 2022-03-02 19:37:20.000000 regex-as-re-globally-0.0.2/README.md
--rw-r--r--   0 brondsem   (502) staff       (20)       59 2022-03-02 15:57:51.000000 regex-as-re-globally-0.0.2/regex-as-re-globally.pth
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/regex_as_re_globally.egg-info/
--rw-r--r--   0 brondsem   (502) staff       (20)     1851 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/regex_as_re_globally.egg-info/PKG-INFO
--rw-r--r--   0 brondsem   (502) staff       (20)      339 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/regex_as_re_globally.egg-info/SOURCES.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/regex_as_re_globally.egg-info/dependency_links.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/regex_as_re_globally.egg-info/not-zip-safe
--rw-r--r--   0 brondsem   (502) staff       (20)       16 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/regex_as_re_globally.egg-info/requires.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/regex_as_re_globally.egg-info/top_level.txt
--rw-r--r--   0 brondsem   (502) staff       (20)       53 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.2/setup.cfg
--rw-r--r--   0 brondsem   (502) staff       (20)     1782 2022-03-02 19:37:19.000000 regex-as-re-globally-0.0.2/setup.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-05-22 21:39:14.000000 regex-as-re-globally-0.0.3/
+-rw-r--r--   0 brondsem   (502) staff       (20)     1315 2022-03-01 23:14:13.000000 regex-as-re-globally-0.0.3/LICENSE.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)       51 2022-03-01 23:14:13.000000 regex-as-re-globally-0.0.3/MANIFEST.in
+-rw-r--r--   0 brondsem   (502) staff       (20)     1709 2023-05-22 21:39:14.000000 regex-as-re-globally-0.0.3/PKG-INFO
+-rw-r--r--   0 brondsem   (502) staff       (20)     1285 2022-03-02 19:37:20.000000 regex-as-re-globally-0.0.3/README.md
+-rw-r--r--   0 brondsem   (502) staff       (20)      284 2023-05-22 21:24:27.000000 regex-as-re-globally-0.0.3/regex-as-re-globally.pth
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-05-22 21:39:14.000000 regex-as-re-globally-0.0.3/regex_as_re_globally.egg-info/
+-rw-r--r--   0 brondsem   (502) staff       (20)     1709 2023-05-22 21:39:12.000000 regex-as-re-globally-0.0.3/regex_as_re_globally.egg-info/PKG-INFO
+-rw-r--r--   0 brondsem   (502) staff       (20)      339 2023-05-22 21:39:14.000000 regex-as-re-globally-0.0.3/regex_as_re_globally.egg-info/SOURCES.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)        1 2023-05-22 21:39:13.000000 regex-as-re-globally-0.0.3/regex_as_re_globally.egg-info/dependency_links.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)        1 2022-03-02 19:42:31.000000 regex-as-re-globally-0.0.3/regex_as_re_globally.egg-info/not-zip-safe
+-rw-r--r--   0 brondsem   (502) staff       (20)       16 2023-05-22 21:39:13.000000 regex-as-re-globally-0.0.3/regex_as_re_globally.egg-info/requires.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)        1 2023-05-22 21:39:13.000000 regex-as-re-globally-0.0.3/regex_as_re_globally.egg-info/top_level.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)       53 2023-05-22 21:39:14.000000 regex-as-re-globally-0.0.3/setup.cfg
+-rw-r--r--   0 brondsem   (502) staff       (20)     1782 2023-05-22 21:37:47.000000 regex-as-re-globally-0.0.3/setup.py
```

### Comparing `regex-as-re-globally-0.0.2/LICENSE.txt` & `regex-as-re-globally-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `regex-as-re-globally-0.0.2/PKG-INFO` & `regex-as-re-globally-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: regex-as-re-globally
-Version: 0.0.2
+Version: 0.0.3
 Summary: Creates a regex-as-re-globally.pth to replace stdlib "re" module with "regex" module globally before any code runs.
 Home-page: https://github.com/brondsem/regex-as-re-globally/
 Author: Dave Brondsema
 Author-email: dave@brondsema.net
-License: UNKNOWN
-Description: ## regex-as-re-globally
-        
-        This package does very unusual things, and you normally don't need it.
-        It helps you use the "[regex](https://pypi.org/project/regex/)" package which is a backwards-compatible replacement for `re`, with additional features and better performance in some situations (and worse performance in others).
-        Normally you can put `import regex as re` in your .py files and that's all you need.
-        
-        However, if you want to use `regex` instead of `re` across your whole environment, even within 3rd-party libraries, then this package is for you.
-        
-        Run `pip install regex-as-re-globally` to install this package.
-        It will create a .pth file in site-packages which modifies `sys.modules` so that `regex` is used _everywhere_ instead of `re`.
-        **This changes behavior within the whole python environment.**
-        
-        The wheel files generated are platform and python specific due to the limitations of wheel files, where the relative directory for site-packages needs to be determined at wheel building time, not install time. The directory is dependent on the version of python and the platform you are on.
-        
-        The site-packages .pth technique is heavily inspired by https://github.com/dougn/coverage_pth and https://nedbatchelder.com/blog/201001/running_code_at_python_startup.html  Thanks!
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+## regex-as-re-globally
+
+This package does very unusual things, and you normally don't need it.
+It helps you use the "[regex](https://pypi.org/project/regex/)" package which is a backwards-compatible replacement for `re`, with additional features and better performance in some situations (and worse performance in others).
+Normally you can put `import regex as re` in your .py files and that's all you need.
+
+However, if you want to use `regex` instead of `re` across your whole environment, even within 3rd-party libraries, then this package is for you.
+
+Run `pip install regex-as-re-globally` to install this package.
+It will create a .pth file in site-packages which modifies `sys.modules` so that `regex` is used _everywhere_ instead of `re`.
+**This changes behavior within the whole python environment.**
+
+The wheel files generated are platform and python specific due to the limitations of wheel files, where the relative directory for site-packages needs to be determined at wheel building time, not install time. The directory is dependent on the version of python and the platform you are on.
+
+The site-packages .pth technique is heavily inspired by https://github.com/dougn/coverage_pth and https://nedbatchelder.com/blog/201001/running_code_at_python_startup.html  Thanks!
```

### Comparing `regex-as-re-globally-0.0.2/README.md` & `regex-as-re-globally-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `regex-as-re-globally-0.0.2/regex_as_re_globally.egg-info/PKG-INFO` & `regex-as-re-globally-0.0.3/regex_as_re_globally.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: regex-as-re-globally
-Version: 0.0.2
+Version: 0.0.3
 Summary: Creates a regex-as-re-globally.pth to replace stdlib "re" module with "regex" module globally before any code runs.
 Home-page: https://github.com/brondsem/regex-as-re-globally/
 Author: Dave Brondsema
 Author-email: dave@brondsema.net
-License: UNKNOWN
-Description: ## regex-as-re-globally
-        
-        This package does very unusual things, and you normally don't need it.
-        It helps you use the "[regex](https://pypi.org/project/regex/)" package which is a backwards-compatible replacement for `re`, with additional features and better performance in some situations (and worse performance in others).
-        Normally you can put `import regex as re` in your .py files and that's all you need.
-        
-        However, if you want to use `regex` instead of `re` across your whole environment, even within 3rd-party libraries, then this package is for you.
-        
-        Run `pip install regex-as-re-globally` to install this package.
-        It will create a .pth file in site-packages which modifies `sys.modules` so that `regex` is used _everywhere_ instead of `re`.
-        **This changes behavior within the whole python environment.**
-        
-        The wheel files generated are platform and python specific due to the limitations of wheel files, where the relative directory for site-packages needs to be determined at wheel building time, not install time. The directory is dependent on the version of python and the platform you are on.
-        
-        The site-packages .pth technique is heavily inspired by https://github.com/dougn/coverage_pth and https://nedbatchelder.com/blog/201001/running_code_at_python_startup.html  Thanks!
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+## regex-as-re-globally
+
+This package does very unusual things, and you normally don't need it.
+It helps you use the "[regex](https://pypi.org/project/regex/)" package which is a backwards-compatible replacement for `re`, with additional features and better performance in some situations (and worse performance in others).
+Normally you can put `import regex as re` in your .py files and that's all you need.
+
+However, if you want to use `regex` instead of `re` across your whole environment, even within 3rd-party libraries, then this package is for you.
+
+Run `pip install regex-as-re-globally` to install this package.
+It will create a .pth file in site-packages which modifies `sys.modules` so that `regex` is used _everywhere_ instead of `re`.
+**This changes behavior within the whole python environment.**
+
+The wheel files generated are platform and python specific due to the limitations of wheel files, where the relative directory for site-packages needs to be determined at wheel building time, not install time. The directory is dependent on the version of python and the platform you are on.
+
+The site-packages .pth technique is heavily inspired by https://github.com/dougn/coverage_pth and https://nedbatchelder.com/blog/201001/running_code_at_python_startup.html  Thanks!
```

### Comparing `regex-as-re-globally-0.0.2/setup.py` & `regex-as-re-globally-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     sys.exit(-1)
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='regex-as-re-globally',
-    version='0.0.2',
+    version='0.0.3',
     description='Creates a regex-as-re-globally.pth to replace stdlib "re" module with "regex" module globally before any code runs.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/brondsem/regex-as-re-globally/',
     author='Dave Brondsema',
     author_email='dave@brondsema.net',
     data_files=[
```

