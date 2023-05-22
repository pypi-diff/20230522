# Comparing `tmp/superpowered-sdk-0.1.3.tar.gz` & `tmp/superpowered-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.1.3.tar", last modified: Mon May 22 17:53:41 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.1.4.tar", last modified: Mon May 22 18:08:50 2023, max compression
```

## Comparing `superpowered-sdk-0.1.3.tar` & `superpowered-sdk-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 17:53:41.824769 superpowered-sdk-0.1.3/
--rw-r--r--   0 justinclark   (501) staff       (20)     6636 2023-05-22 17:53:41.824466 superpowered-sdk-0.1.3/PKG-INFO
--rw-r--r--   0 justinclark   (501) staff       (20)     5136 2023-05-19 14:21:49.000000 superpowered-sdk-0.1.3/README.md
--rw-r--r--   0 justinclark   (501) staff       (20)       38 2023-05-22 17:53:41.824872 superpowered-sdk-0.1.3/setup.cfg
--rw-r--r--   0 justinclark   (501) staff       (20)     2225 2023-05-22 17:50:06.000000 superpowered-sdk-0.1.3/setup.py
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 17:53:41.821669 superpowered-sdk-0.1.3/superpowered/
--rw-r--r--   0 justinclark   (501) staff       (20)      892 2023-05-22 17:50:01.000000 superpowered-sdk-0.1.3/superpowered/__init__.py
--rw-r--r--   0 justinclark   (501) staff       (20)     1301 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.3/superpowered/exceptions.py
--rw-r--r--   0 justinclark   (501) staff       (20)    11202 2023-05-22 17:50:01.000000 superpowered-sdk-0.1.3/superpowered/superpowered.py
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 17:53:41.823996 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/
--rw-r--r--   0 justinclark   (501) staff       (20)     6636 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 justinclark   (501) staff       (20)      298 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 justinclark   (501) staff       (20)        1 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 justinclark   (501) staff       (20)       17 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/requires.txt
--rw-r--r--   0 justinclark   (501) staff       (20)       13 2023-05-22 17:53:41.000000 superpowered-sdk-0.1.3/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 18:08:50.577150 superpowered-sdk-0.1.4/
+-rw-r--r--   0 justinclark   (501) staff       (20)     6636 2023-05-22 18:08:50.576850 superpowered-sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 justinclark   (501) staff       (20)     5136 2023-05-19 14:21:49.000000 superpowered-sdk-0.1.4/README.md
+-rw-r--r--   0 justinclark   (501) staff       (20)       38 2023-05-22 18:08:50.577257 superpowered-sdk-0.1.4/setup.cfg
+-rw-r--r--   0 justinclark   (501) staff       (20)     2277 2023-05-22 18:07:56.000000 superpowered-sdk-0.1.4/setup.py
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 18:08:50.574272 superpowered-sdk-0.1.4/superpowered/
+-rw-r--r--   0 justinclark   (501) staff       (20)      892 2023-05-22 17:50:01.000000 superpowered-sdk-0.1.4/superpowered/__init__.py
+-rw-r--r--   0 justinclark   (501) staff       (20)     4045 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered/errors.json
+-rw-r--r--   0 justinclark   (501) staff       (20)     1301 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.4/superpowered/exceptions.py
+-rw-r--r--   0 justinclark   (501) staff       (20)    11202 2023-05-22 17:50:01.000000 superpowered-sdk-0.1.4/superpowered/superpowered.py
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 18:08:50.576377 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/
+-rw-r--r--   0 justinclark   (501) staff       (20)     6636 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 justinclark   (501) staff       (20)      323 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)        1 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)       17 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/requires.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)       13 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.1.3/PKG-INFO` & `superpowered-sdk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.4 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Keywords: Superpowered AI Knowledge base as a service for LLM
 applications Classifier: Development Status :: 4 - Beta Classifier: Environment
```

### Comparing `superpowered-sdk-0.1.3/README.md` & `superpowered-sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.3/setup.py` & `superpowered-sdk-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         "Contact": "https://superpowered.ai/contact/",
         "End-User License Agreement": "https://superpowered.ai/api-user-agreement/"
     },
     author="superpowered",
     author_email="justin@superpowered.ai",
     keywords="Superpowered AI Knowledge base as a service for LLM applications",
     packages=["superpowered"],
+    package_data={"superpowered": ["errors.json"]},
     # package_dir={"": "superpowered"},
     install_requires=read("requirements.txt"),
     include_package_data=True,
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
```

### Comparing `superpowered-sdk-0.1.3/superpowered/__init__.py` & `superpowered-sdk-0.1.4/superpowered/__init__.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.3/superpowered/exceptions.py` & `superpowered-sdk-0.1.4/superpowered/exceptions.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.3/superpowered/superpowered.py` & `superpowered-sdk-0.1.4/superpowered/superpowered.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.3/superpowered_sdk.egg-info/PKG-INFO` & `superpowered-sdk-0.1.4/superpowered_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.4 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Keywords: Superpowered AI Knowledge base as a service for LLM
 applications Classifier: Development Status :: 4 - Beta Classifier: Environment
```

