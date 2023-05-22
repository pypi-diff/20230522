# Comparing `tmp/kuflow_rest-0.4.5.tar.gz` & `tmp/kuflow_rest-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_rest-0.4.5.tar", max compression
+gzip compressed data, was "kuflow_rest-0.5.0.tar", max compression
```

## Comparing `kuflow_rest-0.4.5.tar` & `kuflow_rest-0.5.0.tar`

### file list

```diff
@@ -1,42 +1,72 @@
--rw-r--r--   0        0        0      875 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/README.md
--rw-r--r--   0        0        0        6 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/VERSION
--rw-r--r--   0        0        0     1335 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/__init__.py
--rw-r--r--   0        0        0     1907 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/__init__.py
--rw-r--r--   0        0        0     7087 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/_client.py
--rw-r--r--   0        0        0     3983 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/_patch.py
--rw-r--r--   0        0        0    77869 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/_serialization.py
--rw-r--r--   0        0        0     1874 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/_vendor.py
--rw-r--r--   0        0        0     1517 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/_version.py
--rw-r--r--   0        0        0     1854 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/__init__.py
--rw-r--r--   0        0        0     7230 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/_client.py
--rw-r--r--   0        0        0     4026 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/_patch.py
--rw-r--r--   0        0        0     2060 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     7223 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_patch.py
--rw-r--r--   0        0        0     7842 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_principal_operations.py
--rw-r--r--   0        0        0    34839 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_process_operations.py
--rw-r--r--   0        0        0    51643 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_task_operations.py
--rw-r--r--   0        0        0     5191 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/models/__init__.py
--rw-r--r--   0        0        0     3294 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/models/_enums.py
--rw-r--r--   0        0        0    71240 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/models/_patch.py
--rw-r--r--   0        0        0     2060 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/operations/__init__.py
--rw-r--r--   0        0        0     7823 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_patch.py
--rw-r--r--   0        0        0     9752 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_principal_operations.py
--rw-r--r--   0        0        0    41609 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_process_operations.py
--rw-r--r--   0        0        0    62943 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_task_operations.py
--rw-r--r--   0        0        0       26 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_generated/py.typed
--rw-r--r--   0        0        0     7622 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/_kuflow_rest_client.py
--rw-r--r--   0        0        0     4336 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/models/__init__.py
--rw-r--r--   0        0        0     3383 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/models/_models.py
--rw-r--r--   0        0        0     1440 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/operations/__init__.py
--rw-r--r--   0        0        0     2501 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/operations/_authentication_operations.py
--rw-r--r--   0        0        0     4073 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/operations/_principal_operations.py
--rw-r--r--   0        0        0     9685 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/operations/_process_operations.py
--rw-r--r--   0        0        0    14938 2023-05-15 11:39:40.703021 kuflow_rest-0.4.5/kuflow_rest/operations/_task_operations.py
--rw-r--r--   0        0        0      756 2023-05-15 11:41:08.582676 kuflow_rest-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 kuflow_rest-0.4.5/setup.py
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-05-22 09:05:44.083853 kuflow_rest-0.5.0/README.md
+-rw-r--r--   0        0        0        6 2023-05-22 09:05:44.083853 kuflow_rest-0.5.0/VERSION
+-rw-r--r--   0        0        0     1335 2023-05-22 09:05:44.083853 kuflow_rest-0.5.0/kuflow_rest/__init__.py
+-rw-r--r--   0        0        0     1907 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-22 09:07:15.606733 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6018 2023-05-22 09:07:15.606733 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
+-rw-r--r--   0        0        0     2365 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2023-05-22 09:07:15.662732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0    57905 2023-05-22 09:07:15.630732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
+-rw-r--r--   0        0        0      731 2023-05-22 09:07:15.646732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc
+-rw-r--r--   0        0        0      178 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0        0        0     7108 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_client.py
+-rw-r--r--   0        0        0     3983 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_patch.py
+-rw-r--r--   0        0        0    78834 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_serialization.py
+-rw-r--r--   0        0        0     2007 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_vendor.py
+-rw-r--r--   0        0        0     1517 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_version.py
+-rw-r--r--   0        0        0     1854 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/__init__.py
+-rw-r--r--   0        0        0     7256 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_client.py
+-rw-r--r--   0        0        0     4026 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_patch.py
+-rw-r--r--   0        0        0     2060 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0     7284 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     7894 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_principal_operations.py
+-rw-r--r--   0        0        0    35197 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_process_operations.py
+-rw-r--r--   0        0        0    62010 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_task_operations.py
+-rw-r--r--   0        0        0     5465 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__init__.py
+-rw-r--r--   0        0        0     3261 2023-05-22 09:07:15.610733 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2558 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
+-rw-r--r--   0        0        0    65326 2023-05-22 09:07:15.618733 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0      739 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     3294 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/models/_enums.py
+-rw-r--r--   0        0        0    75667 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/models/_patch.py
+-rw-r--r--   0        0        0     2060 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__init__.py
+-rw-r--r--   0        0        0      737 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5603 2023-05-22 09:07:15.646732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0      743 2023-05-22 09:07:15.662732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     6811 2023-05-22 09:07:15.646732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    28491 2023-05-22 09:07:15.654732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    51369 2023-05-22 09:07:15.662732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     7884 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_patch.py
+-rw-r--r--   0        0        0     9804 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_principal_operations.py
+-rw-r--r--   0        0        0    41967 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_process_operations.py
+-rw-r--r--   0        0        0    76156 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_task_operations.py
+-rw-r--r--   0        0        0       26 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/py.typed
+-rw-r--r--   0        0        0     7722 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_kuflow_rest_client.py
+-rw-r--r--   0        0        0     4771 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/models/__init__.py
+-rw-r--r--   0        0        0     2858 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4588 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0     4581 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/models/_models.py
+-rw-r--r--   0        0        0     1440 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/operations/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1691 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     3429 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     9070 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    16316 2023-05-22 09:07:15.670732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     2324 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/operations/_authentication_operations.py
+-rw-r--r--   0        0        0     4116 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/operations/_principal_operations.py
+-rw-r--r--   0        0        0     9540 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/operations/_process_operations.py
+-rw-r--r--   0        0        0    17441 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/operations/_task_operations.py
+-rw-r--r--   0        0        0     6837 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/utils/__init__.py
+-rw-r--r--   0        0        0     3980 2023-05-22 09:07:15.670732 kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    31360 2023-05-22 09:07:15.678732 kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc
+-rw-r--r--   0        0        0    17040 2023-05-22 09:07:15.674732 kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc
+-rw-r--r--   0        0        0    41580 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/utils/_element_values.py
+-rw-r--r--   0        0        0    23171 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/utils/_json_forms.py
+-rw-r--r--   0        0        0      977 2023-05-22 09:07:34.462501 kuflow_rest-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-0.5.0/setup.py
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.5.0/PKG-INFO
```

### Comparing `kuflow_rest-0.4.5/README.md` & `kuflow_rest-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/__init__.py` & `kuflow_rest-0.5.0/kuflow_rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from ._kuflow_rest_client import KuFlowRestClient
 from ._generated._serialization import Deserializer, Serializer, Model
 
 __all__ = ["Deserializer", "KuFlowRestClient", "Model", "Serializer"]
-__version__ = "0.4.5"
+__version__ = "0.5.0"
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/__init__.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/_client.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     :paramtype endpoint: str
     """
 
     def __init__(
         self, credential: "TokenCredential", *, endpoint: str = "https://api.kuflow.com/v2022-10-08", **kwargs: Any
     ) -> None:
         self._config = KuFlowRestClientConfiguration(credential=credential, **kwargs)
-        self._client = PipelineClient(base_url=endpoint, config=self._config, **kwargs)
+        self._client: PipelineClient = PipelineClient(base_url=endpoint, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.authentication = AuthenticationOperations(self._client, self._config, self._serialize, self._deserialize)
         self.principal = PrincipalOperations(self._client, self._config, self._serialize, self._deserialize)
@@ -152,9 +152,9 @@
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "KuFlowRestClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/_configuration.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/_patch.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/_serialization.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,47 @@
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
-from typing import Optional, Union, AnyStr, IO, Mapping
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from typing import Dict, Any, cast
-
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
+
 
 class RawDeserializer:
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
     CONTEXT_NAME = "deserialized_data"
@@ -271,43 +288,43 @@
     serialization and deserialization.
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
             cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
@@ -316,30 +333,35 @@
         try:
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any,
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -378,41 +400,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -512,15 +539,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -528,15 +555,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -595,15 +622,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -619,16 +646,15 @@
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
@@ -649,16 +675,16 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
@@ -770,14 +796,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -1154,15 +1182,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1235,15 +1264,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1259,15 +1288,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1325,15 +1354,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1345,15 +1374,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1464,40 +1493,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/_vendor.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/_vendor.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,20 @@
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
 
+from typing import List, cast
+
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/_version.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
 
-VERSION = "0.4.5"
+VERSION = "0.5.0"
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/__init__.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/_client.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     :paramtype endpoint: str
     """
 
     def __init__(
         self, credential: "AsyncTokenCredential", *, endpoint: str = "https://api.kuflow.com/v2022-10-08", **kwargs: Any
     ) -> None:
         self._config = KuFlowRestClientConfiguration(credential=credential, **kwargs)
-        self._client = AsyncPipelineClient(base_url=endpoint, config=self._config, **kwargs)
+        self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=endpoint, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.authentication = AuthenticationOperations(self._client, self._config, self._serialize, self._deserialize)
         self.principal = PrincipalOperations(self._client, self._config, self._serialize, self._deserialize)
