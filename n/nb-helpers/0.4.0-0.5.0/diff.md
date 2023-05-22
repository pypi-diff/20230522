# Comparing `tmp/nb_helpers-0.4.0.tar.gz` & `tmp/nb_helpers-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_helpers-0.4.0.tar", last modified: Wed Mar 22 17:18:55 2023, max compression
+gzip compressed data, was "nb_helpers-0.5.0.tar", last modified: Mon May 22 15:19:20 2023, max compression
```

## Comparing `nb_helpers-0.4.0.tar` & `nb_helpers-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:18:55.637310 nb_helpers-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-03-22 17:18:55.637310 nb_helpers-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:18:55.637310 nb_helpers-0.4.0/nb_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/nb_helpers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:18:55.637310 nb_helpers-0.4.0/nb_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-03-22 17:18:55.000000 nb_helpers-0.4.0/nb_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-22 17:18:55.000000 nb_helpers-0.4.0/nb_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 17:18:55.000000 nb_helpers-0.4.0/nb_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-22 17:18:55.000000 nb_helpers-0.4.0/nb_helpers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 17:18:55.000000 nb_helpers-0.4.0/nb_helpers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-22 17:18:55.000000 nb_helpers-0.4.0/nb_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 17:18:55.000000 nb_helpers-0.4.0/nb_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 17:18:55.637310 nb_helpers-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-22 17:18:47.000000 nb_helpers-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:19:20.165432 nb_helpers-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-22 15:19:20.165432 nb_helpers-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:19:20.161432 nb_helpers-0.5.0/nb_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/nb_helpers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:19:20.165432 nb_helpers-0.5.0/nb_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-22 15:19:20.000000 nb_helpers-0.5.0/nb_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 15:19:20.000000 nb_helpers-0.5.0/nb_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:19:20.000000 nb_helpers-0.5.0/nb_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-22 15:19:20.000000 nb_helpers-0.5.0/nb_helpers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:19:20.000000 nb_helpers-0.5.0/nb_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 15:19:20.000000 nb_helpers-0.5.0/nb_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 15:19:20.000000 nb_helpers-0.5.0/nb_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:19:20.165432 nb_helpers-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-22 15:19:10.000000 nb_helpers-0.5.0/setup.py
```

### Comparing `nb_helpers-0.4.0/LICENSE` & `nb_helpers-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.4.0/PKG-INFO` & `nb_helpers-0.5.0/nb_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nb_helpers
-Version: 0.4.0
+Name: nb-helpers
+Version: 0.5.0
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.4.0/README.md` & `nb_helpers-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.4.0/nb_helpers/_modidx.py` & `nb_helpers-0.5.0/nb_helpers/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,21 @@
             'nb_helpers.colab': { 'nb_helpers.colab._create_colab_cell': ('colab.html#_create_colab_cell', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.add_colab_badge': ('colab.html#add_colab_badge', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.add_colab_metadata': ('colab.html#add_colab_metadata', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.create_colab_badge_cell': ('colab.html#create_colab_badge_cell', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.get_colab_url': ('colab.html#get_colab_url', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.has_colab_badge': ('colab.html#has_colab_badge', 'nb_helpers/colab.py')},
             'nb_helpers.docker': {},
+            'nb_helpers.export': { 'nb_helpers.export._export_code_cell': ('export.html#_export_code_cell', 'nb_helpers/export.py'),
+                                   'nb_helpers.export._export_md_cell': ('export.html#_export_md_cell', 'nb_helpers/export.py'),
+                                   'nb_helpers.export.colab_url': ('export.html#colab_url', 'nb_helpers/export.py'),
+                                   'nb_helpers.export.default_line_filter': ('export.html#default_line_filter', 'nb_helpers/export.py'),
+                                   'nb_helpers.export.export': ('export.html#export', 'nb_helpers/export.py'),
+                                   'nb_helpers.export.export_cell': ('export.html#export_cell', 'nb_helpers/export.py'),
+                                   'nb_helpers.export.filter_out_lines': ('export.html#filter_out_lines', 'nb_helpers/export.py')},
             'nb_helpers.run': { 'nb_helpers.run.CaptureShell.prettytb': ('run.html#captureshell.prettytb', 'nb_helpers/run.py'),
                                 'nb_helpers.run.exec_nb': ('run.html#exec_nb', 'nb_helpers/run.py'),
                                 'nb_helpers.run.run_nbs': ('run.html#run_nbs', 'nb_helpers/run.py'),
                                 'nb_helpers.run.run_one': ('run.html#run_one', 'nb_helpers/run.py'),
                                 'nb_helpers.run.skip_nb': ('run.html#skip_nb', 'nb_helpers/run.py')},
             'nb_helpers.utils': { 'nb_helpers.utils.RichLogger': ('utils.html#richlogger', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.RichLogger.__init__': ('utils.html#richlogger.__init__', 'nb_helpers/utils.py'),
```

### Comparing `nb_helpers-0.4.0/nb_helpers/actions.py` & `nb_helpers-0.5.0/nb_helpers/actions.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.4.0/nb_helpers/clean.py` & `nb_helpers-0.5.0/nb_helpers/clean.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.4.0/nb_helpers/colab.py` & `nb_helpers-0.5.0/nb_helpers/colab.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.4.0/nb_helpers/docker.py` & `nb_helpers-0.5.0/nb_helpers/docker.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.4.0/nb_helpers/run.py` & `nb_helpers-0.5.0/nb_helpers/run.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.4.0/nb_helpers/utils.py` & `nb_helpers-0.5.0/nb_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.4.0/nb_helpers/wandb.py` & `nb_helpers-0.5.0/nb_helpers/wandb.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 PYTHON_LIBS = "torch,keras,tensorflow,sklearn,yolo,jax,pandas,numpy,spacy,transformers,lightning,fastai"
 
 # %% ../nbs/01_wandb.ipynb 7
 def get_wandb_tracker(nb):
     "Get the value inside <!--- @wandbcode{tracker} -->"
     for cell in nb["cells"]:
         if "@wandbcode" in cell["source"]:
-            tracker_id = re.search(r"@wandbcode{(.*?)}", cell["source"]).group(1)
-            return tracker_id.split(",")[0]
+            match = re.search(r"@wandbcode{(.*?)}", cell["source"])
+            if match is not None:
+                tracker_id = match.group(1)  
+                return tracker_id.split(",")[0]
     return ""
 
 # %% ../nbs/01_wandb.ipynb 9
 def search_code(nb, features=WANDB_FEATURES):
     "Search notebook for features"
     present_features = []
     for feat in listify(features.split(",")):
@@ -65,14 +67,15 @@
 
     logger.info(f"Reading {len(files)} notebooks")
 
     repo_path = git_local_repo(files[0])
     branch = git_main_name(repo_path)
 
     for nb_path in files:
+        print(nb_path)
         nb = read_nb(nb_path)
         tracker_id = get_wandb_tracker(nb)
         fname = nb_path.name if not full_path else nb_path.relative_to(repo_path)
         features = search_code(nb, wandb_features)
         libs = detect_imported_libs(nb)
         colab_cell_idx = has_colab_badge(nb)
         row = [
```

### Comparing `nb_helpers-0.4.0/nb_helpers.egg-info/PKG-INFO` & `nb_helpers-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nb-helpers
-Version: 0.4.0
+Name: nb_helpers
+Version: 0.5.0
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.4.0/setup.py` & `nb_helpers-0.5.0/setup.py`

 * *Files identical despite different names*

