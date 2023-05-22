# Comparing `tmp/auto-codebase-documenter-1.0.tar.gz` & `tmp/auto-codebase-documenter-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-1.0.tar", last modified: Mon May 22 07:09:32 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-1.1.tar", last modified: Mon May 22 08:10:48 2023, max compression
```

## Comparing `auto-codebase-documenter-1.0.tar` & `auto-codebase-documenter-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 07:09:32.548570 auto-codebase-documenter-1.0/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-1.0/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 07:09:32.548570 auto-codebase-documenter-1.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     9404 2023-05-22 06:42:01.000000 auto-codebase-documenter-1.0/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 07:09:32.548570 auto-codebase-documenter-1.0/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     6851 2023-05-22 07:07:32.000000 auto-codebase-documenter-1.0/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 05:41:30.000000 auto-codebase-documenter-1.0/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2792 2023-05-22 06:04:12.000000 auto-codebase-documenter-1.0/auto_codebase_documenter/auto_documenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-1.0/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 07:09:32.548570 auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 07:09:32.000000 auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      542 2023-05-22 07:09:32.000000 auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 07:09:32.000000 auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       92 2023-05-22 07:09:32.000000 auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 07:09:32.000000 auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       31 2023-05-22 07:09:32.000000 auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 07:09:32.548570 auto-codebase-documenter-1.0/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      990 2023-05-22 07:08:16.000000 auto-codebase-documenter-1.0/setup.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 07:09:32.548570 auto-codebase-documenter-1.0/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 06:43:49.000000 auto-codebase-documenter-1.0/tests/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1827 2023-05-22 07:07:32.000000 auto-codebase-documenter-1.0/tests/test_auto_documenter.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 08:10:48.552036 auto-codebase-documenter-1.1/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-1.1/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 08:10:48.552036 auto-codebase-documenter-1.1/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     9404 2023-05-22 06:42:01.000000 auto-codebase-documenter-1.1/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 08:10:48.552036 auto-codebase-documenter-1.1/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     7482 2023-05-22 08:09:56.000000 auto-codebase-documenter-1.1/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 05:41:30.000000 auto-codebase-documenter-1.1/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3658 2023-05-22 08:09:56.000000 auto-codebase-documenter-1.1/auto_codebase_documenter/auto_documenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-1.1/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 08:10:48.552036 auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      632 2023-05-22 08:10:48.000000 auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      542 2023-05-22 08:10:48.000000 auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 08:10:48.000000 auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       92 2023-05-22 08:10:48.000000 auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 08:10:48.000000 auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       31 2023-05-22 08:10:48.000000 auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 08:10:48.552036 auto-codebase-documenter-1.1/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      990 2023-05-22 08:10:26.000000 auto-codebase-documenter-1.1/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 08:10:48.552036 auto-codebase-documenter-1.1/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-22 06:43:49.000000 auto-codebase-documenter-1.1/tests/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1827 2023-05-22 07:07:32.000000 auto-codebase-documenter-1.1/tests/test_auto_documenter.py
```

### Comparing `auto-codebase-documenter-1.0/LICENSE` & `auto-codebase-documenter-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-1.0/PKG-INFO` & `auto-codebase-documenter-1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 1.0
+Version: 1.1
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-1.0/README.md` & `auto-codebase-documenter-1.1/README.md`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-1.0/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-1.1/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,23 +11,27 @@
         self,
         openai_api_key,
         root_path=".",
         output_docs_folder_name="docs",
         ignore_folders=["venv"],
         file_types=[".py"],
         single_file=False,
+        skip_existing=False,
         debug=False,
+        gpt_model="gpt-3.5-turbo",
     ):
         self.openai_api_key = openai_api_key
         self.root_path = root_path
         self.output_docs_folder_name = output_docs_folder_name
         self.ignore_folders = ignore_folders
         self.file_types = file_types
-        self.base_dir = root_path
-        self.docs_dir = os.path.join(self.base_dir, self.output_docs_folder_name)
+        self.skip_existing = skip_existing
+        self.gpt_model = gpt_model
+
+        self.docs_dir = os.path.join(self.root_path, self.output_docs_folder_name)
 
         openai.api_key = self.openai_api_key
 
         # Create the docs folder if it doesn't exist
         if not os.path.exists(self.docs_dir):
             os.makedirs(self.docs_dir)
 
@@ -87,18 +91,18 @@
             self.ai_prompt_text = default_ai_prompt
         except Exception as e:
             logging.warning(
                 f"Error reading 'documenter_config.yaml'. Using default AI prompt config. Error: {str(e)}"
             )
             self.ai_prompt_text = default_ai_prompt
 
-    def _get_completion(self, prompt, model="gpt-3.5-turbo"):
+    def _get_completion(self, prompt):
         messages = [{"role": "user", "content": prompt}]
         response = openai.ChatCompletion.create(
-            model=model,
+            model=self.gpt_model,
             messages=messages,
             temperature=0,  # this is the degree of randomness of the model's output
         )
         return response.choices[0].message["content"]
 
     def _get_file_paths(self):
         file_paths = []
@@ -128,45 +132,56 @@
 
             Please assess the following file:
 
             {prompt}
             """
 
             # Get the relative path of the file
-            relative_path = os.path.relpath(file_path, self.base_dir)
+            relative_path = os.path.relpath(file_path, self.root_path)
 
             # Create the directory structure in the docs folder
             output_dir = os.path.dirname(os.path.join(self.docs_dir, relative_path))
             os.makedirs(output_dir, exist_ok=True)
 
             # Define the output file path
             file_name = os.path.basename(file_path)
             output_file = os.path.join(output_dir, f"{file_name}.md")
 
             # Check if the file already exists
             if os.path.exists(output_file):
-                print(
-                    f"WARNING: Documentation file {output_file} already exists and will be overwritten."
-                )
+                if self.skip_existing:
+                    print(f"Skipping existing file: {output_file}")
+                    return True, "File already exists, skipping as per configuration"
+                else:
+                    print(
+                        f"WARNING: Documentation file {output_file} already exists and will be overwritten."
+                    )
 
             with open(output_file, "w") as output:
                 # Add timestamp at the top of the file
                 print(
                     "# Auto generated documentation file from auto-codebase-documenter\n",
                     file=output,
                 )
                 timestamp = datetime.now().strftime("%d %B %Y at %H:%M:%S")
                 print(
                     f"This documentation file was created on {timestamp}\n", file=output
                 )
 
                 print("## File path\n", file=output)
                 print(f"{file_path}\n", file=output)
-                response = self._get_completion(prompt)
-                print(response, file=output)
+
+                try:
+                    response = self._get_completion(prompt)
+                    print(response, file=output)
+                except openai.error.APIConnectionError:
+                    print(
+                        f"Error communicating with OpenAI for file {file_path}. Skipping this file."
+                    )
+                    return False, f"Error processing file {file_path}"
 
                 print(f"Wrote documentation file {output_file}")
 
             return True, "Processed file successfully"
 
     def process_all_files(self):
         file_paths = self._get_file_paths()
```

