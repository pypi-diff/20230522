# Comparing `tmp/PyEng-1.0.2.tar.gz` & `tmp/PyEng-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEng-1.0.2.tar", last modified: Mon May 22 12:57:52 2023, max compression
+gzip compressed data, was "PyEng-1.0.3.tar", last modified: Mon May 22 13:22:26 2023, max compression
```

## Comparing `PyEng-1.0.2.tar` & `PyEng-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 12:57:52.848610 PyEng-1.0.2/
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyEng-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       76 2023-05-20 14:00:41.000000 PyEng-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2480 2023-05-22 12:57:52.845618 PyEng-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 12:57:52.533641 PyEng-1.0.2/PyEng/
--rw-rw-rw-   0        0        0     1668 2023-05-22 12:56:48.000000 PyEng-1.0.2/PyEng/Words.py
--rw-rw-rw-   0        0        0       55 2023-05-20 14:01:19.000000 PyEng-1.0.2/PyEng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 12:57:52.574556 PyEng-1.0.2/PyEng/data/
--rw-rw-rw-   0        0        0 22970019 2023-05-20 13:53:02.000000 PyEng-1.0.2/PyEng/data/dictionary.json
-drwxrwxrwx   0        0        0        0 2023-05-22 12:57:52.570329 PyEng-1.0.2/PyEng.egg-info/
--rw-rw-rw-   0        0        0     2480 2023-05-22 12:57:52.000000 PyEng-1.0.2/PyEng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-22 12:57:52.000000 PyEng-1.0.2/PyEng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 12:57:52.000000 PyEng-1.0.2/PyEng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 12:57:52.000000 PyEng-1.0.2/PyEng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2007 2023-05-22 12:54:56.000000 PyEng-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 12:57:52.849607 PyEng-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-22 12:55:27.000000 PyEng-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:22:26.922455 PyEng-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyEng-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       76 2023-05-20 14:00:41.000000 PyEng-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2480 2023-05-22 13:22:26.920460 PyEng-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 13:22:26.833742 PyEng-1.0.3/PyEng/
+-rw-rw-rw-   0        0        0      486 2023-05-22 13:18:54.000000 PyEng-1.0.3/PyEng/Grammar.py
+-rw-rw-rw-   0        0        0     1668 2023-05-22 12:56:48.000000 PyEng-1.0.3/PyEng/Words.py
+-rw-rw-rw-   0        0        0       55 2023-05-20 14:01:19.000000 PyEng-1.0.3/PyEng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:22:26.851155 PyEng-1.0.3/PyEng/data/
+-rw-rw-rw-   0        0        0 22970019 2023-05-20 13:53:02.000000 PyEng-1.0.3/PyEng/data/dictionary.json
+drwxrwxrwx   0        0        0        0 2023-05-22 13:22:26.848163 PyEng-1.0.3/PyEng.egg-info/
+-rw-rw-rw-   0        0        0     2480 2023-05-22 13:22:26.000000 PyEng-1.0.3/PyEng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-22 13:22:26.000000 PyEng-1.0.3/PyEng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 13:22:26.000000 PyEng-1.0.3/PyEng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 13:22:26.000000 PyEng-1.0.3/PyEng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-05-22 13:19:01.000000 PyEng-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 13:22:26.922455 PyEng-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-22 13:19:06.000000 PyEng-1.0.3/setup.py
```

### Comparing `PyEng-1.0.2/LICENSE.txt` & `PyEng-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyEng-1.0.2/PKG-INFO` & `PyEng-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEng
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyEng is a general-purpose Python package that contains functions related to the English language.
 Home-page: https://github.com/Anikethc/PyEng
 Download-URL: https://pypi.org/project/PyEng
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: English
@@ -18,15 +18,15 @@
 PyEng is a general-purpose Python package that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
 ## Package Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.2</br>
+**Version** - 1.0.3</br>
 **Description** - PyEng is a general-purpose Python package that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
```

### Comparing `PyEng-1.0.2/PyEng/Words.py` & `PyEng-1.0.3/PyEng/Words.py`

 * *Files identical despite different names*

### Comparing `PyEng-1.0.2/PyEng/data/dictionary.json` & `PyEng-1.0.3/PyEng/data/dictionary.json`

 * *Files identical despite different names*

### Comparing `PyEng-1.0.2/PyEng.egg-info/PKG-INFO` & `PyEng-1.0.3/PyEng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEng
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyEng is a general-purpose Python package that contains functions related to the English language.
 Home-page: https://github.com/Anikethc/PyEng
 Download-URL: https://pypi.org/project/PyEng
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: English
@@ -18,15 +18,15 @@
 PyEng is a general-purpose Python package that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
 ## Package Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.2</br>
+**Version** - 1.0.3</br>
 **Description** - PyEng is a general-purpose Python package that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
```

### Comparing `PyEng-1.0.2/README.md` & `PyEng-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PyEng is a general-purpose Python package that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
 ## Package Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.2</br>
+**Version** - 1.0.3</br>
 **Description** - PyEng is a general-purpose Python package that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
```

### Comparing `PyEng-1.0.2/setup.py` & `PyEng-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PyEng",
-    version="1.0.2",
+    version="1.0.3",
     description="PyEng is a general-purpose Python package that contains functions related to the English language.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

