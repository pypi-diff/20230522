# Comparing `tmp/streamlit-auth0-component-0.1.4.tar.gz` & `tmp/streamlit-auth0-component-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-auth0-component-0.1.4.tar", last modified: Wed Nov 30 16:01:37 2022, max compression
+gzip compressed data, was "streamlit-auth0-component-0.1.5.tar", last modified: Mon May 22 12:36:37 2023, max compression
```

## Comparing `streamlit-auth0-component-0.1.4.tar` & `streamlit-auth0-component-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-30 16:01:37.563990 streamlit-auth0-component-0.1.4/
--rw-r--r--   0 conrad     (501) staff       (20)     1063 2022-10-06 00:18:52.000000 streamlit-auth0-component-0.1.4/LICENSE
--rw-r--r--   0 conrad     (501) staff       (20)       50 2022-11-30 16:01:16.000000 streamlit-auth0-component-0.1.4/MANIFEST.in
--rw-r--r--   0 conrad     (501) staff       (20)      187 2022-11-30 16:01:37.563845 streamlit-auth0-component-0.1.4/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)     1360 2022-11-30 15:56:11.000000 streamlit-auth0-component-0.1.4/README.md
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-30 16:01:37.561315 streamlit-auth0-component-0.1.4/auth0_component/
--rw-r--r--   0 conrad     (501) staff       (20)     3148 2022-10-06 08:58:02.000000 streamlit-auth0-component-0.1.4/auth0_component/__init__.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-30 16:01:37.560241 streamlit-auth0-component-0.1.4/auth0_component/frontend/
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-30 16:01:37.561819 streamlit-auth0-component-0.1.4/auth0_component/frontend/dist/
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-30 16:01:37.562394 streamlit-auth0-component-0.1.4/auth0_component/frontend/dist/assets/
--rw-r--r--   0 conrad     (501) staff       (20)     1468 2022-11-30 16:00:53.000000 streamlit-auth0-component-0.1.4/auth0_component/frontend/dist/assets/index.5223bee9.css
--rw-r--r--   0 conrad     (501) staff       (20)   337374 2022-11-30 16:00:53.000000 streamlit-auth0-component-0.1.4/auth0_component/frontend/dist/assets/index.9a5fd6ad.js
--rw-r--r--   0 conrad     (501) staff       (20)      301 2022-11-30 16:00:53.000000 streamlit-auth0-component-0.1.4/auth0_component/frontend/dist/index.html
--rw-r--r--   0 conrad     (501) staff       (20)     1497 2022-11-30 16:00:53.000000 streamlit-auth0-component-0.1.4/auth0_component/frontend/dist/vite.svg
--rw-r--r--   0 conrad     (501) staff       (20)       38 2022-11-30 16:01:37.564031 streamlit-auth0-component-0.1.4/setup.cfg
--rw-r--r--   0 conrad     (501) staff       (20)      601 2022-11-30 16:01:36.000000 streamlit-auth0-component-0.1.4/setup.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-30 16:01:37.563658 streamlit-auth0-component-0.1.4/streamlit_auth0_component.egg-info/
--rw-r--r--   0 conrad     (501) staff       (20)      187 2022-11-30 16:01:37.000000 streamlit-auth0-component-0.1.4/streamlit_auth0_component.egg-info/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      501 2022-11-30 16:01:37.000000 streamlit-auth0-component-0.1.4/streamlit_auth0_component.egg-info/SOURCES.txt
--rw-r--r--   0 conrad     (501) staff       (20)        1 2022-11-30 16:01:37.000000 streamlit-auth0-component-0.1.4/streamlit_auth0_component.egg-info/dependency_links.txt
--rw-r--r--   0 conrad     (501) staff       (20)       35 2022-11-30 16:01:37.000000 streamlit-auth0-component-0.1.4/streamlit_auth0_component.egg-info/requires.txt
--rw-r--r--   0 conrad     (501) staff       (20)       16 2022-11-30 16:01:37.000000 streamlit-auth0-component-0.1.4/streamlit_auth0_component.egg-info/top_level.txt
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2023-05-22 12:36:37.993657 streamlit-auth0-component-0.1.5/
+-rw-r--r--   0 conrad     (501) staff       (20)     1063 2022-10-06 00:18:52.000000 streamlit-auth0-component-0.1.5/LICENSE
+-rw-r--r--   0 conrad     (501) staff       (20)       50 2022-11-30 16:01:16.000000 streamlit-auth0-component-0.1.5/MANIFEST.in
+-rw-r--r--   0 conrad     (501) staff       (20)      187 2023-05-22 12:36:37.993463 streamlit-auth0-component-0.1.5/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)     1360 2022-11-30 16:03:04.000000 streamlit-auth0-component-0.1.5/README.md
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2023-05-22 12:36:37.990470 streamlit-auth0-component-0.1.5/auth0_component/
+-rw-r--r--   0 conrad     (501) staff       (20)     3148 2023-05-22 12:35:36.000000 streamlit-auth0-component-0.1.5/auth0_component/__init__.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2023-05-22 12:36:37.988903 streamlit-auth0-component-0.1.5/auth0_component/frontend/
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2023-05-22 12:36:37.990731 streamlit-auth0-component-0.1.5/auth0_component/frontend/dist/
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2023-05-22 12:36:37.991298 streamlit-auth0-component-0.1.5/auth0_component/frontend/dist/assets/
+-rw-r--r--   0 conrad     (501) staff       (20)     1468 2023-05-22 12:36:06.000000 streamlit-auth0-component-0.1.5/auth0_component/frontend/dist/assets/index.5223bee9.css
+-rw-r--r--   0 conrad     (501) staff       (20)   337374 2023-05-22 12:36:06.000000 streamlit-auth0-component-0.1.5/auth0_component/frontend/dist/assets/index.9a5fd6ad.js
+-rw-r--r--   0 conrad     (501) staff       (20)      301 2023-05-22 12:36:06.000000 streamlit-auth0-component-0.1.5/auth0_component/frontend/dist/index.html
+-rw-r--r--   0 conrad     (501) staff       (20)       38 2023-05-22 12:36:37.993740 streamlit-auth0-component-0.1.5/setup.cfg
+-rw-r--r--   0 conrad     (501) staff       (20)      601 2023-05-22 12:36:12.000000 streamlit-auth0-component-0.1.5/setup.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2023-05-22 12:36:37.993197 streamlit-auth0-component-0.1.5/streamlit_auth0_component.egg-info/
+-rw-r--r--   0 conrad     (501) staff       (20)      187 2023-05-22 12:36:37.000000 streamlit-auth0-component-0.1.5/streamlit_auth0_component.egg-info/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)      462 2023-05-22 12:36:37.000000 streamlit-auth0-component-0.1.5/streamlit_auth0_component.egg-info/SOURCES.txt
+-rw-r--r--   0 conrad     (501) staff       (20)        1 2023-05-22 12:36:37.000000 streamlit-auth0-component-0.1.5/streamlit_auth0_component.egg-info/dependency_links.txt
+-rw-r--r--   0 conrad     (501) staff       (20)       35 2023-05-22 12:36:37.000000 streamlit-auth0-component-0.1.5/streamlit_auth0_component.egg-info/requires.txt
+-rw-r--r--   0 conrad     (501) staff       (20)       16 2023-05-22 12:36:37.000000 streamlit-auth0-component-0.1.5/streamlit_auth0_component.egg-info/top_level.txt
```

### Comparing `streamlit-auth0-component-0.1.4/LICENSE` & `streamlit-auth0-component-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-auth0-component-0.1.4/README.md` & `streamlit-auth0-component-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-auth0-component-0.1.4/auth0_component/__init__.py` & `streamlit-auth0-component-0.1.5/auth0_component/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-auth0-component-0.1.4/auth0_component/frontend/dist/assets/index.5223bee9.css` & `streamlit-auth0-component-0.1.5/auth0_component/frontend/dist/assets/index.5223bee9.css`

 * *Files identical despite different names*

### Comparing `streamlit-auth0-component-0.1.4/auth0_component/frontend/dist/assets/index.9a5fd6ad.js` & `streamlit-auth0-component-0.1.5/auth0_component/frontend/dist/assets/index.9a5fd6ad.js`

 * *Files identical despite different names*

### Comparing `streamlit-auth0-component-0.1.4/setup.py` & `streamlit-auth0-component-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-auth0-component",
-    version="0.1.4",
+    version="0.1.5",
     author="",
     author_email="",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

