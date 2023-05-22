# Comparing `tmp/ffdice-1.0.2.tar.gz` & `tmp/ffdice-1.1.0.tar.gz`

## Comparing `ffdice-1.0.2.tar` & `ffdice-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ffdice-1.0.2/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ffdice-1.0.2/__init__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 ffdice-1.0.2/examples/basic/README.md
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ffdice-1.0.2/examples/basic/__main__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ffdice-1.0.2/examples/colors/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 ffdice-1.0.2/examples/colors/__main__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ffdice-1.0.2/examples/sensehat/README.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 ffdice-1.0.2/examples/sensehat/__main__.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 ffdice-1.0.2/examples/sensehat/matrix.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ffdice-1.0.2/ffdice/Dice.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ffdice-1.0.2/ffdice/RNG.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ffdice-1.0.2/ffdice/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ffdice-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ffdice-1.0.2/tests/test_dice.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 ffdice-1.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ffdice-1.0.2/LICENSE
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ffdice-1.0.2/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ffdice-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 ffdice-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ffdice-1.1.0/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ffdice-1.1.0/__init__.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 ffdice-1.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 ffdice-1.1.0/examples/basic/README.md
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ffdice-1.1.0/examples/basic/__main__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ffdice-1.1.0/examples/colors/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 ffdice-1.1.0/examples/colors/__main__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ffdice-1.1.0/examples/sensehat/README.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 ffdice-1.1.0/examples/sensehat/__main__.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 ffdice-1.1.0/examples/sensehat/matrix.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ffdice-1.1.0/ffdice/Dice.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ffdice-1.1.0/ffdice/RNG.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ffdice-1.1.0/ffdice/__about__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ffdice-1.1.0/ffdice/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ffdice-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ffdice-1.1.0/tests/test_dice.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 ffdice-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ffdice-1.1.0/LICENSE
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ffdice-1.1.0/README.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 ffdice-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 ffdice-1.1.0/PKG-INFO
```

### Comparing `ffdice-1.0.2/examples/sensehat/README.md` & `ffdice-1.1.0/examples/sensehat/README.md`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/examples/sensehat/__main__.py` & `ffdice-1.1.0/examples/sensehat/__main__.py`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/examples/sensehat/matrix.py` & `ffdice-1.1.0/examples/sensehat/matrix.py`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/ffdice/Dice.py` & `ffdice-1.1.0/ffdice/Dice.py`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/ffdice/RNG.py` & `ffdice-1.1.0/ffdice/RNG.py`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/tests/test_dice.py` & `ffdice-1.1.0/tests/test_dice.py`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/.gitignore` & `ffdice-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/LICENSE` & `ffdice-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/README.md` & `ffdice-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ffdice-1.0.2/pyproject.toml` & `ffdice-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [project]
 name = "ffdice"
-version = "1.0.2"
+dynamic = [
+  "version"
+]
 authors = [
   { name="FrisFruitig", email="info@frisfruitig.com" },
 ]
 description = "A basic random number generator (RNG) that can be used for multiple purposes, such as rolling dice."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[tool.hatch.version]
+path = "ffdice/__about__.py"
+
 [project.urls]
 "Homepage" = "https://github.com/frisfruitig/ffdice"
 "Bug Tracker" = "https://github.com/frisfruitig/ffdice/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `ffdice-1.0.2/PKG-INFO` & `ffdice-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffdice
-Version: 1.0.2
+Version: 1.1.0
 Summary: A basic random number generator (RNG) that can be used for multiple purposes, such as rolling dice.
 Project-URL: Homepage, https://github.com/frisfruitig/ffdice
 Project-URL: Bug Tracker, https://github.com/frisfruitig/ffdice/issues
 Author-email: FrisFruitig <info@frisfruitig.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

