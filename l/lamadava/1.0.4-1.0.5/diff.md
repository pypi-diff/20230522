# Comparing `tmp/lamadava-1.0.4.tar.gz` & `tmp/lamadava-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamadava-1.0.4.tar", last modified: Mon May 22 11:38:30 2023, max compression
+gzip compressed data, was "lamadava-1.0.5.tar", last modified: Mon May 22 11:48:35 2023, max compression
```

## Comparing `lamadava-1.0.4.tar` & `lamadava-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:38:30.468874 lamadava-1.0.4/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.4/LICENSE
--rw-r--r--   0 adw0rd     (501) staff       (20)     1706 2023-05-22 11:38:30.468738 lamadava-1.0.4/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      656 2023-05-22 11:28:17.000000 lamadava-1.0.4/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:38:30.467897 lamadava-1.0.4/lamadava/
--rw-r--r--   0 adw0rd     (501) staff       (20)       95 2023-05-22 10:57:32.000000 lamadava-1.0.4/lamadava/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-05-22 11:36:32.000000 lamadava-1.0.4/lamadava/__version__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    28872 2023-05-22 11:00:16.000000 lamadava-1.0.4/lamadava/api.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    30127 2023-05-22 11:00:16.000000 lamadava-1.0.4/lamadava/asyncapi.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4045 2023-05-22 10:57:32.000000 lamadava-1.0.4/lamadava/base.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:38:30.468557 lamadava-1.0.4/lamadava.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1706 2023-05-22 11:38:30.000000 lamadava-1.0.4/lamadava.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-05-22 11:38:30.000000 lamadava-1.0.4/lamadava.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-05-22 11:38:30.000000 lamadava-1.0.4/lamadava.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       14 2023-05-22 11:38:30.000000 lamadava-1.0.4/lamadava.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-05-22 11:38:30.000000 lamadava-1.0.4/lamadava.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-05-22 11:38:30.468928 lamadava-1.0.4/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     1783 2023-05-22 11:37:03.000000 lamadava-1.0.4/setup.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:48:35.311477 lamadava-1.0.5/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.5/LICENSE
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1706 2023-05-22 11:48:35.311354 lamadava-1.0.5/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      656 2023-05-22 11:28:17.000000 lamadava-1.0.5/README.md
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:48:35.310652 lamadava-1.0.5/lamadava/
+-rw-r--r--   0 adw0rd     (501) staff       (20)      186 2023-05-22 11:46:49.000000 lamadava-1.0.5/lamadava/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-05-22 11:46:04.000000 lamadava-1.0.5/lamadava/__version__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    28872 2023-05-22 11:00:16.000000 lamadava-1.0.5/lamadava/api.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    30127 2023-05-22 11:00:16.000000 lamadava-1.0.5/lamadava/asyncapi.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4045 2023-05-22 10:57:32.000000 lamadava-1.0.5/lamadava/base.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:48:35.311190 lamadava-1.0.5/lamadava.egg-info/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1706 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/SOURCES.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/dependency_links.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       14 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/requires.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/top_level.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-05-22 11:48:35.311511 lamadava-1.0.5/setup.cfg
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1783 2023-05-22 11:37:03.000000 lamadava-1.0.5/setup.py
```

### Comparing `lamadava-1.0.4/LICENSE` & `lamadava-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.4/PKG-INFO` & `lamadava-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.4
+Version: 1.0.5
 Summary: Lamadava client, for Python 3.
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lamadava-1.0.4/README.md` & `lamadava-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.4/lamadava/api.py` & `lamadava-1.0.5/lamadava/api.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.4/lamadava/asyncapi.py` & `lamadava-1.0.5/lamadava/asyncapi.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.4/lamadava/base.py` & `lamadava-1.0.5/lamadava/base.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.4/lamadava.egg-info/PKG-INFO` & `lamadava-1.0.5/lamadava.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.4
+Version: 1.0.5
 Summary: Lamadava client, for Python 3.
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lamadava-1.0.4/setup.py` & `lamadava-1.0.5/setup.py`

 * *Files identical despite different names*

