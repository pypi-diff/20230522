# Comparing `tmp/beam-up-1.0.8.tar.gz` & `tmp/beam-up-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beam-up-1.0.8.tar", last modified: Mon May 18 14:52:31 2020, max compression
+gzip compressed data, was "dist/beam-up-1.0.9.tar", last modified: Wed May 27 20:04:42 2020, max compression
```

## Comparing `beam-up-1.0.8.tar` & `beam-up-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-18 14:52:31.000000 beam-up-1.0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      464 2020-05-18 14:52:31.000000 beam-up-1.0.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam/loaders/
--rw-rw-r--   0 travis    (2000) travis    (2000)      298 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/loaders/file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       39 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/loaders/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/loaders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      295 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/context.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam/processors/
--rw-rw-r--   0 travis    (2000) travis    (2000)      967 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/processors/markdown.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3011 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/processors/jinja.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      697 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/processors/base.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      107 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/processors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/processors/plain.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10698 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/site.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2789 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam/builders/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4613 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/builders/pages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3671 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/builders/blog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      563 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/builders/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/builders/sitemap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      143 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/builders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2421 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/builders/static_files.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam/cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)      517 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/cli/up.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      530 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/cli/config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      526 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/cli/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/cli/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)       22 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1255 2020-05-18 14:52:09.000000 beam-up-1.0.8/beam/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      236 2020-05-18 14:52:09.000000 beam-up-1.0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam_up.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      464 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam_up.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam_up.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam_up.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam_up.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      731 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam_up.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       39 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam_up.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2020-05-18 14:52:31.000000 beam-up-1.0.8/beam_up.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-05-18 14:52:31.000000 beam-up-1.0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      837 2020-05-18 14:52:09.000000 beam-up-1.0.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-27 20:04:42.000000 beam-up-1.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      464 2020-05-27 20:04:42.000000 beam-up-1.0.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam/loaders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      298 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/loaders/file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       39 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/loaders/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/loaders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      295 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/context.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam/processors/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      967 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/processors/markdown.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4984 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/processors/jinja.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      793 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/processors/base.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      107 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/processors/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      127 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/processors/plain.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10698 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/site.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2789 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam/builders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4613 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/builders/pages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3671 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/builders/blog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      563 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/builders/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/builders/sitemap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      143 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/builders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2723 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/builders/static_files.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam/cli/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      517 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/cli/up.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      530 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/cli/config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      526 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/cli/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/cli/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       22 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1255 2020-05-27 20:04:19.000000 beam-up-1.0.9/beam/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      236 2020-05-27 20:04:19.000000 beam-up-1.0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam_up.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      464 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam_up.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam_up.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam_up.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam_up.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      731 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam_up.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       39 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam_up.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2020-05-27 20:04:42.000000 beam-up-1.0.9/beam_up.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-05-27 20:04:42.000000 beam-up-1.0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      837 2020-05-27 20:04:19.000000 beam-up-1.0.9/setup.py
```

### Comparing `beam-up-1.0.8/beam/processors/markdown.py` & `beam-up-1.0.9/beam/processors/markdown.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/processors/base.py` & `beam-up-1.0.9/beam/processors/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
     def translate(self, key, *args, **kwargs):
         return self.site.translate(self.language, key, *args, **kwargs)
 
     def file(self, filename):
         return self.site.request('static_file', filename)
 
+    def source_path(self, filename):
+        return self.site.request('source_path', filename)
+
     def href(self, href, language=None):
         if language is None:
             language = self.language
         return self.site.href(language, href)
 
     def full_href(self, href, language=None):
         if language is None:
```

### Comparing `beam-up-1.0.8/beam/site.py` & `beam-up-1.0.9/beam/site.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/config.py` & `beam-up-1.0.9/beam/config.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/builders/pages.py` & `beam-up-1.0.9/beam/builders/pages.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/builders/blog.py` & `beam-up-1.0.9/beam/builders/blog.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/builders/base.py` & `beam-up-1.0.9/beam/builders/base.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/builders/sitemap.py` & `beam-up-1.0.9/beam/builders/sitemap.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/builders/static_files.py` & `beam-up-1.0.9/beam/builders/static_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 class StaticFilesBuilder(BaseBuilder):
 
     def __init__(self, site):
         super().__init__(site)
         self._static_paths = None
         self.providers = {
-            'static_file' : self.get_path
+            'static_file' : self.get_path,
+            'source_path': self.get_source_path
         }
 
     def postprocess(self):
         self.copy_static_files()
 
     def copy_static_files(self):
         dirs = self.get_static_paths()
@@ -42,18 +43,27 @@
     def resolve_path(self, path):
         dirs = self.get_static_paths()
         for dir in dirs:
             full_path = os.path.join(dir, path)
             if os.path.exists(full_path):
                 return full_path
         logger.error("Path '{}' not found!".format(path))
-        return ''
+
+    def get_source_path(self, path):
+        dirs = self.get_static_paths()
+        for dir in dirs:
+            full_path = os.path.join(dir, path)
+            if os.path.exists(full_path):
+                return full_path
+
 
     def get_path(self, path):
         full_path = self.resolve_path(path)
+        if not full_path:
+            return
         return os.path.join(self.site.path, self.site.static_path, path)
 
     def get_static_paths(self):
         if self._static_paths is not None:
             return self._static_paths
         paths = [os.path.join(self.site.src_path, 'static')]
         for language in self.site.config.get('languages', {}):
```

### Comparing `beam-up-1.0.8/beam/cli/up.py` & `beam-up-1.0.9/beam/cli/up.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/cli/config.py` & `beam-up-1.0.9/beam/cli/config.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/cli/main.py` & `beam-up-1.0.9/beam/cli/main.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam/settings.py` & `beam-up-1.0.9/beam/settings.py`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/beam_up.egg-info/SOURCES.txt` & `beam-up-1.0.9/beam_up.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beam-up-1.0.8/setup.py` & `beam-up-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='beam-up',
     python_requires='>=3',
-    version='1.0.8',
+    version='1.0.9',
     author='Andreas Dewes - 7scientists',
     author_email='andreas.dewes@7scientists.com',
     license='MIT',
     url='https://github.com/adewes/beam',
     packages=find_packages(),
     package_data={'': ['*.ini']},
     include_package_data=True,
```

