# Comparing `tmp/django-webpack-loader-1.8.1.tar.gz` & `tmp/django-webpack-loader-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webpack-loader-1.8.1.tar", last modified: Mon Feb  6 13:48:01 2023, max compression
+gzip compressed data, was "django-webpack-loader-2.0.0.tar", last modified: Mon May 22 12:26:10 2023, max compression
```

## Comparing `django-webpack-loader-1.8.1.tar` & `django-webpack-loader-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-02-06 13:48:01.582894 django-webpack-loader-1.8.1/
--rw-r--r--   0 renato    (1000) renato    (1000)     1078 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/LICENSE
--rw-r--r--   0 renato    (1000) renato    (1000)       34 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/MANIFEST.in
--rw-r--r--   0 renato    (1000) renato    (1000)    24812 2023-02-06 13:48:01.582894 django-webpack-loader-1.8.1/PKG-INFO
--rw-r--r--   0 renato    (1000) renato    (1000)    20099 2023-02-06 13:44:38.000000 django-webpack-loader-1.8.1/README.md
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-02-06 13:48:01.582894 django-webpack-loader-1.8.1/django_webpack_loader.egg-info/
--rw-r--r--   0 renato    (1000) renato    (1000)    24812 2023-02-06 13:48:01.000000 django-webpack-loader-1.8.1/django_webpack_loader.egg-info/PKG-INFO
--rw-r--r--   0 renato    (1000) renato    (1000)      589 2023-02-06 13:48:01.000000 django-webpack-loader-1.8.1/django_webpack_loader.egg-info/SOURCES.txt
--rw-r--r--   0 renato    (1000) renato    (1000)        1 2023-02-06 13:48:01.000000 django-webpack-loader-1.8.1/django_webpack_loader.egg-info/dependency_links.txt
--rw-r--r--   0 renato    (1000) renato    (1000)       66 2023-02-06 13:48:01.000000 django-webpack-loader-1.8.1/django_webpack_loader.egg-info/top_level.txt
--rw-r--r--   0 renato    (1000) renato    (1000)       80 2023-02-06 13:48:01.582894 django-webpack-loader-1.8.1/setup.cfg
--rw-r--r--   0 renato    (1000) renato    (1000)     1731 2022-12-09 12:03:45.000000 django-webpack-loader-1.8.1/setup.py
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-02-06 13:48:01.582894 django-webpack-loader-1.8.1/webpack_loader/
--rw-r--r--   0 renato    (1000) renato    (1000)      179 2023-02-06 13:45:41.000000 django-webpack-loader-1.8.1/webpack_loader/__init__.py
--rw-r--r--   0 renato    (1000) renato    (1000)      744 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/apps.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1016 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/config.py
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-02-06 13:48:01.582894 django-webpack-loader-1.8.1/webpack_loader/contrib/
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/contrib/__init__.py
--rw-r--r--   0 renato    (1000) renato    (1000)      481 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/contrib/jinja2ext.py
--rw-r--r--   0 renato    (1000) renato    (1000)      251 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/errors.py
--rw-r--r--   0 renato    (1000) renato    (1000)      700 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/exceptions.py
--rw-r--r--   0 renato    (1000) renato    (1000)     5162 2023-02-06 13:44:38.000000 django-webpack-loader-1.8.1/webpack_loader/loader.py
--rw-r--r--   0 renato    (1000) renato    (1000)       31 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/signals.py
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-02-06 13:48:01.582894 django-webpack-loader-1.8.1/webpack_loader/templatetags/
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/templatetags/__init__.py
--rw-r--r--   0 renato    (1000) renato    (1000)     2141 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/templatetags/webpack_loader.py
--rw-r--r--   0 renato    (1000) renato    (1000)     3840 2022-06-20 14:57:36.000000 django-webpack-loader-1.8.1/webpack_loader/utils.py
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/
+-rw-r--r--   0 renato    (1000) renato    (1000)     1078 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/LICENSE
+-rw-r--r--   0 renato    (1000) renato    (1000)       34 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/MANIFEST.in
+-rw-r--r--   0 renato    (1000) renato    (1000)    24842 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/PKG-INFO
+-rw-r--r--   0 renato    (1000) renato    (1000)    20129 2023-05-22 12:03:11.000000 django-webpack-loader-2.0.0/README.md
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/
+-rw-r--r--   0 renato    (1000) renato    (1000)    24842 2023-05-22 12:26:10.000000 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/PKG-INFO
+-rw-r--r--   0 renato    (1000) renato    (1000)      589 2023-05-22 12:26:10.000000 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)        1 2023-05-22 12:26:10.000000 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)       66 2023-05-22 12:26:10.000000 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/top_level.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)       80 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/setup.cfg
+-rw-r--r--   0 renato    (1000) renato    (1000)     1731 2022-12-09 12:03:45.000000 django-webpack-loader-2.0.0/setup.py
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/webpack_loader/
+-rw-r--r--   0 renato    (1000) renato    (1000)      179 2023-05-22 12:03:11.000000 django-webpack-loader-2.0.0/webpack_loader/__init__.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      744 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/apps.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1016 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/config.py
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/webpack_loader/contrib/
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/contrib/__init__.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      481 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/contrib/jinja2ext.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      251 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/errors.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      700 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/exceptions.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     5207 2023-05-19 19:41:04.000000 django-webpack-loader-2.0.0/webpack_loader/loader.py
+-rw-r--r--   0 renato    (1000) renato    (1000)       31 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/signals.py
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/webpack_loader/templatetags/
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/templatetags/__init__.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     2141 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/templatetags/webpack_loader.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     3840 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/utils.py
```

### Comparing `django-webpack-loader-1.8.1/LICENSE` & `django-webpack-loader-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-1.8.1/PKG-INFO` & `django-webpack-loader-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-webpack-loader
-Version: 1.8.1
+Version: 2.0.0
 Summary: Transparently use webpack with django
 Home-page: https://github.com/django-webpack/django-webpack-loader
 Author: Owais Lone
 Author-email: hello@owaislone.org
 License: UNKNOWN
