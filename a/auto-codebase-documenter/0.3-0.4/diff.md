# Comparing `tmp/auto-codebase-documenter-0.3.tar.gz` & `tmp/auto-codebase-documenter-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-0.3.tar", last modified: Mon May 22 01:46:27 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-0.4.tar", last modified: Mon May 22 02:16:28 2023, max compression
```

## Comparing `auto-codebase-documenter-0.3.tar` & `auto-codebase-documenter-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.3/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     8701 2023-05-22 01:27:45.000000 auto-codebase-documenter-0.3/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     5810 2023-05-22 01:04:32.000000 auto-codebase-documenter-0.3/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 01:40:24.000000 auto-codebase-documenter-0.3/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.3/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       64 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       21 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 01:46:27.000000 auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 01:46:27.111635 auto-codebase-documenter-0.3/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      929 2023-05-22 01:45:41.000000 auto-codebase-documenter-0.3/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.4/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     7698 2023-05-22 02:12:20.000000 auto-codebase-documenter-0.4/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     5814 2023-05-22 02:12:20.000000 auto-codebase-documenter-0.4/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 01:40:24.000000 auto-codebase-documenter-0.4/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.4/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       55 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 02:16:28.000000 auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 02:16:28.534676 auto-codebase-documenter-0.4/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      930 2023-05-22 02:15:56.000000 auto-codebase-documenter-0.4/setup.py
```

### Comparing `auto-codebase-documenter-0.3/LICENSE` & `auto-codebase-documenter-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.3/PKG-INFO` & `auto-codebase-documenter-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.3
+Version: 0.4
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.3/README.md` & `auto-codebase-documenter-0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,47 +13,14 @@
 
 ```bash
 pip install auto-codebase-documenter
 ```
 
 The package is hosted on PyPI and can be found at <https://pypi.org/project/auto-codebase-documenter>. You can visit the link for more information about the package and its available versions.
 
-## Configuration
-
-Edit the `config.yaml` file to configure the tool. The following parameters are available:
-
-- `override_ai_prompt`: A list of intentions you want the AI model to follow when it writes the documentation. This should follow a decent list of prompt items that should get the best out of the AI model.
-
-- `ignore_folders`: A list of directories that you want to exclude from the documentation process.
-
-- `file_types`: A list of file types (by extension) that you want to include in the documentation process.
-
-- `single_file`: A boolean indicating whether a single file should be processed. If True, provide the path to the file. Defaults to False.
-
-- `output_docs_folder_name`: The name of the output docs folder. Defaults to "docs".
-
-Alternatively, these parameters can be passed as command line arguments when running the tool. If command line arguments are provided, they will override the corresponding values in config.yaml.
-
-Here's an example of how your config.yaml could look:
-
-```yaml
-output_docs_folder_name: "docs"
-ignore_folders:
-  - "venv"
-file_types:
-  - ".py"
-single_file: False
-override_ai_prompt:
-  - "You are a highly skilled software engineer and software architect"
-  - "You are analysing another person's code and writing a report on each file in a codebase"
-  - "You will provide feedback for each file and suggest improvements where necessary"
-  - "Please give a detailed account of how every Class, method, decorator, and important variable works in the code and its intention"
-  - "Lay everything out so a new developer can really understand what the code is supposed to do"
-```
-
 ## Setup
 
 Before you start using Auto Codebase Documenter, you need to set up a suitable Python environment. We recommend using a virtual environment (venv). Here's how you can set this up:
 
 1. Install Python 3.9.16. You can download it from the official Python website. Make sure to allow the installer to set the PATH variables for you.
 
 2. Check your Python version by running `python --version` or `python3 --version` from the command line. It should display `Python 3.9.16`.
@@ -88,65 +55,78 @@
 
 6. Now you should be all set! Remember to activate the venv environment every time you work on the project.
 
 7. Finally, ensure you have an OpenAI API key. The API key is necessary for making requests to the OpenAI service.
 
 ## Usage
 
-The easiest way to configure the app is by editing the `config.yaml` file. Once you have configured the app, you can run it by executing the following command:
+### Importing the package
 
-```bash
-python run.py
-```
+The easiest way to use the tool is to create a file called `documenter.py` and add the following code to run the app by importing the `AutoCodebaseDocumenter` class:
 
