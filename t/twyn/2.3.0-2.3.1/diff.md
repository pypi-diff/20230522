# Comparing `tmp/twyn-2.3.0.tar.gz` & `tmp/twyn-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twyn-2.3.0.tar", max compression
+gzip compressed data, was "twyn-2.3.1.tar", max compression
```

## Comparing `twyn-2.3.0.tar` & `twyn-2.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1081 2023-05-21 17:44:36.507727 twyn-2.3.0/LICENSE
--rw-r--r--   0        0        0     3441 2023-05-21 17:44:36.507727 twyn-2.3.0/README.md
--rw-r--r--   0        0        0     3183 2023-05-21 17:44:36.511727 twyn-2.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/base/__init__.py
--rw-r--r--   0        0        0      942 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/base/constants.py
--rw-r--r--   0        0        0      147 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/base/exceptions.py
--rw-r--r--   0        0        0     2331 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/cli.py
--rw-r--r--   0        0        0        0 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/core/__init__.py
--rw-r--r--   0        0        0     3298 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/core/config_handler.py
--rw-r--r--   0        0        0      513 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/core/exceptions.py
--rw-r--r--   0        0        0      221 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/dependency_parser/__init__.py
--rw-r--r--   0        0        0     1380 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/dependency_parser/abstract_parser.py
--rw-r--r--   0        0        0     2149 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/dependency_parser/dependency_selector.py
--rw-r--r--   0        0        0      554 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/dependency_parser/exceptions.py
--rw-r--r--   0        0        0      761 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/dependency_parser/poetry_lock.py
--rw-r--r--   0        0        0      804 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/dependency_parser/requirements_txt.py
--rw-r--r--   0        0        0     5114 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/main.py
--rw-r--r--   0        0        0        0 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/similarity/__init__.py
--rw-r--r--   0        0        0     2210 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/similarity/algorithm.py
--rw-r--r--   0        0        0      275 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/similarity/exceptions.py
--rw-r--r--   0        0        0      189 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/trusted_packages/__init__.py
--rw-r--r--   0        0        0     1497 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/trusted_packages/constants.py
--rw-r--r--   0        0        0      394 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/trusted_packages/exceptions.py
--rw-r--r--   0        0        0     2009 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/trusted_packages/references.py
--rw-r--r--   0        0        0     1907 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/trusted_packages/selectors.py
--rw-r--r--   0        0        0     2816 2023-05-21 17:44:36.511727 twyn-2.3.0/src/twyn/trusted_packages/trusted_packages.py
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 twyn-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-21 17:50:27.767567 twyn-2.3.1/LICENSE
+-rw-r--r--   0        0        0     3441 2023-05-21 17:50:27.767567 twyn-2.3.1/README.md
+-rw-r--r--   0        0        0     3191 2023-05-21 17:50:27.771566 twyn-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/base/__init__.py
+-rw-r--r--   0        0        0      942 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/base/constants.py
+-rw-r--r--   0        0        0      147 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/base/exceptions.py
+-rw-r--r--   0        0        0     2331 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/cli.py
+-rw-r--r--   0        0        0        0 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/core/__init__.py
+-rw-r--r--   0        0        0     3298 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/core/config_handler.py
+-rw-r--r--   0        0        0      513 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/core/exceptions.py
+-rw-r--r--   0        0        0      221 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/dependency_parser/__init__.py
+-rw-r--r--   0        0        0     1380 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/dependency_parser/abstract_parser.py
+-rw-r--r--   0        0        0     2149 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/dependency_parser/dependency_selector.py
+-rw-r--r--   0        0        0      554 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/dependency_parser/exceptions.py
+-rw-r--r--   0        0        0      761 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/dependency_parser/poetry_lock.py
+-rw-r--r--   0        0        0      804 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/dependency_parser/requirements_txt.py
+-rw-r--r--   0        0        0     5114 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/main.py
+-rw-r--r--   0        0        0        0 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/similarity/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/similarity/algorithm.py
+-rw-r--r--   0        0        0      275 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/similarity/exceptions.py
+-rw-r--r--   0        0        0      189 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/trusted_packages/__init__.py
+-rw-r--r--   0        0        0     1497 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/trusted_packages/constants.py
+-rw-r--r--   0        0        0      394 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/trusted_packages/exceptions.py
+-rw-r--r--   0        0        0     2009 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/trusted_packages/references.py
+-rw-r--r--   0        0        0     1907 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/trusted_packages/selectors.py
+-rw-r--r--   0        0        0     2816 2023-05-21 17:50:27.771566 twyn-2.3.1/src/twyn/trusted_packages/trusted_packages.py
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 twyn-2.3.1/PKG-INFO
```

### Comparing `twyn-2.3.0/LICENSE` & `twyn-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/README.md` & `twyn-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/pyproject.toml` & `twyn-2.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "twyn"
-version = "2.3.0"
+version = "2.3.1"
 description = ""
 authors = ["Daniel Sanz, Sergio Castillo, Ludo van Orden, Dmitrii Fedotov"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 requests = "^2.28.2"
 dparse = "^0.6.2"
 click = "^8.1.3"
 rich = "^13.3.1"
-rapidfuzz = "^2.13.7"
+rapidfuzz = ">=2.13.7,<4.0.0"
 pyparsing = "^3.0.9"
 tomlkit = "^0.11.6"
 
 
 [tool.poetry.scripts]
 twyn = "twyn.cli:entry_point"
 
@@ -95,15 +95,15 @@
 [tool.coverage.report]
 fail_under = 95
 exclude_lines = ["if TYPE_CHECKING:", "pragma: no cover"]
 
 
 [tool.commitizen]
 version_files = ["pyproject.toml:version"]
-version = "2.3.0"
+version = "2.3.1"
 tag_format = "v$version"
 name = "cz_customize"
 
 
 [tool.commitizen.customize]
 bump_pattern = "^(BREAKING[\\-\\ ]CHANGE|feat|fix|refactor|perf|ci|docs|style|test|chore|revert|build)(\\(.+\\))?(!)?"
 change_type_order = [
```

### Comparing `twyn-2.3.0/src/twyn/base/constants.py` & `twyn-2.3.1/src/twyn/base/constants.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/cli.py` & `twyn-2.3.1/src/twyn/cli.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/core/config_handler.py` & `twyn-2.3.1/src/twyn/core/config_handler.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/core/exceptions.py` & `twyn-2.3.1/src/twyn/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/dependency_parser/abstract_parser.py` & `twyn-2.3.1/src/twyn/dependency_parser/abstract_parser.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/dependency_parser/dependency_selector.py` & `twyn-2.3.1/src/twyn/dependency_parser/dependency_selector.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/dependency_parser/exceptions.py` & `twyn-2.3.1/src/twyn/dependency_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/dependency_parser/poetry_lock.py` & `twyn-2.3.1/src/twyn/dependency_parser/poetry_lock.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/dependency_parser/requirements_txt.py` & `twyn-2.3.1/src/twyn/dependency_parser/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/main.py` & `twyn-2.3.1/src/twyn/main.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/similarity/algorithm.py` & `twyn-2.3.1/src/twyn/similarity/algorithm.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/trusted_packages/constants.py` & `twyn-2.3.1/src/twyn/trusted_packages/constants.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/trusted_packages/references.py` & `twyn-2.3.1/src/twyn/trusted_packages/references.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/trusted_packages/selectors.py` & `twyn-2.3.1/src/twyn/trusted_packages/selectors.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/src/twyn/trusted_packages/trusted_packages.py` & `twyn-2.3.1/src/twyn/trusted_packages/trusted_packages.py`

 * *Files identical despite different names*

### Comparing `twyn-2.3.0/PKG-INFO` & `twyn-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: twyn
-Version: 2.3.0
+Version: 2.3.1
 Summary: 
 Author: Daniel Sanz, Sergio Castillo, Ludo van Orden, Dmitrii Fedotov
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dparse (>=0.6.2,<0.7.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
-Requires-Dist: rapidfuzz (>=2.13.7,<3.0.0)
+Requires-Dist: rapidfuzz (>=2.13.7,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
 Description-Content-Type: text/markdown
 
 # Twyn
```
