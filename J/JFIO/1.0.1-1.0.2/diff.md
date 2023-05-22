# Comparing `tmp/JFIO-1.0.1.tar.gz` & `tmp/JFIO-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JFIO-1.0.1.tar", last modified: Tue May  2 12:48:04 2023, max compression
+gzip compressed data, was "JFIO-1.0.2.tar", last modified: Mon May 22 12:29:14 2023, max compression
```

## Comparing `JFIO-1.0.1.tar` & `JFIO-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:48:04.082687 JFIO-1.0.1/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:48:04.078687 JFIO-1.0.1/JFIO/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:48:04.082687 JFIO-1.0.1/JFIO/ThirdParty/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-02 10:17:16.000000 JFIO-1.0.1/JFIO/ThirdParty/json.hpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-02 10:05:00.000000 JFIO-1.0.1/JFIO/ThirdParty/pybind11_json.hpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      264 2023-05-02 12:25:30.000000 JFIO-1.0.1/JFIO/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:48:04.082687 JFIO-1.0.1/JFIO/read/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:11:30.000000 JFIO-1.0.1/JFIO/read/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      585 2023-05-02 12:11:18.000000 JFIO-1.0.1/JFIO/read/readJSONFromFile.cpp
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:48:04.082687 JFIO-1.0.1/JFIO/write/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:19:03.000000 JFIO-1.0.1/JFIO/write/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1903 2023-05-02 11:24:46.000000 JFIO-1.0.1/JFIO/write/writeJSON2File.cpp
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:48:04.078687 JFIO-1.0.1/JFIO.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3361 2023-05-02 12:48:04.000000 JFIO-1.0.1/JFIO.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      347 2023-05-02 12:48:04.000000 JFIO-1.0.1/JFIO.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-02 12:48:04.000000 JFIO-1.0.1/JFIO.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        5 2023-05-02 12:48:04.000000 JFIO-1.0.1/JFIO.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-02 09:50:08.000000 JFIO-1.0.1/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      153 2023-05-02 12:46:51.000000 JFIO-1.0.1/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3361 2023-05-02 12:48:04.082687 JFIO-1.0.1/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2617 2023-05-02 12:38:28.000000 JFIO-1.0.1/README.md
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      879 2023-05-02 12:47:52.000000 JFIO-1.0.1/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-02 12:48:04.082687 JFIO-1.0.1/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      786 2023-05-02 12:13:12.000000 JFIO-1.0.1/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-22 12:29:14.875863 JFIO-1.0.2/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-22 12:29:14.875863 JFIO-1.0.2/JFIO/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-22 12:29:14.875863 JFIO-1.0.2/JFIO/ThirdParty/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-02 10:17:16.000000 JFIO-1.0.2/JFIO/ThirdParty/json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-02 10:05:00.000000 JFIO-1.0.2/JFIO/ThirdParty/pybind11_json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      264 2023-05-02 12:25:30.000000 JFIO-1.0.2/JFIO/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-22 12:29:14.875863 JFIO-1.0.2/JFIO/read/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:11:30.000000 JFIO-1.0.2/JFIO/read/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      585 2023-05-02 12:11:18.000000 JFIO-1.0.2/JFIO/read/readJSONFromFile.cpp
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-22 12:29:14.875863 JFIO-1.0.2/JFIO/write/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:19:03.000000 JFIO-1.0.2/JFIO/write/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1878 2023-05-22 12:26:06.000000 JFIO-1.0.2/JFIO/write/writeJSON2File.cpp
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-22 12:29:14.875863 JFIO-1.0.2/JFIO.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3361 2023-05-22 12:29:14.000000 JFIO-1.0.2/JFIO.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      347 2023-05-22 12:29:14.000000 JFIO-1.0.2/JFIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-22 12:29:14.000000 JFIO-1.0.2/JFIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        5 2023-05-22 12:29:14.000000 JFIO-1.0.2/JFIO.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-02 09:50:08.000000 JFIO-1.0.2/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      153 2023-05-02 12:46:51.000000 JFIO-1.0.2/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3361 2023-05-22 12:29:14.875863 JFIO-1.0.2/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2617 2023-05-02 12:38:28.000000 JFIO-1.0.2/README.md
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      879 2023-05-22 12:26:48.000000 JFIO-1.0.2/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-22 12:29:14.875863 JFIO-1.0.2/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      786 2023-05-02 12:13:12.000000 JFIO-1.0.2/setup.py
```

### Comparing `JFIO-1.0.1/JFIO/ThirdParty/json.hpp` & `JFIO-1.0.2/JFIO/ThirdParty/json.hpp`

 * *Files identical despite different names*

### Comparing `JFIO-1.0.1/JFIO/ThirdParty/pybind11_json.hpp` & `JFIO-1.0.2/JFIO/ThirdParty/pybind11_json.hpp`

 * *Files identical despite different names*

### Comparing `JFIO-1.0.1/JFIO/read/readJSONFromFile.cpp` & `JFIO-1.0.2/JFIO/read/readJSONFromFile.cpp`

 * *Files identical despite different names*

### Comparing `JFIO-1.0.1/JFIO/write/writeJSON2File.cpp` & `JFIO-1.0.2/JFIO/write/writeJSON2File.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
       if (c == '[' and prevC == ':' and nextC == '['){
         out << c << '\n' << currentIndent ;
         written = true;
       }
 
       if (c == ']' and nextC == '}'){
-        out << '\n' << currentIndent << c ;
+        out << c ;
         written = true;
       }
 
       if (c == '{'){
         out << c << '\n' << currentIndent ;
         written = true;
       }
```

### Comparing `JFIO-1.0.1/JFIO.egg-info/PKG-INFO` & `JFIO-1.0.2/JFIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JFIO
-Version: 1.0.1
+Version: 1.0.2
 Summary: JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files.
 Home-page: https://github.com/PabloIbannez/JFIO
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JFIO-1.0.1/LICENSE` & `JFIO-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `JFIO-1.0.1/PKG-INFO` & `JFIO-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JFIO
-Version: 1.0.1
+Version: 1.0.2
 Summary: JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files.
 Home-page: https://github.com/PabloIbannez/JFIO
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JFIO-1.0.1/README.md` & `JFIO-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `JFIO-1.0.1/pyproject.toml` & `JFIO-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-cuda-cpp", "setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="JFIO"
-version="1.0.1"
+version="1.0.2"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text = "MIT License"}
```

### Comparing `JFIO-1.0.1/setup.py` & `JFIO-1.0.2/setup.py`

 * *Files identical despite different names*

