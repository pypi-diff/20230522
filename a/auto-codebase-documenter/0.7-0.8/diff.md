# Comparing `tmp/auto-codebase-documenter-0.7.tar.gz` & `tmp/auto-codebase-documenter-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-0.7.tar", last modified: Mon May 22 06:05:07 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-0.8.tar", last modified: Mon May 22 06:11:25 2023, max compression
```

## Comparing `auto-codebase-documenter-0.7.tar` & `auto-codebase-documenter-0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.7/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     8434 2023-05-22 06:01:50.000000 auto-codebase-documenter-0.7/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     6319 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.7/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 05:41:30.000000 auto-codebase-documenter-0.7/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2792 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.7/auto_codebase_documenter/auto_documenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.7/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      494 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       55 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      953 2023-05-22 06:04:44.000000 auto-codebase-documenter-0.7/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.8/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     8434 2023-05-22 06:01:50.000000 auto-codebase-documenter-0.8/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6319 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.8/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 05:41:30.000000 auto-codebase-documenter-0.8/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2792 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.8/auto_codebase_documenter/auto_documenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.8/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      494 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       80 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 06:11:25.000000 auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 06:11:25.664662 auto-codebase-documenter-0.8/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      978 2023-05-22 06:10:56.000000 auto-codebase-documenter-0.8/setup.py
```

### Comparing `auto-codebase-documenter-0.7/LICENSE` & `auto-codebase-documenter-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.7/PKG-INFO` & `auto-codebase-documenter-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.7
+Version: 0.8
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.7/README.md` & `auto-codebase-documenter-0.8/README.md`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.7/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-0.8/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.7/auto_codebase_documenter/auto_documenter.py` & `auto-codebase-documenter-0.8/auto_codebase_documenter/auto_documenter.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.7/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-0.8/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/PKG-INFO` & `auto-codebase-documenter-0.8/auto_codebase_documenter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.7
+Version: 0.8
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.7/setup.py` & `auto-codebase-documenter-0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-codebase-documenter",
-    version="0.7",
+    version="0.8",
     packages=find_packages(),
     install_requires=["openai", "python-dotenv", "PyYAML"],
     entry_points={
         "console_scripts": [
-            "auto-codebase-documenter = run:main",
+            "auto-codebase-documenter = auto_codebase_documenter.run:main",
         ],
     },
     author="Alex Bryant",
     author_email="alexbryant710@gmail.com",
     description="Automatic codebase documentation tool using OpenAI GPT models",
     long_description="This tool utilizes OpenAI GPT models to automatically assess and document a codebase by generating written assessments for each file.",
     long_description_content_type="text/markdown",
```

