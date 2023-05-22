# Comparing `tmp/inmantals-1.3.0.tar.gz` & `tmp/inmantals-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmantals-1.3.0.tar", last modified: Fri Dec 23 08:21:25 2022, max compression
+gzip compressed data, was "inmantals-1.3.1.tar", last modified: Mon May 22 12:22:13 2023, max compression
```

## Comparing `inmantals-1.3.0.tar` & `inmantals-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-12-23 08:21:25.521663 inmantals-1.3.0/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10174 2022-12-23 08:21:07.000000 inmantals-1.3.0/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2316 2022-12-23 08:21:25.521663 inmantals-1.3.0/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1633 2022-12-23 08:21:07.000000 inmantals-1.3.0/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       73 2022-12-23 08:21:07.000000 inmantals-1.3.0/pyproject.toml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      525 2022-12-23 08:21:25.522663 inmantals-1.3.0/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1993 2022-12-23 08:21:18.000000 inmantals-1.3.0/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-12-23 08:21:25.519663 inmantals-1.3.0/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-12-23 08:21:25.520663 inmantals-1.3.0/src/inmantals/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2022-12-23 08:21:07.000000 inmantals-1.3.0/src/inmantals/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9695 2022-12-23 08:21:16.000000 inmantals-1.3.0/src/inmantals/jsonrpc.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3925 2022-12-23 08:21:07.000000 inmantals-1.3.0/src/inmantals/lsp_types.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1219 2022-12-23 08:21:07.000000 inmantals-1.3.0/src/inmantals/pipeserver.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    15227 2022-12-23 08:21:16.000000 inmantals-1.3.0/src/inmantals/server.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1178 2022-12-23 08:21:07.000000 inmantals-1.3.0/src/inmantals/tcpserver.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-12-23 08:21:25.521663 inmantals-1.3.0/src/inmantals.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2316 2022-12-23 08:21:25.000000 inmantals-1.3.0/src/inmantals.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      432 2022-12-23 08:21:25.000000 inmantals-1.3.0/src/inmantals.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2022-12-23 08:21:25.000000 inmantals-1.3.0/src/inmantals.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       73 2022-12-23 08:21:25.000000 inmantals-1.3.0/src/inmantals.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       26 2022-12-23 08:21:25.000000 inmantals-1.3.0/src/inmantals.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       10 2022-12-23 08:21:25.000000 inmantals-1.3.0/src/inmantals.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.010987 inmantals-1.3.1/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10174 2023-05-22 12:21:58.000000 inmantals-1.3.1/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2316 2023-05-22 12:22:13.010987 inmantals-1.3.1/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1633 2023-05-22 12:22:03.000000 inmantals-1.3.1/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       73 2023-05-22 12:21:58.000000 inmantals-1.3.1/pyproject.toml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      525 2023-05-22 12:22:13.011987 inmantals-1.3.1/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1993 2023-05-22 12:22:04.000000 inmantals-1.3.1/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.008987 inmantals-1.3.1/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.010987 inmantals-1.3.1/src/inmantals/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-05-22 12:21:58.000000 inmantals-1.3.1/src/inmantals/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9695 2023-05-22 12:22:03.000000 inmantals-1.3.1/src/inmantals/jsonrpc.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3925 2023-05-22 12:22:03.000000 inmantals-1.3.1/src/inmantals/lsp_types.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1219 2023-05-22 12:22:03.000000 inmantals-1.3.1/src/inmantals/pipeserver.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    15227 2023-05-22 12:22:03.000000 inmantals-1.3.1/src/inmantals/server.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1178 2023-05-22 12:21:58.000000 inmantals-1.3.1/src/inmantals/tcpserver.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.010987 inmantals-1.3.1/src/inmantals.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2316 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      452 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       73 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       26 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       10 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.010987 inmantals-1.3.1/tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11892 2023-05-22 12:22:03.000000 inmantals-1.3.1/tests/test_smoke.py
```

### Comparing `inmantals-1.3.0/LICENSE` & `inmantals-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/PKG-INFO` & `inmantals-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmantals
-Version: 1.3.0
+Version: 1.3.1
 Summary: Inmanta Language Server
 Home-page: https://github.com/inmanta/vscode-inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License
 Keywords: ide,language-server,vscode,inmanta
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inmantals-1.3.0/README.md` & `inmantals-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/setup.cfg` & `inmantals-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/setup.py` & `inmantals-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 setup(
     name="inmantals",
     package_dir={"": "src"},
     packages=find_packages("src"),
     install_requires=requires,
 
-    version="1.3.0",
+    version="1.3.1",
 
     description="Inmanta Language Server",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Inmanta",
     author_email="code@inmanta.com",
     license="Apache Software License",
```

### Comparing `inmantals-1.3.0/src/inmantals/__init__.py` & `inmantals-1.3.1/src/inmantals/__init__.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/src/inmantals/jsonrpc.py` & `inmantals-1.3.1/src/inmantals/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/src/inmantals/lsp_types.py` & `inmantals-1.3.1/src/inmantals/lsp_types.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/src/inmantals/pipeserver.py` & `inmantals-1.3.1/src/inmantals/pipeserver.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/src/inmantals/server.py` & `inmantals-1.3.1/src/inmantals/server.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/src/inmantals/tcpserver.py` & `inmantals-1.3.1/src/inmantals/tcpserver.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.0/src/inmantals.egg-info/PKG-INFO` & `inmantals-1.3.1/src/inmantals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmantals
-Version: 1.3.0
+Version: 1.3.1
 Summary: Inmanta Language Server
 Home-page: https://github.com/inmanta/vscode-inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License
 Keywords: ide,language-server,vscode,inmanta
 Classifier: Development Status :: 5 - Production/Stable
```

