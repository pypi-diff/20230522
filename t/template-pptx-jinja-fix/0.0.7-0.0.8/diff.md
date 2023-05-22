# Comparing `tmp/template-pptx-jinja-fix-0.0.7.tar.gz` & `tmp/template-pptx-jinja-fix-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template-pptx-jinja-fix-0.0.7.tar", last modified: Mon May 22 08:03:06 2023, max compression
+gzip compressed data, was "template-pptx-jinja-fix-0.0.8.tar", last modified: Mon May 22 08:16:48 2023, max compression
```

## Comparing `template-pptx-jinja-fix-0.0.7.tar` & `template-pptx-jinja-fix-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 08:03:06.333341 template-pptx-jinja-fix-0.0.7/
--rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 08:03:06.332883 template-pptx-jinja-fix-0.0.7/PKG-INFO
--rw-r--r--   0 luxiangwang   (501) staff       (20)       38 2023-05-22 08:03:06.333503 template-pptx-jinja-fix-0.0.7/setup.cfg
--rw-r--r--   0 luxiangwang   (501) staff       (20)     1187 2023-05-22 08:02:58.000000 template-pptx-jinja-fix-0.0.7/setup.py
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 08:03:06.329046 template-pptx-jinja-fix-0.0.7/template_pptx_jinja/
--rw-r--r--   0 luxiangwang   (501) staff       (20)        0 2023-05-18 09:12:39.000000 template-pptx-jinja-fix-0.0.7/template_pptx_jinja/__init__.py
--rw-r--r--   0 luxiangwang   (501) staff       (20)      639 2023-05-22 06:07:12.000000 template-pptx-jinja-fix-0.0.7/template_pptx_jinja/pictures.py
--rw-r--r--   0 luxiangwang   (501) staff       (20)     2536 2023-05-22 03:57:59.000000 template-pptx-jinja-fix-0.0.7/template_pptx_jinja/render.py
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 08:03:06.332178 template-pptx-jinja-fix-0.0.7/template_pptx_jinja_fix.egg-info/
--rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 08:03:06.000000 template-pptx-jinja-fix-0.0.7/template_pptx_jinja_fix.egg-info/PKG-INFO
--rw-r--r--   0 luxiangwang   (501) staff       (20)      336 2023-05-22 08:03:06.000000 template-pptx-jinja-fix-0.0.7/template_pptx_jinja_fix.egg-info/SOURCES.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)        1 2023-05-22 08:03:06.000000 template-pptx-jinja-fix-0.0.7/template_pptx_jinja_fix.egg-info/dependency_links.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)       54 2023-05-22 08:03:06.000000 template-pptx-jinja-fix-0.0.7/template_pptx_jinja_fix.egg-info/requires.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)       20 2023-05-22 08:03:06.000000 template-pptx-jinja-fix-0.0.7/template_pptx_jinja_fix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-22 08:16:48.112919 template-pptx-jinja-fix-0.0.8/
+-rw-r--r--   0 root         (0) staff       (20)     1250 2023-05-22 08:16:48.112235 template-pptx-jinja-fix-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-22 08:16:48.113112 template-pptx-jinja-fix-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1002 2023-05-22 08:16:01.000000 template-pptx-jinja-fix-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-22 08:16:48.108940 template-pptx-jinja-fix-0.0.8/template_pptx_jinja/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-18 09:12:39.000000 template-pptx-jinja-fix-0.0.8/template_pptx_jinja/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-05-22 06:07:12.000000 template-pptx-jinja-fix-0.0.8/template_pptx_jinja/pictures.py
+-rw-r--r--   0 root         (0) staff       (20)     2536 2023-05-22 03:57:59.000000 template-pptx-jinja-fix-0.0.8/template_pptx_jinja/render.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-22 08:16:48.111421 template-pptx-jinja-fix-0.0.8/template_pptx_jinja_fix.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1250 2023-05-22 08:16:47.000000 template-pptx-jinja-fix-0.0.8/template_pptx_jinja_fix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      336 2023-05-22 08:16:47.000000 template-pptx-jinja-fix-0.0.8/template_pptx_jinja_fix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-22 08:16:47.000000 template-pptx-jinja-fix-0.0.8/template_pptx_jinja_fix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       54 2023-05-22 08:16:47.000000 template-pptx-jinja-fix-0.0.8/template_pptx_jinja_fix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-05-22 08:16:47.000000 template-pptx-jinja-fix-0.0.8/template_pptx_jinja_fix.egg-info/top_level.txt
```

### Comparing `template-pptx-jinja-fix-0.0.7/PKG-INFO` & `template-pptx-jinja-fix-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-fix
-Version: 0.0.7
+Version: 0.0.8
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: wlx
 Author-email: 409673593@qq.com
 License: UNKNOWN
 Description: # Template pptx Jinja2
```

### Comparing `template-pptx-jinja-fix-0.0.7/setup.py` & `template-pptx-jinja-fix-0.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,34 +2,28 @@
 import os
 
 
 def read(filename):
     if os.path.exists(filename):
         with open(filename, 'r', encoding='utf-8') as myfile:
             return myfile.read()
-    else:
-        return ""
+
 
 setup(name='template-pptx-jinja-fix',
-    version="0.0.7",
+    version="0.0.8",
     description='PowerPoint presentation builder from template using Jinja2',
     long_description=read('readme.md'),
     long_description_content_type='text/markdown',
     url='https://github.com/macheal/template-pptx-jinja',
     author='wlx',
     author_email='409673593@qq.com',
-    install_requires=['Jinja2==3.1.2',
-                      'python_pptx==0.6.21',
-                      'templatepptx==0.0.8',
-                      ],
+    install_requires=read('requirements.txt').split(),
     license='',
     packages=find_packages(),
-    package_data={
-        'template-pptx-jinja': ['readme.md','requirements.txt'],
-    },
+    #include_package_data=True,
     keywords=['powerpoint', 'ppt', 'pptx', 'template'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Topic :: Utilities",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent"
```

### Comparing `template-pptx-jinja-fix-0.0.7/template_pptx_jinja/pictures.py` & `template-pptx-jinja-fix-0.0.8/template_pptx_jinja/pictures.py`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-fix-0.0.7/template_pptx_jinja/render.py` & `template-pptx-jinja-fix-0.0.8/template_pptx_jinja/render.py`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-fix-0.0.7/template_pptx_jinja_fix.egg-info/PKG-INFO` & `template-pptx-jinja-fix-0.0.8/template_pptx_jinja_fix.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-fix
-Version: 0.0.7
+Version: 0.0.8
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: wlx
 Author-email: 409673593@qq.com
 License: UNKNOWN
 Description: # Template pptx Jinja2
```

