# Comparing `tmp/auto-codebase-documenter-0.2.tar.gz` & `tmp/auto-codebase-documenter-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-0.2.tar", last modified: Mon May 22 01:24:41 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-0.3.tar", last modified: Mon May 22 01:46:27 2023, max compression
```

## Comparing `auto-codebase-documenter-0.2.tar` & `auto-codebase-documenter-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.2/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      640 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     8346 2023-05-22 00:14:55.000000 auto-codebase-documenter-0.2/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     5810 2023-05-22 01:04:32.000000 auto-codebase-documenter-0.2/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 00:15:35.000000 auto-codebase-documenter-0.2/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.2/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      640 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       80 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       21 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      926 2023-05-22 01:19:57.000000 auto-codebase-documenter-0.2/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.3/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     8701 2023-05-22 01:27:45.000000 auto-codebase-documenter-0.3/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     5810 2023-05-22 01:04:32.000000 auto-codebase-documenter-0.3/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 01:40:24.000000 auto-codebase-documenter-0.3/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.3/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       64 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       21 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      929 2023-05-22 01:45:41.000000 auto-codebase-documenter-0.3/setup.py
```

### Comparing `auto-codebase-documenter-0.2/LICENSE` & `auto-codebase-documenter-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.2/README.md` & `auto-codebase-documenter-0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Auto Codebase Documenter
 
 Auto Codebase Documenter is a Python-based tool that leverages the power of the OpenAI GPT-3.5-turbo or GPT-4 model to automatically assess and document a codebase.
 
 This tool simplifies the process of documenting your project by walking through the directory of your codebase, selectively ignoring certain directories (such as virtual environments), and processing the Python files found. It harnesses the capabilities of the AI model to generate a comprehensive written assessment of each file. The assessments are then organized and stored in Markdown (`.md`) files within a dedicated `docs` directory.
 
-By automatically analyzing your codebase and providing detailed explanations, suggestions, and insights, the Auto Codebase Documenter facilitates the understanding of your project's structure, purpose, and functionality. The generated documentation can serve as a valuable resource for new developers joining the project or as an aid for code review and refactoring processes.
+By automatically analyzing your codebase and providing detailed explanations, suggestions, and insights, the Auto Codebase Documenter facilitates the understanding of your project's structure, purpose, and functionality. The generated documentation can serve as a
+valuable resource for new developers joining the project or as an aid for code review and refactoring processes.
+
+## Installation
+
+You can install `auto-codebase-documenter` using `pip` from the Python Package Index (PyPI).
+
+```bash
+pip install auto-codebase-documenter
+```
+
+The package is hosted on PyPI and can be found at <https://pypi.org/project/auto-codebase-documenter>. You can visit the link for more information about the package and its available versions.
 
 ## Configuration
 
 Edit the `config.yaml` file to configure the tool. The following parameters are available:
 
 - `override_ai_prompt`: A list of intentions you want the AI model to follow when it writes the documentation. This should follow a decent list of prompt items that should get the best out of the AI model.
```

### Comparing `auto-codebase-documenter-0.2/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-0.3/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.2/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-0.3/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.2/setup.py` & `auto-codebase-documenter-0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-codebase-documenter",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     install_requires=["openai", "python-dotenv"],
     entry_points={
         "console_scripts": [
-            "auto-codebase-documenter = auto_codebase_documenter.run:main",
+            "auto-codebase-documenter = run:document_code",
         ],
     },
     author="Alex Bryant",
     author_email="alexbryant710@gmail.com",
     description="Automatic codebase documentation tool using OpenAI GPT models",
     long_description="This tool utilizes OpenAI GPT models to automatically assess and document a codebase by generating written assessments for each file.",
     long_description_content_type="text/markdown",
     url="https://github.com/abryant710/auto-codebase-documenter",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    license="MIT",
 )
```

