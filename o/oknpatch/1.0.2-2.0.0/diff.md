# Comparing `tmp/oknpatch-1.0.2.tar.gz` & `tmp/oknpatch-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oknpatch-1.0.2.tar", last modified: Mon Feb 27 20:57:02 2023, max compression
+gzip compressed data, was "oknpatch-2.0.0.tar", last modified: Mon May 22 00:04:15 2023, max compression
```

## Comparing `oknpatch-1.0.2.tar` & `oknpatch-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 20:57:02.239834 oknpatch-1.0.2/
--rw-rw-rw-   0        0        0    11558 2022-07-06 00:41:01.000000 oknpatch-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      525 2023-02-27 20:57:02.239834 oknpatch-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2344 2023-02-27 04:55:12.000000 oknpatch-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-27 20:57:02.229847 oknpatch-1.0.2/oknpatch/
--rw-rw-rw-   0        0        0        0 2023-02-12 22:01:11.000000 oknpatch-1.0.2/oknpatch/__init__.py
--rw-rw-rw-   0        0        0     5925 2022-04-19 02:25:13.000000 oknpatch-1.0.2/oknpatch/gazefilters.json
--rw-rw-rw-   0        0        0    24240 2023-02-27 20:56:25.000000 oknpatch-1.0.2/oknpatch/oknpatch.py
-drwxrwxrwx   0        0        0        0 2023-02-27 20:57:02.238823 oknpatch-1.0.2/oknpatch.egg-info/
--rw-rw-rw-   0        0        0      525 2023-02-27 20:57:02.000000 oknpatch-1.0.2/oknpatch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-02-27 20:57:02.000000 oknpatch-1.0.2/oknpatch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 20:57:02.000000 oknpatch-1.0.2/oknpatch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-02-27 20:57:02.000000 oknpatch-1.0.2/oknpatch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 20:56:51.000000 oknpatch-1.0.2/oknpatch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-02-27 20:57:02.000000 oknpatch-1.0.2/oknpatch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-27 20:57:02.000000 oknpatch-1.0.2/oknpatch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-27 20:57:02.239834 oknpatch-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1035 2023-02-27 20:56:25.000000 oknpatch-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 00:04:15.576355 oknpatch-2.0.0/
+-rw-rw-rw-   0        0        0    11558 2022-07-06 00:41:01.000000 oknpatch-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      525 2023-05-22 00:04:15.576355 oknpatch-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2344 2023-02-27 04:55:12.000000 oknpatch-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 00:04:15.565384 oknpatch-2.0.0/oknpatch/
+-rw-rw-rw-   0        0        0        0 2023-02-12 22:01:11.000000 oknpatch-2.0.0/oknpatch/__init__.py
+-rw-rw-rw-   0        0        0     5925 2022-04-19 02:25:13.000000 oknpatch-2.0.0/oknpatch/gazefilters.json
+-rw-rw-rw-   0        0        0    26699 2023-05-22 00:00:36.000000 oknpatch-2.0.0/oknpatch/oknpatch.py
+drwxrwxrwx   0        0        0        0 2023-05-22 00:04:15.575358 oknpatch-2.0.0/oknpatch.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-22 00:03:15.000000 oknpatch-2.0.0/oknpatch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 00:04:15.576355 oknpatch-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2023-05-22 00:00:01.000000 oknpatch-2.0.0/setup.py
```

### Comparing `oknpatch-1.0.2/LICENSE` & `oknpatch-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oknpatch-1.0.2/PKG-INFO` & `oknpatch-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknpatch
-Version: 1.0.2
+Version: 2.0.0
 Summary: issues fixing program
 Home-page: https://github.com/jtur044/oknpatch
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: oknpatch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oknpatch-1.0.2/README.md` & `oknpatch-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oknpatch-1.0.2/oknpatch/gazefilters.json` & `oknpatch-2.0.0/oknpatch/gazefilters.json`

 * *Files identical despite different names*

### Comparing `oknpatch-1.0.2/oknpatch/oknpatch.py` & `oknpatch-2.0.0/oknpatch/oknpatch.py`

 * *Files 16% similar despite different names*

```diff
@@ -202,14 +202,21 @@
 
         input_column = this_filter["input"][0]
         f = y[input_column]
         n = this_filter["npoint"]
         y[this_filter["output"]] = medfilt(f, n)
         print(f"{input_column} column has been median filtered with n point {n}.")
 
