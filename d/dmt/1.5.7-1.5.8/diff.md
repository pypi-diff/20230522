# Comparing `tmp/dmt-1.5.7.tar.gz` & `tmp/dmt-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmt-1.5.7.tar", last modified: Mon May 22 21:44:40 2023, max compression
+gzip compressed data, was "dmt-1.5.8.tar", last modified: Mon May 22 21:47:32 2023, max compression
```

## Comparing `dmt-1.5.7.tar` & `dmt-1.5.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:44:40.182161 dmt-1.5.7/
--rw-r--r--   0 waser     (1000) waser     (1000)    34494 2022-02-08 22:42:22.000000 dmt-1.5.7/LICENSE
--rw-r--r--   0 waser     (1000) waser     (1000)     4154 2023-05-22 21:44:40.182161 dmt-1.5.7/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)     3226 2023-05-22 21:44:25.000000 dmt-1.5.7/README.md
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:44:40.178828 dmt-1.5.7/dmt.egg-info/
--rw-r--r--   0 waser     (1000) waser     (1000)     4154 2023-05-22 21:44:40.000000 dmt-1.5.7/dmt.egg-info/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-05-22 21:44:40.000000 dmt-1.5.7/dmt.egg-info/SOURCES.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-05-22 21:44:40.000000 dmt-1.5.7/dmt.egg-info/dependency_links.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       56 2023-05-22 21:44:40.000000 dmt-1.5.7/dmt.egg-info/entry_points.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       73 2023-05-22 21:44:40.000000 dmt-1.5.7/dmt.egg-info/requires.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        7 2023-05-22 21:44:40.000000 dmt-1.5.7/dmt.egg-info/top_level.txt
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:44:40.178828 dmt-1.5.7/domain/
--rw-r--r--   0 waser     (1000) waser     (1000)     1104 2023-05-22 21:44:25.000000 dmt-1.5.7/domain/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)       48 2022-11-25 03:48:15.000000 dmt-1.5.7/domain/__main__.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:44:40.178828 dmt-1.5.7/domain/entry_points/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2022-03-17 20:13:54.000000 dmt-1.5.7/domain/entry_points/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1317 2023-05-22 21:44:25.000000 dmt-1.5.7/domain/entry_points/run_dmt.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:44:40.182161 dmt-1.5.7/domain/management/
--rw-r--r--   0 waser     (1000) waser     (1000)     1063 2022-11-25 03:28:44.000000 dmt-1.5.7/domain/management/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)    27518 2023-05-22 21:44:25.000000 dmt-1.5.7/domain/management/tools.py
--rw-r--r--   0 waser     (1000) waser     (1000)      633 2022-10-06 04:01:18.000000 dmt-1.5.7/pyproject.toml
--rw-r--r--   0 waser     (1000) waser     (1000)     2020 2023-05-22 21:44:40.182161 dmt-1.5.7/setup.cfg
--rw-r--r--   0 waser     (1000) waser     (1000)     1617 2023-05-22 21:44:25.000000 dmt-1.5.7/setup.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:47:32.200934 dmt-1.5.8/
+-rw-r--r--   0 waser     (1000) waser     (1000)    34494 2022-02-08 22:42:22.000000 dmt-1.5.8/LICENSE
+-rw-r--r--   0 waser     (1000) waser     (1000)     4151 2023-05-22 21:47:32.200934 dmt-1.5.8/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)     3226 2023-05-22 21:44:25.000000 dmt-1.5.8/README.md
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:47:32.200934 dmt-1.5.8/dmt.egg-info/
+-rw-r--r--   0 waser     (1000) waser     (1000)     4151 2023-05-22 21:47:32.000000 dmt-1.5.8/dmt.egg-info/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-05-22 21:47:32.000000 dmt-1.5.8/dmt.egg-info/SOURCES.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-05-22 21:47:32.000000 dmt-1.5.8/dmt.egg-info/dependency_links.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       56 2023-05-22 21:47:32.000000 dmt-1.5.8/dmt.egg-info/entry_points.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       73 2023-05-22 21:47:32.000000 dmt-1.5.8/dmt.egg-info/requires.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        7 2023-05-22 21:47:32.000000 dmt-1.5.8/dmt.egg-info/top_level.txt
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:47:32.200934 dmt-1.5.8/domain/
+-rw-r--r--   0 waser     (1000) waser     (1000)     1104 2023-05-22 21:47:14.000000 dmt-1.5.8/domain/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)       48 2022-11-25 03:48:15.000000 dmt-1.5.8/domain/__main__.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:47:32.200934 dmt-1.5.8/domain/entry_points/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2022-03-17 20:13:54.000000 dmt-1.5.8/domain/entry_points/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1317 2023-05-22 21:44:25.000000 dmt-1.5.8/domain/entry_points/run_dmt.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-05-22 21:47:32.200934 dmt-1.5.8/domain/management/
+-rw-r--r--   0 waser     (1000) waser     (1000)     1063 2022-11-25 03:28:44.000000 dmt-1.5.8/domain/management/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    27518 2023-05-22 21:44:25.000000 dmt-1.5.8/domain/management/tools.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      633 2022-10-06 04:01:18.000000 dmt-1.5.8/pyproject.toml
+-rw-r--r--   0 waser     (1000) waser     (1000)     2020 2023-05-22 21:47:32.200934 dmt-1.5.8/setup.cfg
+-rw-r--r--   0 waser     (1000) waser     (1000)     1614 2023-05-22 21:47:20.000000 dmt-1.5.8/setup.py
```

### Comparing `dmt-1.5.7/LICENSE` & `dmt-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dmt-1.5.7/PKG-INFO` & `dmt-1.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmt
-Version: 1.5.7
+Version: 1.5.8
 Summary: Manage domains like packages.
 Home-page: https://gitlab.com/waser-technologies/technologies/dmt
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://gitlab.com/waser-technologies/technologies/dmt/blob/main/README.md
 Project-URL: Code, https://gitlab.com/waser-technologies/technologies/dmt
 Project-URL: Issue tracker, https://gitlab.com/waser-technologies/technologies/dmt/issues
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
-Requires-Python: >=3.8,<=3.10.9
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Domain Management Tool
 
 DMT (for short) is a collection of tools to manage your [RASA domains](https://rasa.com/docs/rasa/domain/) like if they were packages not unlike pip with python but with YAML for RASA.
```

### Comparing `dmt-1.5.7/README.md` & `dmt-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `dmt-1.5.7/dmt.egg-info/PKG-INFO` & `dmt-1.5.8/dmt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmt
-Version: 1.5.7
+Version: 1.5.8
 Summary: Manage domains like packages.
 Home-page: https://gitlab.com/waser-technologies/technologies/dmt
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://gitlab.com/waser-technologies/technologies/dmt/blob/main/README.md
 Project-URL: Code, https://gitlab.com/waser-technologies/technologies/dmt
 Project-URL: Issue tracker, https://gitlab.com/waser-technologies/technologies/dmt/issues
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
-Requires-Python: >=3.8,<=3.10.9
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Domain Management Tool
 
 DMT (for short) is a collection of tools to manage your [RASA domains](https://rasa.com/docs/rasa/domain/) like if they were packages not unlike pip with python but with YAML for RASA.
```

### Comparing `dmt-1.5.7/domain/__init__.py` & `dmt-1.5.8/domain/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__ = "1.5.7"
+__version__ = "1.5.8"
 
 USERNAME = os.environ.get("USERNAME", 'root')
 HOME = os.environ.get('HOME', f'/home/{USERNAME}' if USERNAME != 'root' else '/root')
 ASSISTANT_PATH = f"{HOME}/.assistant" if USERNAME != "root" else "/usr/share/assistant"
 
 I18N, L10N = (x for x in os.environ.get('LANG', "en_EN.UTF-8").split(".")[0].split("_"))
```

### Comparing `dmt-1.5.7/domain/entry_points/run_dmt.py` & `dmt-1.5.8/domain/entry_points/run_dmt.py`

 * *Files identical despite different names*

### Comparing `dmt-1.5.7/domain/management/__init__.py` & `dmt-1.5.8/domain/management/__init__.py`

 * *Files identical despite different names*

### Comparing `dmt-1.5.7/domain/management/tools.py` & `dmt-1.5.8/domain/management/tools.py`

 * *Files identical despite different names*

### Comparing `dmt-1.5.7/pyproject.toml` & `dmt-1.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dmt-1.5.7/setup.cfg` & `dmt-1.5.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `dmt-1.5.7/setup.py` & `dmt-1.5.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "Code": "https://gitlab.com/waser-technologies/technologies/dmt",
         "Issue tracker": "https://gitlab.com/waser-technologies/technologies/dmt/issues",
     },
     description='Manage domains like packages.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages('.'),
-    python_requires='>=3.8,<=3.10.9',
+    python_requires='>=3.8,<3.12',
     install_requires = [
         'prompt_toolkit>=2.0.0,<3.1.0',
         'tqdm',
         'halo',
         'rich',
         'pyyaml',
         'requests',
```

