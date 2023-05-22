# Comparing `tmp/exergenics-etl-0.1.0.tar.gz` & `tmp/exergenics-etl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-0.1.0.tar", last modified: Thu May 18 03:46:00 2023, max compression
+gzip compressed data, was "exergenics-etl-0.5.0.tar", last modified: Mon May 22 07:07:59 2023, max compression
```

## Comparing `exergenics-etl-0.1.0.tar` & `exergenics-etl-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:46:00.033691 exergenics-etl-0.1.0/
--rw-rw-r--   0 root         (0) root         (0)     1066 2023-05-18 03:44:34.000000 exergenics-etl-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      461 2023-05-18 03:46:00.033691 exergenics-etl-0.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:46:00.029691 exergenics-etl-0.1.0/app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:46:00.029691 exergenics-etl-0.1.0/app/exergenics_etl/
--rw-rw-r--   0 root         (0) root         (0)      262 2023-05-18 03:44:34.000000 exergenics-etl-0.1.0/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:46:00.033691 exergenics-etl-0.1.0/app/exergenics_etl/src/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 03:44:34.000000 exergenics-etl-0.1.0/app/exergenics_etl/src/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9137 2023-05-18 03:44:34.000000 exergenics-etl-0.1.0/app/exergenics_etl/src/exergenics_etl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:46:00.033691 exergenics-etl-0.1.0/app/exergenics_etl/test/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 03:44:34.000000 exergenics-etl-0.1.0/app/exergenics_etl/test/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6517 2023-05-18 03:44:34.000000 exergenics-etl-0.1.0/app/exergenics_etl/test/test_exergenics_etl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:46:00.033691 exergenics-etl-0.1.0/app/exergenics_etl.egg-info/
--rw-r--r--   0 root         (0) root         (0)      461 2023-05-18 03:45:59.000000 exergenics-etl-0.1.0/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-18 03:45:59.000000 exergenics-etl-0.1.0/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 03:45:59.000000 exergenics-etl-0.1.0/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-18 03:45:59.000000 exergenics-etl-0.1.0/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-18 03:45:59.000000 exergenics-etl-0.1.0/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 03:46:00.033691 exergenics-etl-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1094 2023-05-18 03:45:58.000000 exergenics-etl-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.339724 exergenics-etl-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 07:07:59.339724 exergenics-etl-0.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.335723 exergenics-etl-0.5.0/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.335723 exergenics-etl-0.5.0/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.335723 exergenics-etl-0.5.0/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45201 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/src/exergenics_etl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.339724 exergenics-etl-0.5.0/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30249 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/test/test_exergenics_etl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.335723 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:07:59.339724 exergenics-etl-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-22 07:07:58.000000 exergenics-etl-0.5.0/setup.py
```

### Comparing `exergenics-etl-0.1.0/LICENSE` & `exergenics-etl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-0.1.0/setup.py` & `exergenics-etl-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
-with open("app/Readme.md", "r") as f:
-    long_description = f.read()
+# with open("app/Readme.md", "r") as f:
+#     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="0.1.0",
+    version="v0.5.0",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
-    long_description=long_description,
+    long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
     author_email="nobel.wong@exergenics.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
@@ -22,13 +22,18 @@
     ],
     install_requires=["exergenics >= 2.0.0",
                       "DateTime == 5.1",
                       "pandas == 1.4.0",
                       "PyMySQL == 1.0.2",
                       "pytz == 2022.7.1",
                       "SQLAlchemy == 1.4.46",
-                      "python-dotenv == 1.0.0"],
+                      "python-dotenv == 1.0.0",
+                      "openpyxl == 3.0.10",
+                      "Levenshtein == 0.21.0",
+                      "regex == 2022.10.31",
+                      "dateparser == 1.1.5",
+                      "zipp == 3.15.0"],
     extras_require={
         "dev": ["pytest >= 7.0", "twine >= 4.0.2", "bump == 1.3.2"],
     },
     python_requires=">=3.8.10"
 )
```