-The command line arguments can also be provided to override the settings in `config.yaml`. For example:
+```python
+import os
+from dotenv import load_dotenv
+from auto_codebase_documenter import AutoCodebaseDocumenter
 
-```bash
-python run.py --codebase_path /home/alex/projects/test_project --ignore_folders venv another_folder --file_types .py .yaml --output_docs_folder_name docs
+load_dotenv()  # load .env file
+openai_api_key = os.getenv("OPENAI_KEY")  # get OPENAI_KEY value from .env file{}
+
+documenter = AutoCodebaseDocumenter(openai_api_key)
+documenter.process_all_files()
 ```
 
-In the above command:
+The `process_all_files` method will start processing the files.
 
-- `/home/alex/projects/test_project` is the path of the root directory of the codebase that you want to document.
-- `venv another_folder` is a list of directories that you want to exclude from the documentation process.
-- `.py .yaml` is a list of file types that you want to include in the documentation process.
-- `docs` is the name of the output docs folder.
+You can add the `documenter_config.yaml` into the same folder to customize the tool.
 
-Alternatively, you can use the following code to run the app by importing the `AutoCodebaseDocumenter` class:
+### CLI
 
-```python
-from auto_codebase_documenter import AutoCodebaseDocumenter
+TODO: Add CLI usage instructions
 
-documenter = AutoCodebaseDocumenter(
-  'your_openai_api_key',
-  '/home/alex/projects/test_project',
-  'docs',
-  ['venv', 'another_folder'],
-  ['.py', '.yaml']
-)
-documenter.process_all_files()
-```
+## Configuration
 
-In the above code:
+Edit the `documenter_config.yaml` file to configure the tool. The following parameters are available:
 
-- Replace `your_openai_api_key` with your actual OpenAI API key.
-- `/home/alex/projects/test_project` is the path of the root directory of the codebase that you want to document.
-- `docs` is the name of the output docs folder.
-- `['venv', 'another_folder']` is a list of directories that you want to exclude from the documentation process.
-- `['.py', '.yaml']` is a list of file types that you want to include in the documentation process.
+- `override_ai_prompt`: A list of intentions you want the AI model to follow when it writes the documentation. This should follow a decent list of prompt items that should get the best out of the AI model.
 
-The `process_all_files` method will start processing the files.
+- `ignore_folders`: A list of directories that you want to exclude from the documentation process.
+
+- `file_types`: A list of file types (by extension) that you want to include in the documentation process.
+
+- `single_file`: A boolean indicating whether a single file should be processed. If True, provide the path to the file. Defaults to False.
+
+- `output_docs_folder_name`: The name of the output docs folder. Defaults to "docs".
+
+Alternatively, these parameters can be passed as command line arguments when running the tool. If command line arguments are provided, they will override the corresponding values in documenter_config.yaml.
+
+Here's an example of how your documenter_config.yaml could look:
+
+```yaml
+output_docs_folder_name: "docs"
+ignore_folders:
+  - "venv"
+file_types:
+  - ".py"
+single_file: False
+override_ai_prompt:
+  - "You are a highly skilled software engineer and software architect"
+  - "You are analysing another person's code and writing a report on each file in a codebase"
+  - "You will provide feedback for each file and suggest improvements where necessary"
+  - "Please give a detailed account of how every Class, method, decorator, and important variable works in the code and its intention"
+  - "Lay everything out so a new developer can really understand what the code is supposed to do"
+```
 
 ## Output
 
 This tool will create a `docs` directory at the root path of the project or to the location specified by the `output_docs_folder_name` parameter. The structure of the `docs` directory will mimic the structure of your codebase. For each processed file in your codebase, there will be a corresponding `.md` (Markdown) file in the `docs` directory, placed in the same relative location as the original file in the codebase.
 
 The name of the Markdown file will be the same as the name of the processed file in the codebase, retaining the original file extension as part of the name. For example, if the original file was named `main.py`, the corresponding documentation file will be named `main.py.md`.
 
-Each Markdown file will contain an AI-generated assessment of the code in the corresponding file. The assessment is created using the GPT-4 model from OpenAI and follows the intentions specified in the `override_ai_prompt` parameter in `config.yaml`. It will provide an analysis of the code, suggestions for improvements, and detailed explanations of classes, methods, decorators, and important variables in the file.
+Each Markdown file will contain an AI-generated assessment of the code in the corresponding file. The assessment is created using the GPT-4 model from OpenAI and follows the intentions specified in the `override_ai_prompt` parameter in `documenter_config.yaml`. It will provide an analysis of the code, suggestions for improvements, and detailed explanations of classes, methods, decorators, and important variables in the file.
 
 The assessment aims to provide comprehensive information that can help a new developer understand the purpose and functionality of the code, as well as areas that could potentially be refactored or optimized.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `auto-codebase-documenter-0.3/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-0.4/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,39 +30,37 @@
         if not os.path.exists(self.docs_dir):
             os.makedirs(self.docs_dir)
 
         # Load config from file
         self._load_config()
 
     def _load_config(self):
