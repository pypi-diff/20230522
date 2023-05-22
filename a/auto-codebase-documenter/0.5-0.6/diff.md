# Comparing `tmp/auto-codebase-documenter-0.5.tar.gz` & `tmp/auto-codebase-documenter-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-0.5.tar", last modified: Mon May 22 02:37:21 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-0.6.tar", last modified: Mon May 22 02:48:34 2023, max compression
```

## Comparing `auto-codebase-documenter-0.5.tar` & `auto-codebase-documenter-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.5/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     7698 2023-05-22 02:12:20.000000 auto-codebase-documenter-0.5/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     6083 2023-05-22 02:33:17.000000 auto-codebase-documenter-0.5/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 01:40:24.000000 auto-codebase-documenter-0.5/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.5/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       55 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 02:37:21.000000 auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 02:37:21.401154 auto-codebase-documenter-0.5/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      930 2023-05-22 02:37:13.000000 auto-codebase-documenter-0.5/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.6/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     7698 2023-05-22 02:12:20.000000 auto-codebase-documenter-0.6/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6036 2023-05-22 02:43:54.000000 auto-codebase-documenter-0.6/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 01:40:24.000000 auto-codebase-documenter-0.6/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.6/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      636 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       55 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 02:48:34.000000 auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 02:48:34.697793 auto-codebase-documenter-0.6/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      930 2023-05-22 02:48:12.000000 auto-codebase-documenter-0.6/setup.py
```

### Comparing `auto-codebase-documenter-0.5/LICENSE` & `auto-codebase-documenter-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.5/PKG-INFO` & `auto-codebase-documenter-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.5
+Version: 0.6
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.5/README.md` & `auto-codebase-documenter-0.6/README.md`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.5/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-0.6/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         self._load_config()
 
     def _setup_logging(self):
         log_level = logging.DEBUG if self.debug else logging.INFO
         logging.basicConfig(level=log_level)
 
     def _load_config(self):
-        module_dir = dirname(abspath(__file__))
-        config_file = os.path.join(module_dir, "documenter_config.yaml")
+        config_file = os.path.join(os.getcwd(), "documenter_config.yaml")
         logging.debug(f"Looking for config file at {config_file}")
 
         try:
             with open(config_file, "r") as stream:
                 config_data = yaml.safe_load(stream)
                 self.ai_prompt_text = config_data.get("override_ai_prompt", default_ai_prompt)
                 self.ignore_folders = config_data.get("ignore_folders", self.ignore_folders)
```

### Comparing `auto-codebase-documenter-0.5/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-0.6/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.5/auto_codebase_documenter.egg-info/PKG-INFO` & `auto-codebase-documenter-0.6/auto_codebase_documenter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-codebase-documenter
-Version: 0.5
+Version: 0.6
 Summary: Automatic codebase documentation tool using OpenAI GPT models
 Home-page: https://github.com/abryant710/auto-codebase-documenter
 Author: Alex Bryant
 Author-email: alexbryant710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto-codebase-documenter-0.5/setup.py` & `auto-codebase-documenter-0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-codebase-documenter",
-    version="0.5",
+    version="0.6",
     packages=find_packages(),
     install_requires=["openai", "python-dotenv", "PyYAML"],
     entry_points={
         "console_scripts": [
             "auto-codebase-documenter = run:main",
         ],
     },
```

