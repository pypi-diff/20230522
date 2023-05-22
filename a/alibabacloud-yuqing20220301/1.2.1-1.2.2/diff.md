# Comparing `tmp/alibabacloud_yuqing20220301-1.2.1.tar.gz` & `tmp/alibabacloud_yuqing20220301-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_yuqing20220301-1.2.1.tar", last modified: Mon Sep 19 11:42:13 2022, max compression
+gzip compressed data, was "dist/alibabacloud_yuqing20220301-1.2.2.tar", last modified: Mon May 22 02:31:18 2023, max compression
```

## Comparing `alibabacloud_yuqing20220301-1.2.1.tar` & `alibabacloud_yuqing20220301-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      735 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1031 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28844 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301/client.py
--rw-r--r--   0 root         (0) root         (0)    73300 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2625 2022-09-19 11:42:13.000000 alibabacloud_yuqing20220301-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29628 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/client.py
+-rw-r--r--   0 root         (0) root         (0)    81156 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/setup.py
```

### Comparing `alibabacloud_yuqing20220301-1.2.1/LICENSE` & `alibabacloud_yuqing20220301-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_yuqing20220301-1.2.1/PKG-INFO` & `alibabacloud_yuqing20220301-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_yuqing20220301
-Version: 1.2.1
+Version: 1.2.2
 Summary: Alibaba Cloud Yuqing (20220301) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_yuqing20220301-1.2.1/README-CN.md` & `alibabacloud_yuqing20220301-1.2.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_yuqing20220301-1.2.1/README.md` & `alibabacloud_yuqing20220301-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301/client.py` & `alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,30 +37,14 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
