# Comparing `tmp/iiblib-7.0.0.tar.gz` & `tmp/iiblib-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iiblib-7.0.0.tar", last modified: Tue Feb 14 16:08:29 2023, max compression
+gzip compressed data, was "iiblib-7.1.0.tar", last modified: Mon May 22 03:51:22 2023, max compression
```

## Comparing `iiblib-7.0.0.tar` & `iiblib-7.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:08:29.016015 iiblib-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-14 16:08:19.000000 iiblib-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-14 16:08:19.000000 iiblib-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-02-14 16:08:29.016015 iiblib-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-14 16:08:19.000000 iiblib-7.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:08:29.016015 iiblib-7.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-14 16:08:19.000000 iiblib-7.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:08:29.016015 iiblib-7.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-02-14 16:08:19.000000 iiblib-7.0.0/docs/source/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-02-14 16:08:19.000000 iiblib-7.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-14 16:08:19.000000 iiblib-7.0.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:08:29.016015 iiblib-7.0.0/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-14 16:08:19.000000 iiblib-7.0.0/docs/source/modules/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:08:29.016015 iiblib-7.0.0/iiblib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 16:08:19.000000 iiblib-7.0.0/iiblib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-02-14 16:08:19.000000 iiblib-7.0.0/iiblib/iib_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-02-14 16:08:19.000000 iiblib-7.0.0/iiblib/iib_build_details_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-14 16:08:19.000000 iiblib-7.0.0/iiblib/iib_build_details_pager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-02-14 16:08:19.000000 iiblib-7.0.0/iiblib/iib_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-02-14 16:08:19.000000 iiblib-7.0.0/iiblib/iib_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:08:29.016015 iiblib-7.0.0/iiblib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-02-14 16:08:28.000000 iiblib-7.0.0/iiblib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-14 16:08:28.000000 iiblib-7.0.0/iiblib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 16:08:28.000000 iiblib-7.0.0/iiblib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-14 16:08:28.000000 iiblib-7.0.0/iiblib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-14 16:08:28.000000 iiblib-7.0.0/iiblib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-14 16:08:29.016015 iiblib-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-02-14 16:08:19.000000 iiblib-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:51:22.244200 iiblib-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 03:51:11.000000 iiblib-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-22 03:51:11.000000 iiblib-7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-22 03:51:22.244200 iiblib-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-22 03:51:11.000000 iiblib-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:51:22.244200 iiblib-7.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 03:51:11.000000 iiblib-7.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:51:22.244200 iiblib-7.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-22 03:51:11.000000 iiblib-7.1.0/docs/source/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-22 03:51:11.000000 iiblib-7.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-22 03:51:11.000000 iiblib-7.1.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:51:22.244200 iiblib-7.1.0/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-22 03:51:11.000000 iiblib-7.1.0/docs/source/modules/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:51:22.244200 iiblib-7.1.0/iiblib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 03:51:11.000000 iiblib-7.1.0/iiblib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-22 03:51:11.000000 iiblib-7.1.0/iiblib/iib_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-05-22 03:51:11.000000 iiblib-7.1.0/iiblib/iib_build_details_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-22 03:51:11.000000 iiblib-7.1.0/iiblib/iib_build_details_pager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-05-22 03:51:11.000000 iiblib-7.1.0/iiblib/iib_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-22 03:51:11.000000 iiblib-7.1.0/iiblib/iib_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:51:22.244200 iiblib-7.1.0/iiblib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-22 03:51:22.000000 iiblib-7.1.0/iiblib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-22 03:51:22.000000 iiblib-7.1.0/iiblib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:51:22.000000 iiblib-7.1.0/iiblib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-22 03:51:22.000000 iiblib-7.1.0/iiblib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 03:51:22.000000 iiblib-7.1.0/iiblib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-22 03:51:22.244200 iiblib-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-22 03:51:11.000000 iiblib-7.1.0/setup.py
```

### Comparing `iiblib-7.0.0/LICENSE` & `iiblib-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iiblib-7.0.0/PKG-INFO` & `iiblib-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiblib
-Version: 7.0.0
+Version: 7.1.0
 Summary: IIB client library
 Home-page: https://github.com/release-engineering/iiblib
 Author: Jindrich Luza
 Author-email: jluza@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -59,14 +59,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 7.1.0 - 2023-05-18
+
+### Added
+ - Added FBCOperationsModel
+ - Added retry for Kerberos authentication
+
 ## 7.0.0 - 2023-02-14
 
 ### Added
  - Added RecursiveRelatedBundlesModel
  - Added retries for IIB requests
 
 ### Fixed
```

### Comparing `iiblib-7.0.0/README.md` & `iiblib-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `iiblib-7.0.0/docs/Makefile` & `iiblib-7.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iiblib-7.0.0/docs/source/CHANGELOG.md` & `iiblib-7.1.0/docs/source/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 7.1.0 - 2023-05-18
+
+### Added
+ - Added FBCOperationsModel
+ - Added retry for Kerberos authentication
+
 ## 7.0.0 - 2023-02-14
 
 ### Added
  - Added RecursiveRelatedBundlesModel
  - Added retries for IIB requests
 
 ### Fixed
```

