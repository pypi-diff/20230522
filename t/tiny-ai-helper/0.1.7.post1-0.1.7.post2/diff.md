# Comparing `tmp/tiny_ai_helper-0.1.7.post1.tar.gz` & `tmp/tiny_ai_helper-0.1.7.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_ai_helper-0.1.7.post1.tar", last modified: Tue May  2 09:20:17 2023, max compression
+gzip compressed data, was "tiny_ai_helper-0.1.7.post2.tar", last modified: Mon May 22 15:10:22 2023, max compression
```

## Comparing `tiny_ai_helper-0.1.7.post1.tar` & `tiny_ai_helper-0.1.7.post2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.7.post1/LICENSE
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      790 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.7.post1/README.md
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/setup.cfg
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1031 2023-05-02 09:19:12.000000 tiny_ai_helper-0.1.7.post1/setup.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    14107 2023-05-01 18:50:11.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/Model.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    10452 2023-04-30 10:47:53.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/Trainer.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      369 2023-05-02 09:19:24.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/__init__.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/layers.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/mp.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    19915 2023-05-02 09:14:39.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/utils.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      790 2023-05-02 09:20:17.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-05-02 09:20:17.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-02 09:20:17.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-02 09:20:17.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/top_level.txt
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-22 15:10:22.059851 tiny_ai_helper-0.1.7.post2/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.7.post2/LICENSE
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      790 2023-05-22 15:10:22.055851 tiny_ai_helper-0.1.7.post2/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.7.post2/README.md
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-22 15:10:22.059851 tiny_ai_helper-0.1.7.post2/setup.cfg
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1031 2023-05-22 15:08:47.000000 tiny_ai_helper-0.1.7.post2/setup.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-22 15:10:22.055851 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    14107 2023-05-01 18:50:11.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/Model.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    10452 2023-04-30 10:47:53.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/Trainer.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      369 2023-05-22 15:08:38.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/__init__.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/layers.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/mp.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    20035 2023-05-22 13:38:21.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/utils.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-22 15:10:22.055851 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      790 2023-05-22 15:10:22.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-05-22 15:10:22.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-22 15:10:22.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-22 15:10:22.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/top_level.txt
```

### Comparing `tiny_ai_helper-0.1.7.post1/LICENSE` & `tiny_ai_helper-0.1.7.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7.post1/PKG-INFO` & `tiny_ai_helper-0.1.7.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny_ai_helper
-Version: 0.1.7.post1
+Version: 0.1.7.post2
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

### Comparing `tiny_ai_helper-0.1.7.post1/setup.py` & `tiny_ai_helper-0.1.7.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from setuptools import setup, find_packages
 from os.path import abspath, dirname, join
 
 setup(
 	name="tiny_ai_helper",
-	version="0.1.7-1",
+	version="0.1.7-2",
 	description="Tiny AI Helper for PyTorch",
 	long_description=open(join(abspath(dirname(__file__)), 'README.md'), encoding='utf-8').read(),
 	long_description_content_type='text/markdown',
 	author="Ildar Bikmamatov",
 	author_email="support@bayrell.org",
 	license="MIT License",
 	url = "https://github.com/bayrell/ai_helper",
```

### Comparing `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/Model.py` & `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/Model.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/Trainer.py` & `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/Trainer.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/layers.py` & `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/layers.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/mp.py` & `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/mp.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/utils.py` & `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,18 @@
 
 
 def tensor_size(t):
 
     """
     Returns tensor size
     """
-
+    
+    if not isinstance(t, torch.Tensor):
+        return 0, 0
+    
     sz = t.element_size()
     shape = t.shape
     params = 1
 
     for c in shape:
         params = params * c
 
@@ -494,25 +497,25 @@
                 "name": module.__class__.__name__,
                 "class_name": module.__class__.__module__ + "." + module.__class__.__name__,
                 "shape": output.shape,
                 "params": 0
             }
             
             # Get weight
-            if hasattr(module, "weight"):
+            if hasattr(module, "weight") and isinstance(module.weight, torch.Tensor):
                 params, size = tensor_size(module.weight)
                 res["params_count"] += params
                 res["total_size"] += size
                 layer["params"] += params
                 
                 if module.weight.requires_grad:
                     res["params_train_count"] += params
             
             # Get bias
-            if hasattr(module, "bias"):
+            if hasattr(module, "bias") and isinstance(module.bias, torch.Tensor):
                 params, size = tensor_size(module.bias)
                 res["params_count"] += params
                 res["total_size"] += size
                 layer["params"] += params
                 
                 if module.bias.requires_grad:
                     res["params_train_count"] += params
@@ -582,15 +585,15 @@
         # Remove hooks
         for item in hooks:
             item.remove()
         
         res['total_size'] = round(res['total_size'] / 1024 / 1024 * 100) / 100
         
         # Calc info
-        values = [ ["", "Layer", "Output", "Params"] ]
+        values = []
         for i, layer in enumerate(layers):
             shape = layer["shape"]
             shape_str = ""
             if isinstance(shape, list):
                 shape = [ "(" + ", ".join(map(str,s)) + ")" for s in shape ]
                 shape_str = "[" + ", ".join(shape) + "]"
             else:
```

### Comparing `tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/PKG-INFO` & `tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-ai-helper
-Version: 0.1.7.post1
+Version: 0.1.7.post2
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

