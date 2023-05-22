# Comparing `tmp/auto-codebase-documenter-0.8.tar.gz` & `tmp/auto-codebase-documenter-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-0.8.tar", last modified: Mon May 22 06:11:25 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-0.9.tar", last modified: Mon May 22 06:19:40 2023, max compression
```

## Comparing `auto-codebase-documenter-0.8.tar` & `auto-codebase-documenter-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.8/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     8434 2023-05-22 06:01:50.000000 auto-codebase-documenter-0.8/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     6319 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.8/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 05:41:30.000000 auto-codebase-documenter-0.8/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2792 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.8/auto_codebase_documenter/auto_documenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.8/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      494 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       80 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      978 2023-05-22 06:10:56.000000 auto-codebase-documenter-0.8/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:19:40.515934 auto-codebase-documenter-0.9/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.9/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:19:40.515934 auto-codebase-documenter-0.9/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     8434 2023-05-22 06:01:50.000000 auto-codebase-documenter-0.9/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:19:40.505934 auto-codebase-documenter-0.9/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6319 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.9/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 05:41:30.000000 auto-codebase-documenter-0.9/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2792 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.9/auto_codebase_documenter/auto_documenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.9/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:19:40.515934 auto-codebase-documenter-0.9/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:19:40.000000 auto-codebase-documenter-0.9/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      494 2023-05-22 06:19:40.000000 auto-codebase-documenter-0.9/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 06:19:40.000000 auto-codebase-documenter-0.9/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       91 2023-05-22 06:19:40.000000 auto-codebase-documenter-0.9/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 06:19:40.000000 auto-codebase-documenter-0.9/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 06:19:40.000000 auto-codebase-documenter-0.9/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 06:19:40.515934 auto-codebase-documenter-0.9/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      989 2023-05-22 06:18:43.000000 auto-codebase-documenter-0.9/setup.py
```

### Comparing `auto-codebase-documenter-0.8/LICENSE` & `auto-codebase-documenter-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.8/PKG-INFO` & `auto-codebase-documenter-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.8
+Version: 0.9
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.8/README.md` & `auto-codebase-documenter-0.9/README.md`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.8/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-0.9/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.8/auto_codebase_documenter/auto_documenter.py` & `auto-codebase-documenter-0.9/auto_codebase_documenter/auto_documenter.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.8/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-0.9/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/PKG-INFO` & `auto-codebase-documenter-0.9/auto_codebase_documenter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.8
+Version: 0.9
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.8/setup.py` & `auto-codebase-documenter-0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-codebase-documenter",
-    version="0.8",
+    version="0.9",
     packages=find_packages(),
     install_requires=["openai", "python-dotenv", "PyYAML"],
     entry_points={
         "console_scripts": [
-            "auto-codebase-documenter = auto_codebase_documenter.run:main",
+            "auto-codebase-documenter = auto_codebase_documenter.run:auto_documenter",
         ],
     },
     author="Alex Bryant",
     author_email="alexbryant710@gmail.com",
     description="Automatic codebase documentation tool using OpenAI GPT models",
     long_description="This tool utilizes OpenAI GPT models to automatically assess and document a codebase by generating written assessments for each file.",
     long_description_content_type="text/markdown",
```

