# Comparing `tmp/template-pptx-jinja-fix-0.0.5.tar.gz` & `tmp/template-pptx-jinja-fix-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template-pptx-jinja-fix-0.0.5.tar", last modified: Mon May 22 07:52:49 2023, max compression
+gzip compressed data, was "template-pptx-jinja-fix-0.0.6.tar", last modified: Mon May 22 07:59:06 2023, max compression
```

## Comparing `template-pptx-jinja-fix-0.0.5.tar` & `template-pptx-jinja-fix-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:52:49.933121 template-pptx-jinja-fix-0.0.5/
--rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 07:52:49.932818 template-pptx-jinja-fix-0.0.5/PKG-INFO
--rw-r--r--   0 luxiangwang   (501) staff       (20)       38 2023-05-22 07:52:49.933225 template-pptx-jinja-fix-0.0.5/setup.cfg
--rw-r--r--   0 luxiangwang   (501) staff       (20)     1067 2023-05-22 07:52:33.000000 template-pptx-jinja-fix-0.0.5/setup.py
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:52:49.928925 template-pptx-jinja-fix-0.0.5/template_pptx_jinja/
--rw-r--r--   0 luxiangwang   (501) staff       (20)        0 2023-05-18 09:12:39.000000 template-pptx-jinja-fix-0.0.5/template_pptx_jinja/__init__.py
--rw-r--r--   0 luxiangwang   (501) staff       (20)      639 2023-05-22 06:07:12.000000 template-pptx-jinja-fix-0.0.5/template_pptx_jinja/pictures.py
--rw-r--r--   0 luxiangwang   (501) staff       (20)     2536 2023-05-22 03:57:59.000000 template-pptx-jinja-fix-0.0.5/template_pptx_jinja/render.py
-drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:52:49.932257 template-pptx-jinja-fix-0.0.5/template_pptx_jinja_fix.egg-info/
--rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 07:52:49.000000 template-pptx-jinja-fix-0.0.5/template_pptx_jinja_fix.egg-info/PKG-INFO
--rw-r--r--   0 luxiangwang   (501) staff       (20)      336 2023-05-22 07:52:49.000000 template-pptx-jinja-fix-0.0.5/template_pptx_jinja_fix.egg-info/SOURCES.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)        1 2023-05-22 07:52:49.000000 template-pptx-jinja-fix-0.0.5/template_pptx_jinja_fix.egg-info/dependency_links.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)       54 2023-05-22 07:52:49.000000 template-pptx-jinja-fix-0.0.5/template_pptx_jinja_fix.egg-info/requires.txt
--rw-r--r--   0 luxiangwang   (501) staff       (20)       20 2023-05-22 07:52:49.000000 template-pptx-jinja-fix-0.0.5/template_pptx_jinja_fix.egg-info/top_level.txt
+drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:59:06.737046 template-pptx-jinja-fix-0.0.6/
+-rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 07:59:06.736627 template-pptx-jinja-fix-0.0.6/PKG-INFO
+-rw-r--r--   0 luxiangwang   (501) staff       (20)       38 2023-05-22 07:59:06.737208 template-pptx-jinja-fix-0.0.6/setup.cfg
+-rw-r--r--   0 luxiangwang   (501) staff       (20)     1086 2023-05-22 07:59:00.000000 template-pptx-jinja-fix-0.0.6/setup.py
+drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:59:06.733082 template-pptx-jinja-fix-0.0.6/template_pptx_jinja/
+-rw-r--r--   0 luxiangwang   (501) staff       (20)        0 2023-05-18 09:12:39.000000 template-pptx-jinja-fix-0.0.6/template_pptx_jinja/__init__.py
+-rw-r--r--   0 luxiangwang   (501) staff       (20)      639 2023-05-22 06:07:12.000000 template-pptx-jinja-fix-0.0.6/template_pptx_jinja/pictures.py
+-rw-r--r--   0 luxiangwang   (501) staff       (20)     2536 2023-05-22 03:57:59.000000 template-pptx-jinja-fix-0.0.6/template_pptx_jinja/render.py
+drwxr-xr-x   0 luxiangwang   (501) staff       (20)        0 2023-05-22 07:59:06.735968 template-pptx-jinja-fix-0.0.6/template_pptx_jinja_fix.egg-info/
+-rw-r--r--   0 luxiangwang   (501) staff       (20)     1250 2023-05-22 07:59:06.000000 template-pptx-jinja-fix-0.0.6/template_pptx_jinja_fix.egg-info/PKG-INFO
+-rw-r--r--   0 luxiangwang   (501) staff       (20)      336 2023-05-22 07:59:06.000000 template-pptx-jinja-fix-0.0.6/template_pptx_jinja_fix.egg-info/SOURCES.txt
+-rw-r--r--   0 luxiangwang   (501) staff       (20)        1 2023-05-22 07:59:06.000000 template-pptx-jinja-fix-0.0.6/template_pptx_jinja_fix.egg-info/dependency_links.txt
+-rw-r--r--   0 luxiangwang   (501) staff       (20)       54 2023-05-22 07:59:06.000000 template-pptx-jinja-fix-0.0.6/template_pptx_jinja_fix.egg-info/requires.txt
+-rw-r--r--   0 luxiangwang   (501) staff       (20)       20 2023-05-22 07:59:06.000000 template-pptx-jinja-fix-0.0.6/template_pptx_jinja_fix.egg-info/top_level.txt
```

### Comparing `template-pptx-jinja-fix-0.0.5/PKG-INFO` & `template-pptx-jinja-fix-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-fix
-Version: 0.0.5
+Version: 0.0.6
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: wlx
 Author-email: 409673593@qq.com
 License: UNKNOWN
 Description: # Template pptx Jinja2
```

### Comparing `template-pptx-jinja-fix-0.0.5/setup.py` & `template-pptx-jinja-fix-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     # if os.path.exists(filename):
     with open(filename, 'r', encoding='utf-8') as myfile:
         return myfile.read()
     # else:
     #     return ""
 
 setup(name='template-pptx-jinja-fix',
-    version="0.0.5",
+    version="0.0.6",
     description='PowerPoint presentation builder from template using Jinja2',
     long_description=read('readme.md'),
     long_description_content_type='text/markdown',
     url='https://github.com/macheal/template-pptx-jinja',
     author='wlx',
     author_email='409673593@qq.com',
     install_requires=read('requirements.txt').split(),
     license='',
     packages=find_packages(),
     package_data={
-        '': ['readme.md','requirements.txt'],
+        'template-pptx-jinja': ['readme.md','requirements.txt'],
     },
     keywords=['powerpoint', 'ppt', 'pptx', 'template'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Topic :: Utilities",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `template-pptx-jinja-fix-0.0.5/template_pptx_jinja/pictures.py` & `template-pptx-jinja-fix-0.0.6/template_pptx_jinja/pictures.py`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-fix-0.0.5/template_pptx_jinja/render.py` & `template-pptx-jinja-fix-0.0.6/template_pptx_jinja/render.py`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-fix-0.0.5/template_pptx_jinja_fix.egg-info/PKG-INFO` & `template-pptx-jinja-fix-0.0.6/template_pptx_jinja_fix.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-fix
-Version: 0.0.5
+Version: 0.0.6
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: wlx
 Author-email: 409673593@qq.com
 License: UNKNOWN
 Description: # Template pptx Jinja2
```

