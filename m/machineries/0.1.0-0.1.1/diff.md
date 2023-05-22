# Comparing `tmp/machineries-0.1.0.tar.gz` & `tmp/machineries-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineries-0.1.0.tar", max compression
+gzip compressed data, was "machineries-0.1.1.tar", max compression
```

## Comparing `machineries-0.1.0.tar` & `machineries-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1092 2023-05-22 17:52:19.655144 machineries-0.1.0/LICENSE
--rw-r--r--   0        0        0       59 2023-05-22 17:56:45.457885 machineries-0.1.0/machineries/__init__.py
--rw-r--r--   0        0        0      137 2023-05-22 17:57:49.668326 machineries-0.1.0/machineries/main.py
--rw-r--r--   0        0        0      512 2023-05-22 18:25:13.079261 machineries-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-05-22 18:25:04.999910 machineries-0.1.0/README.md
--rw-r--r--   0        0        0      645 2023-05-22 18:25:24.738639 machineries-0.1.0/setup.py
--rw-r--r--   0        0        0      773 2023-05-22 18:25:24.738639 machineries-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-22 18:45:41.510088 machineries-0.1.1/LICENSE
+-rw-r--r--   0        0        0       66 2023-05-22 18:45:41.510088 machineries-0.1.1/README.md
+-rw-r--r--   0        0        0       58 2023-05-22 18:45:41.514088 machineries-0.1.1/machineries/__init__.py
+-rw-r--r--   0        0        0      532 2023-05-22 18:45:41.514088 machineries-0.1.1/machineries/machine.py
+-rw-r--r--   0        0        0      132 2023-05-22 18:45:41.514088 machineries-0.1.1/machineries/main.py
+-rw-r--r--   0        0        0      489 2023-05-22 18:45:41.514088 machineries-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 machineries-0.1.1/PKG-INFO
```

### Comparing `machineries-0.1.0/PKG-INFO` & `machineries-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: machineries
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python framework for controlling machines
 Home-page: https://github.com/tadnir/machineries
 License: MIT
 Author: michael tadnir
 Author-email: tadnir50@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/tadnir/machineries
 Description-Content-Type: text/markdown
 
 # Machineries
 Python framework for controlling different machines
```

