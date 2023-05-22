# Comparing `tmp/newrelic-data-exporter-0.0.8.tar.gz` & `tmp/newrelic-data-exporter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic-data-exporter-0.0.8.tar", last modified: Fri May 19 07:22:59 2023, max compression
+gzip compressed data, was "newrelic-data-exporter-0.0.9.tar", last modified: Mon May 22 08:09:28 2023, max compression
```

## Comparing `newrelic-data-exporter-0.0.8.tar` & `newrelic-data-exporter-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 07:22:59.764496 newrelic-data-exporter-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-05-17 15:36:57.000000 newrelic-data-exporter-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       96 2023-05-17 15:37:07.000000 newrelic-data-exporter-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2453 2023-05-19 07:22:59.763238 newrelic-data-exporter-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1949 2023-05-17 17:02:29.000000 newrelic-data-exporter-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 07:22:59.677161 newrelic-data-exporter-0.0.8/newrelic_data_exporter/
--rw-rw-rw-   0        0        0        0 2023-05-17 15:14:19.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-05-17 17:17:09.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter/newrelic_data_exporter.py
--rw-rw-rw-   0        0        0     1600 2023-05-17 09:30:59.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter/queries.yml
--rw-rw-rw-   0        0        0      415 2023-05-17 10:06:51.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter/resources.yml
-drwxrwxrwx   0        0        0        0 2023-05-19 07:22:59.760679 newrelic-data-exporter-0.0.8/newrelic_data_exporter.egg-info/
--rw-rw-rw-   0        0        0     2453 2023-05-19 07:22:59.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-05-19 07:22:59.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 07:22:59.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-05-19 07:22:59.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-05-19 07:22:59.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-19 07:22:59.000000 newrelic-data-exporter-0.0.8/newrelic_data_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       93 2023-05-17 15:50:39.000000 newrelic-data-exporter-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 07:22:59.765880 newrelic-data-exporter-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-05-19 07:22:28.000000 newrelic-data-exporter-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:09:28.064427 newrelic-data-exporter-0.0.9/
+-rw-rw-rw-   0        0        0       13 2023-05-22 08:05:44.000000 newrelic-data-exporter-0.0.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1090 2023-05-17 15:36:57.000000 newrelic-data-exporter-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       96 2023-05-17 15:37:07.000000 newrelic-data-exporter-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2453 2023-05-22 08:09:28.062731 newrelic-data-exporter-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1949 2023-05-21 20:55:32.000000 newrelic-data-exporter-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 08:09:27.998386 newrelic-data-exporter-0.0.9/newrelic_data_exporter/
+-rw-rw-rw-   0        0        0        0 2023-05-17 15:14:19.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter/__init__.py
+-rw-rw-rw-   0        0        0     5123 2023-05-21 20:54:37.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter/newrelic_data_exporter.py
+-rw-rw-rw-   0        0        0     1600 2023-05-17 09:30:59.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter/queries.yml
+-rw-rw-rw-   0        0        0      625 2023-05-22 07:52:56.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter/resources.yml
+drwxrwxrwx   0        0        0        0 2023-05-22 08:09:28.059476 newrelic-data-exporter-0.0.9/newrelic_data_exporter.egg-info/
+-rw-rw-rw-   0        0        0     2453 2023-05-22 08:09:27.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-05-22 08:09:27.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:09:27.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-05-22 08:09:27.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-05-22 08:09:27.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-22 08:09:27.000000 newrelic-data-exporter-0.0.9/newrelic_data_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       93 2023-05-17 15:50:39.000000 newrelic-data-exporter-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 08:09:28.065435 newrelic-data-exporter-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-05-22 08:08:38.000000 newrelic-data-exporter-0.0.9/setup.py
```

### Comparing `newrelic-data-exporter-0.0.8/LICENSE.txt` & `newrelic-data-exporter-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic-data-exporter-0.0.8/PKG-INFO` & `newrelic-data-exporter-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-data-exporter
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool to export data from New Relic using GraphQL API
 Home-page: https://github.com/atheeque-ahmed/newrelic-data-exporter
 Author: Atheeque Ahmed
 Author-email: hello@atheeque.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 This tool requires Python 3.7 or newer. Before installing and using this tool, ensure that you have the correct Python version installed.
 
 ## Installation
 
 You can install the NewRelic Data Exporter package from PyPI:
 
 ```bash
-pip install newrelic_data_exporter
+pip install newrelic-data-exporter
 ```
 
 ## Usage
 
 After installation, you can run the NewRelic Data Exporter from the command line:
 
 ```bash
```

### Comparing `newrelic-data-exporter-0.0.8/README.md` & `newrelic-data-exporter-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 This tool requires Python 3.7 or newer. Before installing and using this tool, ensure that you have the correct Python version installed.
 
 ## Installation
 
 You can install the NewRelic Data Exporter package from PyPI:
 
 ```bash
-pip install newrelic_data_exporter
+pip install newrelic-data-exporter
 ```
 
 ## Usage
 
 After installation, you can run the NewRelic Data Exporter from the command line:
 
 ```bash
```

### Comparing `newrelic-data-exporter-0.0.8/newrelic_data_exporter/queries.yml` & `newrelic-data-exporter-0.0.9/newrelic_data_exporter/queries.yml`

 * *Files identical despite different names*

### Comparing `newrelic-data-exporter-0.0.8/newrelic_data_exporter.egg-info/PKG-INFO` & `newrelic-data-exporter-0.0.9/newrelic_data_exporter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-data-exporter
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool to export data from New Relic using GraphQL API
 Home-page: https://github.com/atheeque-ahmed/newrelic-data-exporter
 Author: Atheeque Ahmed
 Author-email: hello@atheeque.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 This tool requires Python 3.7 or newer. Before installing and using this tool, ensure that you have the correct Python version installed.
 
 ## Installation
 
 You can install the NewRelic Data Exporter package from PyPI:
 
 ```bash
-pip install newrelic_data_exporter
+pip install newrelic-data-exporter
 ```
 
 ## Usage
 
 After installation, you can run the NewRelic Data Exporter from the command line:
 
 ```bash
```

### Comparing `newrelic-data-exporter-0.0.8/setup.py` & `newrelic-data-exporter-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="newrelic-data-exporter",
-    version="0.0.8",
+    version="0.0.9",
     author="Atheeque Ahmed",
     author_email="hello@atheeque.com",
     description="A tool to export data from New Relic using GraphQL API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/atheeque-ahmed/newrelic-data-exporter",
     packages=find_packages(),
```

