# Comparing `tmp/auto-codebase-documenter-0.6.tar.gz` & `tmp/auto-codebase-documenter-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-0.6.tar", last modified: Mon May 22 02:48:34 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-0.7.tar", last modified: Mon May 22 06:05:07 2023, max compression
```

## Comparing `auto-codebase-documenter-0.6.tar` & `auto-codebase-documenter-0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.6/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     7698 2023-05-22 02:12:20.000000 auto-codebase-documenter-0.6/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     6036 2023-05-22 02:43:54.000000 auto-codebase-documenter-0.6/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 01:40:24.000000 auto-codebase-documenter-0.6/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.6/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       55 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      930 2023-05-22 02:48:12.000000 auto-codebase-documenter-0.6/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.7/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     8434 2023-05-22 06:01:50.000000 auto-codebase-documenter-0.7/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6319 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.7/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 05:41:30.000000 auto-codebase-documenter-0.7/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2792 2023-05-22 06:04:12.000000 auto-codebase-documenter-0.7/auto_codebase_documenter/auto_documenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.7/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      494 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       55 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 06:05:07.000000 auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 06:05:07.279678 auto-codebase-documenter-0.7/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      953 2023-05-22 06:04:44.000000 auto-codebase-documenter-0.7/setup.py
```

### Comparing `auto-codebase-documenter-0.6/LICENSE` & `auto-codebase-documenter-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.6/PKG-INFO` & `auto-codebase-documenter-0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.6
+Version: 0.7
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
-Platform: UNKNOWN
+Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This tool utilizes OpenAI GPT models to automatically assess and document a codebase by generating written assessments for each file.
```

### Comparing `auto-codebase-documenter-0.6/README.md` & `auto-codebase-documenter-0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -62,30 +62,46 @@
 ### Importing the package
 
 The easiest way to use the tool is to create a file called `documenter.py` and add the following code to run the app by importing the `AutoCodebaseDocumenter` class:
 
 ```python
 import os
 from dotenv import load_dotenv
-from auto_codebase_documenter import AutoCodebaseDocumenter
+from auto_codebase_documenter.AutoCodebaseDocumenter import AutoCodebaseDocumenter
 
 load_dotenv()  # load .env file
 openai_api_key = os.getenv("OPENAI_KEY")  # get OPENAI_KEY value from .env file{}
 
 documenter = AutoCodebaseDocumenter(openai_api_key)
 documenter.process_all_files()
+
 ```
 
 The `process_all_files` method will start processing the files.
 
 You can add the `documenter_config.yaml` into the same folder to customize the tool.
 
 ### CLI
 
-TODO: Add CLI usage instructions
+Install the package and then run it with:
+
+```bash
+auto-codebase-documenter
+```
+
+Make sure the environment variable `OPENAI_KEY` is set to your OpenAI API key.
+
+See the section for Configuration for the best way to configure the tool.
+
+It can be run with the following command line arguments:
+
+- `--codebase_path`: The path to the codebase you want to document. Defaults to the current working directory.
+- `--ignore_folders`: A list of directories that you want to exclude from the documentation process. Defaults to ["venv"].
+- `--file_types`: A list of file types (by extension) that you want to include in the documentation process. Defaults to [".py"].
+- `--output_docs_folder_name`: The name of the output docs folder. Defaults to "docs".
 
 ## Configuration
 
 Edit the `documenter_config.yaml` file to configure the tool. The following parameters are available:
 
 - `override_ai_prompt`: A list of intentions you want the AI model to follow when it writes the documentation. This should follow a decent list of prompt items that should get the best out of the AI model.
```

### Comparing `auto-codebase-documenter-0.6/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-0.7/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from datetime import datetime
 import os
 import yaml
 import openai
 import logging
