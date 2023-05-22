# Comparing `tmp/lamadava-1.0.2.tar.gz` & `tmp/lamadava-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamadava-1.0.2.tar", last modified: Mon May 22 11:25:14 2023, max compression
+gzip compressed data, was "lamadava-1.0.3.tar", last modified: Mon May 22 11:28:53 2023, max compression
```

## Comparing `lamadava-1.0.2.tar` & `lamadava-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:25:14.837490 lamadava-1.0.2/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.2/LICENSE
--rw-r--r--   0 adw0rd     (501) staff       (20)     1714 2023-05-22 11:25:14.837344 lamadava-1.0.2/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      661 2023-05-22 11:16:55.000000 lamadava-1.0.2/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:25:14.836612 lamadava-1.0.2/lamadava/
--rw-r--r--   0 adw0rd     (501) staff       (20)       95 2023-05-22 10:57:32.000000 lamadava-1.0.2/lamadava/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-05-22 11:24:55.000000 lamadava-1.0.2/lamadava/__version__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    28872 2023-05-22 11:00:16.000000 lamadava-1.0.2/lamadava/api.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    30127 2023-05-22 11:00:16.000000 lamadava-1.0.2/lamadava/asyncapi.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4045 2023-05-22 10:57:32.000000 lamadava-1.0.2/lamadava/base.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:25:14.837174 lamadava-1.0.2/lamadava.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1714 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       22 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-05-22 11:25:14.000000 lamadava-1.0.2/lamadava.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-05-22 11:25:14.837529 lamadava-1.0.2/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     1784 2023-05-22 11:24:48.000000 lamadava-1.0.2/setup.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:28:53.134767 lamadava-1.0.3/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.3/LICENSE
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1709 2023-05-22 11:28:53.134635 lamadava-1.0.3/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      656 2023-05-22 11:28:17.000000 lamadava-1.0.3/README.md
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:28:53.133836 lamadava-1.0.3/lamadava/
+-rw-r--r--   0 adw0rd     (501) staff       (20)       95 2023-05-22 10:57:32.000000 lamadava-1.0.3/lamadava/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-05-22 11:28:44.000000 lamadava-1.0.3/lamadava/__version__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    28872 2023-05-22 11:00:16.000000 lamadava-1.0.3/lamadava/api.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    30127 2023-05-22 11:00:16.000000 lamadava-1.0.3/lamadava/asyncapi.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4045 2023-05-22 10:57:32.000000 lamadava-1.0.3/lamadava/base.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:28:53.134463 lamadava-1.0.3/lamadava.egg-info/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1709 2023-05-22 11:28:53.000000 lamadava-1.0.3/lamadava.egg-info/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-05-22 11:28:53.000000 lamadava-1.0.3/lamadava.egg-info/SOURCES.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-05-22 11:28:53.000000 lamadava-1.0.3/lamadava.egg-info/dependency_links.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       22 2023-05-22 11:28:53.000000 lamadava-1.0.3/lamadava.egg-info/requires.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-05-22 11:28:53.000000 lamadava-1.0.3/lamadava.egg-info/top_level.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-05-22 11:28:53.134800 lamadava-1.0.3/setup.cfg
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1784 2023-05-22 11:24:48.000000 lamadava-1.0.3/setup.py
```

### Comparing `lamadava-1.0.2/LICENSE` & `lamadava-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.2/PKG-INFO` & `lamadava-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.2
+Version: 1.0.3
 Summary: Instagram Private API SaaS client
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
 Classifier: Development Status :: 4 - Beta
@@ -37,11 +37,11 @@
 
 ## Usage
 
 Create token https://lamadava.com/tokens and copy "Access key"
 
 ```
 from lamadava import Client
-cl = Client(access_key="<ACCESS_KEY>")
+cl = Client(token="<ACCESS_KEY>")
 user = cl.user_by_username_v2("instagram")
 print(user)
 ```
```

### Comparing `lamadava-1.0.2/README.md` & `lamadava-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
 ## Usage
 
 Create token https://lamadava.com/tokens and copy "Access key"
 
 ```
 from lamadava import Client
-cl = Client(access_key="<ACCESS_KEY>")
+cl = Client(token="<ACCESS_KEY>")
 user = cl.user_by_username_v2("instagram")
 print(user)
 ```
```

### Comparing `lamadava-1.0.2/lamadava/api.py` & `lamadava-1.0.3/lamadava/api.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.2/lamadava/asyncapi.py` & `lamadava-1.0.3/lamadava/asyncapi.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.2/lamadava/base.py` & `lamadava-1.0.3/lamadava/base.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.2/lamadava.egg-info/PKG-INFO` & `lamadava-1.0.3/lamadava.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.2
+Version: 1.0.3
 Summary: Instagram Private API SaaS client
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
 Classifier: Development Status :: 4 - Beta
@@ -37,11 +37,11 @@
 
 ## Usage
 
 Create token https://lamadava.com/tokens and copy "Access key"
 
 ```
 from lamadava import Client
-cl = Client(access_key="<ACCESS_KEY>")
+cl = Client(token="<ACCESS_KEY>")
 user = cl.user_by_username_v2("instagram")
 print(user)
 ```
```

### Comparing `lamadava-1.0.2/setup.py` & `lamadava-1.0.3/setup.py`

 * *Files identical despite different names*

