# Comparing `tmp/template-pptx-jinja-fix-0.0.3.tar.gz` & `tmp/template-pptx-jinja-fix-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template-pptx-jinja-fix-0.0.3.tar", last modified: Mon May 22 07:39:09 2023, max compression
+gzip compressed data, was "template-pptx-jinja-fix-0.0.4.tar", last modified: Mon May 22 07:44:34 2023, max compression
```

## Comparing `template-pptx-jinja-fix-0.0.3.tar` & `template-pptx-jinja-fix-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:39:09.021798 template-pptx-jinja-fix-0.0.3/
--rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 07:39:09.021350 template-pptx-jinja-fix-0.0.3/PKG-INFO
--rw-r--r--   0 luxiangwang   (501) staff       (20)       38 2023-05-22 07:39:09.021965 template-pptx-jinja-fix-0.0.3/setup.cfg
--rw-r--r--   0 luxiangwang   (501) staff       (20)      921 2023-05-22 07:38:33.000000 template-pptx-jinja-fix-0.0.3/setup.py
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:39:09.017792 template-pptx-jinja-fix-0.0.3/template_pptx_jinja/
--rw-r--r--   0 luxiangwang   (501) staff       (20)        0 2023-05-18 09:12:39.000000 template-pptx-jinja-fix-0.0.3/template_pptx_jinja/__init__.py
--rw-r--r--   0 luxiangwang   (501) staff       (20)      639 2023-05-22 06:07:12.000000 template-pptx-jinja-fix-0.0.3/template_pptx_jinja/pictures.py
--rw-r--r--   0 luxiangwang   (501) staff       (20)     2536 2023-05-22 03:57:59.000000 template-pptx-jinja-fix-0.0.3/template_pptx_jinja/render.py
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:39:09.020474 template-pptx-jinja-fix-0.0.3/template_pptx_jinja_fix.egg-info/
--rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 07:39:08.000000 template-pptx-jinja-fix-0.0.3/template_pptx_jinja_fix.egg-info/PKG-INFO
--rw-r--r--   0 luxiangwang   (501) staff       (20)      336 2023-05-22 07:39:08.000000 template-pptx-jinja-fix-0.0.3/template_pptx_jinja_fix.egg-info/SOURCES.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)        1 2023-05-22 07:39:08.000000 template-pptx-jinja-fix-0.0.3/template_pptx_jinja_fix.egg-info/dependency_links.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)       54 2023-05-22 07:39:08.000000 template-pptx-jinja-fix-0.0.3/template_pptx_jinja_fix.egg-info/requires.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)       20 2023-05-22 07:39:08.000000 template-pptx-jinja-fix-0.0.3/template_pptx_jinja_fix.egg-info/top_level.txt
+drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:44:34.570748 template-pptx-jinja-fix-0.0.4/
+-rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 07:44:34.570372 template-pptx-jinja-fix-0.0.4/PKG-INFO
+-rw-r--r--   0 luxiangwang   (501) staff       (20)       38 2023-05-22 07:44:34.570862 template-pptx-jinja-fix-0.0.4/setup.cfg
+-rw-r--r--   0 luxiangwang   (501) staff       (20)      970 2023-05-22 07:43:56.000000 template-pptx-jinja-fix-0.0.4/setup.py
+drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:44:34.566761 template-pptx-jinja-fix-0.0.4/template_pptx_jinja/
+-rw-r--r--   0 luxiangwang   (501) staff       (20)        0 2023-05-18 09:12:39.000000 template-pptx-jinja-fix-0.0.4/template_pptx_jinja/__init__.py
+-rw-r--r--   0 luxiangwang   (501) staff       (20)      639 2023-05-22 06:07:12.000000 template-pptx-jinja-fix-0.0.4/template_pptx_jinja/pictures.py
+-rw-r--r--   0 luxiangwang   (501) staff       (20)     2536 2023-05-22 03:57:59.000000 template-pptx-jinja-fix-0.0.4/template_pptx_jinja/render.py
+drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:44:34.569723 template-pptx-jinja-fix-0.0.4/template_pptx_jinja_fix.egg-info/
+-rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 07:44:34.000000 template-pptx-jinja-fix-0.0.4/template_pptx_jinja_fix.egg-info/PKG-INFO
+-rw-r--r--   0 luxiangwang   (501) staff       (20)      336 2023-05-22 07:44:34.000000 template-pptx-jinja-fix-0.0.4/template_pptx_jinja_fix.egg-info/SOURCES.txt
+-rw-r--r--   0 luxiangwang   (501) staff       (20)        1 2023-05-22 07:44:34.000000 template-pptx-jinja-fix-0.0.4/template_pptx_jinja_fix.egg-info/dependency_links.txt
+-rw-r--r--   0 luxiangwang   (501) staff       (20)       54 2023-05-22 07:44:34.000000 template-pptx-jinja-fix-0.0.4/template_pptx_jinja_fix.egg-info/requires.txt
+-rw-r--r--   0 luxiangwang   (501) staff       (20)       20 2023-05-22 07:44:34.000000 template-pptx-jinja-fix-0.0.4/template_pptx_jinja_fix.egg-info/top_level.txt
```

### Comparing `template-pptx-jinja-fix-0.0.3/PKG-INFO` & `template-pptx-jinja-fix-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-fix
-Version: 0.0.3
+Version: 0.0.4
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: wlx
 Author-email: 409673593@qq.com
 License: UNKNOWN
 Description: # Template pptx Jinja2
```

### Comparing `template-pptx-jinja-fix-0.0.3/setup.py` & `template-pptx-jinja-fix-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
+import os
 
 
 def read(filename):
-    with open(filename, 'r', encoding='utf-8') as myfile:
-        return myfile.read()
+    if os.path.exists(filename):
+        with open(filename, 'r', encoding='utf-8') as myfile:
+            return myfile.read()
 
 
 setup(name='template-pptx-jinja-fix',
-    version="0.0.3",
+    version="0.0.4",
     description='PowerPoint presentation builder from template using Jinja2',
-    long_description=read('./readme.md'),
+    long_description=read('readme.md'),
     long_description_content_type='text/markdown',
     url='https://github.com/macheal/template-pptx-jinja',
     author='wlx',
     author_email='409673593@qq.com',
     install_requires=read('requirements.txt').split(),
     license='',
     packages=find_packages(),
```

### Comparing `template-pptx-jinja-fix-0.0.3/template_pptx_jinja/pictures.py` & `template-pptx-jinja-fix-0.0.4/template_pptx_jinja/pictures.py`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-fix-0.0.3/template_pptx_jinja/render.py` & `template-pptx-jinja-fix-0.0.4/template_pptx_jinja/render.py`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-fix-0.0.3/template_pptx_jinja_fix.egg-info/PKG-INFO` & `template-pptx-jinja-fix-0.0.4/template_pptx_jinja_fix.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-fix
-Version: 0.0.3
+Version: 0.0.4
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: wlx
 Author-email: 409673593@qq.com
 License: UNKNOWN
 Description: # Template pptx Jinja2
```

