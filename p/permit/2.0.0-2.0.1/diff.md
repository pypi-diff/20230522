# Comparing `tmp/permit-2.0.0.tar.gz` & `tmp/permit-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.0.0.tar", last modified: Mon May 22 06:46:16 2023, max compression
+gzip compressed data, was "permit-2.0.1.tar", last modified: Mon May 22 12:10:30 2023, max compression
```

## Comparing `permit-2.0.0.tar` & `permit-2.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.451383 permit-2.0.0/
--rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.0/LICENSE
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.0/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-05-22 06:46:16.451267 permit-2.0.0/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.0/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.447027 permit-2.0.0/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.0/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.449668 permit-2.0.0/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     9692 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/base.py
--rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/condition_set_rules.py
--rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/condition_sets.py
--rw-r--r--   0 asafc      (501) staff       (20)     3534 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/context.py
--rw-r--r--   0 asafc      (501) staff       (20)     6793 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/deprecated.py
--rw-r--r--   0 asafc      (501) staff       (20)     1927 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/elements.py
--rw-r--r--   0 asafc      (501) staff       (20)     8821 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/environments.py
--rw-r--r--   0 asafc      (501) staff       (20)   137541 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/models.py
--rw-r--r--   0 asafc      (501) staff       (20)     5098 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/resource_action_groups.py
--rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/sync_api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)     8862 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/users.py
--rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.0/permit/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.449939 permit-2.0.0/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.0/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.0/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.0/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     2859 2023-05-22 06:43:35.000000 permit-2.0.0/permit/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.0/permit/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.0/permit/permit.py
--rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.0/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.450586 permit-2.0.0/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.0/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.0/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.0/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.0/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.447504 permit-2.0.0/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.0/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-22 06:46:16.451418 permit-2.0.0/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      793 2023-05-22 06:43:35.000000 permit-2.0.0/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.451129 permit-2.0.0/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.0/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 06:43:35.000000 permit-2.0.0/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     9232 2023-05-22 06:43:35.000000 permit-2.0.0/tests/test_abac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8745 2023-05-22 06:43:35.000000 permit-2.0.0/tests/test_rbac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8666 2023-05-22 06:43:35.000000 permit-2.0.0/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.0/tests/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.047623 permit-2.0.1/
+-rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.1/LICENSE
+-rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.1/MANIFEST.in
+-rw-r--r--   0 asafc      (501) staff       (20)      467 2023-05-22 12:10:30.047501 permit-2.0.1/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.1/README.md
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.043583 permit-2.0.1/permit/
+-rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.1/permit/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.046121 permit-2.0.1/permit/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9730 2023-05-22 12:10:06.000000 permit-2.0.1/permit/api/base.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/condition_set_rules.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/condition_sets.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3534 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6805 2023-05-22 12:10:06.000000 permit-2.0.1/permit/api/deprecated.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.1/permit/api/elements.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8821 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/environments.py
+-rw-r--r--   0 asafc      (501) staff       (20)   137541 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/models.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5098 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/projects.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/resource_action_groups.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/resource_actions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/resource_attributes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/resources.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/role_assignments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/sync_api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/tenants.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8875 2023-05-22 12:10:06.000000 permit-2.0.1/permit/api/users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.1/permit/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.046393 permit-2.0.1/permit/enforcement/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.1/permit/enforcement/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.1/permit/enforcement/enforcer.py
+-rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.1/permit/enforcement/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2865 2023-05-22 12:10:06.000000 permit-2.0.1/permit/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.1/permit/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.1/permit/permit.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.1/permit/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.046779 permit-2.0.1/permit/utils/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.1/permit/utils/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.1/permit/utils/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.1/permit/utils/dicts.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.1/permit/utils/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.044085 permit-2.0.1/permit.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)      467 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       13 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.1/requirements.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-22 12:10:30.047661 permit-2.0.1/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)      793 2023-05-22 12:10:06.000000 permit-2.0.1/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.047340 permit-2.0.1/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.1/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.1/tests/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9232 2023-05-22 06:43:35.000000 permit-2.0.1/tests/test_abac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8745 2023-05-22 11:43:03.000000 permit-2.0.1/tests/test_rbac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8666 2023-05-22 06:43:35.000000 permit-2.0.1/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.1/tests/utils.py
```

### Comparing `permit-2.0.0/LICENSE` & `permit-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/api_client.py` & `permit-2.0.1/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/base.py` & `permit-2.0.1/permit/api/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import functools
-from typing import Optional, Type, TypeVar
+from typing import Optional, Type, TypeVar, Union
 
 import aiohttp
 from loguru import logger
 from pydantic import BaseModel, Extra, Field, parse_obj_as
 
 from ..config import PermitConfig
 from ..exceptions import PermitContextError, handle_api_error, handle_client_error
