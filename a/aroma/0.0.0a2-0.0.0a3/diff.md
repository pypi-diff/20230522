# Comparing `tmp/aroma-0.0.0a2.tar.gz` & `tmp/aroma-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aroma-0.0.0a2.tar", max compression
+gzip compressed data, was "aroma-0.0.0a3.tar", max compression
```

## Comparing `aroma-0.0.0a2.tar` & `aroma-0.0.0a3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1501 2023-05-19 02:16:20.837941 aroma-0.0.0a2/LICENSE
--rw-r--r--   0        0        0     2077 2023-05-19 16:10:00.359708 aroma-0.0.0a2/README.md
--rw-r--r--   0        0        0     4447 2023-05-21 04:18:06.297198 aroma-0.0.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 02:31:51.411306 aroma-0.0.0a2/src/aroma/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 02:27:22.035804 aroma-0.0.0a2/src/aroma/datasets/__init__.py
--rw-r--r--   0        0        0    19502 2023-05-21 05:06:25.737697 aroma-0.0.0a2/src/aroma/datasets/breakfast.py
--rw-r--r--   0        0        0        0 2023-05-19 05:02:55.991661 aroma-0.0.0a2/src/aroma/utils/__init__.py
--rw-r--r--   0        0        0      745 2023-05-19 14:24:52.685953 aroma-0.0.0a2/src/aroma/utils/imports.py
--rw-r--r--   0        0        0    11816 2023-05-19 05:02:55.992030 aroma-0.0.0a2/src/aroma/utils/vocab.py
--rw-r--r--   0        0        0     3425 1970-01-01 00:00:00.000000 aroma-0.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-22 04:51:41.380201 aroma-0.0.0a3/LICENSE
+-rw-r--r--   0        0        0     2077 2023-05-22 04:51:41.380201 aroma-0.0.0a3/README.md
+-rw-r--r--   0        0        0     4447 2023-05-22 04:51:41.380201 aroma-0.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 04:51:41.380201 aroma-0.0.0a3/src/aroma/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 04:51:41.380201 aroma-0.0.0a3/src/aroma/datasets/__init__.py
+-rw-r--r--   0        0        0    19502 2023-05-22 04:51:41.384201 aroma-0.0.0a3/src/aroma/datasets/breakfast.py
+-rw-r--r--   0        0        0        0 2023-05-22 04:51:41.384201 aroma-0.0.0a3/src/aroma/utils/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-22 04:51:41.384201 aroma-0.0.0a3/src/aroma/utils/imports.py
+-rw-r--r--   0        0        0    11816 2023-05-22 04:51:41.384201 aroma-0.0.0a3/src/aroma/utils/vocab.py
+-rw-r--r--   0        0        0     3425 1970-01-01 00:00:00.000000 aroma-0.0.0a3/PKG-INFO
```

### Comparing `aroma-0.0.0a2/LICENSE` & `aroma-0.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `aroma-0.0.0a2/README.md` & `aroma-0.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `aroma-0.0.0a2/pyproject.toml` & `aroma-0.0.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aroma"
-version = "0.0.0a2"
+version = "0.0.0a3"
 description = "A library to prepare asynchronous time series datasets"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/aroma"
 repository = "https://github.com/durandtibo/aroma"
 keywords = ["dataset", "TPP", "asynchronous time series"]
 license = "BSD-3-Clause"
```

### Comparing `aroma-0.0.0a2/src/aroma/datasets/breakfast.py` & `aroma-0.0.0a3/src/aroma/datasets/breakfast.py`

 * *Files identical despite different names*

### Comparing `aroma-0.0.0a2/src/aroma/utils/imports.py` & `aroma-0.0.0a3/src/aroma/utils/imports.py`

 * *Files identical despite different names*

### Comparing `aroma-0.0.0a2/src/aroma/utils/vocab.py` & `aroma-0.0.0a3/src/aroma/utils/vocab.py`

 * *Files identical despite different names*

### Comparing `aroma-0.0.0a2/PKG-INFO` & `aroma-0.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aroma
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: A library to prepare asynchronous time series datasets
 Home-page: https://github.com/durandtibo/aroma
 License: BSD-3-Clause
 Keywords: dataset,TPP,asynchronous time series
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aroma Version: 0.0.0a2 Summary: A library to
+Metadata-Version: 2.1 Name: aroma Version: 0.0.0a3 Summary: A library to
 prepare asynchronous time series datasets Home-page: https://github.com/
 durandtibo/aroma License: BSD-3-Clause Keywords: dataset,TPP,asynchronous time
 series Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: POSIX ::
```