### Comparing `iiblib-7.0.0/docs/source/conf.py` & `iiblib-7.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `iiblib-7.0.0/iiblib/iib_authentication.py` & `iiblib-7.1.0/iiblib/iib_authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import os
 import kerberos
 import subprocess
 import tempfile
+from tenacity import (
+    retry,
+    stop_after_attempt,
+    retry_if_exception_type,
+    wait_exponential,
+)
 
 
 # pylint: disable=bad-option-value,useless-object-inheritance
 class IIBAuth(object):
     def __init__(self):
         raise NotImplementedError
 
@@ -53,14 +59,19 @@
             gssapi_name_type (str)
                 GSSAPI name type for creating credentials
         """
         self.krb_princ = krb_princ
         self.ktfile = ktfile
         self.service = service
 
+    @retry(
+        retry=retry_if_exception_type(kerberos.KrbError),
+        wait=wait_exponential(multiplier=10, exp_base=5),
+        stop=stop_after_attempt(3),
+    )
     def _krb_auth_header(self):
         retcode = subprocess.Popen(
             ["klist"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
         ).wait()
         krb5ccname = None
         if retcode or self.ktfile:
             # can I define old_krb5ccname on the higher level out of if?
```

### Comparing `iiblib-7.0.0/iiblib/iib_build_details_model.py` & `iiblib-7.1.0/iiblib/iib_build_details_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from copy import deepcopy
+
+
 class IIBBuildDetailsModel(object):
     """
     Model class handling data about index build task
 
     Args:
         id (int)
             An id of build
@@ -237,33 +240,15 @@
         "internal_index_image_copy",
         "internal_index_image_copy_resolved",
         "omps_operator_version",
         "organization",
         "removed_operators",
     ]
 
-    _operation_attrs = [
-        "binary_image",
-        "binary_image_resolved",
-        "build_tags",
-        "bundles",
-        "bundle_mapping",
-        "deprecation_list",
-        "distribution_scope",
-        "from_index",
-        "from_index_resolved",
-        "index_image",
-        "index_image_resolved",
-        "internal_index_image_copy",
-        "internal_index_image_copy_resolved",
-        "removed_operators",
-        "organization",
-        "omps_operator_version",
-    ]
-
+    _operation_attrs = deepcopy(__slots__)
     _accepted_request_type = "add"
 
 
 class RmModel(IIBBuildDetailsModel):
     """
     RmModel class handling data from "builds/rm" endpoint, and
     data from "builds" and "builds/<id>" IIB endpoints defined by
@@ -300,45 +285,29 @@
             A name of organization to push to in the legacy app registry
     """
 
     __slots__ = [
         "binary_image",
         "binary_image_resolved",
         "build_tags",
-        "bundles",
-        "bundle_mapping",
-        "deprecation_list",
-        "distribution_scope",
-        "from_index",
-        "from_index_resolved",
-        "index_image",
-        "index_image_resolved",
-        "internal_index_image_copy",
-        "internal_index_image_copy_resolved",
-        "organization",
-        "removed_operators",
-    ]
-    _operation_attrs = [
-        "binary_image",
-        "binary_image_resolved",
-        "build_tags",
         "bundle_mapping",
         "bundles",
         "deprecation_list",
         "distribution_scope",
         "from_index",
         "from_index_resolved",
         "index_image",
         "index_image_resolved",
         "internal_index_image_copy",
         "internal_index_image_copy_resolved",
         "organization",
         "removed_operators",
     ]
 
+    _operation_attrs = deepcopy(__slots__)
     _accepted_request_type = "rm"
 
 
 class RegenerateBundleModel(IIBBuildDetailsModel):
     """
     RegenerateBundleModel class handling data from
     "builds/regenerate-bundle" endpoint, and data from "builds"
@@ -361,20 +330,15 @@
 
     __slots__ = [
         "bundle_image",
         "from_bundle_image",
         "from_bundle_image_resolved",
         "organization",
     ]
-    _operation_attrs = [
-        "bundle_image",
-        "from_bundle_image",
-        "from_bundle_image_resolved",
-        "organization",
-    ]
+    _operation_attrs = deepcopy(__slots__)
 
     _accepted_request_type = "regenerate-bundle"
 
 
 class MergeIndexImageModel(IIBBuildDetailsModel):
     """
     MergeIndexImageModel class handling data from
@@ -417,27 +381,16 @@
         "distribution_scope",
         "index_image",
         "source_from_index",
         "source_from_index_resolved",
         "target_index",
         "target_index_resolved",
     ]
-    _operation_attrs = [
-        "binary_image",
-        "binary_image_resolved",
-        "build_tags",
-        "deprecation_list",
-        "distribution_scope",
-        "index_image",
-        "source_from_index",
-        "source_from_index_resolved",
-        "target_index",
-        "target_index_resolved",
-    ]
 