-from os.path import dirname, abspath
-from .default_ai_prompt import default_ai_prompt
+from auto_codebase_documenter.default_ai_prompt import default_ai_prompt
 
 
 class AutoCodebaseDocumenter:
     def __init__(
         self,
         openai_api_key,
         root_path=".",
@@ -46,30 +45,40 @@
     def _load_config(self):
         config_file = os.path.join(os.getcwd(), "documenter_config.yaml")
         logging.debug(f"Looking for config file at {config_file}")
 
         try:
             with open(config_file, "r") as stream:
                 config_data = yaml.safe_load(stream)
-                self.ai_prompt_text = config_data.get("override_ai_prompt", default_ai_prompt)
-                self.ignore_folders = config_data.get("ignore_folders", self.ignore_folders)
+                self.ai_prompt_text = config_data.get(
+                    "override_ai_prompt", default_ai_prompt
+                )
+                self.ignore_folders = config_data.get(
+                    "ignore_folders", self.ignore_folders
+                )
                 self.file_types = config_data.get("file_types", self.file_types)
-                logging.debug("Using the prompt override from 'documenter_config.yaml'.")
+                logging.debug(
+                    "Using the prompt override from 'documenter_config.yaml'."
+                )
                 logging.debug("Custom prompt is set to the following:")
                 logging.debug(self.ai_prompt_text)
         except FileNotFoundError:
-            logging.warning("'documenter_config.yaml' file not found. Using default AI prompt config.")
+            logging.warning(
+                "'documenter_config.yaml' file not found. Using default AI prompt config."
+            )
             self.ai_prompt_text = default_ai_prompt
         except KeyError:
             logging.warning(
                 "'override_ai_prompt' key not found in 'documenter_config.yaml'. Using default AI prompt config."
             )
             self.ai_prompt_text = default_ai_prompt
         except Exception as e:
-            logging.warning(f"Error reading 'documenter_config.yaml'. Using default AI prompt config. Error: {str(e)}")
+            logging.warning(
+                f"Error reading 'documenter_config.yaml'. Using default AI prompt config. Error: {str(e)}"
+            )
             self.ai_prompt_text = default_ai_prompt
 
     def _get_completion(self, prompt, model="gpt-3.5-turbo"):
         messages = [{"role": "user", "content": prompt}]
         response = openai.ChatCompletion.create(
             model=model,
             messages=messages,
@@ -83,15 +92,17 @@
             for ignore_folder in self.ignore_folders:
                 if ignore_folder in dirnames:
                     dirnames.remove(ignore_folder)
             file_paths.extend(
                 [
                     os.path.join(dirpath, filename)
                     for filename in filenames
-                    if any(filename.endswith(file_type) for file_type in self.file_types)
+                    if any(
+                        filename.endswith(file_type) for file_type in self.file_types
+                    )
                 ]
             )
         return file_paths
 
     def _process_file(self, file_path):
         with open(file_path, "r") as file:
             prompt = file.read()
@@ -115,24 +126,28 @@
 
             # Define the output file path
             file_name = os.path.basename(file_path)
             output_file = os.path.join(output_dir, f"{file_name}.md")
 
             # Check if the file already exists
             if os.path.exists(output_file):
-                print(f"WARNING: Documentation file {output_file} already exists and will be overwritten.")
+                print(
+                    f"WARNING: Documentation file {output_file} already exists and will be overwritten."
+                )
 
             with open(output_file, "w") as output:
                 # Add timestamp at the top of the file
                 print(
                     "# Auto generated documentation file from auto-codebase-documenter\n",
                     file=output,
                 )
                 timestamp = datetime.now().strftime("%d %B %Y at %H:%M:%S")
-                print(f"This documentation file was created on {timestamp}\n", file=output)
+                print(
+                    f"This documentation file was created on {timestamp}\n", file=output
+                )
 
                 print("## File path\n", file=output)
                 print(f"{file_path}\n", file=output)
                 response = self._get_completion(prompt)
                 print(response, file=output)
 
                 print(f"Wrote documentation file {output_file}")
```

### Comparing `auto-codebase-documenter-0.6/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-0.7/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/PKG-INFO` & `auto-codebase-documenter-0.7/auto_codebase_documenter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.6
+Version: 0.7
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
-Platform: UNKNOWN
+Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This tool utilizes OpenAI GPT models to automatically assess and document a codebase by generating written assessments for each file.
```

### Comparing `auto-codebase-documenter-0.6/setup.py` & `auto-codebase-documenter-0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-codebase-documenter",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     install_requires=["openai", "python-dotenv", "PyYAML"],
     entry_points={
         "console_scripts": [
             "auto-codebase-documenter = run:main",
         ],
     },
@@ -18,8 +18,9 @@
     url="https://github.com/abryant710/auto-codebase-documenter",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     license="MIT",
+    platforms=["any"],
 )
```

