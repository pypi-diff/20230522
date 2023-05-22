# Comparing `tmp/remyxai-0.1.1.tar.gz` & `tmp/remyxai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remyxai-0.1.1.tar", last modified: Tue Apr 25 14:41:46 2023, max compression
+gzip compressed data, was "remyxai-0.1.2.tar", last modified: Mon May 22 05:50:22 2023, max compression
```

## Comparing `remyxai-0.1.1.tar` & `remyxai-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 14:41:46.511942 remyxai-0.1.1/
--rw-rw-r--   0 funk      (1000) funk      (1000)     1065 2023-04-25 04:59:23.000000 remyxai-0.1.1/LICENSE
--rw-rw-r--   0 funk      (1000) funk      (1000)     2200 2023-04-25 14:41:46.511942 remyxai-0.1.1/PKG-INFO
--rw-rw-r--   0 funk      (1000) funk      (1000)     2086 2023-04-25 14:19:52.000000 remyxai-0.1.1/README.md
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 14:41:46.511942 remyxai-0.1.1/remyxai/
--rw-rw-r--   0 funk      (1000) funk      (1000)        0 2023-04-24 16:17:23.000000 remyxai-0.1.1/remyxai/__init__.py
--rw-rw-r--   0 funk      (1000) funk      (1000)     1490 2023-04-25 14:41:30.000000 remyxai-0.1.1/remyxai/api.py
--rw-rw-r--   0 funk      (1000) funk      (1000)     3222 2023-04-25 14:41:30.000000 remyxai-0.1.1/remyxai/cli.py
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 14:41:46.511942 remyxai-0.1.1/remyxai.egg-info/
--rw-rw-r--   0 funk      (1000) funk      (1000)     2200 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/PKG-INFO
--rw-rw-r--   0 funk      (1000) funk      (1000)      264 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/SOURCES.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)        1 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/dependency_links.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)       45 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/entry_points.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)        9 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/requires.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)        8 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/top_level.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)       38 2023-04-25 14:41:46.511942 remyxai-0.1.1/setup.cfg
--rw-rw-r--   0 funk      (1000) funk      (1000)      522 2023-04-25 14:41:30.000000 remyxai-0.1.1/setup.py
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-22 05:50:22.554465 remyxai-0.1.2/
+-rw-rw-r--   0 funk      (1000) funk      (1000)     1065 2023-04-25 04:59:23.000000 remyxai-0.1.2/LICENSE
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2565 2023-05-22 05:50:22.554465 remyxai-0.1.2/PKG-INFO
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2451 2023-05-22 05:49:17.000000 remyxai-0.1.2/README.md
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-22 05:50:22.550465 remyxai-0.1.2/remyxai/
+-rw-rw-r--   0 funk      (1000) funk      (1000)        0 2023-04-24 16:17:23.000000 remyxai-0.1.2/remyxai/__init__.py
+-rw-rw-r--   0 funk      (1000) funk      (1000)     1685 2023-05-22 02:50:15.000000 remyxai-0.1.2/remyxai/api.py
+-rw-rw-r--   0 funk      (1000) funk      (1000)     4343 2023-05-22 02:45:56.000000 remyxai-0.1.2/remyxai/cli.py
+-rw-rw-r--   0 funk      (1000) funk      (1000)     5721 2023-05-22 05:22:13.000000 remyxai-0.1.2/remyxai/utils.py
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-22 05:50:22.554465 remyxai-0.1.2/remyxai.egg-info/
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2565 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/PKG-INFO
+-rw-rw-r--   0 funk      (1000) funk      (1000)      281 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/SOURCES.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)        1 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/dependency_links.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)       45 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/entry_points.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)       44 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/requires.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)        8 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/top_level.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)       38 2023-05-22 05:50:22.554465 remyxai-0.1.2/setup.cfg
+-rw-rw-r--   0 funk      (1000) funk      (1000)      632 2023-05-22 01:31:37.000000 remyxai-0.1.2/setup.py
```

### Comparing `remyxai-0.1.1/LICENSE` & `remyxai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remyxai-0.1.1/PKG-INFO` & `remyxai-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remyxai
-Version: 0.1.1
+Version: 0.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Remyx AI command-line client
 
 ## Installation
 To install the Remyx AI CLI in Python virtual environment, run:
