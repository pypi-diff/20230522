# Comparing `tmp/lamadava-1.0.1.tar.gz` & `tmp/lamadava-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamadava-1.0.1.tar", last modified: Mon May 22 11:18:57 2023, max compression
+gzip compressed data, was "lamadava-1.0.2.tar", last modified: Mon May 22 11:25:14 2023, max compression
```

## Comparing `lamadava-1.0.1.tar` & `lamadava-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:18:57.521953 lamadava-1.0.1/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.1/LICENSE
--rw-r--r--   0 adw0rd     (501) staff       (20)     1012 2023-05-22 11:18:57.521820 lamadava-1.0.1/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      661 2023-05-22 11:16:55.000000 lamadava-1.0.1/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:18:57.521098 lamadava-1.0.1/lamadava/
--rw-r--r--   0 adw0rd     (501) staff       (20)       95 2023-05-22 10:57:32.000000 lamadava-1.0.1/lamadava/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-05-22 11:18:09.000000 lamadava-1.0.1/lamadava/__version__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    28872 2023-05-22 11:00:16.000000 lamadava-1.0.1/lamadava/api.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    30127 2023-05-22 11:00:16.000000 lamadava-1.0.1/lamadava/asyncapi.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4045 2023-05-22 10:57:32.000000 lamadava-1.0.1/lamadava/base.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:18:57.521638 lamadava-1.0.1/lamadava.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1012 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       22 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-05-22 11:18:57.000000 lamadava-1.0.1/lamadava.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-05-22 11:18:57.521989 lamadava-1.0.1/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     1398 2023-05-22 11:11:01.000000 lamadava-1.0.1/setup.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:25:14.837490 lamadava-1.0.2/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.2/LICENSE
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1714 2023-05-22 11:25:14.837344 lamadava-1.0.2/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      661 2023-05-22 11:16:55.000000 lamadava-1.0.2/README.md
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:25:14.836612 lamadava-1.0.2/lamadava/
+-rw-r--r--   0 adw0rd     (501) staff       (20)       95 2023-05-22 10:57:32.000000 lamadava-1.0.2/lamadava/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-05-22 11:24:55.000000 lamadava-1.0.2/lamadava/__version__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    28872 2023-05-22 11:00:16.000000 lamadava-1.0.2/lamadava/api.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    30127 2023-05-22 11:00:16.000000 lamadava-1.0.2/lamadava/asyncapi.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4045 2023-05-22 10:57:32.000000 lamadava-1.0.2/lamadava/base.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:25:14.837174 lamadava-1.0.2/lamadava.egg-info/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1714 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/SOURCES.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/dependency_links.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       22 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/requires.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/top_level.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-05-22 11:25:14.837529 lamadava-1.0.2/setup.cfg
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1784 2023-05-22 11:24:48.000000 lamadava-1.0.2/setup.py
```

### Comparing `lamadava-1.0.1/LICENSE` & `lamadava-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.1/README.md` & `lamadava-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.1/lamadava/api.py` & `lamadava-1.0.2/lamadava/api.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.1/lamadava/asyncapi.py` & `lamadava-1.0.2/lamadava/asyncapi.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.1/lamadava/base.py` & `lamadava-1.0.2/lamadava/base.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.1/setup.py` & `lamadava-1.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,64 @@
+from pathlib import Path
 from setuptools import find_packages, setup
 
 from lamadava.__version__ import __version__
 
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 requirements = [
-    'requests<3.0,>=2.25.1',
+    "requests<3.0,>=2.25.1",
 ]
 
 setup(
-    name='lamadava',
+    name="lamadava",
     version=__version__,
-    author='Lamadava',
-    author_email='support@lamadava.com',
-    license='MIT',
-    url='https://lamadava.com',
+    author="Lamadava",
+    author_email="support@lamadava.com",
+    license="MIT",
+    url="https://lamadava.com",
     install_requires=requirements,
     keywords=[
-        'instagram private api', 'instagram-private-api', 'instagram api', 'instagram-api', 'instagram',
-        'instagram-scraper', 'instagram-client', 'instagram-stories', 'instagram-feed', 'instagram-reels', 'instagram-insights',
-        'downloader', 'uploader', 'videos', 'photos', 'albums', 'igtv', 'reels', 'stories', 'pictures',
-        'instagram-user-photos', 'instagram-photos', 'instagram-metadata', 'instagram-downloader', 'instagram-uploader'
+        "instagram private api",
+        "instagram-private-api",
+        "instagram api",
+        "instagram-api",
+        "instagram",
+        "instagram-scraper",
+        "instagram-client",
+        "instagram-stories",
+        "instagram-feed",
+        "instagram-reels",
+        "instagram-insights",
+        "downloader",
+        "uploader",
+        "videos",
+        "photos",
+        "albums",
+        "igtv",
+        "reels",
+        "stories",
+        "pictures",
+        "instagram-user-photos",
+        "instagram-photos",
+        "instagram-metadata",
+        "instagram-downloader",
+        "instagram-uploader",
     ],
-    description='Instagram Private API SaaS client',
+    description="Instagram Private API SaaS client",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     packages=find_packages(),
     python_requires=">=3.8",
     include_package_data=True,
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ]
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
 )
```

