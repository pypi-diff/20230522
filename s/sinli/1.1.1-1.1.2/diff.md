# Comparing `tmp/sinli-1.1.1.tar.gz` & `tmp/sinli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinli-1.1.1.tar", last modified: Wed May  3 16:33:01 2023, max compression
+gzip compressed data, was "sinli-1.1.2.tar", last modified: Mon May 22 21:37:53 2023, max compression
```

## Comparing `sinli-1.1.1.tar` & `sinli-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    34449 2023-05-03 16:31:54.000000 sinli-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    44158 2023-05-03 16:33:01.105139 sinli-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3934 2023-05-03 16:31:54.000000 sinli-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-05-03 16:31:54.000000 sinli-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 16:33:01.105139 sinli-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-03 16:31:54.000000 sinli-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.097139 sinli-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/common/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/common/encoded_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/doctype/
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/doctype/envio/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/envio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/envio/v8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/doctype/factul/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/factul/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/factul/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/src/sinli/doctype/libros/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/libros/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4967 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/libros/v8.py
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/libros/v9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/src/sinli/doctype/mensaj/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/mensaj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/mensaj/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/src/sinli/doctype/pedido/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/pedido/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/pedido/v7.py
--rw-rw-rw-   0 root         (0) root         (0)     4639 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/document.py
--rw-rw-rw-   0 root         (0) root         (0)     7220 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    44158 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      753 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-03 16:31:54.000000 sinli-1.1.1/tests/test_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.510726 sinli-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34449 2023-05-22 21:37:43.000000 sinli-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    44158 2023-05-22 21:37:53.506726 sinli-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3934 2023-05-22 21:37:43.000000 sinli-1.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-05-22 21:37:43.000000 sinli-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 21:37:53.510726 sinli-1.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/common/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/common/encoded_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/envio/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/envio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/envio/v8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/factul/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/factul/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/factul/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/libros/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/libros/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4967 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/libros/v8.py
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/libros/v9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/mensaj/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/mensaj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/mensaj/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/pedido/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/pedido/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/pedido/v7.py
+-rw-rw-rw-   0 root         (0) root         (0)     4639 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     7220 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    44158 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-22 21:37:43.000000 sinli-1.1.2/tests/test_document.py
```

### Comparing `sinli-1.1.1/LICENSE` & `sinli-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/PKG-INFO` & `sinli-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.1
+Version: 1.1.2
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -663,15 +663,15 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SINLI
 
 ## Introduction and purpose
```

### Comparing `sinli-1.1.1/README.md` & `sinli-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/pyproject.toml` & `sinli-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "sinli"
-version = "1.1.1"
+version = "1.1.2"
 dependencies = [
     "typing-extensions==4.3.0",
     "pycountry==22.3.5"
 ]
 authors = [
     {name = "Devcontrol", email = "devcontrol@zici.fr"},
 ]
 description = "Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
 ]
 
 [tool.setuptools.packages.find]
```

### Comparing `sinli-1.1.1/src/sinli/common/encoded_values.py` & `sinli-1.1.2/src/sinli/common/encoded_values.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/doctype/__init__.py` & `sinli-1.1.2/src/sinli/doctype/__init__.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/doctype/envio/v8.py` & `sinli-1.1.2/src/sinli/doctype/envio/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/doctype/factul/v1.py` & `sinli-1.1.2/src/sinli/doctype/factul/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/doctype/libros/v8.py` & `sinli-1.1.2/src/sinli/doctype/libros/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/doctype/libros/v9.py` & `sinli-1.1.2/src/sinli/doctype/libros/v9.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/doctype/mensaj/v1.py` & `sinli-1.1.2/src/sinli/doctype/mensaj/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/doctype/pedido/v7.py` & `sinli-1.1.2/src/sinli/doctype/pedido/v7.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/document.py` & `sinli-1.1.2/src/sinli/document.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli/line.py` & `sinli-1.1.2/src/sinli/line.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.1/src/sinli.egg-info/PKG-INFO` & `sinli-1.1.2/src/sinli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.1
+Version: 1.1.2
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -663,15 +663,15 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SINLI
 
 ## Introduction and purpose
```

### Comparing `sinli-1.1.1/src/sinli.egg-info/SOURCES.txt` & `sinli-1.1.2/src/sinli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 src/sinli/__init__.py
 src/sinli/document.py
 src/sinli/line.py
 src/sinli.egg-info/PKG-INFO
 src/sinli.egg-info/SOURCES.txt
 src/sinli.egg-info/dependency_links.txt
 src/sinli.egg-info/requires.txt
```