@@ -103,9 +103,23 @@
 * python command:
 ```python
 from remyxai.api import get_user_credits
 
 print(get_user_credits())
 ```
 
+### Utils
+*New!* Label images locally:
+* cli command:
+```
+$ remyxai utils label --labels="comma,separated,labels" --image_dir="/path/to/image/dir"
+```
 
+* python command:
+```
+from remyxai.utils import labeler
+model_name = "<your-model-name>"
+labels = ["comma", "separated", "labels"]
+image_dir = "/path/to/image/dir"
+print(labeler(labels, image_dir, model_name))
+```
```

### Comparing `remyxai-0.1.1/README.md` & `remyxai-0.1.2/remyxai.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: remyxai
+Version: 0.1.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Remyx AI command-line client
 
 ## Installation
 To install the Remyx AI CLI in Python virtual environment, run:
 
 ```
 pip install remyxai
@@ -97,9 +103,23 @@
 * python command:
 ```python
 from remyxai.api import get_user_credits
 
 print(get_user_credits())
 ```
 
+### Utils
+*New!* Label images locally:
+* cli command:
+```
+$ remyxai utils label --labels="comma,separated,labels" --image_dir="/path/to/image/dir"
+```
 
+* python command:
+```
+from remyxai.utils import labeler
+model_name = "<your-model-name>"
+labels = ["comma", "separated", "labels"]
+image_dir = "/path/to/image/dir"
+print(labeler(labels, image_dir, model_name))
+```
```

### Comparing `remyxai-0.1.1/remyxai/api.py` & `remyxai-0.1.2/remyxai/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,35 +14,41 @@
 
 # Models
 def list_models():
     url = f"{BASE_URL}model/list"
     response = requests.get(url, headers=HEADERS)
     return response.json()
 
-def delete_model(model_name):
+def get_model_summary(model_name):
+    url = f"{BASE_URL}model/summary/{model_name}"
+    response = requests.get(url, headers=HEADERS)
+    return response.json()
+
+def delete_model(model_name: str):
     url = f"{BASE_URL}model/delete/{model_name}"
     response = requests.post(url, headers=HEADERS)
     return response.json()
 
-def download_model(model_name, model_format):
+def download_model(model_name: str, model_format: str):
     url = f"{BASE_URL}model/download/{model_name}/{model_format}"
     response = requests.post(url, headers=HEADERS, stream=True)
     with open(f"{model_name}.zip", "wb") as out_file:
         shutil.copyfileobj(response.raw, out_file)
     return f"The file {model_name}.zip was saved successfully"
 
 # Engines
-def train_classifier(model_name, labels, model_selector):
+def train_classifier(model_name: str, labels: list, model_selector: str):
     url = f"{BASE_URL}task/classify/{model_name}/{','.join(labels)}/{model_selector}"
     response = requests.post(url, headers=HEADERS)
     return response.json()
 
 # User
 def get_user_profile():
     url = f"{BASE_URL}user"
     response = requests.get(url, headers=HEADERS)
     return response.json()
 
 def get_user_credits():
     url = f"{BASE_URL}user/credits"
     response = requests.get(url, headers=HEADERS)
     return response.json()
+
```

### Comparing `remyxai-0.1.1/remyxai/cli.py` & `remyxai-0.1.2/remyxai/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .api import *
+from .utils import labeler
 import argparse
 from pprint import pprint
 
 def main():
     parser = argparse.ArgumentParser(description="Model management script")
 
     # Define top-level actions
@@ -22,27 +23,39 @@
     download_parser.add_argument("--model_name", required=True, help="Name of the model to delete")
     download_parser.add_argument("--model_format", required=True, help="of the model to delete")
 
     # Define 'delete' subaction
     delete_parser = subparsers_model.add_parser("delete", help="Delete a model")
     delete_parser.add_argument("--model_name", required=True, help="Name of the model to delete")
 
