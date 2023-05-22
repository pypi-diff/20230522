# Comparing `tmp/srec-1.0.1.tar.gz` & `tmp/srec-1.1.tar.gz`

## Comparing `srec-1.0.1.tar` & `srec-1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 srec-1.0.1/setup.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 srec-1.0.1/srec/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 srec-1.0.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 srec-1.0.1/LICENSE
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 srec-1.0.1/README.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 srec-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 srec-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 srec-1.1/setup.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 srec-1.1/srec/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 srec-1.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 srec-1.1/LICENSE
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 srec-1.1/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 srec-1.1/pyproject.toml
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 srec-1.1/PKG-INFO
```

### Comparing `srec-1.0.1/setup.py` & `srec-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `srec-1.0.1/srec/__init__.py` & `srec-1.1/srec/__init__.py`

 * *Files identical despite different names*

### Comparing `srec-1.0.1/LICENSE` & `srec-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `srec-1.0.1/README.md` & `srec-1.1/README.md`

 * *Files identical despite different names*

### Comparing `srec-1.0.1/pyproject.toml` & `srec-1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "srec"
-version = "1.0.1"
+version = "1.1"
 authors = [
   { name="Trrrrw", email="wzhhenry@qq.com" },
 ]
 description = "A simple module to calculate the time required for leveling up in Honkai: Star rail."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `srec-1.0.1/PKG-INFO` & `srec-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srec
-Version: 1.0.1
+Version: 1.1
 Summary: A simple module to calculate the time required for leveling up in Honkai: Star rail.
 Project-URL: Homepage, https://github.com/Trrrrw/srec
 Project-URL: Bug Tracker, https://github.com/Trrrrw/srec/issues
 Author-email: Trrrrw <wzhhenry@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

