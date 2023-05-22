# Comparing `tmp/tigerblog-0.1.7.tar.gz` & `tmp/tigerblog-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigerblog-0.1.7.tar", last modified: Fri May 19 21:40:04 2023, max compression
+gzip compressed data, was "tigerblog-0.1.8.tar", last modified: Mon May 22 08:52:56 2023, max compression
```

## Comparing `tigerblog-0.1.7.tar` & `tigerblog-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-19 21:40:04.235322 tigerblog-0.1.7/
--rw-r--r--   0 user      (1000) user      (1000)    11358 2023-05-13 19:28:39.000000 tigerblog-0.1.7/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)       36 2023-05-17 08:15:37.000000 tigerblog-0.1.7/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)      842 2023-05-19 21:40:04.235322 tigerblog-0.1.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      358 2023-05-13 19:37:09.000000 tigerblog-0.1.7/README.md
--rw-r--r--   0 user      (1000) user      (1000)      344 2023-05-19 21:40:04.235322 tigerblog-0.1.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1035 2023-05-19 21:39:19.000000 tigerblog-0.1.7/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-19 21:40:04.231322 tigerblog-0.1.7/tigerblog/
--rw-r--r--   0 user      (1000) user      (1000)      162 2023-05-17 08:15:37.000000 tigerblog-0.1.7/tigerblog/config.json
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-19 21:40:04.230322 tigerblog-0.1.7/tigerblog/themes/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-19 21:40:04.233322 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/
--rw-r--r--   0 user      (1000) user      (1000)     1651 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/contact.html
--rw-r--r--   0 user      (1000) user      (1000)      372 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/listing.html
--rw-r--r--   0 user      (1000) user      (1000)      555 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/macros.html
--rw-r--r--   0 user      (1000) user      (1000)     3370 2023-05-13 21:02:45.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/master.html
--rw-r--r--   0 user      (1000) user      (1000)       94 2023-05-13 19:52:56.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/navlinks.html
--rw-r--r--   0 user      (1000) user      (1000)     6398 2023-05-19 21:25:29.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/post.html
--rw-r--r--   0 user      (1000) user      (1000)      211 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/sidebar.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-19 21:40:04.230322 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-19 21:40:04.234322 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/css/
--rw-r--r--   0 user      (1000) user      (1000)     3527 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/css/single-blog.css
--rw-r--r--   0 user      (1000) user      (1000)     6888 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/css/style.css
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-19 21:40:04.235322 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/
--rw-r--r--   0 user      (1000) user      (1000)    45454 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/aside-logo.svg
--rw-r--r--   0 user      (1000) user      (1000)     1150 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/favicon.ico
--rw-r--r--   0 user      (1000) user      (1000)    30029 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/logo-white.png
--rw-r--r--   0 user      (1000) user      (1000)   268427 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/logo.jpg
--rw-r--r--   0 user      (1000) user      (1000)    45423 2023-05-13 19:28:39.000000 tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/nav-logo.svg
--rwxr-xr-x   0 user      (1000) user      (1000)    11665 2023-05-19 21:39:10.000000 tigerblog-0.1.7/tigerblog/tigerblog.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-19 21:40:04.232322 tigerblog-0.1.7/tigerblog.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      842 2023-05-19 21:40:04.000000 tigerblog-0.1.7/tigerblog.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1056 2023-05-19 21:40:04.000000 tigerblog-0.1.7/tigerblog.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-19 21:40:04.000000 tigerblog-0.1.7/tigerblog.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       54 2023-05-19 21:40:04.000000 tigerblog-0.1.7/tigerblog.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)      108 2023-05-19 21:40:04.000000 tigerblog-0.1.7/tigerblog.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       10 2023-05-19 21:40:04.000000 tigerblog-0.1.7/tigerblog.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-13 20:05:19.000000 tigerblog-0.1.7/tigerblog.egg-info/zip-safe
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:52:56.086317 tigerblog-0.1.8/
+-rw-r--r--   0 user      (1000) user      (1000)    11358 2023-05-13 19:28:39.000000 tigerblog-0.1.8/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)       36 2023-05-17 08:15:37.000000 tigerblog-0.1.8/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)      842 2023-05-22 08:52:56.086317 tigerblog-0.1.8/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      358 2023-05-13 19:37:09.000000 tigerblog-0.1.8/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      344 2023-05-22 08:52:56.086317 tigerblog-0.1.8/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1035 2023-05-22 08:52:45.000000 tigerblog-0.1.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:52:56.080317 tigerblog-0.1.8/tigerblog/
+-rw-r--r--   0 user      (1000) user      (1000)      162 2023-05-17 08:15:37.000000 tigerblog-0.1.8/tigerblog/config.json
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:52:56.079316 tigerblog-0.1.8/tigerblog/themes/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:52:56.083317 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/
+-rw-r--r--   0 user      (1000) user      (1000)     1651 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/contact.html
+-rw-r--r--   0 user      (1000) user      (1000)      372 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/listing.html
+-rw-r--r--   0 user      (1000) user      (1000)      555 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/macros.html
+-rw-r--r--   0 user      (1000) user      (1000)     3370 2023-05-13 21:02:45.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/master.html
+-rw-r--r--   0 user      (1000) user      (1000)       94 2023-05-13 19:52:56.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/navlinks.html
+-rw-r--r--   0 user      (1000) user      (1000)     6398 2023-05-19 21:25:29.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/post.html
+-rw-r--r--   0 user      (1000) user      (1000)      211 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/sidebar.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:52:56.079316 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:52:56.084317 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/css/
+-rw-r--r--   0 user      (1000) user      (1000)     3527 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/css/single-blog.css
+-rw-r--r--   0 user      (1000) user      (1000)     6888 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/css/style.css
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:52:56.085317 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/
+-rw-r--r--   0 user      (1000) user      (1000)    45454 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/aside-logo.svg
+-rw-r--r--   0 user      (1000) user      (1000)     1150 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/favicon.ico
+-rw-r--r--   0 user      (1000) user      (1000)    30029 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/logo-white.png
+-rw-r--r--   0 user      (1000) user      (1000)   268427 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/logo.jpg
+-rw-r--r--   0 user      (1000) user      (1000)    45423 2023-05-13 19:28:39.000000 tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/nav-logo.svg
+-rwxr-xr-x   0 user      (1000) user      (1000)    11665 2023-05-19 21:39:10.000000 tigerblog-0.1.8/tigerblog/tigerblog.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:52:56.082316 tigerblog-0.1.8/tigerblog.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      842 2023-05-22 08:52:56.000000 tigerblog-0.1.8/tigerblog.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1056 2023-05-22 08:52:56.000000 tigerblog-0.1.8/tigerblog.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-22 08:52:56.000000 tigerblog-0.1.8/tigerblog.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       54 2023-05-22 08:52:56.000000 tigerblog-0.1.8/tigerblog.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      108 2023-05-22 08:52:56.000000 tigerblog-0.1.8/tigerblog.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2023-05-22 08:52:56.000000 tigerblog-0.1.8/tigerblog.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-13 20:05:19.000000 tigerblog-0.1.8/tigerblog.egg-info/zip-safe
```

### Comparing `tigerblog-0.1.7/LICENSE.txt` & `tigerblog-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/PKG-INFO` & `tigerblog-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigerblog
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simplest Blog Engine for Developers
 Home-page: https://github.com/tigerteamx/tigerblog
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: blog,productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tigerblog-0.1.7/setup.py` & `tigerblog-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name="tigerblog",
     packages=["tigerblog"],
     package_dir={"tigerblog": "tigerblog"},
     package_data={
         'tigerblog': ['config.json', 'themes/*'],
         'tigerblog.themes.abc': ["**"],
     },