-    # Define 'classify' subaction
+    # Define 'classify' action
     classify_parser = subparsers_action.add_parser("classify", help="Classifier-related actions")
     classify_parser.add_argument("--model_name", required=True, help="Name of the model")
     classify_parser.add_argument("--labels", required=True, help="Comma separated list of labels, e.g. 'cat,dog'")
     classify_parser.add_argument("--model_size", required=True, help="Integer value for model size from 1=small up to 5=large")
 
     # Define 'user' action
     user_parser = subparsers_action.add_parser("user", help="User-related actions")
 
     # Define subactions for 'user' action
     subparsers_user = user_parser.add_subparsers(dest="subaction", help="User subactions")
     profile_parser = subparsers_user.add_parser("profile", help="Get user profile")
     credits_parser = subparsers_user.add_parser("credits", help="Get user credits and subscription info if it exists")
+    
+    # Define 'utils' action
+    utils_parser = subparsers_action.add_parser("utils", help="Utility actions")
+    
+    # Define subactions for 'utils' action
+    subparsers_utils = utils_parser.add_subparsers(dest="subaction", help="Utility subactions")
+
+    # Define 'labeler' subaction
+    labeler_parser = subparsers_utils.add_parser("label", help="Extract labels from a directory of images")
+    labeler_parser.add_argument("--labels", required=True, help="Comma separated list of labels, e.g. 'cat,dog'")
+    labeler_parser.add_argument("--image_dir", required=True, help="Directory of images in '.jpg', '.jpeg', '.png' format")
+    labeler_parser.add_argument("--model_name", default=None, help="Name of the model")
 
     args = parser.parse_args()
 
     if args.action == "model":
         if args.subaction == "list":
             models = list_models()
             pprint(models)
@@ -52,23 +65,32 @@
         elif args.subaction == "download":
             downloaded_model = download_model(args.model_name, args.model_format)
             print(downloaded_model)
         else:
             print("Invalid argument for 'model'")
     elif args.action == "classify":
         labels = args.labels.split(",")
+        labels = [x.strip() for x in labels]
         training_classifier = train_classifier(args.model_name, labels, args.model_size)
         pprint(training_classifier) 
     elif args.action == "user":
         if args.subaction == "profile":
             profile = get_user_profile()
             pprint(profile)
         elif args.subaction == "credits":
             user_credits = get_user_credits()
             pprint(user_credits)
         else:
             print("Invalid argument for 'user'")
+    elif args.action == "utils":
+        if args.subaction == "label":
+            labels = args.labels.split(",")
+            labels = [x.strip() for x in labels]
+            results = labeler(labels, args.image_dir, args.model_name)
+            print(results)
+        else:
+            print("Invalid argument for 'utils'")
     else:
         print("Invalid action")
 
 if __name__ == "__main__":
     main()
```

### Comparing `remyxai-0.1.1/remyxai.egg-info/PKG-INFO` & `remyxai-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: remyxai
-Version: 0.1.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Remyx AI command-line client
 
 ## Installation
 To install the Remyx AI CLI in Python virtual environment, run:
 
 ```
 pip install remyxai
@@ -103,9 +97,23 @@
 * python command:
 ```python
 from remyxai.api import get_user_credits
 
 print(get_user_credits())
 ```
 
+### Utils
+*New!* Label images locally:
+* cli command:
+```
+$ remyxai utils label --labels="comma,separated,labels" --image_dir="/path/to/image/dir"
+```
 
+* python command:
+```
+from remyxai.utils import labeler
+model_name = "<your-model-name>"
+labels = ["comma", "separated", "labels"]
+image_dir = "/path/to/image/dir"
+print(labeler(labels, image_dir, model_name))
+```
```

### Comparing `remyxai-0.1.1/setup.py` & `remyxai-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,24 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="remyxai",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
-    install_requires=["requests"],
+    install_requires=[
+        "numpy",
+        "onnx", 
+        "onnxruntime",
+        "pillow",
+        "requests",
+        "tqdm",
+        ],
     entry_points={
         "console_scripts": [
             "remyxai=remyxai.cli:main",
         ],
     },
     long_description=long_description,
     long_description_content_type='text/markdown'
```