### Comparing `auto-codebase-documenter-1.0/auto_codebase_documenter/auto_documenter.py` & `auto-codebase-documenter-1.1/auto_codebase_documenter/auto_documenter.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,29 +18,39 @@
         print(
             f"Warning: Error reading 'documenter_config.yaml'. Using defaults. Error: {str(e)}"
         )
         return {}
 
 
 def document_code(
-    codebase_path, output_docs_folder_name, ignore_folders, file_types, single_file
+    codebase_path,
+    output_docs_folder_name,
+    ignore_folders,
+    file_types,
+    single_file,
+    skip_existing,
+    debug,
+    gpt_model,
 ):
     load_dotenv()  # load .env file
     openai_api_key = os.getenv("OPENAI_KEY")  # get OPENAI_KEY value from .env file
 
     if openai_api_key is None:
         raise ValueError("The OPENAI_KEY environment variable is required to proceed.")
 
     documenter = AutoCodebaseDocumenter(
         openai_api_key,
         codebase_path,
         output_docs_folder_name,
         ignore_folders,
         file_types,
         single_file,
+        skip_existing,
+        debug,
+        gpt_model,
     )
 
     if single_file:
         documenter.process_single_file(single_file)
     else:
         documenter.process_all_files()
 
@@ -59,14 +69,25 @@
     )
     parser.add_argument(
         "--ignore_folders", nargs="+", help="List of folders to ignore."
     )
     parser.add_argument(
         "--file_types", nargs="+", help="List of file types to document."
     )
+    parser.add_argument(
+        "--skip_existing",
+        action="store_true",
+        help="Skip existing documentation files.",
+    )
+    parser.add_argument("--debug", action="store_true", help="Enable debug logging.")
+    parser.add_argument(
+        "--gpt_model",
+        type=str,
+        help="The GPT model to use. E.g., gpt-3.5-turbo gpt-4",
+    )
     # parser.add_argument("--single_file", type=str, help="The path to a single file to document.")
     args = parser.parse_args()
 
     codebase_path = (
         args.codebase_path if args.codebase_path else config.get("codebase_path", ".")
     )
     ignore_folders = (
@@ -79,14 +100,28 @@
     )
     # single_file = args.single_file if args.single_file else config.get("single_file", False)
     output_docs_folder_name = (
         args.output_docs_folder_name
         if args.output_docs_folder_name
         else config.get("output_docs_folder_name", "docs")
     )
+    skip_existing = (
+        args.skip_existing if args.skip_existing else config.get("skip_existing", False)
+    )
+    debug = args.debug if args.debug else config.get("debug", False)
+    gpt_model = (
+        args.gpt_model if args.gpt_model else config.get("gpt_model", "gpt-3.5-turbo")
+    )
     document_code(
-        codebase_path, output_docs_folder_name, ignore_folders, file_types, False
+        codebase_path,
+        output_docs_folder_name,
+        ignore_folders,
+        file_types,
+        False,
+        skip_existing,
+        debug,
+        gpt_model,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `auto-codebase-documenter-1.0/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-1.1/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/PKG-INFO` & `auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 1.0
+Version: 1.1
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-1.0/auto_codebase_documenter.egg-info/SOURCES.txt` & `auto-codebase-documenter-1.1/auto_codebase_documenter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-1.0/setup.py` & `auto-codebase-documenter-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-codebase-documenter",
-    version="1.0",
+    version="1.1",
     packages=find_packages(),
     install_requires=["openai", "python-dotenv", "PyYAML"],
     entry_points={
         "console_scripts": [
             "auto-codebase-documenter = auto_codebase_documenter.auto_documenter:main",
         ],
     },
```

### Comparing `auto-codebase-documenter-1.0/tests/test_auto_documenter.py` & `auto-codebase-documenter-1.1/tests/test_auto_documenter.py`

 * *Files identical despite different names*