-    version="0.1.7",
+    version="0.1.8",
     author="Martin F",
     author_email="pypi.org@tigerteamx.com",
     description="Simplest Blog Engine for Developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tigerteamx/tigerblog",
     install_requires=[],  # Used for dependencies
```

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/contact.html` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/contact.html`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/macros.html` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/macros.html`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/master.html` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/master.html`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/post.html` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/post.html`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/css/single-blog.css` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/css/single-blog.css`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/css/style.css` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/css/style.css`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/aside-logo.svg` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/aside-logo.svg`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/favicon.ico` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/logo-white.png` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/logo-white.png`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/logo.jpg` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/themes/beautiful-tiger/static/images/nav-logo.svg` & `tigerblog-0.1.8/tigerblog/themes/beautiful-tiger/static/images/nav-logo.svg`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog/tigerblog.py` & `tigerblog-0.1.8/tigerblog/tigerblog.py`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.7/tigerblog.egg-info/PKG-INFO` & `tigerblog-0.1.8/tigerblog.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigerblog
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simplest Blog Engine for Developers
 Home-page: https://github.com/tigerteamx/tigerblog
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: blog,productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tigerblog-0.1.7/tigerblog.egg-info/SOURCES.txt` & `tigerblog-0.1.8/tigerblog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

