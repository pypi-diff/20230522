# Comparing `tmp/neulabs-cdk-constructs-0.4.0.tar.gz` & `tmp/neulabs-cdk-constructs-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.4.0.tar", last modified: Fri May 19 14:10:33 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.4.1.tar", last modified: Mon May 22 14:21:54 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.4.0.tar` & `neulabs-cdk-constructs-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100996 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-19 14:10:32.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-19 14:10:33.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:10:32.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-19 14:10:32.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 14:10:32.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.339555 neulabs-cdk-constructs-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.339555 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100995 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.343555 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-22 14:21:40.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:21:54.339555 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-22 14:21:54.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-22 14:21:54.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:21:54.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-22 14:21:54.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 14:21:54.000000 neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.4.0/LICENSE` & `neulabs-cdk-constructs-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.0/PKG-INFO` & `neulabs-cdk-constructs-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.4.0
+Version: 0.4.1
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.4.0/README.md` & `neulabs-cdk-constructs-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.0/setup.py` & `neulabs-cdk-constructs-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.4.0",
+    "version": "0.4.1",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.4.0.jsii.tgz"
+            "neulabs-cdk-constructs@0.4.1.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.4.0",
+    "0.4.1",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.4.0.jsii.tgz",
+    "neulabs-cdk-constructs@0.4.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.4.0
+Version: 0.4.1
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.4.1/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.0.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.1.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