-Download-URL: https://github.com/django-webpack/django-webpack-loader/tarball/1.8.1
+Download-URL: https://github.com/django-webpack/django-webpack-loader/tarball/2.0.0
 Description: # django-webpack-loader
         
         [![Build Status](https://circleci.com/gh/django-webpack/django-webpack-loader/tree/master.svg?style=svg)](https://circleci.com/gh/django-webpack/django-webpack-loader/tree/master)
         [![Coverage Status](https://coveralls.io/repos/github/django-webpack/django-webpack-loader/badge.svg?branch=master)](https://coveralls.io/github/django-webpack/django-webpack-loader?branch=master)
         ![pyversions](https://img.shields.io/pypi/pyversions/django-webpack-loader)
         ![djversions](https://img.shields.io/pypi/djversions/django-webpack-loader)
         
@@ -50,15 +50,15 @@
           context: __dirname,
           entry: './assets/js/index',
           output: {
             path: path.resolve('./assets/webpack_bundles/'),
             filename: "[name]-[hash].js"
           },
           plugins: [
-            new BundleTracker({filename: './webpack-stats.json'})
+            new BundleTracker({path: __dirname, filename: 'webpack-stats.json'})
           ],
         }
         ```
         
         The configuration above expects the `index.js` (the app entrypoint file) to live inside the `/assets/js/` directory (this guide going forward will assume that all front-end related files are placed inside the `/assets/` directory, with the different kinds of files arranged within its subdirectories).
         
         The generated compiled files will be placed inside the `/assets/webpack_bundles/` directory and the file with the information regarding the bundles and assets (`webpack-stats.json`) will be stored in the project root.
@@ -377,15 +377,15 @@
             // This is required otherwise webpack will try to fetch 
             // our chunk generated by the dynamic import from "/" instead of "/dist/".
             publicPath: '/dist/', 
             chunkFilename: '[name].bundle.js',
             filename: "[name]-[hash].js"
           },
           plugins: [
-            new BundleTracker({ filename: './webpack-stats.json' })
+            new BundleTracker({ path: __dirname, filename: 'webpack-stats.json' })
           ]
         }
         ```
         
         If you're using Webpack 5 instead of 4, do the following:
         - Change `filename: "[name]-[hash].js"` to `filename: "[name]-[fullhash].js"`;
         - Remove `/* webpackChunkName: "lodash" */`, which is not needed anymore.
```

### Comparing `django-webpack-loader-1.8.1/README.md` & `django-webpack-loader-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
   context: __dirname,
   entry: './assets/js/index',
   output: {
     path: path.resolve('./assets/webpack_bundles/'),
     filename: "[name]-[hash].js"
   },
   plugins: [
-    new BundleTracker({filename: './webpack-stats.json'})
+    new BundleTracker({path: __dirname, filename: 'webpack-stats.json'})
   ],
 }
 ```
 
 The configuration above expects the `index.js` (the app entrypoint file) to live inside the `/assets/js/` directory (this guide going forward will assume that all front-end related files are placed inside the `/assets/` directory, with the different kinds of files arranged within its subdirectories).
 
 The generated compiled files will be placed inside the `/assets/webpack_bundles/` directory and the file with the information regarding the bundles and assets (`webpack-stats.json`) will be stored in the project root.
@@ -368,15 +368,15 @@
     // This is required otherwise webpack will try to fetch 
     // our chunk generated by the dynamic import from "/" instead of "/dist/".
     publicPath: '/dist/', 
     chunkFilename: '[name].bundle.js',
     filename: "[name]-[hash].js"
   },
   plugins: [
-    new BundleTracker({ filename: './webpack-stats.json' })
+    new BundleTracker({ path: __dirname, filename: 'webpack-stats.json' })
   ]
 }
 ```
 
 If you're using Webpack 5 instead of 4, do the following:
 - Change `filename: "[name]-[hash].js"` to `filename: "[name]-[fullhash].js"`;
 - Remove `/* webpackChunkName: "lodash" */`, which is not needed anymore.
```

### Comparing `django-webpack-loader-1.8.1/django_webpack_loader.egg-info/PKG-INFO` & `django-webpack-loader-2.0.0/django_webpack_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-webpack-loader
-Version: 1.8.1
+Version: 2.0.0
 Summary: Transparently use webpack with django
 Home-page: https://github.com/django-webpack/django-webpack-loader
 Author: Owais Lone
 Author-email: hello@owaislone.org
 License: UNKNOWN
-Download-URL: https://github.com/django-webpack/django-webpack-loader/tarball/1.8.1
+Download-URL: https://github.com/django-webpack/django-webpack-loader/tarball/2.0.0
 Description: # django-webpack-loader
         
         [![Build Status](https://circleci.com/gh/django-webpack/django-webpack-loader/tree/master.svg?style=svg)](https://circleci.com/gh/django-webpack/django-webpack-loader/tree/master)
         [![Coverage Status](https://coveralls.io/repos/github/django-webpack/django-webpack-loader/badge.svg?branch=master)](https://coveralls.io/github/django-webpack/django-webpack-loader?branch=master)
         ![pyversions](https://img.shields.io/pypi/pyversions/django-webpack-loader)
         ![djversions](https://img.shields.io/pypi/djversions/django-webpack-loader)
         
@@ -50,15 +50,15 @@
           context: __dirname,
           entry: './assets/js/index',
           output: {
             path: path.resolve('./assets/webpack_bundles/'),
             filename: "[name]-[hash].js"
           },
           plugins: [
-            new BundleTracker({filename: './webpack-stats.json'})
+            new BundleTracker({path: __dirname, filename: 'webpack-stats.json'})
           ],
         }
         ```
         
         The configuration above expects the `index.js` (the app entrypoint file) to live inside the `/assets/js/` directory (this guide going forward will assume that all front-end related files are placed inside the `/assets/` directory, with the different kinds of files arranged within its subdirectories).
         
         The generated compiled files will be placed inside the `/assets/webpack_bundles/` directory and the file with the information regarding the bundles and assets (`webpack-stats.json`) will be stored in the project root.
@@ -377,15 +377,15 @@
             // This is required otherwise webpack will try to fetch 
             // our chunk generated by the dynamic import from "/" instead of "/dist/".
             publicPath: '/dist/', 
             chunkFilename: '[name].bundle.js',
             filename: "[name]-[hash].js"
           },
           plugins: [
-            new BundleTracker({ filename: './webpack-stats.json' })
+            new BundleTracker({ path: __dirname, filename: 'webpack-stats.json' })
           ]
         }
         ```
         
         If you're using Webpack 5 instead of 4, do the following:
         - Change `filename: "[name]-[hash].js"` to `filename: "[name]-[fullhash].js"`;
         - Remove `/* webpackChunkName: "lodash" */`, which is not needed anymore.
```

### Comparing `django-webpack-loader-1.8.1/django_webpack_loader.egg-info/SOURCES.txt` & `django-webpack-loader-2.0.0/django_webpack_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-1.8.1/setup.py` & `django-webpack-loader-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-1.8.1/webpack_loader/apps.py` & `django-webpack-loader-2.0.0/webpack_loader/apps.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-1.8.1/webpack_loader/config.py` & `django-webpack-loader-2.0.0/webpack_loader/config.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-1.8.1/webpack_loader/exceptions.py` & `django-webpack-loader-2.0.0/webpack_loader/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-1.8.1/webpack_loader/loader.py` & `django-webpack-loader-2.0.0/webpack_loader/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,17 @@
 class FakeWebpackLoader(WebpackLoader):
     """
     A fake loader to help run Django tests.
 
     For running tests where `render_bundle` is used but assets aren't built.
     """
 
+    def get_assets(self):
+        return {}
+
     def get_bundle(self, _bundle_name):
         return [
             {
                 'name': 'test.bundle.js',
                 'url': 'http://localhost/static/bundles/test.bundle.js',
             }
         ]
```

### Comparing `django-webpack-loader-1.8.1/webpack_loader/templatetags/webpack_loader.py` & `django-webpack-loader-2.0.0/webpack_loader/templatetags/webpack_loader.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-1.8.1/webpack_loader/utils.py` & `django-webpack-loader-2.0.0/webpack_loader/utils.py`

 * *Files identical despite different names*