-    def close_product(
-        self,
-        request: yuqing_20220301_models.CloseProductRequest,
-    ) -> yuqing_20220301_models.CloseProductResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.close_product_with_options(request, headers, runtime)
-
-    async def close_product_async(
-        self,
-        request: yuqing_20220301_models.CloseProductRequest,
-    ) -> yuqing_20220301_models.CloseProductResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.close_product_with_options_async(request, headers, runtime)
-
     def close_product_with_options(
         self,
         request: yuqing_20220301_models.CloseProductRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.CloseProductResponse:
         UtilClient.validate_model(request)
@@ -121,40 +105,40 @@
             body_type='json'
         )
         return TeaCore.from_map(
             yuqing_20220301_models.CloseProductResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def console_api_proxy(
+    def close_product(
         self,
-        request: yuqing_20220301_models.ConsoleApiProxyRequest,
-    ) -> yuqing_20220301_models.ConsoleApiProxyResponse:
+        request: yuqing_20220301_models.CloseProductRequest,
+    ) -> yuqing_20220301_models.CloseProductResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.console_api_proxy_with_options(request, headers, runtime)
+        return self.close_product_with_options(request, headers, runtime)
 
-    async def console_api_proxy_async(
+    async def close_product_async(
         self,
-        request: yuqing_20220301_models.ConsoleApiProxyRequest,
-    ) -> yuqing_20220301_models.ConsoleApiProxyResponse:
+        request: yuqing_20220301_models.CloseProductRequest,
+    ) -> yuqing_20220301_models.CloseProductResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.console_api_proxy_with_options_async(request, headers, runtime)
+        return await self.close_product_with_options_async(request, headers, runtime)
 
     def console_api_proxy_with_options(
         self,
         request: yuqing_20220301_models.ConsoleApiProxyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.ConsoleApiProxyResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ConsoleApiProxy',
             version='2022-03-01',
             protocol='HTTPS',
             pathname=f'/openapi/aliyun/consoleApiProxy.json',
             method='POST',
@@ -173,15 +157,15 @@
         request: yuqing_20220301_models.ConsoleApiProxyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.ConsoleApiProxyResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ConsoleApiProxy',
             version='2022-03-01',
             protocol='HTTPS',
             pathname=f'/openapi/aliyun/consoleApiProxy.json',
             method='POST',
@@ -191,36 +175,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             yuqing_20220301_models.ConsoleApiProxyResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def console_proxy(
+    def console_api_proxy(
         self,
-        request: yuqing_20220301_models.ConsoleProxyRequest,
-    ) -> yuqing_20220301_models.ConsoleProxyResponse:
+        request: yuqing_20220301_models.ConsoleApiProxyRequest,
+    ) -> yuqing_20220301_models.ConsoleApiProxyResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.console_proxy_with_options(request, headers, runtime)
+        return self.console_api_proxy_with_options(request, headers, runtime)
 
-    async def console_proxy_async(
+    async def console_api_proxy_async(
         self,
-        request: yuqing_20220301_models.ConsoleProxyRequest,
-    ) -> yuqing_20220301_models.ConsoleProxyResponse:
+        request: yuqing_20220301_models.ConsoleApiProxyRequest,
+    ) -> yuqing_20220301_models.ConsoleApiProxyResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.console_proxy_with_options_async(request, headers, runtime)
+        return await self.console_api_proxy_with_options_async(request, headers, runtime)
 
     def console_proxy_with_options(
         self,
         request: yuqing_20220301_models.ConsoleProxyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.ConsoleProxyResponse:
+        """
+        @deprecated
+        
+        @param request: ConsoleProxyRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConsoleProxyResponse
+        Deprecated
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.request_id):
             query['requestId'] = request.request_id
         body = {}
         if not UtilClient.is_unset(request.app_code):
             body['appCode'] = request.app_code
@@ -253,14 +246,23 @@
 
     async def console_proxy_with_options_async(
         self,
         request: yuqing_20220301_models.ConsoleProxyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.ConsoleProxyResponse:
+        """
+        @deprecated
+        
+        @param request: ConsoleProxyRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConsoleProxyResponse
+        Deprecated
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.request_id):
             query['requestId'] = request.request_id
         body = {}
         if not UtilClient.is_unset(request.app_code):
             body['appCode'] = request.app_code
@@ -287,29 +289,43 @@
             body_type='json'
         )
         return TeaCore.from_map(
             yuqing_20220301_models.ConsoleProxyResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_analysis_task_result(
+    def console_proxy(
         self,
-        request: yuqing_20220301_models.GetAnalysisTaskResultRequest,
-    ) -> yuqing_20220301_models.GetAnalysisTaskResultResponse:
+        request: yuqing_20220301_models.ConsoleProxyRequest,
+    ) -> yuqing_20220301_models.ConsoleProxyResponse:
+        """
+        @deprecated
+        
+        @param request: ConsoleProxyRequest
+        @return: ConsoleProxyResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_analysis_task_result_with_options(request, headers, runtime)
+        return self.console_proxy_with_options(request, headers, runtime)
 
-    async def get_analysis_task_result_async(
+    async def console_proxy_async(
         self,
-        request: yuqing_20220301_models.GetAnalysisTaskResultRequest,
-    ) -> yuqing_20220301_models.GetAnalysisTaskResultResponse:
+        request: yuqing_20220301_models.ConsoleProxyRequest,
+    ) -> yuqing_20220301_models.ConsoleProxyResponse:
+        """
+        @deprecated
+        
+        @param request: ConsoleProxyRequest
+        @return: ConsoleProxyResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_analysis_task_result_with_options_async(request, headers, runtime)
+        return await self.console_proxy_with_options_async(request, headers, runtime)
 
     def get_analysis_task_result_with_options(
         self,
         request: yuqing_20220301_models.GetAnalysisTaskResultRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.GetAnalysisTaskResultResponse:
@@ -371,29 +387,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             yuqing_20220301_models.GetAnalysisTaskResultResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def open_product(
+    def get_analysis_task_result(
         self,
-        request: yuqing_20220301_models.OpenProductRequest,
-    ) -> yuqing_20220301_models.OpenProductResponse:
+        request: yuqing_20220301_models.GetAnalysisTaskResultRequest,
+    ) -> yuqing_20220301_models.GetAnalysisTaskResultResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.open_product_with_options(request, headers, runtime)
+        return self.get_analysis_task_result_with_options(request, headers, runtime)
 
-    async def open_product_async(
+    async def get_analysis_task_result_async(
         self,
-        request: yuqing_20220301_models.OpenProductRequest,
-    ) -> yuqing_20220301_models.OpenProductResponse:
+        request: yuqing_20220301_models.GetAnalysisTaskResultRequest,
+    ) -> yuqing_20220301_models.GetAnalysisTaskResultResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.open_product_with_options_async(request, headers, runtime)
+        return await self.get_analysis_task_result_with_options_async(request, headers, runtime)
 
     def open_product_with_options(
         self,
         request: yuqing_20220301_models.OpenProductRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.OpenProductResponse:
@@ -459,29 +475,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             yuqing_20220301_models.OpenProductResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def query_product_instance_list(
+    def open_product(
         self,
-        request: yuqing_20220301_models.QueryProductInstanceListRequest,
-    ) -> yuqing_20220301_models.QueryProductInstanceListResponse:
+        request: yuqing_20220301_models.OpenProductRequest,
+    ) -> yuqing_20220301_models.OpenProductResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_product_instance_list_with_options(request, headers, runtime)
+        return self.open_product_with_options(request, headers, runtime)
 
-    async def query_product_instance_list_async(
+    async def open_product_async(
         self,
-        request: yuqing_20220301_models.QueryProductInstanceListRequest,
-    ) -> yuqing_20220301_models.QueryProductInstanceListResponse:
+        request: yuqing_20220301_models.OpenProductRequest,
+    ) -> yuqing_20220301_models.OpenProductResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_product_instance_list_with_options_async(request, headers, runtime)
+        return await self.open_product_with_options_async(request, headers, runtime)
 
     def query_product_instance_list_with_options(
         self,
         request: yuqing_20220301_models.QueryProductInstanceListRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.QueryProductInstanceListResponse:
@@ -551,29 +567,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             yuqing_20220301_models.QueryProductInstanceListResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def query_yuqing_message(
+    def query_product_instance_list(
         self,
-        request: yuqing_20220301_models.QueryYuqingMessageRequest,
-    ) -> yuqing_20220301_models.QueryYuqingMessageResponse:
+        request: yuqing_20220301_models.QueryProductInstanceListRequest,
+    ) -> yuqing_20220301_models.QueryProductInstanceListResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_yuqing_message_with_options(request, headers, runtime)
+        return self.query_product_instance_list_with_options(request, headers, runtime)
 
-    async def query_yuqing_message_async(
+    async def query_product_instance_list_async(
         self,
-        request: yuqing_20220301_models.QueryYuqingMessageRequest,
-    ) -> yuqing_20220301_models.QueryYuqingMessageResponse:
+        request: yuqing_20220301_models.QueryProductInstanceListRequest,
+    ) -> yuqing_20220301_models.QueryProductInstanceListResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_yuqing_message_with_options_async(request, headers, runtime)
+        return await self.query_product_instance_list_with_options_async(request, headers, runtime)
 
     def query_yuqing_message_with_options(
         self,
         request: yuqing_20220301_models.QueryYuqingMessageRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.QueryYuqingMessageResponse:
@@ -639,29 +655,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             yuqing_20220301_models.QueryYuqingMessageResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def submit_analysis_task(
+    def query_yuqing_message(
         self,
-        request: yuqing_20220301_models.SubmitAnalysisTaskRequest,
-    ) -> yuqing_20220301_models.SubmitAnalysisTaskResponse:
+        request: yuqing_20220301_models.QueryYuqingMessageRequest,
+    ) -> yuqing_20220301_models.QueryYuqingMessageResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.submit_analysis_task_with_options(request, headers, runtime)
+        return self.query_yuqing_message_with_options(request, headers, runtime)
 
-    async def submit_analysis_task_async(
+    async def query_yuqing_message_async(
         self,
-        request: yuqing_20220301_models.SubmitAnalysisTaskRequest,
-    ) -> yuqing_20220301_models.SubmitAnalysisTaskResponse:
+        request: yuqing_20220301_models.QueryYuqingMessageRequest,
+    ) -> yuqing_20220301_models.QueryYuqingMessageResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.submit_analysis_task_with_options_async(request, headers, runtime)
+        return await self.query_yuqing_message_with_options_async(request, headers, runtime)
 
     def submit_analysis_task_with_options(
         self,
         request: yuqing_20220301_models.SubmitAnalysisTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> yuqing_20220301_models.SubmitAnalysisTaskResponse:
@@ -730,7 +746,23 @@
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             yuqing_20220301_models.SubmitAnalysisTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
+
+    def submit_analysis_task(
+        self,
+        request: yuqing_20220301_models.SubmitAnalysisTaskRequest,
+    ) -> yuqing_20220301_models.SubmitAnalysisTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_analysis_task_with_options(request, headers, runtime)
+
+    async def submit_analysis_task_async(
+        self,
+        request: yuqing_20220301_models.SubmitAnalysisTaskRequest,
+    ) -> yuqing_20220301_models.SubmitAnalysisTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_analysis_task_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301/models.py` & `alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -554,14 +554,167 @@
         if m.get('updateTimeEnd') is not None:
             self.update_time_end = m.get('updateTimeEnd')
         if m.get('updateTimeStart') is not None:
             self.update_time_start = m.get('updateTimeStart')
         return self
 
 
+class YuqingFinanceEvent(TeaModel):
+    def __init__(
+        self,
+        comprehensive_risk: float = None,
+        entity_area: str = None,
+        entity_crn: str = None,
+        entity_emotion_score: float = None,
+        entity_id: int = None,
+        entity_name: str = None,
+        entity_relevance_score: float = None,
+        entity_show_name: str = None,
+        entity_summary: str = None,
+        entity_type: str = None,
+        event_id: str = None,
+        event_level_3code: int = None,
+        event_level_3name: str = None,
+        event_tags: str = None,
+        event_time: int = None,
+        security_abbreviation: str = None,
+        security_category_codes: List[str] = None,
+        security_codes: List[str] = None,
+        security_markets_codes: List[str] = None,
+        spam_score: float = None,
+        user_subscribe_entity_tags: List[str] = None,
+        user_subscribe_event_tags: List[int] = None,
+    ):
+        self.comprehensive_risk = comprehensive_risk
+        self.entity_area = entity_area
+        self.entity_crn = entity_crn
+        self.entity_emotion_score = entity_emotion_score
+        self.entity_id = entity_id
+        self.entity_name = entity_name
+        self.entity_relevance_score = entity_relevance_score
+        self.entity_show_name = entity_show_name
+        self.entity_summary = entity_summary
+        self.entity_type = entity_type
+        self.event_id = event_id
+        self.event_level_3code = event_level_3code
+        self.event_level_3name = event_level_3name
+        self.event_tags = event_tags
+        self.event_time = event_time
+        self.security_abbreviation = security_abbreviation
+        self.security_category_codes = security_category_codes
+        self.security_codes = security_codes
+        self.security_markets_codes = security_markets_codes
+        self.spam_score = spam_score
+        self.user_subscribe_entity_tags = user_subscribe_entity_tags
+        self.user_subscribe_event_tags = user_subscribe_event_tags
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comprehensive_risk is not None:
+            result['comprehensiveRisk'] = self.comprehensive_risk
+        if self.entity_area is not None:
+            result['entityArea'] = self.entity_area
+        if self.entity_crn is not None:
+            result['entityCrn'] = self.entity_crn
+        if self.entity_emotion_score is not None:
+            result['entityEmotionScore'] = self.entity_emotion_score
+        if self.entity_id is not None:
+            result['entityId'] = self.entity_id
+        if self.entity_name is not None:
+            result['entityName'] = self.entity_name
+        if self.entity_relevance_score is not None:
+            result['entityRelevanceScore'] = self.entity_relevance_score
+        if self.entity_show_name is not None:
+            result['entityShowName'] = self.entity_show_name
+        if self.entity_summary is not None:
+            result['entitySummary'] = self.entity_summary
+        if self.entity_type is not None:
+            result['entityType'] = self.entity_type
+        if self.event_id is not None:
+            result['eventId'] = self.event_id
+        if self.event_level_3code is not None:
+            result['eventLevel3Code'] = self.event_level_3code
+        if self.event_level_3name is not None:
+            result['eventLevel3Name'] = self.event_level_3name
+        if self.event_tags is not None:
+            result['eventTags'] = self.event_tags
+        if self.event_time is not None:
+            result['eventTime'] = self.event_time
+        if self.security_abbreviation is not None:
+            result['securityAbbreviation'] = self.security_abbreviation
+        if self.security_category_codes is not None:
+            result['securityCategoryCodes'] = self.security_category_codes
+        if self.security_codes is not None:
+            result['securityCodes'] = self.security_codes
+        if self.security_markets_codes is not None:
+            result['securityMarketsCodes'] = self.security_markets_codes
+        if self.spam_score is not None:
+            result['spamScore'] = self.spam_score
+        if self.user_subscribe_entity_tags is not None:
+            result['userSubscribeEntityTags'] = self.user_subscribe_entity_tags
+        if self.user_subscribe_event_tags is not None:
+            result['userSubscribeEventTags'] = self.user_subscribe_event_tags
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('comprehensiveRisk') is not None:
+            self.comprehensive_risk = m.get('comprehensiveRisk')
+        if m.get('entityArea') is not None:
+            self.entity_area = m.get('entityArea')
+        if m.get('entityCrn') is not None:
+            self.entity_crn = m.get('entityCrn')
+        if m.get('entityEmotionScore') is not None:
+            self.entity_emotion_score = m.get('entityEmotionScore')
+        if m.get('entityId') is not None:
+            self.entity_id = m.get('entityId')
+        if m.get('entityName') is not None:
+            self.entity_name = m.get('entityName')
+        if m.get('entityRelevanceScore') is not None:
+            self.entity_relevance_score = m.get('entityRelevanceScore')
+        if m.get('entityShowName') is not None:
+            self.entity_show_name = m.get('entityShowName')
+        if m.get('entitySummary') is not None:
+            self.entity_summary = m.get('entitySummary')
+        if m.get('entityType') is not None:
+            self.entity_type = m.get('entityType')
+        if m.get('eventId') is not None:
+            self.event_id = m.get('eventId')
+        if m.get('eventLevel3Code') is not None:
+            self.event_level_3code = m.get('eventLevel3Code')
+        if m.get('eventLevel3Name') is not None:
+            self.event_level_3name = m.get('eventLevel3Name')
+        if m.get('eventTags') is not None:
+            self.event_tags = m.get('eventTags')
+        if m.get('eventTime') is not None:
+            self.event_time = m.get('eventTime')
+        if m.get('securityAbbreviation') is not None:
+            self.security_abbreviation = m.get('securityAbbreviation')
+        if m.get('securityCategoryCodes') is not None:
+            self.security_category_codes = m.get('securityCategoryCodes')
+        if m.get('securityCodes') is not None:
+            self.security_codes = m.get('securityCodes')
+        if m.get('securityMarketsCodes') is not None:
+            self.security_markets_codes = m.get('securityMarketsCodes')
+        if m.get('spamScore') is not None:
+            self.spam_score = m.get('spamScore')
+        if m.get('userSubscribeEntityTags') is not None:
+            self.user_subscribe_entity_tags = m.get('userSubscribeEntityTags')
+        if m.get('userSubscribeEventTags') is not None:
+            self.user_subscribe_event_tags = m.get('userSubscribeEventTags')
+        return self
+
+
 class YuqingMessage(TeaModel):
     def __init__(
         self,
         app_name: str = None,
         app_score: int = None,
         app_store_name: str = None,
         at_author_names: List[str] = None,
@@ -603,27 +756,29 @@
         doc_self_content_sign: str = None,
         doc_title: str = None,
         doc_url: str = None,
         emotion_score: float = None,
         emotion_type: int = None,
         ext_info: Dict[str, str] = None,
         fin_event_count: int = None,
+        finance_event_list: YuqingFinanceEvent = None,
         highlight_keywords: List[str] = None,
         image_count: int = None,
         influence_score: float = None,
         media_hosts: List[str] = None,
         media_influence_level: int = None,
         media_name: str = None,
         media_propagation_level: int = None,
         media_type: str = None,
         message_type: str = None,
         parent_doc_id: str = None,
         propagation_score: float = None,
         publish_time: int = None,
         relevance_score: float = None,
+        report_material_tags: List[str] = None,
         repost_list: List[str] = None,
         similar_number: int = None,
         topics: List[str] = None,
         video_count: int = None,
         weibo_comment_id: str = None,
         weibo_mid: str = None,
     ):
@@ -669,36 +824,39 @@
         self.doc_self_content_sign = doc_self_content_sign
         self.doc_title = doc_title
         self.doc_url = doc_url
         self.emotion_score = emotion_score
         self.emotion_type = emotion_type
         self.ext_info = ext_info
         self.fin_event_count = fin_event_count
+        self.finance_event_list = finance_event_list
         self.highlight_keywords = highlight_keywords
         self.image_count = image_count
         self.influence_score = influence_score
         self.media_hosts = media_hosts
         self.media_influence_level = media_influence_level
         self.media_name = media_name
         self.media_propagation_level = media_propagation_level
         self.media_type = media_type
         self.message_type = message_type
         self.parent_doc_id = parent_doc_id
         self.propagation_score = propagation_score
         self.publish_time = publish_time
         self.relevance_score = relevance_score
+        self.report_material_tags = report_material_tags
         self.repost_list = repost_list
         self.similar_number = similar_number
         self.topics = topics
         self.video_count = video_count
         self.weibo_comment_id = weibo_comment_id
         self.weibo_mid = weibo_mid
 
     def validate(self):
-        pass
+        if self.finance_event_list:
+            self.finance_event_list.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -790,14 +948,16 @@
             result['emotionScore'] = self.emotion_score
         if self.emotion_type is not None:
             result['emotionType'] = self.emotion_type
         if self.ext_info is not None:
             result['extInfo'] = self.ext_info
         if self.fin_event_count is not None:
             result['finEventCount'] = self.fin_event_count
+        if self.finance_event_list is not None:
+            result['financeEventList'] = self.finance_event_list.to_map()
         if self.highlight_keywords is not None:
             result['highlightKeywords'] = self.highlight_keywords
         if self.image_count is not None:
             result['imageCount'] = self.image_count
         if self.influence_score is not None:
             result['influenceScore'] = self.influence_score
         if self.media_hosts is not None:
@@ -816,14 +976,16 @@
             result['parentDocId'] = self.parent_doc_id
         if self.propagation_score is not None:
             result['propagationScore'] = self.propagation_score
         if self.publish_time is not None:
             result['publishTime'] = self.publish_time
         if self.relevance_score is not None:
             result['relevanceScore'] = self.relevance_score
+        if self.report_material_tags is not None:
+            result['reportMaterialTags'] = self.report_material_tags
         if self.repost_list is not None:
             result['repostList'] = self.repost_list
         if self.similar_number is not None:
             result['similarNumber'] = self.similar_number
         if self.topics is not None:
             result['topics'] = self.topics
         if self.video_count is not None:
@@ -924,14 +1086,17 @@
             self.emotion_score = m.get('emotionScore')
         if m.get('emotionType') is not None:
             self.emotion_type = m.get('emotionType')
         if m.get('extInfo') is not None:
             self.ext_info = m.get('extInfo')
         if m.get('finEventCount') is not None:
             self.fin_event_count = m.get('finEventCount')
+        if m.get('financeEventList') is not None:
+            temp_model = YuqingFinanceEvent()
+            self.finance_event_list = temp_model.from_map(m['financeEventList'])
         if m.get('highlightKeywords') is not None:
             self.highlight_keywords = m.get('highlightKeywords')
         if m.get('imageCount') is not None:
             self.image_count = m.get('imageCount')
         if m.get('influenceScore') is not None:
             self.influence_score = m.get('influenceScore')
         if m.get('mediaHosts') is not None:
@@ -950,14 +1115,16 @@
             self.parent_doc_id = m.get('parentDocId')
         if m.get('propagationScore') is not None:
             self.propagation_score = m.get('propagationScore')
         if m.get('publishTime') is not None:
             self.publish_time = m.get('publishTime')
         if m.get('relevanceScore') is not None:
             self.relevance_score = m.get('relevanceScore')
+        if m.get('reportMaterialTags') is not None:
+            self.report_material_tags = m.get('reportMaterialTags')
         if m.get('repostList') is not None:
             self.repost_list = m.get('repostList')
         if m.get('similarNumber') is not None:
             self.similar_number = m.get('similarNumber')
         if m.get('topics') is not None:
             self.topics = m.get('topics')
         if m.get('videoCount') is not None:
@@ -1735,14 +1902,15 @@
 class QueryYuqingMessageResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         total_count: int = None,
         yuqing_messages: List[YuqingMessage] = None,
     ):
+        # Id of the request
         self.request_id = request_id
         self.total_count = total_count
         self.yuqing_messages = yuqing_messages
 
     def validate(self):
         if self.yuqing_messages:
             for k in self.yuqing_messages:
```

### Comparing `alibabacloud_yuqing20220301-1.2.1/alibabacloud_yuqing20220301.egg-info/PKG-INFO` & `alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-yuqing20220301
-Version: 1.2.1
+Version: 1.2.2
 Summary: Alibaba Cloud Yuqing (20220301) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_yuqing20220301-1.2.1/setup.py` & `alibabacloud_yuqing20220301-1.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_yuqing20220301.
 
-Created on 19/09/2022
+Created on 22/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_yuqing20220301"
 NAME = "alibabacloud_yuqing20220301" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Yuqing (20220301) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

