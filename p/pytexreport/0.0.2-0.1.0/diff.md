# Comparing `tmp/pytexreport-0.0.2.tar.gz` & `tmp/pytexreport-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytexreport-0.0.2.tar", max compression
+gzip compressed data, was "pytexreport-0.1.0.tar", max compression
```

## Comparing `pytexreport-0.0.2.tar` & `pytexreport-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,15 @@
--rw-r--r--   0        0        0     2867 2023-05-21 23:24:14.220839 pytexreport-0.0.2/README.md
--rw-r--r--   0        0        0     2130 2023-05-21 23:24:14.220839 pytexreport-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-21 23:24:14.220839 pytexreport-0.0.2/src/pytexreport/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 23:24:14.220839 pytexreport-0.0.2/src/pytexreport/py.typed
--rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 pytexreport-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2867 2023-05-22 00:11:22.842595 pytexreport-0.1.0/README.md
+-rw-r--r--   0        0        0     2222 2023-05-22 00:11:22.846595 pytexreport-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/py.typed
+-rw-r--r--   0        0        0    10563 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/pytexreport.py
+-rw-r--r--   0        0        0        0 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/basicHomework/__init__.py
+-rw-r--r--   0        0        0     2010 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/basicHomework/basicHomework.cls
+-rw-r--r--   0        0        0     1366 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/basicHomework/basicHomework.py
+-rw-r--r--   0        0        0       37 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/basicReport/__init__.py
+-rw-r--r--   0        0        0     6711 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/basicReport/basicReport.py
+-rw-r--r--   0        0        0       43 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/ieeeConference/__init__.py
+-rw-r--r--   0        0        0   281786 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/ieeeConference/ieeeConference.cls
+-rw-r--r--   0        0        0     3582 2023-05-22 00:11:22.846595 pytexreport-0.1.0/src/pytexreport/style/ieeeConference/ieeeConference.py
+-rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 pytexreport-0.1.0/PKG-INFO
```

### Comparing `pytexreport-0.0.2/README.md` & `pytexreport-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pytexreport-0.0.2/pyproject.toml` & `pytexreport-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytexreport"
-version = "0.0.2"
+version = "0.1.0"
 description = "A short description of the project"
 authors = [
     "nkalis <n.kalis98@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -26,15 +26,19 @@
 ]
 
 packages = [
     { include = "pytexreport", from = "src" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7.1, <4.0"
+python = ">=3.8, <3.11"
+latexify-py = "^0.2.0"
+matplotlib = "^3.7.1"
+loguru = "^0.7.0"
+pylatex = "^1.4.1"
 
 [tool.poetry.dev-dependencies]
 autoflake = "*"
 black = "*"
 flake8 = "*"
 flake8-bugbear = "*"
 flake8-builtins = "*"
@@ -51,25 +55,26 @@
 pymdown-extensions = "*"
 pytest = "*"
 pytest-github-actions-annotate-failures = "*"
 pytest-cov = "*"
 python-kacl = "*"
 pyupgrade = "*"
 tryceratops = "*"
+urllib3 = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 src_paths = ["src", "tests"]
 
 [tool.black]
-target-version = ["py37", "py38", "py39"]
+target-version = ["py38", "py39"]
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """\
     --cov pytexreport \
     --cov tests \
     --cov-report term-missing \
```

### Comparing `pytexreport-0.0.2/PKG-INFO` & `pytexreport-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: pytexreport
-Version: 0.0.2
+Version: 0.1.0
 Summary: A short description of the project
 Home-page: https://nkalis.github.io/pytexreport
 License: MIT
 Author: nkalis
 Author-email: n.kalis98@gmail.com
-Requires-Python: >=3.7.1,<4.0
+Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires-Dist: latexify-py (>=0.2.0,<0.3.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: pylatex (>=1.4.1,<2.0.0)
 Project-URL: Documentation, https://nkalis.github.io/pytexreport
 Project-URL: Repository, https://github.com/nkalis/pytexreport
 Description-Content-Type: text/markdown
 
 # pytexreport
 
 [![PyPI](https://img.shields.io/pypi/v/pytexreport?style=flat-square)](https://pypi.python.org/pypi/pytexreport/)
```