+    _operation_attrs = deepcopy(__slots__)
     _accepted_request_type = "merge-index-image"
 
 
 class CreateEmptyIndexModel(IIBBuildDetailsModel):
     """
     CreateEmptyIndexModel class handling data from
     "builds/create-empty-index
@@ -474,25 +427,16 @@
         "distribution_scope",
         "from_index",
         "from_index_resolved",
         "index_image",
         "index_image_resolved",
         "labels",
     ]
-    _operation_attrs = [
-        "binary_image",
-        "binary_image_resolved",
-        "distribution_scope",
-        "from_index",
-        "from_index_resolved",
-        "index_image",
-        "index_image_resolved",
-        "labels",
-    ]
 
+    _operation_attrs = deepcopy(__slots__)
     _accepted_request_type = "create-empty-index"
 
 
 class RecursiveRelatedBundlesModel(IIBBuildDetailsModel):
     """
     RecursiveRelatedBundles class handling data from "builds/recursive-related-bundles" endpoint,
     and data from "builds" and "builds/<id>" IIB endpoints defined by
@@ -513,15 +457,62 @@
 
     __slots__ = [
         "nested_bundles",
         "organization",
         "parent_bundle_image",
         "parent_bundle_image_resolved",
     ]
-    _operation_attrs = [
-        "nested_bundles",
-        "organization",
-        "parent_bundle_image",
-        "parent_bundle_image_resolved",
-    ]
 
+    _operation_attrs = deepcopy(__slots__)
     _accepted_request_type = "recursive-related-bundles"
+
+
+class FBCOperationsModel(IIBBuildDetailsModel):
+    """
+    FBCOperationModel class handling data from "builds/fbc-operations" endpoint,
+    and data from "builds" and "builds/<id>" IIB endpoints defined by
+    "fbc-operations" request_type .
+    FBCOperationModel class inherits arguments from IIBBuildDetailsModel.
+    For a complete list of arguments check IIBBuildDetailsModel.
+
+    Args:
+        binary_image (str)
+            A reference of binary image used for rebuilding
+        binary_image_resolved (str)
+            A checksum reference of binary image that was used for rebuilding
+        distribution_scope (str)
+            A distribution where is the product used (prod, stage, etc.)
+        fbc_fragment (str)
+            A reference to fbc fragment.
+        fbc_fragment_resolved (str)
+            A checksum reference of fbc fragment that was used for rebuilding
+        from_index (str)
+            A reference of index image used as source for rebuild
+        from_index_resolved (str)
+            A checksum reference of index image that was used for rebuilding
+        index_image (str)
+            A reference of index image to rebuild
+        index_image_resolved (str)
+            A reference of resolved index image copy of the index image
+        internal_index_image_copy (str)
+            A reference of IIB's internal copy of the built index image
+        internal_index_image_copy_resolved (str)
+            A reference of resolved IIB's internal copy of the built index image
+    """
+
+    __slots__ = [
+        "binary_image",
+        "binary_image_resolved",
+        "build_tags",
+        "distribution_scope",
+        "fbc_fragment",
+        "fbc_fragment_resolved",
+        "from_index",
+        "from_index_resolved",
+        "index_image",
+        "index_image_resolved",
+        "internal_index_image_copy",
+        "internal_index_image_copy_resolved",
+    ]
+
+    _operation_attrs = deepcopy(__slots__)
+    _accepted_request_type = "fbc-operations"
```

### Comparing `iiblib-7.0.0/iiblib/iib_build_details_pager.py` & `iiblib-7.1.0/iiblib/iib_build_details_pager.py`

 * *Files identical despite different names*

### Comparing `iiblib-7.0.0/iiblib/iib_client.py` & `iiblib-7.1.0/iiblib/iib_client.py`

 * *Files identical despite different names*

### Comparing `iiblib-7.0.0/iiblib/iib_session.py` & `iiblib-7.1.0/iiblib/iib_session.py`

 * *Files identical despite different names*

### Comparing `iiblib-7.0.0/iiblib.egg-info/PKG-INFO` & `iiblib-7.1.0/iiblib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiblib
-Version: 7.0.0
+Version: 7.1.0
 Summary: IIB client library
 Home-page: https://github.com/release-engineering/iiblib
 Author: Jindrich Luza
 Author-email: jluza@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -59,14 +59,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 7.1.0 - 2023-05-18
+
+### Added
+ - Added FBCOperationsModel
+ - Added retry for Kerberos authentication
+
 ## 7.0.0 - 2023-02-14
 
 ### Added
  - Added RecursiveRelatedBundlesModel
  - Added retries for IIB requests
 
 ### Fixed
```

### Comparing `iiblib-7.0.0/setup.py` & `iiblib-7.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 extras_require = {"reST": ["Sphinx"]}
 
 if os.environ.get("READTHEDOCS", None):
     extras_require["reST"].append("recommonmark")
 
 setup(
     name="iiblib",
-    version="7.0.0",
+    version="7.1.0",
     description="IIB client library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jindrich Luza",
     author_email="jluza@redhat.com",
     url="https://github.com/release-engineering/iiblib",
     classifiers=classifiers,
```

