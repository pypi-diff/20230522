# Comparing `tmp/nb_helpers-0.5.1.tar.gz` & `tmp/nb_helpers-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_helpers-0.5.1.tar", last modified: Mon May 22 16:03:51 2023, max compression
+gzip compressed data, was "nb_helpers-0.5.2.tar", last modified: Mon May 22 16:44:20 2023, max compression
```

## Comparing `nb_helpers-0.5.1.tar` & `nb_helpers-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:03:51.008817 nb_helpers-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-22 16:03:51.008817 nb_helpers-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:03:51.008817 nb_helpers-0.5.1/nb_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/nb_helpers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:03:51.008817 nb_helpers-0.5.1/nb_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-22 16:03:50.000000 nb_helpers-0.5.1/nb_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 16:03:50.000000 nb_helpers-0.5.1/nb_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:03:50.000000 nb_helpers-0.5.1/nb_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-22 16:03:50.000000 nb_helpers-0.5.1/nb_helpers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:03:50.000000 nb_helpers-0.5.1/nb_helpers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 16:03:50.000000 nb_helpers-0.5.1/nb_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 16:03:50.000000 nb_helpers-0.5.1/nb_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:03:51.008817 nb_helpers-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-22 16:03:40.000000 nb_helpers-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/nb_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/nb_helpers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/nb_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 16:44:19.000000 nb_helpers-0.5.2/nb_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:44:20.022426 nb_helpers-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-22 16:44:08.000000 nb_helpers-0.5.2/setup.py
```

### Comparing `nb_helpers-0.5.1/LICENSE` & `nb_helpers-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/PKG-INFO` & `nb_helpers-0.5.2/nb_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nb_helpers
-Version: 0.5.1
+Name: nb-helpers
+Version: 0.5.2
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.5.1/README.md` & `nb_helpers-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/nb_helpers/_modidx.py` & `nb_helpers-0.5.2/nb_helpers/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,22 @@
                                   'nb_helpers.colab.add_colab_metadata': ('colab.html#add_colab_metadata', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.create_colab_badge_cell': ('colab.html#create_colab_badge_cell', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.get_colab_url': ('colab.html#get_colab_url', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.has_colab_badge': ('colab.html#has_colab_badge', 'nb_helpers/colab.py')},
             'nb_helpers.docker': {},
             'nb_helpers.export': { 'nb_helpers.export._export_code_cell': ('export.html#_export_code_cell', 'nb_helpers/export.py'),
                                    'nb_helpers.export._export_md_cell': ('export.html#_export_md_cell', 'nb_helpers/export.py'),
+                                   'nb_helpers.export._export_one': ('export.html#_export_one', 'nb_helpers/export.py'),
                                    'nb_helpers.export.colab_url': ('export.html#colab_url', 'nb_helpers/export.py'),
                                    'nb_helpers.export.default_line_filter': ('export.html#default_line_filter', 'nb_helpers/export.py'),
                                    'nb_helpers.export.export': ('export.html#export', 'nb_helpers/export.py'),
                                    'nb_helpers.export.export_cell': ('export.html#export_cell', 'nb_helpers/export.py'),
-                                   'nb_helpers.export.filter_out_lines': ('export.html#filter_out_lines', 'nb_helpers/export.py')},
+                                   'nb_helpers.export.export_nbs': ('export.html#export_nbs', 'nb_helpers/export.py'),
+                                   'nb_helpers.export.filter_out_lines': ('export.html#filter_out_lines', 'nb_helpers/export.py'),
+                                   'nb_helpers.export.read_list_file': ('export.html#read_list_file', 'nb_helpers/export.py')},
             'nb_helpers.run': { 'nb_helpers.run.CaptureShell.prettytb': ('run.html#captureshell.prettytb', 'nb_helpers/run.py'),
                                 'nb_helpers.run.exec_nb': ('run.html#exec_nb', 'nb_helpers/run.py'),
                                 'nb_helpers.run.run_nbs': ('run.html#run_nbs', 'nb_helpers/run.py'),
                                 'nb_helpers.run.run_one': ('run.html#run_one', 'nb_helpers/run.py'),
                                 'nb_helpers.run.skip_nb': ('run.html#skip_nb', 'nb_helpers/run.py')},
             'nb_helpers.utils': { 'nb_helpers.utils.RichLogger': ('utils.html#richlogger', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.RichLogger.__init__': ('utils.html#richlogger.__init__', 'nb_helpers/utils.py'),
```

### Comparing `nb_helpers-0.5.1/nb_helpers/actions.py` & `nb_helpers-0.5.2/nb_helpers/actions.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/nb_helpers/clean.py` & `nb_helpers-0.5.2/nb_helpers/clean.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/nb_helpers/colab.py` & `nb_helpers-0.5.2/nb_helpers/colab.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/nb_helpers/docker.py` & `nb_helpers-0.5.2/nb_helpers/docker.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/nb_helpers/export.py` & `nb_helpers-0.5.2/nb_helpers/export.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/06_export.ipynb.
 
 # %% auto 0
-__all__ = ['default_line_filter', 'filter_out_lines', 'export_cell', 'colab_url', 'export']
+__all__ = ['default_line_filter', 'filter_out_lines', 'export_cell', 'colab_url', 'export', 'read_list_file', 'export_nbs']
 
 # %% ../nbs/06_export.ipynb 3
 import os
 from pathlib import Path
 from rich.markdown import Markdown
 from fastcore.script import call_parse, Param, store_true
 
@@ -51,27 +51,64 @@
 # %% ../nbs/06_export.ipynb 12
 def colab_url(file):
     "Create a fresh colab URL from file, must be on github repo"
     url = get_colab_url(file, branch="master")
     return f'\n[![](https://colab.research.google.com/assets/colab-badge.svg)]({url})\n\n'
 
 # %% ../nbs/06_export.ipynb 17
+def _export_one(path, outfile, verbose=False):
+    
+    notebook = read_nb(path)
+    
+    cells = notebook["cells"]
+    
+    exported_cells = []
+    for cell in cells:
+        md_cell = export_cell(cell)
+        source = cell["source"]
+        if verbose:
+            print(f"=================\nInput: \n {source}")
+            print(f"-----------------\nMD: \n {md_cell}")
+        exported_cells.append(md_cell)
+    
+    with open(outfile, "w") as f:
+        f.writelines(exported_cells)
+
+# %% ../nbs/06_export.ipynb 18
 @call_parse
 def export(
     path: Param("A path to nb files", Path, nargs="?", opt=False) = os.getcwd(),
     verbose: Param("Print errors along the way", store_true) = False,
     outfile: Param("An output file to save") = None,
 ):
-    if is_nb(path):
-        notebook = read_nb(path)
-    else:
-        raise Error(f"This {path} is not a notebook!")
+    if not is_nb(path):
+        raise Exception(f"This {path} is not a notebook!")
     
     if outfile is None:
         outfile = path.with_suffix(".md")
         print(f"Exporting notebook {path} -> {outfile}")
     
-    cells = notebook["cells"]
-    export_cells = [export_cell(c) for c in cells]
+    _export_one(path, outfile, verbose)
+
+# %% ../nbs/06_export.ipynb 20
+def read_list_file(fname):
+    "Reads a file into a list"
+    with open(fname, "r") as f:
+        lines = f.readlines()
+        
+    return [Path(l.replace("\n", "")) for l in lines if l is not ""]
+
+# %% ../nbs/06_export.ipynb 21
+@call_parse
+def export_nbs(
+    file: Param("A text file containing a list of notebooks to export", Path),
+    verbose: Param("Print errors along the way", store_true) = False,
+    outpath: Param("An output folder to save the exported notebooks", Path) = Path(".") ,
+):
+    nb_paths = read_list_file(file)
     
-    with open(outfile, "w") as f:
-        f.writelines(export_cells)
+    for nb_path in nb_paths:
+        if not is_nb(nb_path):
+            raise Exception(f"This {nb_path} is not a notebook!")
+        outfile = outpath/(nb_path.with_suffix(".md").name)
+        print(f"Exporting notebook {nb_path} -> {outfile}")
+        _export_one(nb_path, outfile, verbose=verbose)
```

### Comparing `nb_helpers-0.5.1/nb_helpers/run.py` & `nb_helpers-0.5.2/nb_helpers/run.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/nb_helpers/utils.py` & `nb_helpers-0.5.2/nb_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/nb_helpers/wandb.py` & `nb_helpers-0.5.2/nb_helpers/wandb.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.1/nb_helpers.egg-info/PKG-INFO` & `nb_helpers-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nb-helpers
-Version: 0.5.1
+Name: nb_helpers
+Version: 0.5.2
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.5.1/setup.py` & `nb_helpers-0.5.2/setup.py`

 * *Files identical despite different names*

