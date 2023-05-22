# Comparing `tmp/flask_matomo2-0.2.1.tar.gz` & `tmp/flask_matomo2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_matomo2-0.2.1.tar", max compression
+gzip compressed data, was "flask_matomo2-0.2.6.tar", max compression
```

## Comparing `flask_matomo2-0.2.1.tar` & `flask_matomo2-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-05-15 10:56:36.633278 flask_matomo2-0.2.1/LICENSE
--rw-r--r--   0        0        0     4491 2023-05-22 08:28:32.297042 flask_matomo2-0.2.1/README.md
--rw-r--r--   0        0        0      114 2023-05-22 08:27:37.428989 flask_matomo2-0.2.1/flask_matomo2/__init__.py
--rw-r--r--   0        0        0     8650 2023-05-22 08:31:03.560264 flask_matomo2-0.2.1/flask_matomo2/core.py
--rw-r--r--   0        0        0     1250 2023-05-22 08:32:23.265051 flask_matomo2-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5628 1970-01-01 00:00:00.000000 flask_matomo2-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4756 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/README.md
+-rw-r--r--   0        0        0      114 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/flask_matomo2/__init__.py
+-rw-r--r--   0        0        0     8650 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/flask_matomo2/core.py
+-rw-r--r--   0        0        0     1250 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     5893 1970-01-01 00:00:00.000000 flask_matomo2-0.2.6/PKG-INFO
```

### Comparing `flask_matomo2-0.2.1/LICENSE` & `flask_matomo2-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_matomo2-0.2.1/README.md` & `flask_matomo2-0.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,38 @@
 
 Flask-Matomo is a library which lets you track the requests of your Flask website using Matomo (Piwik).
 
 Forked from [LucasHild/flask-matomo](https://github.com/LucasHild/flask-matomo).
 ## Installation
 
 ```
-pip install flask-matomo
+pip install flask-matomo2
+```
+
+## Using flask-matomo2 in your project
+
+Simply add `flask-matomo2` to your dependencies:
+
+```toml
+# pyproject.toml
+dependencies = [
+  "flask-matomo2",
+]
+
+```
+### Using Poetry
+
+```bash
+poetry add flask-matomo2
+```
+
+### Using PDM
+
+```bash
+pdm add flask-matomo2
 ```
 
 ## Usage
 
 ```python
 from flask import Flask, jsonify
 from flask_matomo2 import Matomo
```

### Comparing `flask_matomo2-0.2.1/flask_matomo2/core.py` & `flask_matomo2-0.2.6/flask_matomo2/core.py`

 * *Files identical despite different names*

### Comparing `flask_matomo2-0.2.1/pyproject.toml` & `flask_matomo2-0.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-matomo2"
-version = "0.2.1"
+version = "0.2.6"
 description = "Track requests to your Flask server with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "flask_matomo2"}]
 classifiers=[
     "Environment :: Web Environment",
```

### Comparing `flask_matomo2-0.2.1/PKG-INFO` & `flask_matomo2-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-matomo2
-Version: 0.2.1
+Version: 0.2.6
 Summary: Track requests to your Flask server with Matomo
 Home-page: https://spraakbanken.gu.se
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
@@ -33,15 +33,38 @@
 
 Flask-Matomo is a library which lets you track the requests of your Flask website using Matomo (Piwik).
 
 Forked from [LucasHild/flask-matomo](https://github.com/LucasHild/flask-matomo).
 ## Installation
 
 ```
-pip install flask-matomo
+pip install flask-matomo2
+```
+
+## Using flask-matomo2 in your project
+
+Simply add `flask-matomo2` to your dependencies:
+
+```toml
+# pyproject.toml
+dependencies = [
+  "flask-matomo2",
+]
+
+```
+### Using Poetry
+
+```bash
+poetry add flask-matomo2
+```
+
+### Using PDM
+
+```bash
+pdm add flask-matomo2
 ```
 
 ## Usage
 
 ```python
 from flask import Flask, jsonify
 from flask_matomo2 import Matomo
```

