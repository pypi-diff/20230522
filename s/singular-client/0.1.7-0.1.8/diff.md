# Comparing `tmp/singular_client-0.1.7.tar.gz` & `tmp/singular_client-0.1.8.tar.gz`

## Comparing `singular_client-0.1.7.tar` & `singular_client-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/__init__.py
--rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/_bases.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/api.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/documents.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/models.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/utils.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/__init__.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/governance.py
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/links.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/links_legacy.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/monetization.py
--rw-r--r--   0        0        0     8945 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/reporting.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/skan.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 singular_client-0.1.7/.gitignore
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 singular_client-0.1.7/LICENSE
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 singular_client-0.1.7/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 singular_client-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 singular_client-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/__init__.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/_bases.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/api.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/documents.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/models.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/utils.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/endpoints/__init__.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/endpoints/governance.py
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/endpoints/links.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/endpoints/links_legacy.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/endpoints/monetization.py
+-rw-r--r--   0        0        0     8945 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/endpoints/reporting.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 singular_client-0.1.8/singular_client/endpoints/skan.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 singular_client-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 singular_client-0.1.8/LICENSE
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 singular_client-0.1.8/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 singular_client-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 singular_client-0.1.8/PKG-INFO
```

### Comparing `singular_client-0.1.7/singular_client/__init__.py` & `singular_client-0.1.8/singular_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,30 +53,32 @@
     LinkLegacyDoc,
     CustomLinkLegacyDoc,
     AdMonetizationDoc,
     ConversionModelDoc,
     AppConversionModelDoc,
 )
 
+import sys
 
-from singular_client.models import (
-    NameModel,
-    IDModel,
-    NameValuesModel,
-    DataConnectorModel,
-    ReportStatusModel,
-    CohortMetricsModel,
-    CreateLinkModel,
-    LinkModel,
-    AppModel,
-    PartnerAppModel,
-    PartnerModel,
-    Redirection,
-    DomainModel,
-    AppLegacyModel,
-    PartnerLegacyModel,
-    LinkLegacyModel,
-    CustomLinkLegacyModel,
-    AdMonetizationModel,
-    ConversionModelModel,
-    AppConversionModelModel,
-)
+if 'pydantic' in sys.modules:
+    from singular_client.models import (
+        NameModel,
+        IDModel,
+        NameValuesModel,
+        DataConnectorModel,
+        ReportStatusModel,
+        CohortMetricsModel,
+        CreateLinkModel,
+        LinkModel,
+        AppModel,
+        PartnerAppModel,
+        PartnerModel,
+        Redirection,
+        DomainModel,
+        AppLegacyModel,
+        PartnerLegacyModel,
+        LinkLegacyModel,
+        CustomLinkLegacyModel,
+        AdMonetizationModel,
+        ConversionModelModel,
+        AppConversionModelModel,
+    )
```

### Comparing `singular_client-0.1.7/singular_client/_bases.py` & `singular_client-0.1.8/singular_client/_bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 D = TypeVar("D", bound=Union[TypedDict, dict])
 
 
 class ResponseDocList(Generic[D], List[D]):
     pass
 
 
-KwargsKey = Tuple[Hashable, Hashable]
-CacheKey = KwargsKey
+CacheKey = Tuple[Hashable, Hashable]
 ResType = TypeVar("ResType")
 
 
 class _Endpoint(Generic[ResType]):
     """
     Base class for all endpoints
     ----
```

### Comparing `singular_client-0.1.7/singular_client/api.py` & `singular_client-0.1.8/singular_client/api.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/documents.py` & `singular_client-0.1.8/singular_client/documents.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/models.py` & `singular_client-0.1.8/singular_client/models.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/utils.py` & `singular_client-0.1.8/singular_client/utils.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/endpoints/__init__.py` & `singular_client-0.1.8/singular_client/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/endpoints/links.py` & `singular_client-0.1.8/singular_client/endpoints/links.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/endpoints/links_legacy.py` & `singular_client-0.1.8/singular_client/endpoints/links_legacy.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/endpoints/monetization.py` & `singular_client-0.1.8/singular_client/endpoints/monetization.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/endpoints/reporting.py` & `singular_client-0.1.8/singular_client/endpoints/reporting.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/singular_client/endpoints/skan.py` & `singular_client-0.1.8/singular_client/endpoints/skan.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/.gitignore` & `singular_client-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/LICENSE` & `singular_client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.7/pyproject.toml` & `singular_client-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "singular-client"
-version = "0.1.7"
+version = "0.1.8"
 python_requires = ">=3.8"
 description = "A modern Singular API client."
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
@@ -21,15 +21,14 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries"
 ]
 dependencies = [
     'requests',
-    'pydantic',
 ]
 
 # [project.urls]
 # Bug Tracker = "https://github.com/ryayoung/singular-client/issues"
 
 # [project.scripts]
 # Uncomment and modify the lines below to create command-line scripts
```