@@ -67,15 +67,15 @@
 
     def _log_response(self, url: str, method: str, status: int) -> None:
         logger.debug(
             "Received HTTP response: {} {}, status: {}".format(method, url, status)
         )
 
     def _prepare_json(
-        self, json: Optional[TData | dict | list] = None
+        self, json: Optional[Union[TData, dict, list]] = None
     ) -> Optional[dict]:
         if json is None:
             return None
 
         if isinstance(json, dict):
             return json
 
@@ -96,15 +96,15 @@
                 return parse_obj_as(model, data)
 
     @handle_client_error
     async def post(
         self,
         url,
         model: Type[TModel],
-        json: Optional[TData | dict | list] = None,
+        json: Optional[Union[TData, dict, list]] = None,
         **kwargs,
     ) -> TModel:
         url = f"{self._base_url}{url}"
         async with aiohttp.ClientSession(**self._client_config) as client:
             self._log_request(url, "POST")
             async with client.post(
                 url, json=self._prepare_json(json), **kwargs
@@ -115,15 +115,15 @@
                 return parse_obj_as(model, data)
 
     @handle_client_error
     async def put(
         self,
         url,
         model: Type[TModel],
-        json: Optional[TData | dict | list] = None,
+        json: Optional[Union[TData, dict, list]] = None,
         **kwargs,
     ) -> TModel:
         url = f"{self._base_url}{url}"
         async with aiohttp.ClientSession(**self._client_config) as client:
             self._log_request(url, "PUT")
             async with client.put(
                 url, json=self._prepare_json(json), **kwargs
@@ -134,15 +134,15 @@
                 return parse_obj_as(model, data)
 
     @handle_client_error
     async def patch(
         self,
         url,
         model: Type[TModel],
-        json: Optional[TData | dict | list] = None,
+        json: Optional[Union[TData, dict, list]] = None,
         **kwargs,
     ) -> TModel:
         url = f"{self._base_url}{url}"
         async with aiohttp.ClientSession(**self._client_config) as client:
             self._log_request(url, "PATCH")
             async with client.patch(
                 url, json=self._prepare_json(json), **kwargs
@@ -152,18 +152,18 @@
                 data = await response.json()
                 return parse_obj_as(model, data)
 
     @handle_client_error
     async def delete(
         self,
         url,
-        model: Type[TModel] | None = None,
-        json: Optional[TData | dict | list] = None,
+        model: Optional[Type[TModel]] = None,
+        json: Optional[Union[TData, dict, list]] = None,
         **kwargs,
-    ) -> TModel | None:
+    ) -> Optional[TModel]:
         url = f"{self._base_url}{url}"
         async with aiohttp.ClientSession(**self._client_config) as client:
             self._log_request(url, "DELETE")
             async with client.delete(
                 url, json=self._prepare_json(json), **kwargs
             ) as response:
                 await handle_api_error(response)
```

### Comparing `permit-2.0.0/permit/api/condition_set_rules.py` & `permit-2.0.1/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/condition_sets.py` & `permit-2.0.1/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/context.py` & `permit-2.0.1/permit/api/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/deprecated.py` & `permit-2.0.1/permit/api/deprecated.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,10 +178,10 @@
 
     @deprecated("use permit.api.resources.delete() instead")
     async def delete_resource(self, resource_key: str):
         return await self.__resources.delete(resource_key)
 
     @deprecated("use permit.elements.login_as() instead")
     async def elements_login_as(
-        self, user_id: str | UUID, tenant_id: str | UUID
+        self, user_id: Union[str, UUID], tenant_id: Union[str, UUID]
     ) -> EmbeddedLoginRequestOutput:
         return await self.__elements.login_as(user_id=user_id, tenant_id=tenant_id)
```

### Comparing `permit-2.0.0/permit/api/elements.py` & `permit-2.0.1/permit/api/elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Optional
+from typing import Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, Field
 
 from ..config import PermitConfig
 from ..utils.sync import SyncClass
 from .base import BasePermitApi
@@ -41,15 +41,15 @@
 
 class ElementsApi(BasePermitApi):
     def __init__(self, config: PermitConfig):
         super().__init__(config)
         self.__auth = self._build_http_client("/v2/auth")
 
     async def login_as(
-        self, user_id: str | UUID, tenant_id: str | UUID
+        self, user_id: Union[str, UUID], tenant_id: Union[str, UUID]
     ) -> UserLoginAsResponse:
         if isinstance(user_id, UUID):
             user_id = user_id.hex
         if isinstance(tenant_id, UUID):
             tenant_id = tenant_id.hex
         ticket = await self.__auth.post(
             "/elements_login_as",
```

### Comparing `permit-2.0.0/permit/api/environments.py` & `permit-2.0.1/permit/api/environments.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/models.py` & `permit-2.0.1/permit/api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/projects.py` & `permit-2.0.1/permit/api/projects.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/resource_action_groups.py` & `permit-2.0.1/permit/api/resource_action_groups.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/resource_actions.py` & `permit-2.0.1/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/resource_attributes.py` & `permit-2.0.1/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/resources.py` & `permit-2.0.1/permit/api/resources.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/role_assignments.py` & `permit-2.0.1/permit/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/roles.py` & `permit-2.0.1/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/sync_api_client.py` & `permit-2.0.1/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/tenants.py` & `permit-2.0.1/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/api/users.py` & `permit-2.0.1/permit/api/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Union
 
 from pydantic import validate_arguments
 
 from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
 from .context import ApiKeyLevel
 from .models import (
     PaginatedResultUserRead,
@@ -148,15 +148,15 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__users.patch(f"/{user_key}", model=UserRead, json=user_data)
 
     @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
     @validate_arguments
-    async def sync(self, user: UserCreate | dict) -> UserRead:
+    async def sync(self, user: Union[UserCreate, dict]) -> UserRead:
         """
         Synchronizes user data by creating or updating a user.
 
         Args:
             user: The data of the user to be synchronized.
 
         Returns:
```

### Comparing `permit-2.0.0/permit/config.py` & `permit-2.0.1/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/enforcement/enforcer.py` & `permit-2.0.1/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/enforcement/interfaces.py` & `permit-2.0.1/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/exceptions.py` & `permit-2.0.1/permit/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     Wraps an error HTTP Response that occured during a Permit REST API request.
     """
 
     def __init__(
         self,
         message: str,
         response: aiohttp.ClientResponse,
-        response_json: dict | None = None,
+        response_json: Optional[dict] = None,
     ):
         super().__init__(message)
         self._response = response
         self._response_json = response_json
 
     @property
     def response(self) -> aiohttp.ClientResponse:
@@ -51,15 +51,15 @@
 
         Returns:
             The HTTP response object.
         """
         return self._response
 
     @property
-    def details(self) -> dict | None:
+    def details(self) -> Optional[dict]:
         """
         Get the HTTP response JSON body. Contains details about the error.
 
         Returns:
             The HTTP response json. If no content will return None.
         """
         return self._response_json
```

### Comparing `permit-2.0.0/permit/permit.py` & `permit-2.0.1/permit/permit.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/sync.py` & `permit-2.0.1/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/utils/context.py` & `permit-2.0.1/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit/utils/sync.py` & `permit-2.0.1/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/permit.egg-info/SOURCES.txt` & `permit-2.0.1/permit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/setup.py` & `permit-2.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,20 @@
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
 setup(
     name="permit",
-    version="2.0.0",
+    version="2.0.1",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
     classifiers=[
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

### Comparing `permit-2.0.0/tests/conftest.py` & `permit-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/tests/test_abac_e2e.py` & `permit-2.0.1/tests/test_abac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/tests/test_rbac_e2e.py` & `permit-2.0.1/tests/test_rbac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.0/tests/test_rbac_e2e_sync.py` & `permit-2.0.1/tests/test_rbac_e2e_sync.py`

 * *Files identical despite different names*

