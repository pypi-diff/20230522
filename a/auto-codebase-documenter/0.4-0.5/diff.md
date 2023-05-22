# Comparing `tmp/auto-codebase-documenter-0.4.tar.gz` & `tmp/auto-codebase-documenter-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-0.4.tar", last modified: Mon May 22 02:16:28 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-0.5.tar", last modified: Mon May 22 02:37:21 2023, max compression
```

## Comparing `auto-codebase-documenter-0.4.tar` & `auto-codebase-documenter-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.4/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     7698 2023-05-22 02:12:20.000000 auto-codebase-documenter-0.4/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     5814 2023-05-22 02:12:20.000000 auto-codebase-documenter-0.4/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 01:40:24.000000 auto-codebase-documenter-0.4/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.4/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       55 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      930 2023-05-22 02:15:56.000000 auto-codebase-documenter-0.4/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.5/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     7698 2023-05-22 02:12:20.000000 auto-codebase-documenter-0.5/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6083 2023-05-22 02:33:17.000000 auto-codebase-documenter-0.5/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 01:40:24.000000 auto-codebase-documenter-0.5/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.5/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       55 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      930 2023-05-22 02:37:13.000000 auto-codebase-documenter-0.5/setup.py
```

### Comparing `auto-codebase-documenter-0.4/LICENSE` & `auto-codebase-documenter-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.4/PKG-INFO` & `auto-codebase-documenter-0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.4
+Version: 0.5
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.4/README.md` & `auto-codebase-documenter-0.5/README.md`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.4/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-0.5/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from datetime import datetime
 import os
 import yaml
 import openai
+import logging
 from os.path import dirname, abspath
 from .default_ai_prompt import default_ai_prompt
 
 
 class AutoCodebaseDocumenter:
     def __init__(
         self,
         openai_api_key,
         root_path=".",
         output_docs_folder_name="docs",
         ignore_folders=["venv"],
         file_types=[".py"],
         single_file=False,
+        debug=False,
     ):
         self.openai_api_key = openai_api_key
         self.root_path = root_path
         self.output_docs_folder_name = output_docs_folder_name
         self.ignore_folders = ignore_folders
         self.file_types = file_types
         self.base_dir = root_path
@@ -26,41 +28,49 @@
 
         openai.api_key = self.openai_api_key
 
         # Create the docs folder if it doesn't exist
         if not os.path.exists(self.docs_dir):
             os.makedirs(self.docs_dir)
 
+        # Set up logging
+        self.debug = debug
+        self._setup_logging()
+
         # Load config from file
         self._load_config()
 
+    def _setup_logging(self):
+        log_level = logging.DEBUG if self.debug else logging.INFO
+        logging.basicConfig(level=log_level)
+
     def _load_config(self):
         module_dir = dirname(abspath(__file__))
         config_file = os.path.join(module_dir, "documenter_config.yaml")
+        logging.debug(f"Looking for config file at {config_file}")
 
         try:
             with open(config_file, "r") as stream:
                 config_data = yaml.safe_load(stream)
                 self.ai_prompt_text = config_data.get("override_ai_prompt", default_ai_prompt)
                 self.ignore_folders = config_data.get("ignore_folders", self.ignore_folders)
                 self.file_types = config_data.get("file_types", self.file_types)
-                # self.single_file = config_data.get("single_file", self.single_file)
-                print("Using the prompt override from 'documenter_config.yaml'.")
-                print("Custom prompt is set to the following:")
-                print(self.ai_prompt_text)
+                logging.debug("Using the prompt override from 'documenter_config.yaml'.")
+                logging.debug("Custom prompt is set to the following:")
+                logging.debug(self.ai_prompt_text)
         except FileNotFoundError:
-            print("Warning: 'documenter_config.yaml' file not found. Using default ai prompt config.")
+            logging.warning("'documenter_config.yaml' file not found. Using default AI prompt config.")
             self.ai_prompt_text = default_ai_prompt
         except KeyError:
-            print(
-                "Warning: 'override_ai_prompt' key not found in 'documenter_config.yaml'. Using default ai prompt config."
+            logging.warning(
+                "'override_ai_prompt' key not found in 'documenter_config.yaml'. Using default AI prompt config."
             )
             self.ai_prompt_text = default_ai_prompt
         except Exception as e:
-            print(f"Warning: Error reading 'documenter_config.yaml'. Using default ai prompt config. Error: {str(e)}")
+            logging.warning(f"Error reading 'documenter_config.yaml'. Using default AI prompt config. Error: {str(e)}")
             self.ai_prompt_text = default_ai_prompt
 
     def _get_completion(self, prompt, model="gpt-3.5-turbo"):
         messages = [{"role": "user", "content": prompt}]
         response = openai.ChatCompletion.create(
             model=model,
             messages=messages,
```

### Comparing `auto-codebase-documenter-0.4/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-0.5/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/PKG-INFO` & `auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.4
+Version: 0.5
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.4/setup.py` & `auto-codebase-documenter-0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-codebase-documenter",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
     install_requires=["openai", "python-dotenv", "PyYAML"],
     entry_points={
         "console_scripts": [
             "auto-codebase-documenter = run:main",
         ],
     },
```