-        # Check for config.yaml in the application's root directory
-        parent_dir = dirname(abspath(__file__))  # directory of the current script
-        root_dir = dirname(parent_dir)  # root directory of the application
+        module_dir = dirname(abspath(__file__))
+        config_file = os.path.join(module_dir, "documenter_config.yaml")
 
         try:
-            with open(os.path.join(root_dir, "config.yaml"), "r") as stream:
+            with open(config_file, "r") as stream:
                 config_data = yaml.safe_load(stream)
                 self.ai_prompt_text = config_data.get("override_ai_prompt", default_ai_prompt)
                 self.ignore_folders = config_data.get("ignore_folders", self.ignore_folders)
                 self.file_types = config_data.get("file_types", self.file_types)
                 # self.single_file = config_data.get("single_file", self.single_file)
-                print("Using the prompt override from 'config.yaml'.")
+                print("Using the prompt override from 'documenter_config.yaml'.")
                 print("Custom prompt is set to the following:")
                 print(self.ai_prompt_text)
         except FileNotFoundError:
-            print("Warning: 'config.yaml' file not found. Using default doc intentions.")
-
+            print("Warning: 'documenter_config.yaml' file not found. Using default ai prompt config.")
             self.ai_prompt_text = default_ai_prompt
         except KeyError:
-            print("Warning: 'override_ai_prompt' key not found in 'config.yaml'. Using default doc intentions.")
-
+            print(
+                "Warning: 'override_ai_prompt' key not found in 'documenter_config.yaml'. Using default ai prompt config."
+            )
             self.ai_prompt_text = default_ai_prompt
         except Exception as e:
-            print(f"Warning: Error reading 'config.yaml'. Using default doc intentions. Error: {str(e)}")
-
+            print(f"Warning: Error reading 'documenter_config.yaml'. Using default ai prompt config. Error: {str(e)}")
             self.ai_prompt_text = default_ai_prompt
 
     def _get_completion(self, prompt, model="gpt-3.5-turbo"):
         messages = [{"role": "user", "content": prompt}]
         response = openai.ChatCompletion.create(
             model=model,
             messages=messages,
@@ -112,15 +110,18 @@
 
             # Check if the file already exists
             if os.path.exists(output_file):
                 print(f"WARNING: Documentation file {output_file} already exists and will be overwritten.")
 
             with open(output_file, "w") as output:
                 # Add timestamp at the top of the file
-                print("# Auto generated documentation file from auto-codebase-documenter\n", file=output)
+                print(
+                    "# Auto generated documentation file from auto-codebase-documenter\n",
+                    file=output,
+                )
                 timestamp = datetime.now().strftime("%d %B %Y at %H:%M:%S")
                 print(f"This documentation file was created on {timestamp}\n", file=output)
 
                 print("## File path\n", file=output)
                 print(f"{file_path}\n", file=output)
                 response = self._get_completion(prompt)
                 print(response, file=output)
```

### Comparing `auto-codebase-documenter-0.3/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-0.4/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.3/auto_codebase_documenter.egg-info/PKG-INFO` & `auto-codebase-documenter-0.4/auto_codebase_documenter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.3
+Version: 0.4
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.3/setup.py` & `auto-codebase-documenter-0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-codebase-documenter",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
-    install_requires=["openai", "python-dotenv"],
+    install_requires=["openai", "python-dotenv", "PyYAML"],
     entry_points={
         "console_scripts": [
-            "auto-codebase-documenter = run:document_code",
+            "auto-codebase-documenter = run:main",
         ],
     },
     author="Alex Bryant",
     author_email="alexbryant710@gmail.com",
     description="Automatic codebase documentation tool using OpenAI GPT models",
     long_description="This tool utilizes OpenAI GPT models to automatically assess and document a codebase by generating written assessments for each file.",
     long_description_content_type="text/markdown",
```

