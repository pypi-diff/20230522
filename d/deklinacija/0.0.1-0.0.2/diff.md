# Comparing `tmp/deklinacija-0.0.1.tar.gz` & `tmp/deklinacija-0.0.2.tar.gz`

## Comparing `deklinacija-0.0.1.tar` & `deklinacija-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 deklinacija-0.0.1/deklinacija/__init__.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 deklinacija-0.0.1/deklinacija/module.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 deklinacija-0.0.1/deklinacija/utils.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-0.0.1/LICENSE
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 deklinacija-0.0.1/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 deklinacija-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 deklinacija-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-0.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 deklinacija-0.0.2/deklinacija/__init__.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 deklinacija-0.0.2/deklinacija/module.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 deklinacija-0.0.2/deklinacija/utils.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 deklinacija-0.0.2/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 deklinacija-0.0.2/PKG-INFO
```

### Comparing `deklinacija-0.0.1/deklinacija/module.py` & `deklinacija-0.0.2/deklinacija/module.py`

 * *Files identical despite different names*

### Comparing `deklinacija-0.0.1/deklinacija/utils.py` & `deklinacija-0.0.2/deklinacija/utils.py`

 * *Files identical despite different names*

### Comparing `deklinacija-0.0.1/LICENSE` & `deklinacija-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-0.0.1/README.md` & `deklinacija-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-# deklinacija-imena
-A Python library for declension of personal names in Serbian, Croatian and Bosnian.
+# deklinacija
+A Python library for declension of personal names in Serbian. The  grammatical rules utlized in this library also apply to Croatian and Bosnian.
 
+## Installation
+The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
+
+The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/).
+```properties
+pip install deklinacija
+```
 ## Usage
 Simply `import` the package. It is recommended to set the alias to `dek`.
 
 ```python
 import deklinacija as dek
 ```
-**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. There is also the third `latin` parameter, which indicates whether the provided `name` parameter is written in Cyrillic or Latin script. **Currently, only Latin script is supported.**
+**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. There is also the third `latin` parameter, which indicates whether the provided `name` parameter is written in the Cyrillic or Latin script. **Currently, only the Latin script is supported.**
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
 
 changedName1 = dek.genitiv("Velja","male") #Velje
 changedName2 = dek.dativ("Petar","male") #Petru
@@ -35,8 +42,8 @@
 print("Dali ste poklon",Nikola['dativ']) #Dali ste poklon Nikoli - Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
 - The vocative case
 - Support for both Latin and Cyrillic scripts
-- Declension of last names
+- Declension of last names
```

### Comparing `deklinacija-0.0.1/pyproject.toml` & `deklinacija-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/urelja/deklinacija-imena"
-"Bug Tracker" = "https://github.com/urelja/deklinacija-imena/issues"
+"Homepage" = "https://github.com/urelja/deklinacija"
+"Bug Tracker" = "https://github.com/urelja/deklinacija/issues"
```

### Comparing `deklinacija-0.0.1/PKG-INFO` & `deklinacija-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for declension of personal names in Serbian
-Project-URL: Homepage, https://github.com/urelja/deklinacija-imena
-Project-URL: Bug Tracker, https://github.com/urelja/deklinacija-imena/issues
+Project-URL: Homepage, https://github.com/urelja/deklinacija
+Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# deklinacija-imena
-A Python library for declension of personal names in Serbian, Croatian and Bosnian.
+# deklinacija
+A Python library for declension of personal names in Serbian. The  grammatical rules utlized in this library also apply to Croatian and Bosnian.
 
+## Installation
+The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
+
+The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/).
+```properties
+pip install deklinacija
+```
 ## Usage
 Simply `import` the package. It is recommended to set the alias to `dek`.
 
 ```python
 import deklinacija as dek
 ```
-**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. There is also the third `latin` parameter, which indicates whether the provided `name` parameter is written in Cyrillic or Latin script. **Currently, only Latin script is supported.**
+**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. There is also the third `latin` parameter, which indicates whether the provided `name` parameter is written in the Cyrillic or Latin script. **Currently, only the Latin script is supported.**
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
 
 changedName1 = dek.genitiv("Velja","male") #Velje
 changedName2 = dek.dativ("Petar","male") #Petru
@@ -49,8 +56,8 @@
 print("Dali ste poklon",Nikola['dativ']) #Dali ste poklon Nikoli - Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
 - The vocative case
 - Support for both Latin and Cyrillic scripts
-- Declension of last names
+- Declension of last names
```