+    elif match_item == 'replaceNanBy':
+
+        input_column = this_filter["input"][0]
+        input_array = y[input_column]
+        pointer = this_filter["pointer"]
+        y[this_filter["output"]] = replace_nan_by(y, input_array, pointer)
+
     elif match_item == 'applymask':
         print(match_item)
     elif match_item == 'detrender':
         print(match_item)
     elif match_item == 'detectblinkV':
         print(match_item)
     elif match_item == 'gradient':
@@ -251,14 +258,72 @@
                 M[key] = temp_array
     else:
         print("The number of loop input must be number!")
 
     return M
 
 
+def replace_nan_by(y, input_array, pointer):
+    if "<=" in pointer:
+        try:
+            column_name, value = str(pointer).split("<=")
+            pointer_column__array = y[column_name]
+            array_length = len(input_array)
+            for ind in range(array_length):
+                if float(pointer_column__array[ind]) <= float(value):
+                    input_array[ind] = np.nan
+        except KeyError:
+            pass
+    elif "==" in pointer:
+        try:
+            column_name, value = str(pointer).split("==")
+            pointer_column__array = y[column_name]
+            array_length = len(input_array)
+            for ind in range(array_length):
+                if float(pointer_column__array[ind]) == float(value):
+                    input_array[ind] = np.nan
+        except KeyError:
+            pass
+    elif ">=" in pointer:
+        try:
+            column_name, value = str(pointer).split(">=")
+            pointer_column__array = y[column_name]
+            array_length = len(input_array)
+            for ind in range(array_length):
+                if float(pointer_column__array[ind]) >= float(value):
+                    input_array[ind] = np.nan
+        except KeyError:
+            pass
+    else:
+        if ">" in pointer:
+            try:
+                column_name, value = str(pointer).split(">")
+                pointer_column__array = y[column_name]
+                array_length = len(input_array)
+                for ind in range(array_length):
+                    if float(pointer_column__array[ind]) > float(value):
+                        input_array[ind] = np.nan
+            except KeyError:
+                pass
+        elif "<" in pointer:
+            try:
+                column_name, value = str(pointer).split("<")
+                pointer_column__array = y[column_name]
+                array_length = len(input_array)
+                for ind in range(array_length):
+                    if float(pointer_column__array[ind]) < float(value):
+                        input_array[ind] = np.nan
+            except KeyError:
+                pass
+        else:
+            pass
+
+    return input_array
+
+
 def waveleter(x, levelForReconstruction, waveletType, level):
     [x1, i] = fillmissing(x)
     x11 = x1
 
     return x11
 
 
@@ -588,15 +653,15 @@
 
     return config_dir
 
 
 def main():
     parser = argparse.ArgumentParser(prog='oknpatch',
                                      description='OKNPATCH package.')
-    parser.add_argument('--version', action='version', version='1.0.2'),
+    parser.add_argument('--version', action='version', version='2.0.0'),
     parser.add_argument("-t", dest="type_input", required=True, default=sys.stdin,
                         help="issue type to fix", metavar="issue type")
     parser.add_argument("-i", dest="first_input", required=False, default=sys.stdin,
                         help="first input", metavar="first input")
     parser.add_argument("-si", dest="second_input", required=False, default=sys.stdin,
                         help="second input", metavar="second input")
     parser.add_argument("-ti", dest="third_input", required=False, default=sys.stdin,
```

### Comparing `oknpatch-1.0.2/oknpatch.egg-info/PKG-INFO` & `oknpatch-2.0.0/oknpatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknpatch
-Version: 1.0.2
+Version: 2.0.0
 Summary: issues fixing program
 Home-page: https://github.com/jtur044/oknpatch
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: oknpatch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oknpatch-1.0.2/setup.py` & `oknpatch-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to fix okn and pim related issues.'
 
 setup(
     name='oknpatch',
-    version='1.0.2',
+    version='2.0.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/oknpatch',
     description='issues fixing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