@@ -152,9 +152,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "KuFlowRestClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/_configuration.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/_patch.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/__init__.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_authentication_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -112,16 +113,16 @@
     async def create_authentication(
         self, authentication: Union[_models.Authentication, IO], **kwargs: Any
     ) -> _models.Authentication:
         """Create an authentication for the current principal.
 
         Create an authentication for the current principal.
 
-        :param authentication: Authentication to be created. Is either a model type or a IO type.
-         Required.
+        :param authentication: Authentication to be created. Is either a Authentication type or a IO
+         type. Required.
         :type authentication: ~kuflow.rest.models.Authentication or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Authentication
         :rtype: ~kuflow.rest.models.Authentication
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -139,30 +140,31 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Authentication] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(authentication, (IO, bytes)):
+        if isinstance(authentication, (IOBase, bytes)):
             _content = authentication
         else:
             _json = self._serialize.body(authentication, "Authentication")
 
         request = build_create_authentication_request(
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_patch.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_principal_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_principal_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,16 +128,17 @@
             type=type,
             group_id=group_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -178,16 +179,17 @@
         request = build_retrieve_principal_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_process_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_process_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -125,16 +126,17 @@
             page=page,
             sort=sort,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -221,15 +223,15 @@
         * If you know the ``principal ID`` you can assign it to ``initiator.id``
         * If you know the ``user ID`` you can assign it to ``initiator.user.id``
         * If you know the ``user email`` you can assign it to ``initiator.user.email``
         * If you know the ``application ID`` you can assign it to ``initiator.application.id``
 
         If you want the method to be idempotent, please specify the ``id`` field in the request body.
 
-        :param process: Process to create. Is either a model type or a IO type. Required.
+        :param process: Process to create. Is either a Process type or a IO type. Required.
         :type process: ~kuflow.rest.models.Process or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -247,30 +249,31 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Process] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(process, (IO, bytes)):
+        if isinstance(process, (IOBase, bytes)):
             _content = process
         else:
             _json = self._serialize.body(process, "Process")
 
         request = build_create_process_request(
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -315,16 +318,17 @@
         request = build_retrieve_process_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -400,16 +404,16 @@
 
         Allows you to choose a user (by email or principal identifier) or an application (principal
         identifier).
         Only one option will be necessary.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to change the process initiator. Is either a model type or a IO type.
-         Required.
+        :param command: Command to change the process initiator. Is either a
+         ProcessChangeInitiatorCommand type or a IO type. Required.
         :type command: ~kuflow.rest.models.ProcessChangeInitiatorCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -427,31 +431,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Process] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "ProcessChangeInitiatorCommand")
 
         request = build_actions_process_change_initiator_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -533,15 +538,16 @@
         otherwise it creates them. The values of the previous elements that no longer exist will be
         deleted.
 
         If the process is already finished the invocations fails with an error.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to save an element. Is either a model type or a IO type. Required.
+        :param command: Command to save an element. Is either a ProcessSaveElementCommand type or a IO
+         type. Required.
         :type command: ~kuflow.rest.models.ProcessSaveElementCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -559,31 +565,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Process] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "ProcessSaveElementCommand")
 
         request = build_actions_process_save_element_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -653,15 +660,16 @@
 
         Allow to delete a process element by specifying the item definition code.
 
         Remove all the element values.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete an element. Is either a model type or a IO type. Required.
+        :param command: Command to delete an element. Is either a ProcessDeleteElementCommand type or a
+         IO type. Required.
         :type command: ~kuflow.rest.models.ProcessDeleteElementCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -679,31 +687,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Process] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "ProcessDeleteElementCommand")
 
         request = build_actions_process_delete_element_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -746,16 +755,17 @@
         request = build_actions_process_complete_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -800,16 +810,17 @@
         request = build_actions_process_cancel_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -868,16 +879,17 @@
             content_type=content_type,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 304]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/aio/operations/_task_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_task_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, AsyncIterator, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -52,16 +53,19 @@
     build_actions_task_assign_request,
     build_actions_task_claim_request,
     build_actions_task_complete_request,
     build_actions_task_delete_element_request,
     build_actions_task_delete_element_value_document_request,
     build_actions_task_download_element_value_document_request,
     build_actions_task_download_element_value_rendered_request,
+    build_actions_task_download_json_forms_value_document_request,
     build_actions_task_save_element_request,
     build_actions_task_save_element_value_document_request,
+    build_actions_task_save_json_forms_value_data_request,
+    build_actions_task_save_json_forms_value_document_request,
     build_create_task_request,
     build_find_tasks_request,
     build_retrieve_task_request,
 )
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
@@ -148,16 +152,17 @@
             state=state,
             task_definition_code=task_definition_code,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -268,15 +273,15 @@
         * If you know the ``principal ID`` you can assign it to ``owner.id``
         * If you know the ``user ID`` you can assign it to ``owner.user.id``
         * If you know the ``user email`` you can assign it to ``owner.user.email``
         * If you know the ``application ID`` you can assign it to ``owner.application.id``
 
         If you want the method to be idempotent, please specify the ``id`` field in the request body.
 
-        :param task: Task to be created. Is either a model type or a IO type. Required.
+        :param task: Task to be created. Is either a Task type or a IO type. Required.
         :type task: ~kuflow.rest.models.Task or IO
         :keyword activity_token: When create a Kuflow Task backed with a Temporal.io servers, this
          value is required and must be set with the context task token of Temporal.io activity. Default
          value is None.
         :paramtype activity_token: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
@@ -298,31 +303,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(task, (IO, bytes)):
+        if isinstance(task, (IOBase, bytes)):
             _content = task
         else:
             _json = self._serialize.body(task, "Task")
 
         request = build_create_task_request(
             activity_token=activity_token,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -367,16 +373,17 @@
         request = build_retrieve_task_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -417,16 +424,17 @@
         request = build_actions_task_claim_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -485,16 +493,16 @@
     ) -> _models.Task:
         """Assign a task.
 
         Allow to assign a task to a user or application. Only one option will be necessary.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to change the task owner. Is either a model type or a IO type.
-         Required.
+        :param command: Command to change the task owner. Is either a TaskAssignCommand type or a IO
+         type. Required.
         :type command: ~kuflow.rest.models.TaskAssignCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -512,31 +520,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "TaskAssignCommand")
 
         request = build_actions_task_assign_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -619,15 +628,16 @@
         to add a new document, please use the corresponding API method. If values already exist for the
         provided element code, it replaces them with the new ones, otherwise it creates them. The
         values of the previous elements that no longer exist will be deleted. To remove an element, use
         the appropriate API method.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to save an element. Is either a model type or a IO type. Required.
+        :param command: Command to save an element. Is either a TaskSaveElementCommand type or a IO
+         type. Required.
         :type command: ~kuflow.rest.models.TaskSaveElementCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -645,31 +655,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "TaskSaveElementCommand")
 
         request = build_actions_task_save_element_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -747,16 +758,17 @@
             content_type=content_type,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -826,15 +838,16 @@
 
         Allow to delete task element by specifying the item definition code.
 
         Remove all the element values.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete an element. Is either a model type or a IO type. Required.
+        :param command: Command to delete an element. Is either a TaskDeleteElementCommand type or a IO
+         type. Required.
         :type command: ~kuflow.rest.models.TaskDeleteElementCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -852,31 +865,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "TaskDeleteElementCommand")
 
         request = build_actions_task_delete_element_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -903,15 +917,15 @@
         Allow to delete a specific document from an element of document type using its id.
 
         Note: If it is a multiple item, it will only delete the specified document. If it is a single
         element, in addition to the document, it will also delete the element.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete a document elemente value. Required.
+        :param command: Command to delete a document element value. Required.
         :type command: ~kuflow.rest.models.TaskDeleteElementValueDocumentCommand
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -926,15 +940,15 @@
         Allow to delete a specific document from an element of document type using its id.
 
         Note: If it is a multiple item, it will only delete the specified document. If it is a single
         element, in addition to the document, it will also delete the element.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete a document elemente value. Required.
+        :param command: Command to delete a document element value. Required.
         :type command: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -949,16 +963,16 @@
         Allow to delete a specific document from an element of document type using its id.
 
         Note: If it is a multiple item, it will only delete the specified document. If it is a single
         element, in addition to the document, it will also delete the element.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete a document elemente value. Is either a model type or a IO
