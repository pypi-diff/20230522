# Comparing `tmp/lamadava-1.0.0.tar.gz` & `tmp/lamadava-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamadava-1.0.0.tar", last modified: Wed Dec 15 09:39:23 2021, max compression
+gzip compressed data, was "lamadava-1.0.1.tar", last modified: Mon May 22 11:18:57 2023, max compression
```

## Comparing `lamadava-1.0.0.tar` & `lamadava-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-12-15 09:39:23.765122 lamadava-1.0.0/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2021-12-15 09:36:05.000000 lamadava-1.0.0/LICENSE
--rw-r--r--   0 adw0rd     (501) staff       (20)     1027 2021-12-15 09:39:23.765015 lamadava-1.0.0/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)       17 2021-12-15 09:36:05.000000 lamadava-1.0.0/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-12-15 09:39:23.764868 lamadava-1.0.0/lamadava.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1027 2021-12-15 09:39:23.000000 lamadava-1.0.0/lamadava.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      185 2021-12-15 09:39:23.000000 lamadava-1.0.0/lamadava.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2021-12-15 09:39:23.000000 lamadava-1.0.0/lamadava.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       22 2021-12-15 09:39:23.000000 lamadava-1.0.0/lamadava.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2021-12-15 09:39:23.000000 lamadava-1.0.0/lamadava.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2021-12-15 09:39:23.765164 lamadava-1.0.0/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     1345 2021-12-15 09:39:20.000000 lamadava-1.0.0/setup.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:18:57.521953 lamadava-1.0.1/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.1/LICENSE
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1012 2023-05-22 11:18:57.521820 lamadava-1.0.1/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      661 2023-05-22 11:16:55.000000 lamadava-1.0.1/README.md
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:18:57.521098 lamadava-1.0.1/lamadava/
+-rw-r--r--   0 adw0rd     (501) staff       (20)       95 2023-05-22 10:57:32.000000 lamadava-1.0.1/lamadava/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-05-22 11:18:09.000000 lamadava-1.0.1/lamadava/__version__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    28872 2023-05-22 11:00:16.000000 lamadava-1.0.1/lamadava/api.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    30127 2023-05-22 11:00:16.000000 lamadava-1.0.1/lamadava/asyncapi.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4045 2023-05-22 10:57:32.000000 lamadava-1.0.1/lamadava/base.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:18:57.521638 lamadava-1.0.1/lamadava.egg-info/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1012 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/SOURCES.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/dependency_links.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       22 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/requires.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/top_level.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-05-22 11:18:57.521989 lamadava-1.0.1/setup.cfg
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1398 2023-05-22 11:11:01.000000 lamadava-1.0.1/setup.py
```

### Comparing `lamadava-1.0.0/LICENSE` & `lamadava-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.0/PKG-INFO` & `lamadava-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.0
+Version: 1.0.1
 Summary: Instagram Private API SaaS client
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
-Description: UNKNOWN
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+License-File: LICENSE
```

### Comparing `lamadava-1.0.0/lamadava.egg-info/PKG-INFO` & `lamadava-1.0.1/lamadava.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.0
+Version: 1.0.1
 Summary: Instagram Private API SaaS client
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
-Description: UNKNOWN
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+License-File: LICENSE
```

### Comparing `lamadava-1.0.0/setup.py` & `lamadava-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from setuptools import find_packages, setup
 
+from lamadava.__version__ import __version__
+
+
 requirements = [
     'requests<3.0,>=2.25.1',
 ]
 
 setup(
     name='lamadava',
-    version='1.0.0',
+    version=__version__,
     author='Lamadava',
     author_email='support@lamadava.com',
     license='MIT',
     url='https://lamadava.com',
     install_requires=requirements,
     keywords=[
         'instagram private api', 'instagram-private-api', 'instagram api', 'instagram-api', 'instagram',
         'instagram-scraper', 'instagram-client', 'instagram-stories', 'instagram-feed', 'instagram-reels', 'instagram-insights',
         'downloader', 'uploader', 'videos', 'photos', 'albums', 'igtv', 'reels', 'stories', 'pictures',
         'instagram-user-photos', 'instagram-photos', 'instagram-metadata', 'instagram-downloader', 'instagram-uploader'
     ],
     description='Instagram Private API SaaS client',
     packages=find_packages(),
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     include_package_data=True,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Topic :: Software Development :: Libraries :: Python Modules',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ]
 )
```

