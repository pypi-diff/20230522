# Comparing `tmp/natalify-2.2.tar.gz` & `tmp/natalify-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natalify-2.2.tar", last modified: Mon May 22 11:17:50 2023, max compression
+gzip compressed data, was "natalify-2.4.tar", last modified: Mon May 22 11:29:39 2023, max compression
```

## Comparing `natalify-2.2.tar` & `natalify-2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 11:17:50.957840 natalify-2.2/
--rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-2.2/LICENSE
--rw-rw-rw-   0        0        0     2154 2023-05-22 11:17:50.957840 natalify-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1655 2023-05-22 11:17:27.000000 natalify-2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 11:17:50.942216 natalify-2.2/natalify/
--rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-2.2/natalify/__init__.py
--rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-2.2/natalify/__main__.py
--rw-rw-rw-   0        0        0    63371 2023-05-22 10:12:00.000000 natalify-2.2/natalify/natalify.py
-drwxrwxrwx   0        0        0        0 2023-05-22 11:17:50.957840 natalify-2.2/natalify.egg-info/
--rw-rw-rw-   0        0        0     2154 2023-05-22 11:17:50.000000 natalify-2.2/natalify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-22 11:17:50.000000 natalify-2.2/natalify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 11:17:50.000000 natalify-2.2/natalify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-22 11:17:50.000000 natalify-2.2/natalify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 11:17:50.000000 natalify-2.2/natalify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 11:17:50.957840 natalify-2.2/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-22 11:17:41.000000 natalify-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 11:29:39.131970 natalify-2.4/
+-rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-2.4/LICENSE
+-rw-rw-rw-   0        0        0     2163 2023-05-22 11:29:39.131970 natalify-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1664 2023-05-22 11:28:41.000000 natalify-2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 11:29:39.100722 natalify-2.4/natalify/
+-rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-2.4/natalify/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-2.4/natalify/__main__.py
+-rw-rw-rw-   0        0        0    63371 2023-05-22 10:12:00.000000 natalify-2.4/natalify/natalify.py
+drwxrwxrwx   0        0        0        0 2023-05-22 11:29:39.116346 natalify-2.4/natalify.egg-info/
+-rw-rw-rw-   0        0        0     2163 2023-05-22 11:29:39.000000 natalify-2.4/natalify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-22 11:29:39.000000 natalify-2.4/natalify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 11:29:39.000000 natalify-2.4/natalify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-22 11:29:39.000000 natalify-2.4/natalify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 11:29:39.000000 natalify-2.4/natalify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 11:29:39.131970 natalify-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-22 11:29:34.000000 natalify-2.4/setup.py
```

### Comparing `natalify-2.2/LICENSE` & `natalify-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `natalify-2.2/PKG-INFO` & `natalify-2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 2.2
+Version: 2.4
 Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -60,18 +60,19 @@
 ```python
 import natalify
 
 natalify.start()
 
 ```
 
-License
+## License
 Natalify is released under the GNU General Public License v3.0 (GPL-3.0).
 
 Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
 
-Contact
+## Contact
+
 For any inquiries or feedback, please contact the author:
 
-Name: Jack
+Name: Jack.
 Email: kinginjack@gmail.com
```

### Comparing `natalify-2.2/README.md` & `natalify-2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,18 +45,19 @@
 ```python
 import natalify
 
 natalify.start()
 
 ```
 
-License
+## License
 Natalify is released under the GNU General Public License v3.0 (GPL-3.0).
 
 Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
 
-Contact
+## Contact
+
 For any inquiries or feedback, please contact the author:
 
-Name: Jack
+Name: Jack.
 Email: kinginjack@gmail.com
```

### Comparing `natalify-2.2/natalify/natalify.py` & `natalify-2.4/natalify/natalify.py`

 * *Files identical despite different names*

### Comparing `natalify-2.2/natalify.egg-info/PKG-INFO` & `natalify-2.4/natalify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 2.2
+Version: 2.4
 Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -60,18 +60,19 @@
 ```python
 import natalify
 
 natalify.start()
 
 ```
 
-License
+## License
 Natalify is released under the GNU General Public License v3.0 (GPL-3.0).
 
 Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
 
-Contact
+## Contact
+
 For any inquiries or feedback, please contact the author:
 
-Name: Jack
+Name: Jack.
 Email: kinginjack@gmail.com
```

### Comparing `natalify-2.2/setup.py` & `natalify-2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='natalify',
-    version='2.2',
+    version='2.4',
     packages=setuptools.find_packages(),
     license='GPL-3.0',
     author='jack',
     author_email='kinginjack@gmail.com',
     description='A simple automation software for various tasks',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