-         type. Required.
+        :param command: Command to delete a document element value. Is either a
+         TaskDeleteElementValueDocumentCommand type or a IO type. Required.
         :type command: ~kuflow.rest.models.TaskDeleteElementValueDocumentCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -976,31 +990,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "TaskDeleteElementValueDocumentCommand")
 
         request = build_actions_task_delete_element_value_document_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1046,16 +1061,17 @@
             id=id,
             document_id=document_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = True
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=True, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1105,16 +1121,265 @@
             id=id,
             element_definition_code=element_definition_code,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = True
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
+            raise HttpResponseError(response=response, model=error)
+
+        deserialized = response.iter_bytes()
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    async def actions_task_save_json_forms_value_data(
+        self,
+        id: str,
+        command: _models.TaskSaveJsonFormsValueDataCommand,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> _models.Task:
+        """Save JSON data.
+
+        Allow to save a JSON data validating that the data follow the related schema. If the data is
+        invalid, then
+        the json form is marked as invalid.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param command: Command to save the JSON value. Required.
+        :type command: ~kuflow.rest.models.TaskSaveJsonFormsValueDataCommand
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: Task
+        :rtype: ~kuflow.rest.models.Task
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def actions_task_save_json_forms_value_data(
+        self, id: str, command: IO, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.Task:
+        """Save JSON data.
+
+        Allow to save a JSON data validating that the data follow the related schema. If the data is
+        invalid, then
+        the json form is marked as invalid.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param command: Command to save the JSON value. Required.
+        :type command: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: Task
+        :rtype: ~kuflow.rest.models.Task
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def actions_task_save_json_forms_value_data(
+        self, id: str, command: Union[_models.TaskSaveJsonFormsValueDataCommand, IO], **kwargs: Any
+    ) -> _models.Task:
+        """Save JSON data.
+
+        Allow to save a JSON data validating that the data follow the related schema. If the data is
+        invalid, then
+        the json form is marked as invalid.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param command: Command to save the JSON value. Is either a TaskSaveJsonFormsValueDataCommand
+         type or a IO type. Required.
+        :type command: ~kuflow.rest.models.TaskSaveJsonFormsValueDataCommand or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: Task
+        :rtype: ~kuflow.rest.models.Task
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Task] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(command, (IOBase, bytes)):
+            _content = command
+        else:
+            _json = self._serialize.body(command, "TaskSaveJsonFormsValueDataCommand")
+
+        request = build_actions_task_save_json_forms_value_data_request(
+            id=id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
+            raise HttpResponseError(response=response, model=error)
+
+        deserialized = self._deserialize("Task", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace_async
+    async def actions_task_save_json_forms_value_document(
+        self, id: str, file: IO, *, file_content_type: str, file_name: str, schema_path: str, **kwargs: Any
+    ) -> _models.TaskSaveJsonFormsValueDocumentResponseCommand:
+        """Save a JSON Forms document.
+
+        Save a document in the task to later be linked into the JSON data.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param file: Document to save. Required.
+        :type file: IO
+        :keyword file_content_type: Document content type. Required.
+        :paramtype file_content_type: str
+        :keyword file_name: Document name. Required.
+        :paramtype file_name: str
+        :keyword schema_path: JSON Schema path related to the document. The uploaded document must be
+         validated by the passed schema path. Required.
+        :paramtype schema_path: str
+        :return: TaskSaveJsonFormsValueDocumentResponseCommand
+        :rtype: ~kuflow.rest.models.TaskSaveJsonFormsValueDocumentResponseCommand
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: str = kwargs.pop("content_type", _headers.pop("Content-Type", "application/octet-stream"))
+        cls: ClsType[_models.TaskSaveJsonFormsValueDocumentResponseCommand] = kwargs.pop("cls", None)
+
+        _content = file
+
+        request = build_actions_task_save_json_forms_value_document_request(
+            id=id,
+            file_content_type=file_content_type,
+            file_name=file_name,
+            schema_path=schema_path,
+            content_type=content_type,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
+            raise HttpResponseError(response=response, model=error)
+
+        deserialized = self._deserialize("TaskSaveJsonFormsValueDocumentResponseCommand", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace_async
+    async def actions_task_download_json_forms_value_document(
+        self, id: str, *, document_uri: str, **kwargs: Any
+    ) -> AsyncIterator[bytes]:
+        """Download document.
+
+        Given a task, download a document from a json form data.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :keyword document_uri: Document URI to download. Required.
+        :paramtype document_uri: str
+        :return: Async iterator of the response bytes
+        :rtype: AsyncIterator[bytes]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[AsyncIterator[bytes]] = kwargs.pop("cls", None)
+
+        request = build_actions_task_download_json_forms_value_document_request(
+            id=id,
+            document_uri=document_uri,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = True
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=True, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1155,16 +1420,17 @@
         request = build_actions_task_complete_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1224,15 +1490,15 @@
         """Append a log to the task.
 
         A log entry is added to the task. If the number of log entries is reached, the oldest log entry
         is removed.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param log: Log to be created. Is either a model type or a IO type. Required.
+        :param log: Log to be created. Is either a Log type or a IO type. Required.
         :type log: ~kuflow.rest.models.Log or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1250,31 +1516,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(log, (IO, bytes)):
+        if isinstance(log, (IOBase, bytes)):
             _content = log
         else:
             _json = self._serialize.body(log, "Log")
 
         request = build_actions_task_append_log_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/models/__init__.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 #
 # --------------------------------------------------------------------------
 
 from ._models import AbstractAudited
 from ._models import Authentication
 from ._models import DefaultError
 from ._models import DefaultErrorInfo
+from ._models import JsonFormsValue
 from ._models import Log
 from ._models import Page
 from ._models import PageMetadata
 from ._models import Principal
 from ._models import PrincipalApplication
 from ._models import PrincipalPage
 from ._models import PrincipalUser
@@ -64,14 +65,16 @@
 from ._models import TaskElementValueObject
 from ._models import TaskElementValuePrincipal
 from ._models import TaskElementValuePrincipalItem
 from ._models import TaskElementValueString
 from ._models import TaskPage
 from ._models import TaskPageItem
 from ._models import TaskSaveElementCommand
+from ._models import TaskSaveJsonFormsValueDataCommand
+from ._models import TaskSaveJsonFormsValueDocumentResponseCommand
 from ._models import WebhookEvent
 from ._models import WebhookEventProcessStateChanged
 from ._models import WebhookEventProcessStateChangedData
 from ._models import WebhookEventTaskStateChanged
 from ._models import WebhookEventTaskStateChangedData
 
 from ._enums import AuditedObjectType
@@ -88,14 +91,15 @@
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AbstractAudited",
     "Authentication",
     "DefaultError",
     "DefaultErrorInfo",
+    "JsonFormsValue",
     "Log",
     "Page",
     "PageMetadata",
     "Principal",
     "PrincipalApplication",
     "PrincipalPage",
     "PrincipalUser",
@@ -122,14 +126,16 @@
     "TaskElementValueObject",
     "TaskElementValuePrincipal",
     "TaskElementValuePrincipalItem",
     "TaskElementValueString",
     "TaskPage",
     "TaskPageItem",
     "TaskSaveElementCommand",
+    "TaskSaveJsonFormsValueDataCommand",
+    "TaskSaveJsonFormsValueDocumentResponseCommand",
     "WebhookEvent",
     "WebhookEventProcessStateChanged",
     "WebhookEventProcessStateChangedData",
     "WebhookEventTaskStateChanged",
     "WebhookEventTaskStateChangedData",
     "AuditedObjectType",
     "LogLevel",
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/models/_enums.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/models/_enums.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/models/_models.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/models/_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -93,16 +93,16 @@
     def __init__(
         self,
         *,
         created_by: Optional[str] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_at: Optional[datetime.datetime] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword created_by: Who create this model.
         :paramtype created_by: str
         :keyword created_at: When this model was created.
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: Who was last update this model.
         :paramtype last_modified_by: str
@@ -168,16 +168,16 @@
         self,
         *,
         created_by: Optional[str] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_at: Optional[datetime.datetime] = None,
         type: Optional[Literal["ENGINE"]] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword created_by: Who create this model.
         :paramtype created_by: str
         :keyword created_at: When this model was created.
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: Who was last update this model.
         :paramtype last_modified_by: str
@@ -231,16 +231,16 @@
     def __init__(
         self,
         *,
         timestamp: datetime.datetime,
         status: int,
         message: str,
         errors: Optional[List["_models.DefaultErrorInfo"]] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword timestamp: Timestamp indicating when the error happened. Required.
         :paramtype timestamp: ~datetime.datetime
         :keyword status: HTTP Status. Required.
         :paramtype status: int
         :keyword message: Message Status. Required.
         :paramtype message: str
@@ -278,16 +278,22 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "location": {"key": "location", "type": "str"},
         "location_type": {"key": "locationType", "type": "str"},
     }
 
     def __init__(
-        self, *, code: str, message: str, location: Optional[str] = None, location_type: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        code: str,
+        message: str,
+        location: Optional[str] = None,
+        location_type: Optional[str] = None,
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword code: Required.
         :paramtype code: str
         :keyword message: Required.
         :paramtype message: str
         :keyword location:
         :paramtype location: str
@@ -297,14 +303,40 @@
         super().__init__(**kwargs)
         self.code = code
         self.message = message
         self.location = location
         self.location_type = location_type
 
 
+class JsonFormsValue(_serialization.Model):
+    """Json form values, used when the render type selected is JSON Forms.
+
+    :ivar valid: true if the data complain the related json schema.
+    :vartype valid: bool
+    :ivar data: json value filled that complain with the related json schema.
+    :vartype data: dict[str, any]
+    """
+
+    _attribute_map = {
+        "valid": {"key": "valid", "type": "bool"},
+        "data": {"key": "data", "type": "{object}"},
+    }
+
+    def __init__(self, *, valid: Optional[bool] = None, data: Optional[Dict[str, Any]] = None, **kwargs: Any) -> None:
+        """
+        :keyword valid: true if the data complain the related json schema.
+        :paramtype valid: bool
+        :keyword data: json value filled that complain with the related json schema.
+        :paramtype data: dict[str, any]
+        """
+        super().__init__(**kwargs)
+        self.valid = valid
+        self.data = data
+
+
 class Log(_serialization.Model):
     """Log.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id:
     :vartype id: str
@@ -331,16 +363,16 @@
     def __init__(
         self,
         *,
         message: str,
         level: Union[str, "_models.LogLevel"],
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         created_at: Optional[datetime.datetime] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword created_at: When this model was created.
         :paramtype created_at: ~datetime.datetime
         :keyword message: Required.
         :paramtype message: str
@@ -379,15 +411,15 @@
         "metadata": {"key": "metadata", "type": "PageMetadata"},
     }
 
     _subtype_map = {
         "object_type": {"PRINCIPAL_PAGE": "PrincipalPage", "PROCESS_PAGE": "ProcessPage", "TASK_PAGE": "TaskPage"}
     }
 
-    def __init__(self, *, metadata: "_models.PageMetadata", **kwargs):
+    def __init__(self, *, metadata: "_models.PageMetadata", **kwargs: Any) -> None:
         """
         :keyword metadata: Required.
         :paramtype metadata: ~kuflow.rest.models.PageMetadata
         """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
         self.metadata = metadata
@@ -418,15 +450,15 @@
     _attribute_map = {
         "size": {"key": "size", "type": "int"},
         "page": {"key": "page", "type": "int"},
         "total_elements": {"key": "totalElements", "type": "int"},
         "total_pages": {"key": "totalPages", "type": "int"},
     }
 
-    def __init__(self, *, size: int, page: int, total_elements: int, total_pages: int, **kwargs):
+    def __init__(self, *, size: int, page: int, total_elements: int, total_pages: int, **kwargs: Any) -> None:
         """
         :keyword size: Required.
         :paramtype size: int
         :keyword page: Required.
         :paramtype page: int
         :keyword total_elements: Required.
         :paramtype total_elements: int
@@ -467,16 +499,16 @@
         self,
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         type: Optional[Union[str, "_models.PrincipalType"]] = None,
         name: Optional[str] = None,
         user: Optional["_models.PrincipalUser"] = None,
         application: Optional["_models.PrincipalApplication"] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword type: Known values are: "USER", "APPLICATION", and "SYSTEM".
         :paramtype type: str or ~kuflow.rest.models.PrincipalType
         :keyword name:
         :paramtype name: str
@@ -500,15 +532,15 @@
     :vartype id: str
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: Optional[str] = None, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: Optional[str] = None, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id:
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -535,15 +567,15 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "metadata": {"key": "metadata", "type": "PageMetadata"},
         "content": {"key": "content", "type": "[Principal]"},
     }
 
-    def __init__(self, *, metadata: "_models.PageMetadata", content: List["_models.Principal"], **kwargs):
+    def __init__(self, *, metadata: "_models.PageMetadata", content: List["_models.Principal"], **kwargs: Any) -> None:
         """
         :keyword metadata: Required.
         :paramtype metadata: ~kuflow.rest.models.PageMetadata
         :keyword content: Required.
         :paramtype content: list[~kuflow.rest.models.Principal]
         """
         super().__init__(metadata=metadata, **kwargs)
@@ -562,16 +594,20 @@
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "email": {"key": "email", "type": "str"},
     }
 
     def __init__(
-        self, *, id: Optional[str] = None, email: Optional[str] = None, **kwargs  # pylint: disable=redefined-builtin
-    ):
+        self,
+        *,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        email: Optional[str] = None,
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword email:
         :paramtype email: str
         """
         super().__init__(**kwargs)
@@ -642,16 +678,16 @@
         last_modified_at: Optional[datetime.datetime] = None,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         subject: Optional[str] = None,
         state: Optional[Union[str, "_models.ProcessState"]] = None,
         element_values: Optional[Dict[str, List["_models.ProcessElementValue"]]] = None,
         initiator: Optional["_models.Principal"] = None,
         related_process: Optional["_models.RelatedProcess"] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword created_by: Who create this model.
         :paramtype created_by: str
         :keyword created_at: When this model was created.
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: Who was last update this model.
         :paramtype last_modified_by: str
@@ -699,15 +735,15 @@
     """
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "email": {"key": "email", "type": "str"},
     }
 
-    def __init__(self, *, principal_id: Optional[str] = None, email: Optional[str] = None, **kwargs):
+    def __init__(self, *, principal_id: Optional[str] = None, email: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword principal_id:
         :paramtype principal_id: str
         :keyword email:
         :paramtype email: str
         """
         super().__init__(**kwargs)
@@ -741,16 +777,16 @@
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         version: Optional[str] = None,
         name: Optional[str] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword version:
         :paramtype version: str
         :keyword name:
         :paramtype name: str
@@ -774,15 +810,15 @@
         "element_definition_code": {"required": True},
     }
 
     _attribute_map = {
         "element_definition_code": {"key": "elementDefinitionCode", "type": "str"},
     }
 
-    def __init__(self, *, element_definition_code: str, **kwargs):
+    def __init__(self, *, element_definition_code: str, **kwargs: Any) -> None:
         """
         :keyword element_definition_code: Code of task element to delete. Required.
         :paramtype element_definition_code: str
         """
         super().__init__(**kwargs)
         self.element_definition_code = element_definition_code
 
@@ -808,15 +844,15 @@
     _attribute_map = {
         "valid": {"key": "valid", "type": "bool"},
         "type": {"key": "type", "type": "str"},
     }
 
     _subtype_map = {"type": {"NUMBER": "ProcessElementValueNumber", "STRING": "ProcessElementValueString"}}
 
-    def __init__(self, *, valid: bool = True, **kwargs):
+    def __init__(self, *, valid: bool = True, **kwargs: Any) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         """
         super().__init__(**kwargs)
         self.valid = valid
         self.type: Optional[str] = None
@@ -841,15 +877,15 @@
 
     _attribute_map = {
         "valid": {"key": "valid", "type": "bool"},
         "type": {"key": "type", "type": "str"},
         "value": {"key": "value", "type": "float"},
     }
 
-    def __init__(self, *, valid: bool = True, value: Optional[float] = None, **kwargs):
+    def __init__(self, *, valid: bool = True, value: Optional[float] = None, **kwargs: Any) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         :keyword value:
         :paramtype value: float
         """
         super().__init__(valid=valid, **kwargs)
@@ -876,15 +912,15 @@
 
     _attribute_map = {
         "valid": {"key": "valid", "type": "bool"},
         "type": {"key": "type", "type": "str"},
         "value": {"key": "value", "type": "str"},
     }
 
-    def __init__(self, *, valid: bool = True, value: Optional[str] = None, **kwargs):
+    def __init__(self, *, valid: bool = True, value: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         :keyword value:
         :paramtype value: str
         """
         super().__init__(valid=valid, **kwargs)
@@ -914,15 +950,17 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "metadata": {"key": "metadata", "type": "PageMetadata"},
         "content": {"key": "content", "type": "[ProcessPageItem]"},
     }
 
-    def __init__(self, *, metadata: "_models.PageMetadata", content: List["_models.ProcessPageItem"], **kwargs):
+    def __init__(
+        self, *, metadata: "_models.PageMetadata", content: List["_models.ProcessPageItem"], **kwargs: Any
+    ) -> None:
         """
         :keyword metadata: Required.
         :paramtype metadata: ~kuflow.rest.models.PageMetadata
         :keyword content: Required.
         :paramtype content: list[~kuflow.rest.models.ProcessPageItem]
         """
         super().__init__(metadata=metadata, **kwargs)
@@ -989,16 +1027,16 @@
         last_modified_by: Optional[str] = None,
         last_modified_at: Optional[datetime.datetime] = None,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         subject: Optional[str] = None,
         state: Optional[Union[str, "_models.ProcessState"]] = None,
         element_values: Optional[Dict[str, List["_models.ProcessElementValue"]]] = None,
         initiator: Optional["_models.Principal"] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword created_by: Who create this model.
         :paramtype created_by: str
         :keyword created_at: When this model was created.
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: Who was last update this model.
         :paramtype last_modified_by: str
@@ -1054,16 +1092,16 @@
     }
 
     def __init__(
         self,
         *,
         element_definition_code: str,
         element_values: Optional[List["_models.ProcessElementValue"]] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword element_definition_code: Required.
         :paramtype element_definition_code: str
         :keyword element_values:
         :paramtype element_values: list[~kuflow.rest.models.ProcessElementValue]
         """
         super().__init__(**kwargs)
@@ -1081,15 +1119,17 @@
     """
 
     _attribute_map = {
         "incoming": {"key": "incoming", "type": "[str]"},
         "outcoming": {"key": "outcoming", "type": "[str]"},
     }
 
-    def __init__(self, *, incoming: Optional[List[str]] = None, outcoming: Optional[List[str]] = None, **kwargs):
+    def __init__(
+        self, *, incoming: Optional[List[str]] = None, outcoming: Optional[List[str]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword incoming: Processes whose relationship target is the current process.
         :paramtype incoming: list[str]
         :keyword outcoming: Processes to which the current process relates.
         :paramtype outcoming: list[str]
         """
         super().__init__(**kwargs)
@@ -1117,16 +1157,20 @@
     :vartype id: str
     :ivar state: Task state. Known values are: "READY", "CLAIMED", "COMPLETED", and "CANCELLED".
     :vartype state: str or ~kuflow.rest.models.TaskState
     :ivar task_definition: In creation task, one of 'id, version or code' is mandatory. Required.
     :vartype task_definition: ~kuflow.rest.models.TaskDefinitionSummary
     :ivar process_id: Required.
     :vartype process_id: str
-    :ivar element_values: Task element values, en ElementValueDocument is not allowed.
+    :ivar element_values: Task element values, en ElementValueDocument is not allowed, used when
+     the task render type selected is
+     JSON Forms.
     :vartype element_values: dict[str, list[~kuflow.rest.models.TaskElementValue]]
+    :ivar json_forms_value: Json form values, used when the render type selected is JSON Forms.
+    :vartype json_forms_value: ~kuflow.rest.models.JsonFormsValue
     :ivar logs:
     :vartype logs: list[~kuflow.rest.models.Log]
     :ivar owner:
     :vartype owner: ~kuflow.rest.models.Principal
     """
 
     _validation = {
@@ -1142,14 +1186,15 @@
         "last_modified_by": {"key": "lastModifiedBy", "type": "str"},
         "last_modified_at": {"key": "lastModifiedAt", "type": "iso-8601"},
         "id": {"key": "id", "type": "str"},
         "state": {"key": "state", "type": "str"},
         "task_definition": {"key": "taskDefinition", "type": "TaskDefinitionSummary"},
         "process_id": {"key": "processId", "type": "str"},
         "element_values": {"key": "elementValues", "type": "{[TaskElementValue]}"},
+        "json_forms_value": {"key": "jsonFormsValue", "type": "JsonFormsValue"},
         "logs": {"key": "logs", "type": "[Log]"},
         "owner": {"key": "owner", "type": "Principal"},
     }
 
     def __init__(
         self,
         *,
@@ -1158,18 +1203,19 @@
         created_by: Optional[str] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_at: Optional[datetime.datetime] = None,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         state: Optional[Union[str, "_models.TaskState"]] = None,
         element_values: Optional[Dict[str, List["_models.TaskElementValue"]]] = None,
+        json_forms_value: Optional["_models.JsonFormsValue"] = None,
         logs: Optional[List["_models.Log"]] = None,
         owner: Optional["_models.Principal"] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword created_by: Who create this model.
         :paramtype created_by: str
         :keyword created_at: When this model was created.
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: Who was last update this model.
         :paramtype last_modified_by: str
@@ -1180,16 +1226,20 @@
         :keyword state: Task state. Known values are: "READY", "CLAIMED", "COMPLETED", and "CANCELLED".
         :paramtype state: str or ~kuflow.rest.models.TaskState
         :keyword task_definition: In creation task, one of 'id, version or code' is mandatory.
          Required.
         :paramtype task_definition: ~kuflow.rest.models.TaskDefinitionSummary
         :keyword process_id: Required.
         :paramtype process_id: str
-        :keyword element_values: Task element values, en ElementValueDocument is not allowed.
+        :keyword element_values: Task element values, en ElementValueDocument is not allowed, used when
+         the task render type selected is
+         JSON Forms.
         :paramtype element_values: dict[str, list[~kuflow.rest.models.TaskElementValue]]
+        :keyword json_forms_value: Json form values, used when the render type selected is JSON Forms.
+        :paramtype json_forms_value: ~kuflow.rest.models.JsonFormsValue
         :keyword logs:
         :paramtype logs: list[~kuflow.rest.models.Log]
         :keyword owner:
         :paramtype owner: ~kuflow.rest.models.Principal
         """
         super().__init__(
             created_by=created_by,
@@ -1200,14 +1250,15 @@
         )
         self.object_type: str = "TASK"
         self.id = id
         self.state = state
         self.task_definition = task_definition
         self.process_id = process_id
         self.element_values = element_values
+        self.json_forms_value = json_forms_value
         self.logs = logs
         self.owner = owner
 
 
 class TaskAssignCommand(_serialization.Model):
     """Command to assign task, only one option is required.
 
@@ -1218,15 +1269,15 @@
     """
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "email": {"key": "email", "type": "str"},
     }
 
-    def __init__(self, *, principal_id: Optional[str] = None, email: Optional[str] = None, **kwargs):
+    def __init__(self, *, principal_id: Optional[str] = None, email: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword principal_id:
         :paramtype principal_id: str
         :keyword email:
         :paramtype email: str
         """
         super().__init__(**kwargs)
@@ -1261,16 +1312,16 @@
     def __init__(
         self,
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         version: Optional[str] = None,
         code: Optional[str] = None,
         name: Optional[str] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword version:
         :paramtype version: str
         :keyword code:
         :paramtype code: str
@@ -1297,15 +1348,15 @@
         "element_definition_code": {"required": True},
     }
 
     _attribute_map = {
         "element_definition_code": {"key": "elementDefinitionCode", "type": "str"},
     }
 
-    def __init__(self, *, element_definition_code: str, **kwargs):
+    def __init__(self, *, element_definition_code: str, **kwargs: Any) -> None:
         """
         :keyword element_definition_code: Code of task element to delete. Required.
         :paramtype element_definition_code: str
         """
         super().__init__(**kwargs)
         self.element_definition_code = element_definition_code
 
@@ -1323,15 +1374,15 @@
         "document_id": {"required": True},
     }
 
     _attribute_map = {
         "document_id": {"key": "documentId", "type": "str"},
     }
 
-    def __init__(self, *, document_id: str, **kwargs):
+    def __init__(self, *, document_id: str, **kwargs: Any) -> None:
         """
         :keyword document_id: Document ID to delete. Required.
         :paramtype document_id: str
         """
         super().__init__(**kwargs)
         self.document_id = document_id
 
@@ -1367,15 +1418,15 @@
             "NUMBER": "TaskElementValueNumber",
             "OBJECT": "TaskElementValueObject",
             "PRINCIPAL": "TaskElementValuePrincipal",
             "STRING": "TaskElementValueString",
         }
     }
 
-    def __init__(self, *, valid: bool = True, **kwargs):
+    def __init__(self, *, valid: bool = True, **kwargs: Any) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         """
         super().__init__(**kwargs)
         self.valid = valid
         self.type: Optional[str] = None
@@ -1401,15 +1452,17 @@
 
     _attribute_map = {
         "valid": {"key": "valid", "type": "bool"},
         "type": {"key": "type", "type": "str"},
         "value": {"key": "value", "type": "TaskElementValueDocumentItem"},
     }
 
-    def __init__(self, *, valid: bool = True, value: Optional["_models.TaskElementValueDocumentItem"] = None, **kwargs):
+    def __init__(
+        self, *, valid: bool = True, value: Optional["_models.TaskElementValueDocumentItem"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         :keyword value:
         :paramtype value: ~kuflow.rest.models.TaskElementValueDocumentItem
         """
         super().__init__(valid=valid, **kwargs)
@@ -1448,16 +1501,16 @@
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         uri: Optional[str] = None,
         name: Optional[str] = None,
         content_path: Optional[str] = None,
         content_type: Optional[str] = None,
         content_length: Optional[int] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword uri:
         :paramtype uri: str
         :keyword name:
         :paramtype name: str
@@ -1497,15 +1550,15 @@
 
     _attribute_map = {
         "valid": {"key": "valid", "type": "bool"},
         "type": {"key": "type", "type": "str"},
         "value": {"key": "value", "type": "float"},
     }
 
-    def __init__(self, *, valid: bool = True, value: Optional[float] = None, **kwargs):
+    def __init__(self, *, valid: bool = True, value: Optional[float] = None, **kwargs: Any) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         :keyword value:
         :paramtype value: float
         """
         super().__init__(valid=valid, **kwargs)
@@ -1533,15 +1586,15 @@
 
     _attribute_map = {
         "valid": {"key": "valid", "type": "bool"},
         "type": {"key": "type", "type": "str"},
         "value": {"key": "value", "type": "{object}"},
     }
 
-    def __init__(self, *, valid: bool = True, value: Optional[Dict[str, Any]] = None, **kwargs):
+    def __init__(self, *, valid: bool = True, value: Optional[Dict[str, Any]] = None, **kwargs: Any) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         :keyword value: Dictionary of :code:`<any>`.
         :paramtype value: dict[str, any]
         """
         super().__init__(valid=valid, **kwargs)
@@ -1570,16 +1623,16 @@
     _attribute_map = {
         "valid": {"key": "valid", "type": "bool"},
         "type": {"key": "type", "type": "str"},
         "value": {"key": "value", "type": "TaskElementValuePrincipalItem"},
     }
 
     def __init__(
-        self, *, valid: bool = True, value: Optional["_models.TaskElementValuePrincipalItem"] = None, **kwargs
-    ):
+        self, *, valid: bool = True, value: Optional["_models.TaskElementValuePrincipalItem"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         :keyword value:
         :paramtype value: ~kuflow.rest.models.TaskElementValuePrincipalItem
         """
         super().__init__(valid=valid, **kwargs)
@@ -1613,16 +1666,16 @@
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         type: Union[str, "_models.PrincipalType"],
         name: Optional[str] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword type: Required. Known values are: "USER", "APPLICATION", and "SYSTEM".
         :paramtype type: str or ~kuflow.rest.models.PrincipalType
         :keyword name:
         :paramtype name: str
@@ -1653,15 +1706,15 @@
 
     _attribute_map = {
         "valid": {"key": "valid", "type": "bool"},
         "type": {"key": "type", "type": "str"},
         "value": {"key": "value", "type": "str"},
     }
 
-    def __init__(self, *, valid: bool = True, value: Optional[str] = None, **kwargs):
+    def __init__(self, *, valid: bool = True, value: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword valid:
         :paramtype valid: bool
         :keyword value:
         :paramtype value: str
         """
         super().__init__(valid=valid, **kwargs)
@@ -1691,15 +1744,17 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "metadata": {"key": "metadata", "type": "PageMetadata"},
         "content": {"key": "content", "type": "[TaskPageItem]"},
     }
 
-    def __init__(self, *, metadata: "_models.PageMetadata", content: List["_models.TaskPageItem"], **kwargs):
+    def __init__(
+        self, *, metadata: "_models.PageMetadata", content: List["_models.TaskPageItem"], **kwargs: Any
+    ) -> None:
         """
         :keyword metadata: Required.
         :paramtype metadata: ~kuflow.rest.models.PageMetadata
         :keyword content: Required.
         :paramtype content: list[~kuflow.rest.models.TaskPageItem]
         """
         super().__init__(metadata=metadata, **kwargs)
@@ -1729,14 +1784,16 @@
     :vartype state: str or ~kuflow.rest.models.TaskState
     :ivar task_definition: In creation task, one of 'id, version or code' is mandatory. Required.
     :vartype task_definition: ~kuflow.rest.models.TaskDefinitionSummary
     :ivar process_id: Required.
     :vartype process_id: str
     :ivar element_values: Task element values, en ElementValueDocument is not allowed.
     :vartype element_values: dict[str, list[~kuflow.rest.models.TaskElementValue]]
+    :ivar json_forms_value: Json form values, used when the render type selected is JSON Forms.
+    :vartype json_forms_value: ~kuflow.rest.models.JsonFormsValue
     :ivar owner:
     :vartype owner: ~kuflow.rest.models.Principal
     """
 
     _validation = {
         "object_type": {"required": True},
         "task_definition": {"required": True},
@@ -1750,14 +1807,15 @@
         "last_modified_by": {"key": "lastModifiedBy", "type": "str"},
         "last_modified_at": {"key": "lastModifiedAt", "type": "iso-8601"},
         "id": {"key": "id", "type": "str"},
         "state": {"key": "state", "type": "str"},
         "task_definition": {"key": "taskDefinition", "type": "TaskDefinitionSummary"},
         "process_id": {"key": "processId", "type": "str"},
         "element_values": {"key": "elementValues", "type": "{[TaskElementValue]}"},
+        "json_forms_value": {"key": "jsonFormsValue", "type": "JsonFormsValue"},
         "owner": {"key": "owner", "type": "Principal"},
     }
 
     def __init__(
         self,
         *,
         task_definition: "_models.TaskDefinitionSummary",
@@ -1765,17 +1823,18 @@
         created_by: Optional[str] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_at: Optional[datetime.datetime] = None,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         state: Optional[Union[str, "_models.TaskState"]] = None,
         element_values: Optional[Dict[str, List["_models.TaskElementValue"]]] = None,
+        json_forms_value: Optional["_models.JsonFormsValue"] = None,
         owner: Optional["_models.Principal"] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword created_by: Who create this model.
         :paramtype created_by: str
         :keyword created_at: When this model was created.
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: Who was last update this model.
         :paramtype last_modified_by: str
@@ -1788,14 +1847,16 @@
         :keyword task_definition: In creation task, one of 'id, version or code' is mandatory.
          Required.
         :paramtype task_definition: ~kuflow.rest.models.TaskDefinitionSummary
         :keyword process_id: Required.
         :paramtype process_id: str
         :keyword element_values: Task element values, en ElementValueDocument is not allowed.
         :paramtype element_values: dict[str, list[~kuflow.rest.models.TaskElementValue]]
+        :keyword json_forms_value: Json form values, used when the render type selected is JSON Forms.
+        :paramtype json_forms_value: ~kuflow.rest.models.JsonFormsValue
         :keyword owner:
         :paramtype owner: ~kuflow.rest.models.Principal
         """
         super().__init__(
             created_by=created_by,
             created_at=created_at,
             last_modified_by=last_modified_by,
@@ -1804,14 +1865,15 @@
         )
         self.object_type: str = "TASK_PAGE_ITEM"
         self.id = id
         self.state = state
         self.task_definition = task_definition
         self.process_id = process_id
         self.element_values = element_values
+        self.json_forms_value = json_forms_value
         self.owner = owner
 
 
 class TaskSaveElementCommand(_serialization.Model):
     """TaskSaveElementCommand.
 
     All required parameters must be populated in order to send to Azure.
@@ -1832,27 +1894,79 @@
     }
 
     def __init__(
         self,
         *,
         element_definition_code: str,
         element_values: Optional[List["_models.TaskElementValue"]] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword element_definition_code: Required.
         :paramtype element_definition_code: str
         :keyword element_values:
         :paramtype element_values: list[~kuflow.rest.models.TaskElementValue]
         """
         super().__init__(**kwargs)
         self.element_definition_code = element_definition_code
         self.element_values = element_values
 
 
+class TaskSaveJsonFormsValueDataCommand(_serialization.Model):
+    """TaskSaveJsonFormsValueDataCommand.
+
+    :ivar data: json value filled that complain with the related json schema.
+    :vartype data: dict[str, any]
+    """
+
+    _attribute_map = {
+        "data": {"key": "data", "type": "{object}"},
+    }
+
+    def __init__(self, *, data: Optional[Dict[str, Any]] = None, **kwargs: Any) -> None:
+        """
+        :keyword data: json value filled that complain with the related json schema.
+        :paramtype data: dict[str, any]
+        """
+        super().__init__(**kwargs)
+        self.data = data
+
+
+class TaskSaveJsonFormsValueDocumentResponseCommand(_serialization.Model):
+    """TaskSaveJsonFormsValueDocumentResponseCommand.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar value: JSON value representing the uploaded file.
+
+     Example: ``kuflow-file:uri=xxx-yyy-zzz;type=application/json;size=500;name=file.json;``.
+     Required.
+    :vartype value: str
+    """
+
+    _validation = {
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "str"},
+    }
+
+    def __init__(self, *, value: str, **kwargs: Any) -> None:
+        """
+        :keyword value: JSON value representing the uploaded file.
+
+         Example: ``kuflow-file:uri=xxx-yyy-zzz;type=application/json;size=500;name=file.json;``.
+         Required.
+        :paramtype value: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+
+
 class WebhookEvent(_serialization.Model):
     """WebhookEvent.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
     WebhookEventProcessStateChanged, WebhookEventTaskStateChanged
 
     All required parameters must be populated in order to send to Azure.
@@ -1881,15 +1995,17 @@
     _subtype_map = {
         "type": {
             "PROCESS.STATE_CHANGED": "WebhookEventProcessStateChanged",
             "TASK.STATE_CHANGED": "WebhookEventTaskStateChanged",
         }
     }
 
-    def __init__(self, *, id: str, timestamp: datetime.datetime, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(
+        self, *, id: str, timestamp: datetime.datetime, **kwargs: Any  # pylint: disable=redefined-builtin
+    ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword timestamp: Required.
         :paramtype timestamp: ~datetime.datetime
         """
         super().__init__(**kwargs)
@@ -1930,16 +2046,16 @@
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         timestamp: datetime.datetime,
         data: "_models.WebhookEventProcessStateChangedData",
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword timestamp: Required.
         :paramtype timestamp: ~datetime.datetime
         :keyword data: Required.
         :paramtype data: ~kuflow.rest.models.WebhookEventProcessStateChangedData
@@ -1967,15 +2083,15 @@
     }
 
     _attribute_map = {
         "process_id": {"key": "processId", "type": "str"},
         "process_state": {"key": "processState", "type": "str"},
     }
 
-    def __init__(self, *, process_id: str, process_state: Union[str, "_models.ProcessState"], **kwargs):
+    def __init__(self, *, process_id: str, process_state: Union[str, "_models.ProcessState"], **kwargs: Any) -> None:
         """
         :keyword process_id: Required.
         :paramtype process_id: str
         :keyword process_state: Process state. Required. Known values are: "RUNNING", "COMPLETED", and
          "CANCELLED".
         :paramtype process_state: str or ~kuflow.rest.models.ProcessState
         """
@@ -2016,16 +2132,16 @@
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         timestamp: datetime.datetime,
         data: "_models.WebhookEventTaskStateChangedData",
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword timestamp: Required.
         :paramtype timestamp: ~datetime.datetime
         :keyword data: Required.
         :paramtype data: ~kuflow.rest.models.WebhookEventTaskStateChangedData
@@ -2062,16 +2178,22 @@
         "process_id": {"key": "processId", "type": "str"},
         "task_id": {"key": "taskId", "type": "str"},
         "task_code": {"key": "taskCode", "type": "str"},
         "task_state": {"key": "taskState", "type": "str"},
     }
 
     def __init__(
-        self, *, process_id: str, task_id: str, task_code: str, task_state: Union[str, "_models.TaskState"], **kwargs
-    ):
+        self,
+        *,
+        process_id: str,
+        task_id: str,
+        task_code: str,
+        task_state: Union[str, "_models.TaskState"],
+        **kwargs: Any,
+    ) -> None:
         """
         :keyword process_id: Required.
         :paramtype process_id: str
         :keyword task_id: Required.
         :paramtype task_id: str
         :keyword task_code: Required.
         :paramtype task_code: str
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/models/_patch.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/operations/__init__.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_authentication_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_authentication_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -132,16 +133,16 @@
     def create_authentication(
         self, authentication: Union[_models.Authentication, IO], **kwargs: Any
     ) -> _models.Authentication:
         """Create an authentication for the current principal.
 
         Create an authentication for the current principal.
 
-        :param authentication: Authentication to be created. Is either a model type or a IO type.
-         Required.
+        :param authentication: Authentication to be created. Is either a Authentication type or a IO
+         type. Required.
         :type authentication: ~kuflow.rest.models.Authentication or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Authentication
         :rtype: ~kuflow.rest.models.Authentication
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -159,30 +160,31 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Authentication] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(authentication, (IO, bytes)):
+        if isinstance(authentication, (IOBase, bytes)):
             _content = authentication
         else:
             _json = self._serialize.body(authentication, "Authentication")
 
         request = build_create_authentication_request(
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_patch.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_principal_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_principal_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,16 +187,17 @@
             type=type,
             group_id=group_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -237,16 +238,17 @@
         request = build_retrieve_principal_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_process_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_process_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -314,16 +315,17 @@
             page=page,
             sort=sort,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -408,15 +410,15 @@
         * If you know the ``principal ID`` you can assign it to ``initiator.id``
         * If you know the ``user ID`` you can assign it to ``initiator.user.id``
         * If you know the ``user email`` you can assign it to ``initiator.user.email``
         * If you know the ``application ID`` you can assign it to ``initiator.application.id``
 
         If you want the method to be idempotent, please specify the ``id`` field in the request body.
 
-        :param process: Process to create. Is either a model type or a IO type. Required.
+        :param process: Process to create. Is either a Process type or a IO type. Required.
         :type process: ~kuflow.rest.models.Process or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -434,30 +436,31 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Process] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(process, (IO, bytes)):
+        if isinstance(process, (IOBase, bytes)):
             _content = process
         else:
             _json = self._serialize.body(process, "Process")
 
         request = build_create_process_request(
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -502,16 +505,17 @@
         request = build_retrieve_process_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -587,16 +591,16 @@
 
         Allows you to choose a user (by email or principal identifier) or an application (principal
         identifier).
         Only one option will be necessary.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to change the process initiator. Is either a model type or a IO type.
-         Required.
+        :param command: Command to change the process initiator. Is either a
+         ProcessChangeInitiatorCommand type or a IO type. Required.
         :type command: ~kuflow.rest.models.ProcessChangeInitiatorCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -614,31 +618,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Process] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "ProcessChangeInitiatorCommand")
 
         request = build_actions_process_change_initiator_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -720,15 +725,16 @@
         otherwise it creates them. The values of the previous elements that no longer exist will be
         deleted.
 
         If the process is already finished the invocations fails with an error.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to save an element. Is either a model type or a IO type. Required.
+        :param command: Command to save an element. Is either a ProcessSaveElementCommand type or a IO
+         type. Required.
         :type command: ~kuflow.rest.models.ProcessSaveElementCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -746,31 +752,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Process] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "ProcessSaveElementCommand")
 
         request = build_actions_process_save_element_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -840,15 +847,16 @@
 
         Allow to delete a process element by specifying the item definition code.
 
         Remove all the element values.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete an element. Is either a model type or a IO type. Required.
+        :param command: Command to delete an element. Is either a ProcessDeleteElementCommand type or a
+         IO type. Required.
         :type command: ~kuflow.rest.models.ProcessDeleteElementCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -866,31 +874,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Process] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "ProcessDeleteElementCommand")
 
         request = build_actions_process_delete_element_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -933,16 +942,17 @@
         request = build_actions_process_complete_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -987,16 +997,17 @@
         request = build_actions_process_cancel_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1055,16 +1066,17 @@
             content_type=content_type,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 304]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_generated/operations/_task_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_task_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterator, List, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -333,14 +334,91 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_actions_task_save_json_forms_value_data_request(id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/tasks/{id}/~actions/save-json-forms-value-data"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_actions_task_save_json_forms_value_document_request(
+    id: str, *, file_content_type: str, file_name: str, schema_path: str, content: IO, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/tasks/{id}/~actions/save-json-forms-value-document"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["fileContentType"] = _SERIALIZER.query("file_content_type", file_content_type, "str")
+    _params["fileName"] = _SERIALIZER.query("file_name", file_name, "str")
+    _params["schemaPath"] = _SERIALIZER.query("schema_path", schema_path, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, content=content, **kwargs)
+
+
+def build_actions_task_download_json_forms_value_document_request(
+    id: str, *, document_uri: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/octet-stream, application/json")
+
+    # Construct URL
+    _url = "/tasks/{id}/~actions/download-json-forms-value-document"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["documentUri"] = _SERIALIZER.query("document_uri", document_uri, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 def build_actions_task_complete_request(id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/tasks/{id}/~actions/complete"
@@ -459,16 +537,17 @@
             state=state,
             task_definition_code=task_definition_code,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -579,15 +658,15 @@
         * If you know the ``principal ID`` you can assign it to ``owner.id``
         * If you know the ``user ID`` you can assign it to ``owner.user.id``
         * If you know the ``user email`` you can assign it to ``owner.user.email``
         * If you know the ``application ID`` you can assign it to ``owner.application.id``
 
         If you want the method to be idempotent, please specify the ``id`` field in the request body.
 
-        :param task: Task to be created. Is either a model type or a IO type. Required.
+        :param task: Task to be created. Is either a Task type or a IO type. Required.
         :type task: ~kuflow.rest.models.Task or IO
         :keyword activity_token: When create a Kuflow Task backed with a Temporal.io servers, this
          value is required and must be set with the context task token of Temporal.io activity. Default
          value is None.
         :paramtype activity_token: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
@@ -609,31 +688,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(task, (IO, bytes)):
+        if isinstance(task, (IOBase, bytes)):
             _content = task
         else:
             _json = self._serialize.body(task, "Task")
 
         request = build_create_task_request(
             activity_token=activity_token,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -678,16 +758,17 @@
         request = build_retrieve_task_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -728,16 +809,17 @@
         request = build_actions_task_claim_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -796,16 +878,16 @@
     ) -> _models.Task:
         """Assign a task.
 
         Allow to assign a task to a user or application. Only one option will be necessary.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to change the task owner. Is either a model type or a IO type.
-         Required.
+        :param command: Command to change the task owner. Is either a TaskAssignCommand type or a IO
+         type. Required.
         :type command: ~kuflow.rest.models.TaskAssignCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -823,31 +905,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "TaskAssignCommand")
 
         request = build_actions_task_assign_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -930,15 +1013,16 @@
         to add a new document, please use the corresponding API method. If values already exist for the
         provided element code, it replaces them with the new ones, otherwise it creates them. The
         values of the previous elements that no longer exist will be deleted. To remove an element, use
         the appropriate API method.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to save an element. Is either a model type or a IO type. Required.
+        :param command: Command to save an element. Is either a TaskSaveElementCommand type or a IO
+         type. Required.
         :type command: ~kuflow.rest.models.TaskSaveElementCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -956,31 +1040,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "TaskSaveElementCommand")
 
         request = build_actions_task_save_element_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1058,16 +1143,17 @@
             content_type=content_type,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1137,15 +1223,16 @@
 
         Allow to delete task element by specifying the item definition code.
 
         Remove all the element values.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete an element. Is either a model type or a IO type. Required.
+        :param command: Command to delete an element. Is either a TaskDeleteElementCommand type or a IO
+         type. Required.
         :type command: ~kuflow.rest.models.TaskDeleteElementCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1163,31 +1250,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "TaskDeleteElementCommand")
 
         request = build_actions_task_delete_element_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1214,15 +1302,15 @@
         Allow to delete a specific document from an element of document type using its id.
 
         Note: If it is a multiple item, it will only delete the specified document. If it is a single
         element, in addition to the document, it will also delete the element.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete a document elemente value. Required.
