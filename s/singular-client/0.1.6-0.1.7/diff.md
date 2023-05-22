# Comparing `tmp/singular_client-0.1.6.tar.gz` & `tmp/singular_client-0.1.7.tar.gz`

## Comparing `singular_client-0.1.6.tar` & `singular_client-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/__init__.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/_bases.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/api.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/documents.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/models.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/utils.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/__init__.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/governance.py
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/links.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/links_legacy.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/monetization.py
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/reporting.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/skan.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 singular_client-0.1.6/.gitignore
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 singular_client-0.1.6/LICENSE
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 singular_client-0.1.6/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 singular_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 singular_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/__init__.py
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/_bases.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/api.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/documents.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/models.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/utils.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/__init__.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/governance.py
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/links.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/links_legacy.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/monetization.py
+-rw-r--r--   0        0        0     8945 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/reporting.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 singular_client-0.1.7/singular_client/endpoints/skan.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 singular_client-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 singular_client-0.1.7/LICENSE
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 singular_client-0.1.7/README.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 singular_client-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 singular_client-0.1.7/PKG-INFO
```

### Comparing `singular_client-0.1.6/singular_client/__init__.py` & `singular_client-0.1.7/singular_client/__init__.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/singular_client/_bases.py` & `singular_client-0.1.7/singular_client/_bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 class ResponseDocList(Generic[D], List[D]):
     pass
 
 
 KwargsKey = Tuple[Hashable, Hashable]
-CacheKey = Tuple[KwargsKey, ...]
+CacheKey = KwargsKey
 ResType = TypeVar("ResType")
 
 
 class _Endpoint(Generic[ResType]):
     """
     Base class for all endpoints
     ----
```

### Comparing `singular_client-0.1.6/singular_client/api.py` & `singular_client-0.1.7/singular_client/api.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/singular_client/documents.py` & `singular_client-0.1.7/singular_client/documents.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/singular_client/models.py` & `singular_client-0.1.7/singular_client/models.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/singular_client/utils.py` & `singular_client-0.1.7/singular_client/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 def _convert_list_arg(
     arg: Union[List[T], T, str], default: Optional[List[T]] = None
 ) -> str:
     ...
 
 
 @overload
-def _convert_list_arg(arg: None = None, default: List[T] = None) -> str:
+def _convert_list_arg(arg: None = None, default: List = []) -> str:
     ...
 
 
 @overload
 def _convert_list_arg(arg: None = None, default: None = None) -> None:
     ...
```

### Comparing `singular_client-0.1.6/singular_client/endpoints/__init__.py` & `singular_client-0.1.7/singular_client/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/singular_client/endpoints/links.py` & `singular_client-0.1.7/singular_client/endpoints/links.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/singular_client/endpoints/links_legacy.py` & `singular_client-0.1.7/singular_client/endpoints/links_legacy.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/singular_client/endpoints/monetization.py` & `singular_client-0.1.7/singular_client/endpoints/monetization.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/singular_client/endpoints/reporting.py` & `singular_client-0.1.7/singular_client/endpoints/reporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
     Returned by a check on the status of a report, through the ReportStatusEndpoint,
     or indirectly, through the CreateReportResponse object.
 
     Its boolean value is True if the report is done, OR if it has failed.
     """
 
-    cached_download: Optional[Union[requests.Response, "pd.DataFrame"]]
+    cached_download: Optional[requests.Response]
     raw: ReportStatusDoc
     failed = property(lambda x: x.raw["status"] == "FAILED")
     done = property(lambda x: x.raw["status"] == "DONE")
     queued = property(lambda x: x.raw["status"] == "QUEUED")
     started = property(lambda x: x.raw["status"] == "STARTED")
     url = property(lambda x: x.raw["download_url"])
```

### Comparing `singular_client-0.1.6/singular_client/endpoints/skan.py` & `singular_client-0.1.7/singular_client/endpoints/skan.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/.gitignore` & `singular_client-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/LICENSE` & `singular_client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.6/pyproject.toml` & `singular_client-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "singular-client"
-version = "0.1.6"
+version = "0.1.7"
 python_requires = ">=3.8"
 description = "A modern Singular API client."
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `singular_client-0.1.6/PKG-INFO` & `singular_client-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: singular-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: A modern Singular API client.
 Author-email: Ryan Young <dev@ryayoung.com>
+License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
```

