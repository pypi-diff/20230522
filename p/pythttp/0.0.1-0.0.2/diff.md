# Comparing `tmp/pythttp-0.0.1.tar.gz` & `tmp/pythttp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.0.1.tar", last modified: Wed May  3 09:50:28 2023, max compression
+gzip compressed data, was "pythttp-0.0.2.tar", last modified: Mon May 22 10:02:09 2023, max compression
```

## Comparing `pythttp-0.0.1.tar` & `pythttp-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:50:28.505860 pythttp-0.0.1/
--rw-rw-rw-   0        0        0     1093 2023-05-03 09:50:28.504356 pythttp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:51.000000 pythttp-0.0.1/README.md
--rw-rw-rw-   0        0        0      419 2023-05-03 09:49:12.000000 pythttp-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-03 09:50:28.504356 pythttp-0.0.1/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-03 09:50:28.000000 pythttp-0.0.1/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-03 09:50:28.000000 pythttp-0.0.1/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:50:28.000000 pythttp-0.0.1/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:50:28.000000 pythttp-0.0.1/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 09:50:28.505860 pythttp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-05-03 09:49:49.000000 pythttp-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:02:09.453462 pythttp-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-05-22 10:02:09.452461 pythttp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.2/README.md
+-rw-rw-rw-   0        0        0      419 2023-05-22 09:55:24.000000 pythttp-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-22 10:02:09.451460 pythttp-0.0.2/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-05-22 10:02:09.000000 pythttp-0.0.2/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-22 10:02:09.000000 pythttp-0.0.2/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:02:09.000000 pythttp-0.0.2/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:02:09.000000 pythttp-0.0.2/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:02:09.453462 pythttp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-05-22 09:55:14.000000 pythttp-0.0.2/setup.py
```

### Comparing `pythttp-0.0.1/PKG-INFO` & `pythttp-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.1/README.md` & `pythttp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.1/pythttp.egg-info/PKG-INFO` & `pythttp-0.0.2/pythttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.1/setup.py` & `pythttp-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.0.1",
+    version="0.0.2",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

