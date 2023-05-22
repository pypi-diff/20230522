# Comparing `tmp/pydantic_tools-0.1.0.tar.gz` & `tmp/pydantic_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_tools-0.1.0.tar", last modified: Mon May 22 00:10:08 2023, max compression
+gzip compressed data, was "pydantic_tools-0.2.0.tar", last modified: Mon May 22 13:48:53 2023, max compression
```

## Comparing `pydantic_tools-0.1.0.tar` & `pydantic_tools-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1326 2023-05-21 14:02:10.710540 pydantic_tools-0.1.0/README.md
--rw-r--r--   0        0        0      735 2023-05-22 00:10:08.321851 pydantic_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-20 15:34:52.102521 pydantic_tools-0.1.0/src/alias/__init__.py
--rw-r--r--   0        0        0      181 2023-05-21 13:36:01.963863 pydantic_tools-0.1.0/src/i18n/__init__.py
--rw-r--r--   0        0        0     1881 2023-05-21 14:06:01.710783 pydantic_tools-0.1.0/src/i18n/__main__.py
--rw-r--r--   0        0        0        0 2023-05-20 03:41:40.806311 pydantic_tools-0.1.0/src/i18n/locales/__init__.py
--rw-r--r--   0        0        0     6932 2023-05-20 15:56:43.387030 pydantic_tools-0.1.0/src/i18n/locales/zh_cn.py
--rw-r--r--   0        0        0      897 2023-05-21 13:36:02.037013 pydantic_tools-0.1.0/src/i18n/model.py
--rw-r--r--   0        0        0     1267 2023-05-21 13:36:10.764355 pydantic_tools-0.1.0/src/i18n/templates.py
--rw-r--r--   0        0        0     1676 2023-05-21 07:26:37.197197 pydantic_tools-0.1.0/src/i18n/translate.py
--rw-r--r--   0        0        0     2597 2023-05-21 13:36:02.095934 pydantic_tools-0.1.0/tests/test_i18n.py
--rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 pydantic_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1326 2023-05-21 14:02:10.710540 pydantic_tools-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 13:35:56.162801 pydantic_tools-0.2.0/pydantic_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:34:52.102521 pydantic_tools-0.2.0/pydantic_tools/alias/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-21 13:36:01.963863 pydantic_tools-0.2.0/pydantic_tools/i18n/__init__.py
+-rw-r--r--   0        0        0     1881 2023-05-21 14:06:01.710783 pydantic_tools-0.2.0/pydantic_tools/i18n/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-20 03:41:40.806311 pydantic_tools-0.2.0/pydantic_tools/i18n/locales/__init__.py
+-rw-r--r--   0        0        0     6932 2023-05-20 15:56:43.387030 pydantic_tools-0.2.0/pydantic_tools/i18n/locales/zh_cn.py
+-rw-r--r--   0        0        0      897 2023-05-21 13:36:02.037013 pydantic_tools-0.2.0/pydantic_tools/i18n/model.py
+-rw-r--r--   0        0        0     1267 2023-05-21 13:36:10.764355 pydantic_tools-0.2.0/pydantic_tools/i18n/templates.py
+-rw-r--r--   0        0        0     1676 2023-05-21 07:26:37.197197 pydantic_tools-0.2.0/pydantic_tools/i18n/translate.py
+-rw-r--r--   0        0        0      735 2023-05-22 13:48:53.659571 pydantic_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2597 2023-05-21 13:36:02.095934 pydantic_tools-0.2.0/tests/test_i18n.py
+-rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 pydantic_tools-0.2.0/PKG-INFO
```

### Comparing `pydantic_tools-0.1.0/README.md` & `pydantic_tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.1.0/pyproject.toml` & `pydantic_tools-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "pydantic-tools"
-version = "0.1.0"
+name = "pydantic_tools"
+version = "0.2.0"
 description = "Useful tools for pydantic"
 authors = [
     { name = "icebear", email = "iiiicebeaaaar@gmail.com" },
 ]
 dependencies = [
     "pydantic>=1.10.7",
     "pytest>=7.3.1",
```

### Comparing `pydantic_tools-0.1.0/src/i18n/__main__.py` & `pydantic_tools-0.2.0/pydantic_tools/i18n/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.1.0/src/i18n/locales/zh_cn.py` & `pydantic_tools-0.2.0/pydantic_tools/i18n/locales/zh_cn.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.1.0/src/i18n/model.py` & `pydantic_tools-0.2.0/pydantic_tools/i18n/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.1.0/src/i18n/templates.py` & `pydantic_tools-0.2.0/pydantic_tools/i18n/templates.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.1.0/src/i18n/translate.py` & `pydantic_tools-0.2.0/pydantic_tools/i18n/translate.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.1.0/tests/test_i18n.py` & `pydantic_tools-0.2.0/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.1.0/PKG-INFO` & `pydantic_tools-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Useful tools for pydantic
 Author-Email: icebear <iiiicebeaaaar@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: pytest>=7.3.1
 Requires-Dist: rich>=13.3.5
```