+        :param command: Command to delete a document element value. Required.
         :type command: ~kuflow.rest.models.TaskDeleteElementValueDocumentCommand
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1237,15 +1325,15 @@
         Allow to delete a specific document from an element of document type using its id.
 
         Note: If it is a multiple item, it will only delete the specified document. If it is a single
         element, in addition to the document, it will also delete the element.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete a document elemente value. Required.
+        :param command: Command to delete a document element value. Required.
         :type command: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1260,16 +1348,16 @@
         Allow to delete a specific document from an element of document type using its id.
 
         Note: If it is a multiple item, it will only delete the specified document. If it is a single
         element, in addition to the document, it will also delete the element.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete a document elemente value. Is either a model type or a IO
-         type. Required.
+        :param command: Command to delete a document element value. Is either a
+         TaskDeleteElementValueDocumentCommand type or a IO type. Required.
         :type command: ~kuflow.rest.models.TaskDeleteElementValueDocumentCommand or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1287,31 +1375,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(command, (IO, bytes)):
+        if isinstance(command, (IOBase, bytes)):
             _content = command
         else:
             _json = self._serialize.body(command, "TaskDeleteElementValueDocumentCommand")
 
         request = build_actions_task_delete_element_value_document_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1357,16 +1446,17 @@
             id=id,
             document_id=document_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = True
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=True, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1416,16 +1506,265 @@
             id=id,
             element_definition_code=element_definition_code,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = True
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
+            raise HttpResponseError(response=response, model=error)
+
+        deserialized = response.iter_bytes()
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    def actions_task_save_json_forms_value_data(
+        self,
+        id: str,
+        command: _models.TaskSaveJsonFormsValueDataCommand,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> _models.Task:
+        """Save JSON data.
+
+        Allow to save a JSON data validating that the data follow the related schema. If the data is
+        invalid, then
+        the json form is marked as invalid.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param command: Command to save the JSON value. Required.
+        :type command: ~kuflow.rest.models.TaskSaveJsonFormsValueDataCommand
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: Task
+        :rtype: ~kuflow.rest.models.Task
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def actions_task_save_json_forms_value_data(
+        self, id: str, command: IO, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.Task:
+        """Save JSON data.
+
+        Allow to save a JSON data validating that the data follow the related schema. If the data is
+        invalid, then
+        the json form is marked as invalid.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param command: Command to save the JSON value. Required.
+        :type command: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: Task
+        :rtype: ~kuflow.rest.models.Task
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def actions_task_save_json_forms_value_data(
+        self, id: str, command: Union[_models.TaskSaveJsonFormsValueDataCommand, IO], **kwargs: Any
+    ) -> _models.Task:
+        """Save JSON data.
+
+        Allow to save a JSON data validating that the data follow the related schema. If the data is
+        invalid, then
+        the json form is marked as invalid.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param command: Command to save the JSON value. Is either a TaskSaveJsonFormsValueDataCommand
+         type or a IO type. Required.
+        :type command: ~kuflow.rest.models.TaskSaveJsonFormsValueDataCommand or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: Task
+        :rtype: ~kuflow.rest.models.Task
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Task] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(command, (IOBase, bytes)):
+            _content = command
+        else:
+            _json = self._serialize.body(command, "TaskSaveJsonFormsValueDataCommand")
+
+        request = build_actions_task_save_json_forms_value_data_request(
+            id=id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
+            raise HttpResponseError(response=response, model=error)
+
+        deserialized = self._deserialize("Task", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace
+    def actions_task_save_json_forms_value_document(
+        self, id: str, file: IO, *, file_content_type: str, file_name: str, schema_path: str, **kwargs: Any
+    ) -> _models.TaskSaveJsonFormsValueDocumentResponseCommand:
+        """Save a JSON Forms document.
+
+        Save a document in the task to later be linked into the JSON data.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param file: Document to save. Required.
+        :type file: IO
+        :keyword file_content_type: Document content type. Required.
+        :paramtype file_content_type: str
+        :keyword file_name: Document name. Required.
+        :paramtype file_name: str
+        :keyword schema_path: JSON Schema path related to the document. The uploaded document must be
+         validated by the passed schema path. Required.
+        :paramtype schema_path: str
+        :return: TaskSaveJsonFormsValueDocumentResponseCommand
+        :rtype: ~kuflow.rest.models.TaskSaveJsonFormsValueDocumentResponseCommand
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: str = kwargs.pop("content_type", _headers.pop("Content-Type", "application/octet-stream"))
+        cls: ClsType[_models.TaskSaveJsonFormsValueDocumentResponseCommand] = kwargs.pop("cls", None)
+
+        _content = file
+
+        request = build_actions_task_save_json_forms_value_document_request(
+            id=id,
+            file_content_type=file_content_type,
+            file_name=file_name,
+            schema_path=schema_path,
+            content_type=content_type,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
+            raise HttpResponseError(response=response, model=error)
+
+        deserialized = self._deserialize("TaskSaveJsonFormsValueDocumentResponseCommand", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace
+    def actions_task_download_json_forms_value_document(
+        self, id: str, *, document_uri: str, **kwargs: Any
+    ) -> Iterator[bytes]:
+        """Download document.
+
+        Given a task, download a document from a json form data.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :keyword document_uri: Document URI to download. Required.
+        :paramtype document_uri: str
+        :return: Iterator of the response bytes
+        :rtype: Iterator[bytes]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Iterator[bytes]] = kwargs.pop("cls", None)
+
+        request = build_actions_task_download_json_forms_value_document_request(
+            id=id,
+            document_uri=document_uri,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = True
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=True, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1466,16 +1805,17 @@
         request = build_actions_task_complete_request(
             id=id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
@@ -1535,15 +1875,15 @@
         """Append a log to the task.
 
         A log entry is added to the task. If the number of log entries is reached, the oldest log entry
         is removed.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param log: Log to be created. Is either a model type or a IO type. Required.
+        :param log: Log to be created. Is either a Log type or a IO type. Required.
         :type log: ~kuflow.rest.models.Log or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1561,31 +1901,32 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Task] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(log, (IO, bytes)):
+        if isinstance(log, (IOBase, bytes)):
             _content = log
         else:
             _json = self._serialize.body(log, "Log")
 
         request = build_actions_task_append_log_request(
             id=id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultError, pipeline_response)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/_kuflow_rest_client.py` & `kuflow_rest-0.5.0/kuflow_rest/_kuflow_rest_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,20 +49,21 @@
         self.token = base64.b64encode("{}:{}".format(client_id, client_secret).encode("utf-8")).decode("utf-8")
 
     def get_token(
         self, *scopes: str, claims: Optional[str] = None, tenant_id: Optional[str] = None, **kwargs: Any
     ) -> AccessToken:
         """Request an access token for `scopes`.
 
-        :param str scopes: The type of access needed.
-
-        :keyword str claims: Additional claims required in the token, such as those returned in a resource
-            provider's claims challenge following an authorization failure.
-        :keyword str tenant_id: Optional tenant to include in the token request.
-
+        :param scopes: The type of access needed.
+        :type scopes: str
+        :keyword claims: Additional claims required in the token, such as those returned in a resource provider's
+                         claims challenge following an authorization failure.
+        :type claims: Optional[str]
+        :keyword tenant_id: Optional tenant to include in the token request.
+        :type tenant_id: Optional[str]
         :rtype: AccessToken
         :return: An AccessToken instance containing the token string and its expiration time in Unix time.
         """
         return AccessToken(token=self.token, expires_on=sys.maxsize)
 
 
 class AllowHttpPolicy(SansIOHTTPPolicy):
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/models/__init__.py` & `kuflow_rest-0.5.0/kuflow_rest/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from .._generated.models import __all__ as _all_generated_models
 
 from .._generated.models import (
     AbstractAudited,
     Authentication,
     DefaultError,
     DefaultErrorInfo,
+    JsonFormsValue,
     Log,
     Page,
     PageMetadata,
     Principal,
     PrincipalApplication,
     PrincipalPage,
     PrincipalUser,
@@ -60,14 +61,16 @@
     TaskElementValueObject,
     TaskElementValuePrincipal,
     TaskElementValuePrincipalItem,
     TaskElementValueString,
     TaskPage,
     TaskPageItem,
     TaskSaveElementCommand,
+    TaskSaveJsonFormsValueDataCommand,
+    TaskSaveJsonFormsValueDocumentResponseCommand,
     WebhookEvent,
     WebhookEventProcessStateChanged,
     WebhookEventProcessStateChangedData,
     WebhookEventTaskStateChanged,
     WebhookEventTaskStateChangedData,
     AuditedObjectType,
     LogLevel,
@@ -76,23 +79,31 @@
     ProcessElementValueType,
     ProcessState,
     TaskElementValueType,
     TaskState,
     WebhookType,
 )
 
-from ._models import Document, TaskSaveElementValueDocumentCommand, ProcessSaveUserActionValueDocumentCommand
+from ._models import (
+    Document,
+    JsonFormsFile,
+    JsonFormsPrincipal,
+    TaskSaveElementValueDocumentCommand,
+    TaskSaveJsonFormsValueDocumentRequestCommand,
+    ProcessSaveUserActionValueDocumentCommand,
+)
 
 
 __all__ = [
     # From _generated.models
     "AbstractAudited",
     "Authentication",
     "DefaultError",
     "DefaultErrorInfo",
+    "JsonFormsValue",
     "Log",
     "Page",
     "PageMetadata",
     "Principal",
     "PrincipalApplication",
     "PrincipalPage",
     "PrincipalUser",
@@ -119,14 +130,16 @@
     "TaskElementValueObject",
     "TaskElementValuePrincipal",
     "TaskElementValuePrincipalItem",
     "TaskElementValueString",
     "TaskPage",
     "TaskPageItem",
     "TaskSaveElementCommand",
+    "TaskSaveJsonFormsValueDataCommand",
+    "TaskSaveJsonFormsValueDocumentResponseCommand",
     "WebhookEvent",
     "WebhookEventProcessStateChanged",
     "WebhookEventProcessStateChangedData",
     "WebhookEventTaskStateChanged",
     "WebhookEventTaskStateChangedData",
     "AuditedObjectType",
     "LogLevel",
@@ -135,15 +148,18 @@
     "ProcessElementValueType",
     "ProcessState",
     "TaskElementValueType",
     "TaskState",
     "WebhookType",
     # From models
     "Document",
-    "ProcessSaveUserActionValueDocumentCommand",
+    "JsonFormsFile",
+    "JsonFormsPrincipal",
     "TaskSaveElementValueDocumentCommand",
+    "TaskSaveJsonFormsValueDocumentRequestCommand",
+    "ProcessSaveUserActionValueDocumentCommand",
 ]
 
 
 # For usability, we must include in __all__, all the items of the model generated package
 # So this assertion is to avoid forgetfulness.
 assert all(item in __all__ for item in _all_generated_models)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/operations/__init__.py` & `kuflow_rest-0.5.0/kuflow_rest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.5/kuflow_rest/operations/_authentication_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/operations/_authentication_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,19 +43,14 @@
         self.__kuflow_client = kuflow_client
 
     def create_authentication(self, authentication: _models.Authentication, **kwargs: Any) -> _models.Authentication:
         """Create an authentication for the current principal.
 
         Create an authentication for the current principal.
 
-        :param authentication: Authentication to be created. Is either a model type or a IO type.
-         Required.
+        :param authentication: Authentication to be created. Is either a model type or a IO type. Required.
         :type authentication: ~kuflow.rest.models.Authentication or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
         :return: Authentication
         :rtype: ~kuflow.rest.models.Authentication
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-
         return self.__kuflow_client.authentication.create_authentication(authentication=authentication, **kwargs)
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/operations/_principal_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/operations/_principal_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,34 +54,31 @@
         """Find all accessible Principals.
 
         List all the Principals that have been created and the used credentials has access.
 
         Available sort query values: id, name.
 
         :keyword size: The number of records returned within a single API call. Default value is 25.
-        :paramtype size: int
-        :keyword page: The page number of the current page in the returned records, 0 is the first
-         page. Default value is 0.
-        :paramtype page: int
+        :type size: int
+        :keyword page: The page number of the current page in the returned records, 0 is the first page.
+                       Default value is 0.
+        :type page: int
         :keyword sort: Sorting criteria in the format: property{,asc|desc}. Example: createdAt,desc
-
-         Default sort order is ascending. Multiple sort criteria are supported.
-
-         Please refer to the method description for supported properties. Default value is None.
-        :paramtype sort: Union[str, List[str]]
+                       Default sort order is ascending. Multiple sort criteria are supported.
+                       Please refer to the method description for supported properties. Default value is None.
+        :type sort: Optional[Union[str, List[str]]]
         :keyword type: Filter principals by type. Known values are: "USER", "APPLICATION", and
-         "SYSTEM". Default value is None.
-        :paramtype type: str or ~kuflow.rest.models.PrincipalType
+                      "SYSTEM". Default value is None.
+        :type type: Optional[_models.PrincipalType]
         :keyword group_id: Filter principals that exists in one of group ids. Default value is None.
-        :paramtype group_id: str or List[str]
+        :type group_id: Optional[Union[str, List[str]]]
         :return: PrincipalPage
         :rtype: ~kuflow.rest.models.PrincipalPage
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-
         if sort is not None and isinstance(sort, str):
             sort = [sort]
 
         if group_id is not None and isinstance(group_id, str):
             group_id = [group_id]
 
         return self.__kuflow_client.principal.find_principals(
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/operations/_process_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/operations/_process_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-
 from typing import Any, List, Optional, Union
 
 from .._generated import KuFlowRestClient as KuFlowRestClientGenerated
 
 from .. import models as _models
 
 
@@ -50,24 +49,24 @@
         """Find all accessible Processes.
 
         List all the Processes that have been created and the credentials has access.
 
         Available sort query values: id, createdAt, lastModifiedAt.
 
         :keyword size: The number of records returned within a single API call. Default value is 25.
-        :paramtype size: int
-        :keyword page: The page number of the current page in the returned records, 0 is the first
-         page. Default value is 0.
-        :paramtype page: int
+        :type size: int
+        :keyword page: The page number of the current page in the returned records, 0 is the first page.
+                       Default value is 0.
+        :type page: int
         :keyword sort: Sorting criteria in the format: property{,asc|desc}. Example: createdAt,desc
 
-         Default sort order is ascending. Multiple sort criteria are supported.
+                       Default sort order is ascending. Multiple sort criteria are supported.
 
-         Please refer to the method description for supported properties. Default value is None.
-        :paramtype sort: Union[str, List[str]]
+                       Please refer to the method description for supported properties. Default value is None.
+        :type sort: Optional[Union[str, List[str]]]
         :return: ProcessPage
         :rtype: ~kuflow.rest.models.ProcessPage
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         if sort is not None and isinstance(sort, str):
             sort = [sort]
 
@@ -86,16 +85,16 @@
         * If you know the ``principal ID`` you can assign it to ``initiator.id``
         * If you know the ``user ID`` you can assign it to ``initiator.user.id``
         * If you know the ``user email`` you can assign it to ``initiator.user.email``
         * If you know the ``application ID`` you can assign it to ``initiator.application.id``
 
         If you want the method to be idempotent, please specify the ``id`` field in the request body.
 
-        :param process: Process to create. Is either a model type or a IO type. Required.
-        :type process: ~kuflow.rest.models.Process or IO
+        :param process: Process to create. Required.
+        :type process: ~kuflow.rest.models.Process
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.process.create_process(process=process, **kwargs)
 
     def retrieve_process(self, id: str, **kwargs: Any) -> _models.Process:
@@ -120,17 +119,16 @@
 
         Allows you to choose a user (by email or principal identifier) or an application (principal
         identifier).
         Only one option will be necessary.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to change the process initiator. Is either a model type or a IO type.
-         Required.
-        :type command: ~kuflow.rest.models.ProcessChangeInitiatorCommand or IO
+        :param command: Command to change the process initiator. Required.
+        :type command: ~kuflow.rest.models.ProcessChangeInitiatorCommand
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.process.actions_process_change_initiator(id=id, command=command, **kwargs)
 
     def actions_process_save_element(
@@ -144,16 +142,16 @@
         otherwise it creates them. The values of the previous elements that no longer exist will be
         deleted.
 
         If the process is already finished the invocations fails with an error.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to save an element. Is either a model type or a IO type. Required.
-        :type command: ~kuflow.rest.models.ProcessSaveElementCommand or IO
+        :param command: Command to save an element. Required.
+        :type command: ~kuflow.rest.models.ProcessSaveElementCommand
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.process.actions_process_save_element(id=id, command=command, **kwargs)
 
     def actions_process_delete_element(
@@ -163,16 +161,16 @@
 
         Allow to delete a process element by specifying the item definition code.
 
         Remove all the element values.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete an element. Is either a model type or a IO type. Required.
-        :type command: ~kuflow.rest.models.ProcessDeleteElementCommand or IO
+        :param command: Command to delete an element. Required.
+        :type command: ~kuflow.rest.models.ProcessDeleteElementCommand
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.process.actions_process_delete_element(id=id, command=command, **kwargs)
 
     def actions_process_complete(self, id: str, **kwargs: Any) -> _models.Process:
```

### Comparing `kuflow_rest-0.4.5/kuflow_rest/operations/_task_operations.py` & `kuflow_rest-0.5.0/kuflow_rest/operations/_task_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 
-from typing import Any, IO, Iterator, List, Optional, Union
+from typing import Any, Iterator, List, Optional, Union
 
 from .._generated import KuFlowRestClient as KuFlowRestClientGenerated
 
 from .. import models as _models
 
 
 class TaskOperations:
@@ -58,31 +58,28 @@
 
         List all Tasks that have been created and the credentials has access.
 
         Available sort query values: id, createdAt, lastModifiedAt, claimedAt, completedAt,
         cancelledAt.
 
         :keyword size: The number of records returned within a single API call. Default value is 25.
-        :paramtype size: int
-        :keyword page: The page number of the current page in the returned records, 0 is the first
-         page. Default value is 0.
-        :paramtype page: int
+        :type size: int
+        :keyword page: The page number of the current page in the returned records, 0 is the first page.
+                       Default value is 0.
+        :type page: int
         :keyword sort: Sorting criteria in the format: property{,asc|desc}. Example: createdAt,desc
-
-         Default sort order is ascending. Multiple sort criteria are supported.
-
-         Please refer to the method description for supported properties. Default value is None.
-        :paramtype sort: list[str]
+                       Default sort order is ascending. Multiple sort criteria are supported.
+                       Please refer to the method description for supported properties. Default value is None.
+        :type sort: list[str]
         :keyword process_id: Filter by an array of process ids. Default value is None.
-        :paramtype process_id: list[str]
+        :type process_id: list[str]
         :keyword state: Filter by an array of task states. Default value is None.
-        :paramtype state: list[str or ~kuflow.rest.models.TaskState]
-        :keyword task_definition_code: Filter by an array of task definition codes. Default value is
-         None.
-        :paramtype task_definition_code: list[str]
+        :type state: list[str or ~kuflow.rest.models.TaskState]
+        :keyword task_definition_code: Filter by an array of task definition codes. Default value is None.
+        :type task_definition_code: list[str]
         :return: TaskPage
         :rtype: ~kuflow.rest.models.TaskPage
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         if sort is not None and isinstance(sort, str):
             sort = [sort]
         if process_id is not None and isinstance(process_id, str):
@@ -118,20 +115,20 @@
         * If you know the ``principal ID`` you can assign it to ``owner.id``
         * If you know the ``user ID`` you can assign it to ``owner.user.id``
         * If you know the ``user email`` you can assign it to ``owner.user.email``
         * If you know the ``application ID`` you can assign it to ``owner.application.id``
 
         If you want the method to be idempotent, please specify the ``id`` field in the request body.
 
-        :param task: Task to be created. Is either a model type or a IO type. Required.
+        :param task: Task to be created. Required.
         :type task: ~kuflow.rest.models.Task
         :keyword activity_token: When create a Kuflow Task backed with a Temporal.io servers, this
          value is required and must be set with the context task token of Temporal.io activity. Default
          value is None.
-        :paramtype activity_token: str
+        :type activity_token: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.task.create_task(task=task, activity_token=activity_token, **kwargs)
 
     def retrieve_task(self, id: str, **kwargs: Any) -> _models.Task:
@@ -163,17 +160,16 @@
     def actions_task_assign(self, id: str, command: _models.TaskAssignCommand, **kwargs: Any) -> _models.Task:
         """Assign a task.
 
         Allow to assign a task to a user or application. Only one option will be necessary.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to change the task owner. Is either a model type or a IO type.
-         Required.
-        :type command: ~kuflow.rest.models.TaskAssignCommand or IO
+        :param command: Command to change the task owner. Required.
+        :type command: ~kuflow.rest.models.TaskAssignCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.task.actions_task_assign(id=id, command=command, **kwargs)
 
     def actions_task_save_element(
@@ -189,16 +185,16 @@
         to add a new document, please use the corresponding API method. If values already exist for the
         provided element code, it replaces them with the new ones, otherwise it creates them. The
         values of the previous elements that no longer exist will be deleted. To remove an element, use
         the appropriate API method.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to save an element. Is either a model type or a IO type. Required.
-        :type command: ~kuflow.rest.models.TaskSaveElementCommand or IO
+        :param command: Command to save an element. Required.
+        :type command: ~kuflow.rest.models.TaskSaveElementCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.task.actions_task_save_element(id=id, command=command, **kwargs)
 
     def actions_task_save_element_value_document(
@@ -230,26 +226,26 @@
             element_definition_code=command.element_definition_code,
             element_value_id=command.element_value_id,
             element_value_valid=command.element_value_valid,
             **kwargs,
         )
 
     def actions_task_delete_element(
-        self, id: str, command: Union[_models.TaskDeleteElementCommand, IO], **kwargs: Any
+        self, id: str, command: _models.TaskDeleteElementCommand, **kwargs: Any
     ) -> _models.Task:
         """Delete an element by code.
 
         Allow to delete task element by specifying the item definition code.
 
         Remove all the element values.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete an element. Is either a model type or a IO type. Required.
-        :type command: ~kuflow.rest.models.TaskDeleteElementCommand or IO
+        :param command: Command to delete an element. Required.
+        :type command: ~kuflow.rest.models.TaskDeleteElementCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.task.actions_task_delete_element(id=id, command=command, **kwargs)
 
     def actions_task_delete_element_value_document(
@@ -260,32 +256,31 @@
         Allow to delete a specific document from an element of document type using its id.
 
         Note: If it is a multiple item, it will only delete the specified document. If it is a single
         element, in addition to the document, it will also delete the element.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param command: Command to delete a document element value. Is either a model type or a IO
-         type. Required.
-        :type command: ~kuflow.rest.models.TaskDeleteElementValueDocumentCommand or IO
+        :param command: Command to delete a document element value. Required.
+        :type command: ~kuflow.rest.models.TaskDeleteElementValueDocumentCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.task.actions_task_delete_element_value_document(id=id, command=command, **kwargs)
 
     def actions_task_download_element_value_document(self, id: str, document_id: str, **kwargs: Any) -> Iterator[bytes]:
         """Download document.
 
         Given a task, download a document from an element of document type.
 
         :param id: The resource ID. Required.
         :type id: str
         :keyword document_id: Document ID to download. Required.
-        :paramtype document_id: str
+        :type document_id: str
         :return: Iterator of the response bytes
         :rtype: Iterator[bytes]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.task.actions_task_download_element_value_document(
             id=id, document_id=document_id, **kwargs
         )
@@ -308,14 +303,87 @@
         :rtype: Iterator[bytes]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.task.actions_task_download_element_value_rendered(
             id=id, element_definition_code=element_definition_code, **kwargs
         )
 
+    def actions_task_save_json_forms_value_data(
+        self,
+        id: str,
+        command: _models.TaskSaveJsonFormsValueDataCommand,
+        **kwargs: Any,
+    ) -> _models.Task:
+        """Save JSON data.
+
+        Allow to save a JSON data validating that the data follow the related schema. If the data is
+        invalid, then
+        the json form is marked as invalid.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param command: Command to save the JSON value. Required.
+        :type command: ~kuflow.rest.models.TaskSaveJsonFormsValueDataCommand
+        :return: Task
+        :rtype: ~kuflow.rest.models.Task
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return self.__kuflow_client.task.actions_task_save_json_forms_value_data(id=id, command=command, **kwargs)
+
+    def actions_task_save_json_forms_value_document(
+        self,
+        id: str,
+        file: _models.Document,
+        command: _models.TaskSaveJsonFormsValueDocumentRequestCommand,
+        **kwargs: Any,
+    ) -> _models.TaskSaveJsonFormsValueDocumentResponseCommand:
+        """Save a JSON Forms document.
+
+        Save a document in the task to later be linked into the JSON data.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param file: Document to save. Required.
+        :type file: ~kuflow.rest.models.Document
+        :param command: Command to save the JSON value. Required.
+        :type command: ~kuflow.rest.models.TaskSaveJsonFormsValueDataCommand
+        :return: TaskSaveJsonFormsValueDocumentResponseCommand
+        :rtype: ~kuflow.rest.models.TaskSaveJsonFormsValueDocumentResponseCommand
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return self.__kuflow_client.task.actions_task_save_json_forms_value_document(
+            id=id,
+            file=file.file_content,
+            file_content_type=file.content_type,
+            file_name=file.file_mame,
+            schema_path=command.schema_path,
+            **kwargs,
+        )
+
+    def actions_task_download_json_forms_value_document(
+        self, id: str, *, document_uri: str, **kwargs: Any
+    ) -> Iterator[bytes]:
+        """Download document.
+
+        Given a task, download a document from a json form data.
+
+        :param id: The resource ID. Required.
+        :type id: str
+        :param document_uri: Document URI to download. Required.
+        :type document_uri: str
+        :return: Iterator of the response bytes
+        :rtype: Iterator[bytes]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return self.__kuflow_client.task.actions_task_download_json_forms_value_document(
+            id=id,
+            document_uri=document_uri,
+            **kwargs,
+        )
+
     def actions_task_complete(self, id: str, **kwargs: Any) -> _models.Task:
         """Complete a task.
 
         Allow to complete a claimed task by the principal.
 
         :param id: The resource ID. Required.
         :type id: str
@@ -329,14 +397,14 @@
         """Append a log to the task.
 
         A log entry is added to the task. If the number of log entries is reached, the oldest log entry
         is removed.
 
         :param id: The resource ID. Required.
         :type id: str
-        :param log: Log to be created. Is either a model type or a IO type. Required.
-        :type log: ~kuflow.rest.models.Log or IO
+        :param log: Log to be created. Required.
+        :type log: ~kuflow.rest.models.Log
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self.__kuflow_client.task.actions_task_append_log(id=id, log=log, **kwargs)
```

### Comparing `kuflow_rest-0.4.5/pyproject.toml` & `kuflow_rest-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-rest"
-version = "0.4.5"
+version = "0.5.0"
 description = "Client for KuFlow Rest Api"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,19 +13,27 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-azure-core = "^1.26.3"
+azure-core = "^1.26.4"
 isodate = "^0.6.1"
 
 [tool.poetry.group.dev.dependencies]
-mypy = "0.910"
-flake8 = "4.0.1"
-black = "^23.1.0"
-pytest = "^7.2.1"
+mypy = "^1.3.0"
+ipython = "^7.34.0"
+flake8 = "^5.0.4"
+black = "^23.3.0"
+pytest = "^7.3.1"
+
+[tool.pytest.ini_options]
+log_cli = true
+log_cli_level = "INFO"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+testpaths = ["tests"]
+python_files= "test_*.py"
 
 [tool.black]
 line-length = 120
 target-version = ["py38", "py39"]
```

### Comparing `kuflow_rest-0.4.5/setup.py` & `kuflow_rest-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 ['kuflow_rest',
  'kuflow_rest._generated',
  'kuflow_rest._generated.aio',
  'kuflow_rest._generated.aio.operations',
  'kuflow_rest._generated.models',
  'kuflow_rest._generated.operations',
  'kuflow_rest.models',
- 'kuflow_rest.operations']
+ 'kuflow_rest.operations',
+ 'kuflow_rest.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['azure-core>=1.26.3,<2.0.0', 'isodate>=0.6.1,<0.7.0']
+['azure-core>=1.26.4,<2.0.0', 'isodate>=0.6.1,<0.7.0']
 
 setup_kwargs = {
     'name': 'kuflow-rest',
-    'version': '0.4.5',
+    'version': '0.5.0',
     'description': 'Client for KuFlow Rest Api',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n\n# KuFlow Rest\n\nThis is a client for the KuFlow API Rest that allows you to interact with our API in a comfortable way in the creation of your workers and tools.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_rest-0.4.5/PKG-INFO` & `kuflow_rest-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-rest
-Version: 0.4.5
+Version: 0.5.0
 Summary: Client for KuFlow Rest Api
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: azure-core (>=1.26.3,<2.0.0)
+Requires-Dist: azure-core (>=1.26.4,<2.0.0)
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)
```

