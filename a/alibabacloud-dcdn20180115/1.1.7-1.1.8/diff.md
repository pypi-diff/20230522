# Comparing `tmp/alibabacloud_dcdn20180115-1.1.7.tar.gz` & `tmp/alibabacloud_dcdn20180115-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dcdn20180115-1.1.7.tar", last modified: Fri May 19 01:38:08 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dcdn20180115-1.1.8.tar", last modified: Mon May 22 10:55:18 2023, max compression
```

## Comparing `alibabacloud_dcdn20180115-1.1.7.tar` & `alibabacloud_dcdn20180115-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/
--rw-r--r--   0 root         (0) root         (0)     1997 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115/__init__.py
--rw-r--r--   0 root         (0) root         (0)   903676 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115/client.py
--rw-r--r--   0 root         (0) root         (0)  1214603 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-19 01:38:08.000000 alibabacloud_dcdn20180115-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2615 2023-05-19 01:38:07.000000 alibabacloud_dcdn20180115-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   869608 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115/client.py
+-rw-r--r--   0 root         (0) root         (0)  1256089 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 10:55:18.000000 alibabacloud_dcdn20180115-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-05-22 10:55:17.000000 alibabacloud_dcdn20180115-1.1.8/setup.py
```

### Comparing `alibabacloud_dcdn20180115-1.1.7/ChangeLog.md` & `alibabacloud_dcdn20180115-1.1.8/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-19 Version: 1.1.7
+- Add DescribeDcdnDomainMd5Info.
+
 2023-04-25 Version: 1.1.6
 - Add CheckDcdnDomainExist.
 
 2023-03-24 Version: 1.1.5
 - Add GetDcdnKv.
 
 2023-03-04 Version: 1.1.4
```

### Comparing `alibabacloud_dcdn20180115-1.1.7/LICENSE` & `alibabacloud_dcdn20180115-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-1.1.7/PKG-INFO` & `alibabacloud_dcdn20180115-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dcdn20180115
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115-1.1.7/README-CN.md` & `alibabacloud_dcdn20180115-1.1.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-1.1.7/README.md` & `alibabacloud_dcdn20180115-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115/client.py` & `alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.AddDcdnIpaDomainResponse:
         """
         >
         *   Make sure that the IPA service is activated before you add a domain name to accelerate.
         *   Make sure that the Internet content provider (ICP) filling is complete for the domain name to accelerate.
         *   If the content on the origin server is not stored on Alibaba Cloud, the content must be reviewed. The review is complete by the end of the next business day after you submit the request.
-        *   You can call this operation up to 10 times per second per account.
+        *   You can call this operation up to 10 times per second per user.
         
         @param request: AddDcdnIpaDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AddDcdnIpaDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -308,15 +308,15 @@
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.AddDcdnIpaDomainResponse:
         """
         >
         *   Make sure that the IPA service is activated before you add a domain name to accelerate.
         *   Make sure that the Internet content provider (ICP) filling is complete for the domain name to accelerate.
         *   If the content on the origin server is not stored on Alibaba Cloud, the content must be reviewed. The review is complete by the end of the next business day after you submit the request.
-        *   You can call this operation up to 10 times per second per account.
+        *   You can call this operation up to 10 times per second per user.
         
         @param request: AddDcdnIpaDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AddDcdnIpaDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -364,15 +364,15 @@
         request: dcdn_20180115_models.AddDcdnIpaDomainRequest,
     ) -> dcdn_20180115_models.AddDcdnIpaDomainResponse:
         """
         >
         *   Make sure that the IPA service is activated before you add a domain name to accelerate.
         *   Make sure that the Internet content provider (ICP) filling is complete for the domain name to accelerate.
         *   If the content on the origin server is not stored on Alibaba Cloud, the content must be reviewed. The review is complete by the end of the next business day after you submit the request.
-        *   You can call this operation up to 10 times per second per account.
+        *   You can call this operation up to 10 times per second per user.
         
         @param request: AddDcdnIpaDomainRequest
         @return: AddDcdnIpaDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.add_dcdn_ipa_domain_with_options(request, runtime)
 
@@ -381,35 +381,29 @@
         request: dcdn_20180115_models.AddDcdnIpaDomainRequest,
     ) -> dcdn_20180115_models.AddDcdnIpaDomainResponse:
         """
         >
         *   Make sure that the IPA service is activated before you add a domain name to accelerate.
         *   Make sure that the Internet content provider (ICP) filling is complete for the domain name to accelerate.
         *   If the content on the origin server is not stored on Alibaba Cloud, the content must be reviewed. The review is complete by the end of the next business day after you submit the request.
-        *   You can call this operation up to 10 times per second per account.
+        *   You can call this operation up to 10 times per second per user.
         
         @param request: AddDcdnIpaDomainRequest
         @return: AddDcdnIpaDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.add_dcdn_ipa_domain_with_options_async(request, runtime)
 
     def batch_add_dcdn_domain_with_options(
         self,
         request: dcdn_20180115_models.BatchAddDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchAddDcdnDomainResponse:
         """
-        *Prerequisites**:
-        *   The [DCDN service is activated](~~64926~~).
-        *   Internet Content Provider (ICP) filing is complete for the accelerated domain names.
-        >
-        *   If the content of the origin server is not stored on Alibaba Cloud, the content must be reviewed. After you submit the request, the review is complete by the end of the following business day.
-        *   The maximum number of domain names configured at a time is 50.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The URL that is used to check whether the origin server can be accessed.
         
         @param request: BatchAddDcdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchAddDcdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -452,21 +446,15 @@
 
     async def batch_add_dcdn_domain_with_options_async(
         self,
         request: dcdn_20180115_models.BatchAddDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchAddDcdnDomainResponse:
         """
-        *Prerequisites**:
-        *   The [DCDN service is activated](~~64926~~).
-        *   Internet Content Provider (ICP) filing is complete for the accelerated domain names.
-        >
-        *   If the content of the origin server is not stored on Alibaba Cloud, the content must be reviewed. After you submit the request, the review is complete by the end of the following business day.
-        *   The maximum number of domain names configured at a time is 50.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The URL that is used to check whether the origin server can be accessed.
         
         @param request: BatchAddDcdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchAddDcdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -508,54 +496,42 @@
         )
 
     def batch_add_dcdn_domain(
         self,
         request: dcdn_20180115_models.BatchAddDcdnDomainRequest,
     ) -> dcdn_20180115_models.BatchAddDcdnDomainResponse:
         """
-        *Prerequisites**:
-        *   The [DCDN service is activated](~~64926~~).
-        *   Internet Content Provider (ICP) filing is complete for the accelerated domain names.
-        >
-        *   If the content of the origin server is not stored on Alibaba Cloud, the content must be reviewed. After you submit the request, the review is complete by the end of the following business day.
-        *   The maximum number of domain names configured at a time is 50.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The URL that is used to check whether the origin server can be accessed.
         
         @param request: BatchAddDcdnDomainRequest
         @return: BatchAddDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_add_dcdn_domain_with_options(request, runtime)
 
     async def batch_add_dcdn_domain_async(
         self,
         request: dcdn_20180115_models.BatchAddDcdnDomainRequest,
     ) -> dcdn_20180115_models.BatchAddDcdnDomainResponse:
         """
-        *Prerequisites**:
-        *   The [DCDN service is activated](~~64926~~).
-        *   Internet Content Provider (ICP) filing is complete for the accelerated domain names.
-        >
-        *   If the content of the origin server is not stored on Alibaba Cloud, the content must be reviewed. After you submit the request, the review is complete by the end of the following business day.
-        *   The maximum number of domain names configured at a time is 50.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The URL that is used to check whether the origin server can be accessed.
         
         @param request: BatchAddDcdnDomainRequest
         @return: BatchAddDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_add_dcdn_domain_with_options_async(request, runtime)
 
     def batch_create_dcdn_waf_rules_with_options(
         self,
         request: dcdn_20180115_models.BatchCreateDcdnWafRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchCreateDcdnWafRulesResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
         @param request: BatchCreateDcdnWafRulesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchCreateDcdnWafRulesResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -584,15 +560,15 @@
 
     async def batch_create_dcdn_waf_rules_with_options_async(
         self,
         request: dcdn_20180115_models.BatchCreateDcdnWafRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchCreateDcdnWafRulesResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
         @param request: BatchCreateDcdnWafRulesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchCreateDcdnWafRulesResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -620,28 +596,28 @@
         )
 
     def batch_create_dcdn_waf_rules(
         self,
         request: dcdn_20180115_models.BatchCreateDcdnWafRulesRequest,
     ) -> dcdn_20180115_models.BatchCreateDcdnWafRulesResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
         @param request: BatchCreateDcdnWafRulesRequest
         @return: BatchCreateDcdnWafRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_create_dcdn_waf_rules_with_options(request, runtime)
 
     async def batch_create_dcdn_waf_rules_async(
         self,
         request: dcdn_20180115_models.BatchCreateDcdnWafRulesRequest,
     ) -> dcdn_20180115_models.BatchCreateDcdnWafRulesResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
         @param request: BatchCreateDcdnWafRulesRequest
         @return: BatchCreateDcdnWafRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_create_dcdn_waf_rules_with_options_async(request, runtime)
 
@@ -771,16 +747,17 @@
 
     def batch_delete_dcdn_waf_rules_with_options(
         self,
         request: dcdn_20180115_models.BatchDeleteDcdnWafRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchDeleteDcdnWafRulesResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        # Usage notes
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: BatchDeleteDcdnWafRulesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchDeleteDcdnWafRulesResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -807,16 +784,17 @@
 
     async def batch_delete_dcdn_waf_rules_with_options_async(
         self,
         request: dcdn_20180115_models.BatchDeleteDcdnWafRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchDeleteDcdnWafRulesResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        # Usage notes
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: BatchDeleteDcdnWafRulesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchDeleteDcdnWafRulesResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -842,30 +820,32 @@
         )
 
     def batch_delete_dcdn_waf_rules(
         self,
         request: dcdn_20180115_models.BatchDeleteDcdnWafRulesRequest,
     ) -> dcdn_20180115_models.BatchDeleteDcdnWafRulesResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        # Usage notes
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: BatchDeleteDcdnWafRulesRequest
         @return: BatchDeleteDcdnWafRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_delete_dcdn_waf_rules_with_options(request, runtime)
 
     async def batch_delete_dcdn_waf_rules_async(
         self,
         request: dcdn_20180115_models.BatchDeleteDcdnWafRulesRequest,
     ) -> dcdn_20180115_models.BatchDeleteDcdnWafRulesResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        # Usage notes
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: BatchDeleteDcdnWafRulesRequest
         @return: BatchDeleteDcdnWafRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_delete_dcdn_waf_rules_with_options_async(request, runtime)
 
@@ -971,15 +951,15 @@
 
     def batch_set_dcdn_domain_certificate_with_options(
         self,
         request: dcdn_20180115_models.BatchSetDcdnDomainCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchSetDcdnDomainCertificateResponse:
         """
-        >  You can call this operation up to 10 times per second per account.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: BatchSetDcdnDomainCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetDcdnDomainCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1022,15 +1002,15 @@
 
     async def batch_set_dcdn_domain_certificate_with_options_async(
         self,
         request: dcdn_20180115_models.BatchSetDcdnDomainCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchSetDcdnDomainCertificateResponse:
         """
-        >  You can call this operation up to 10 times per second per account.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: BatchSetDcdnDomainCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetDcdnDomainCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1072,28 +1052,28 @@
         )
 
     def batch_set_dcdn_domain_certificate(
         self,
         request: dcdn_20180115_models.BatchSetDcdnDomainCertificateRequest,
     ) -> dcdn_20180115_models.BatchSetDcdnDomainCertificateResponse:
         """
-        >  You can call this operation up to 10 times per second per account.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: BatchSetDcdnDomainCertificateRequest
         @return: BatchSetDcdnDomainCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_set_dcdn_domain_certificate_with_options(request, runtime)
 
     async def batch_set_dcdn_domain_certificate_async(
         self,
         request: dcdn_20180115_models.BatchSetDcdnDomainCertificateRequest,
     ) -> dcdn_20180115_models.BatchSetDcdnDomainCertificateResponse:
         """
-        >  You can call this operation up to 10 times per second per account.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: BatchSetDcdnDomainCertificateRequest
         @return: BatchSetDcdnDomainCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_set_dcdn_domain_certificate_with_options_async(request, runtime)
 
@@ -1211,15 +1191,15 @@
 
     def batch_set_dcdn_ipa_domain_configs_with_options(
         self,
         request: dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: BatchSetDcdnIpaDomainConfigsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetDcdnIpaDomainConfigsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1254,15 +1234,15 @@
 
     async def batch_set_dcdn_ipa_domain_configs_with_options_async(
         self,
         request: dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: BatchSetDcdnIpaDomainConfigsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetDcdnIpaDomainConfigsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1296,43 +1276,44 @@
         )
 
     def batch_set_dcdn_ipa_domain_configs(
         self,
         request: dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsRequest,
     ) -> dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: BatchSetDcdnIpaDomainConfigsRequest
         @return: BatchSetDcdnIpaDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_set_dcdn_ipa_domain_configs_with_options(request, runtime)
 
     async def batch_set_dcdn_ipa_domain_configs_async(
         self,
         request: dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsRequest,
     ) -> dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: BatchSetDcdnIpaDomainConfigsRequest
         @return: BatchSetDcdnIpaDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_set_dcdn_ipa_domain_configs_with_options_async(request, runtime)
 
     def batch_set_dcdn_waf_domain_configs_with_options(
         self,
         request: dcdn_20180115_models.BatchSetDcdnWafDomainConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchSetDcdnWafDomainConfigsResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: BatchSetDcdnWafDomainConfigsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetDcdnWafDomainConfigsResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1363,16 +1344,17 @@
 
     async def batch_set_dcdn_waf_domain_configs_with_options_async(
         self,
         request: dcdn_20180115_models.BatchSetDcdnWafDomainConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchSetDcdnWafDomainConfigsResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: BatchSetDcdnWafDomainConfigsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetDcdnWafDomainConfigsResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1402,30 +1384,32 @@
         )
 
     def batch_set_dcdn_waf_domain_configs(
         self,
         request: dcdn_20180115_models.BatchSetDcdnWafDomainConfigsRequest,
     ) -> dcdn_20180115_models.BatchSetDcdnWafDomainConfigsResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: BatchSetDcdnWafDomainConfigsRequest
         @return: BatchSetDcdnWafDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_set_dcdn_waf_domain_configs_with_options(request, runtime)
 
     async def batch_set_dcdn_waf_domain_configs_async(
         self,
         request: dcdn_20180115_models.BatchSetDcdnWafDomainConfigsRequest,
     ) -> dcdn_20180115_models.BatchSetDcdnWafDomainConfigsResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: BatchSetDcdnWafDomainConfigsRequest
         @return: BatchSetDcdnWafDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_set_dcdn_waf_domain_configs_with_options_async(request, runtime)
 
@@ -1627,15 +1611,15 @@
 
     def create_dcdn_deliver_task_with_options(
         self,
         request: dcdn_20180115_models.CreateDcdnDeliverTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateDcdnDeliverTaskResponse:
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
         @param request: CreateDcdnDeliverTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDcdnDeliverTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1670,15 +1654,15 @@
 
     async def create_dcdn_deliver_task_with_options_async(
         self,
         request: dcdn_20180115_models.CreateDcdnDeliverTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateDcdnDeliverTaskResponse:
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
         @param request: CreateDcdnDeliverTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDcdnDeliverTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1712,42 +1696,42 @@
         )
 
     def create_dcdn_deliver_task(
         self,
         request: dcdn_20180115_models.CreateDcdnDeliverTaskRequest,
     ) -> dcdn_20180115_models.CreateDcdnDeliverTaskResponse:
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
         @param request: CreateDcdnDeliverTaskRequest
         @return: CreateDcdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dcdn_deliver_task_with_options(request, runtime)
 
     async def create_dcdn_deliver_task_async(
         self,
         request: dcdn_20180115_models.CreateDcdnDeliverTaskRequest,
     ) -> dcdn_20180115_models.CreateDcdnDeliverTaskResponse:
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
         @param request: CreateDcdnDeliverTaskRequest
         @return: CreateDcdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_dcdn_deliver_task_with_options_async(request, runtime)
 
     def create_dcdn_slsreal_time_log_delivery_with_options(
         self,
         request: dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: CreateDcdnSLSRealTimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDcdnSLSRealTimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1788,15 +1772,15 @@
 
     async def create_dcdn_slsreal_time_log_delivery_with_options_async(
         self,
         request: dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: CreateDcdnSLSRealTimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDcdnSLSRealTimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1836,28 +1820,28 @@
         )
 
     def create_dcdn_slsreal_time_log_delivery(
         self,
         request: dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryRequest,
     ) -> dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: CreateDcdnSLSRealTimeLogDeliveryRequest
         @return: CreateDcdnSLSRealTimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dcdn_slsreal_time_log_delivery_with_options(request, runtime)
 
     async def create_dcdn_slsreal_time_log_delivery_async(
         self,
         request: dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryRequest,
     ) -> dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: CreateDcdnSLSRealTimeLogDeliveryRequest
         @return: CreateDcdnSLSRealTimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_dcdn_slsreal_time_log_delivery_with_options_async(request, runtime)
 
@@ -2103,18 +2087,15 @@
 
     def create_routine_with_options(
         self,
         tmp_req: dcdn_20180115_models.CreateRoutineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateRoutineResponse:
         """
-        >
-        *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
-        *   This operation creates a routine that contains only production and staging environments.
-        *   You can call this operation up to 100 times per second.
+        The message returned, such as ""Status": "OK"".
         
         @param tmp_req: CreateRoutineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateRoutineResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dcdn_20180115_models.CreateRoutineShrinkRequest()
@@ -2149,18 +2130,15 @@
 
     async def create_routine_with_options_async(
         self,
         tmp_req: dcdn_20180115_models.CreateRoutineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateRoutineResponse:
         """
-        >
-        *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
-        *   This operation creates a routine that contains only production and staging environments.
-        *   You can call this operation up to 100 times per second.
+        The message returned, such as ""Status": "OK"".
         
         @param tmp_req: CreateRoutineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateRoutineResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dcdn_20180115_models.CreateRoutineShrinkRequest()
@@ -2194,48 +2172,43 @@
         )
 
     def create_routine(
         self,
         request: dcdn_20180115_models.CreateRoutineRequest,
     ) -> dcdn_20180115_models.CreateRoutineResponse:
         """
-        >
-        *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
-        *   This operation creates a routine that contains only production and staging environments.
-        *   You can call this operation up to 100 times per second.
+        The message returned, such as ""Status": "OK"".
         
         @param request: CreateRoutineRequest
         @return: CreateRoutineResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_routine_with_options(request, runtime)
 
     async def create_routine_async(
         self,
         request: dcdn_20180115_models.CreateRoutineRequest,
     ) -> dcdn_20180115_models.CreateRoutineResponse:
         """
-        >
-        *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
-        *   This operation creates a routine that contains only production and staging environments.
-        *   You can call this operation up to 100 times per second.
+        The message returned, such as ""Status": "OK"".
         
         @param request: CreateRoutineRequest
         @return: CreateRoutineResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_routine_with_options_async(request, runtime)
 
     def create_slr_and_sls_project_with_options(
         self,
         request: dcdn_20180115_models.CreateSlrAndSlsProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateSlrAndSlsProjectResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        *\
+        ****\
         
         @param request: CreateSlrAndSlsProjectRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSlrAndSlsProjectResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -2264,15 +2237,16 @@
 
     async def create_slr_and_sls_project_with_options_async(
         self,
         request: dcdn_20180115_models.CreateSlrAndSlsProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateSlrAndSlsProjectResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        *\
+        ****\
         
         @param request: CreateSlrAndSlsProjectRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSlrAndSlsProjectResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -2300,28 +2274,30 @@
         )
 
     def create_slr_and_sls_project(
         self,
         request: dcdn_20180115_models.CreateSlrAndSlsProjectRequest,
     ) -> dcdn_20180115_models.CreateSlrAndSlsProjectResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        *\
+        ****\
         
         @param request: CreateSlrAndSlsProjectRequest
         @return: CreateSlrAndSlsProjectResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_slr_and_sls_project_with_options(request, runtime)
 
     async def create_slr_and_sls_project_async(
         self,
         request: dcdn_20180115_models.CreateSlrAndSlsProjectRequest,
     ) -> dcdn_20180115_models.CreateSlrAndSlsProjectResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        *\
+        ****\
         
         @param request: CreateSlrAndSlsProjectRequest
         @return: CreateSlrAndSlsProjectResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_slr_and_sls_project_with_options_async(request, runtime)
 
@@ -2427,18 +2403,19 @@
 
     def delete_dcdn_domain_with_options(
         self,
         request: dcdn_20180115_models.DeleteDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnDomainResponse:
         """
-        >
-        *   Before you delete your domain name, you must request the Domain Name System (DNS) provider to restore the A record of the domain name. Otherwise, the domain name may become inaccessible after you delete it.
-        *   If you call the **DeleteDcdnDomain** operation, all the information about the accelerated domain name is deleted. If you want to disable an accelerated domain name, call the [StopDcdnDomain](~~130622~~) operation.
-        *   The maximum number of times that each user can call this operation per second is 10.
+        *\
+        ****\
+        *\
+        *   ****[](~~130622~~)
+        *\
         
         @param request: DeleteDcdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDcdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2471,18 +2448,19 @@
 
     async def delete_dcdn_domain_with_options_async(
         self,
         request: dcdn_20180115_models.DeleteDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnDomainResponse:
         """
-        >
-        *   Before you delete your domain name, you must request the Domain Name System (DNS) provider to restore the A record of the domain name. Otherwise, the domain name may become inaccessible after you delete it.
-        *   If you call the **DeleteDcdnDomain** operation, all the information about the accelerated domain name is deleted. If you want to disable an accelerated domain name, call the [StopDcdnDomain](~~130622~~) operation.
-        *   The maximum number of times that each user can call this operation per second is 10.
+        *\
+        ****\
+        *\
+        *   ****[](~~130622~~)
+        *\
         
         @param request: DeleteDcdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDcdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2514,34 +2492,36 @@
         )
 
     def delete_dcdn_domain(
         self,
         request: dcdn_20180115_models.DeleteDcdnDomainRequest,
     ) -> dcdn_20180115_models.DeleteDcdnDomainResponse:
         """
-        >
-        *   Before you delete your domain name, you must request the Domain Name System (DNS) provider to restore the A record of the domain name. Otherwise, the domain name may become inaccessible after you delete it.
-        *   If you call the **DeleteDcdnDomain** operation, all the information about the accelerated domain name is deleted. If you want to disable an accelerated domain name, call the [StopDcdnDomain](~~130622~~) operation.
-        *   The maximum number of times that each user can call this operation per second is 10.
+        *\
+        ****\
+        *\
+        *   ****[](~~130622~~)
+        *\
         
         @param request: DeleteDcdnDomainRequest
         @return: DeleteDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_domain_with_options(request, runtime)
 
     async def delete_dcdn_domain_async(
         self,
         request: dcdn_20180115_models.DeleteDcdnDomainRequest,
     ) -> dcdn_20180115_models.DeleteDcdnDomainResponse:
         """
-        >
-        *   Before you delete your domain name, you must request the Domain Name System (DNS) provider to restore the A record of the domain name. Otherwise, the domain name may become inaccessible after you delete it.
-        *   If you call the **DeleteDcdnDomain** operation, all the information about the accelerated domain name is deleted. If you want to disable an accelerated domain name, call the [StopDcdnDomain](~~130622~~) operation.
-        *   The maximum number of times that each user can call this operation per second is 10.
+        *\
+        ****\
+        *\
+        *   ****[](~~130622~~)
+        *\
         
         @param request: DeleteDcdnDomainRequest
         @return: DeleteDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dcdn_domain_with_options_async(request, runtime)
 
@@ -2667,15 +2647,15 @@
 
     def delete_dcdn_ipa_specific_config_with_options(
         self,
         request: dcdn_20180115_models.DeleteDcdnIpaSpecificConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnIpaSpecificConfigResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: DeleteDcdnIpaSpecificConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDcdnIpaSpecificConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2708,15 +2688,15 @@
 
     async def delete_dcdn_ipa_specific_config_with_options_async(
         self,
         request: dcdn_20180115_models.DeleteDcdnIpaSpecificConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnIpaSpecificConfigResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: DeleteDcdnIpaSpecificConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDcdnIpaSpecificConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2748,47 +2728,40 @@
         )
 
     def delete_dcdn_ipa_specific_config(
         self,
         request: dcdn_20180115_models.DeleteDcdnIpaSpecificConfigRequest,
     ) -> dcdn_20180115_models.DeleteDcdnIpaSpecificConfigResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: DeleteDcdnIpaSpecificConfigRequest
         @return: DeleteDcdnIpaSpecificConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_ipa_specific_config_with_options(request, runtime)
 
     async def delete_dcdn_ipa_specific_config_async(
         self,
         request: dcdn_20180115_models.DeleteDcdnIpaSpecificConfigRequest,
     ) -> dcdn_20180115_models.DeleteDcdnIpaSpecificConfigResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: DeleteDcdnIpaSpecificConfigRequest
         @return: DeleteDcdnIpaSpecificConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dcdn_ipa_specific_config_with_options_async(request, runtime)
 
     def delete_dcdn_kv_with_options(
         self,
         request: dcdn_20180115_models.DeleteDcdnKvRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnKvResponse:
-        """
-        >  You can call this operation up to 50 times per second per account.
-        
-        @param request: DeleteDcdnKvRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteDcdnKvResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key):
             query['Key'] = request.key
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         req = open_api_models.OpenApiRequest(
@@ -2811,21 +2784,14 @@
         )
 
     async def delete_dcdn_kv_with_options_async(
         self,
         request: dcdn_20180115_models.DeleteDcdnKvRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnKvResponse:
-        """
-        >  You can call this operation up to 50 times per second per account.
-        
-        @param request: DeleteDcdnKvRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteDcdnKvResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key):
             query['Key'] = request.key
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         req = open_api_models.OpenApiRequest(
@@ -2847,33 +2813,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dcdn_kv(
         self,
         request: dcdn_20180115_models.DeleteDcdnKvRequest,
     ) -> dcdn_20180115_models.DeleteDcdnKvResponse:
-        """
-        >  You can call this operation up to 50 times per second per account.
-        
-        @param request: DeleteDcdnKvRequest
-        @return: DeleteDcdnKvResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_kv_with_options(request, runtime)
 
     async def delete_dcdn_kv_async(
         self,
         request: dcdn_20180115_models.DeleteDcdnKvRequest,
     ) -> dcdn_20180115_models.DeleteDcdnKvResponse:
-        """
-        >  You can call this operation up to 50 times per second per account.
-        
-        @param request: DeleteDcdnKvRequest
-        @return: DeleteDcdnKvResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dcdn_kv_with_options_async(request, runtime)
 
     def delete_dcdn_real_time_log_project_with_options(
         self,
         request: dcdn_20180115_models.DeleteDcdnRealTimeLogProjectRequest,
         runtime: util_models.RuntimeOptions,
@@ -3186,15 +3140,15 @@
         return await self.delete_dcdn_specific_staging_config_with_options_async(request, runtime)
 
     def delete_dcdn_sub_task_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnSubTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to 3 times per second per account.
         
         @param request: DeleteDcdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDcdnSubTaskResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -3214,15 +3168,15 @@
         )
 
     async def delete_dcdn_sub_task_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnSubTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to 3 times per second per account.
         
         @param request: DeleteDcdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDcdnSubTaskResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -3239,38 +3193,39 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DeleteDcdnSubTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dcdn_sub_task(self) -> dcdn_20180115_models.DeleteDcdnSubTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to 3 times per second per account.
         
         @return: DeleteDcdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_sub_task_with_options(runtime)
 
     async def delete_dcdn_sub_task_async(self) -> dcdn_20180115_models.DeleteDcdnSubTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to 3 times per second per account.
         
         @return: DeleteDcdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dcdn_sub_task_with_options_async(runtime)
 
     def delete_dcdn_waf_policy_with_options(
         self,
         request: dcdn_20180115_models.DeleteDcdnWafPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnWafPolicyResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: DeleteDcdnWafPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDcdnWafPolicyResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -3297,16 +3252,17 @@
 
     async def delete_dcdn_waf_policy_with_options_async(
         self,
         request: dcdn_20180115_models.DeleteDcdnWafPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteDcdnWafPolicyResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: DeleteDcdnWafPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDcdnWafPolicyResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -3332,44 +3288,46 @@
         )
 
     def delete_dcdn_waf_policy(
         self,
         request: dcdn_20180115_models.DeleteDcdnWafPolicyRequest,
     ) -> dcdn_20180115_models.DeleteDcdnWafPolicyResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: DeleteDcdnWafPolicyRequest
         @return: DeleteDcdnWafPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_waf_policy_with_options(request, runtime)
 
     async def delete_dcdn_waf_policy_async(
         self,
         request: dcdn_20180115_models.DeleteDcdnWafPolicyRequest,
     ) -> dcdn_20180115_models.DeleteDcdnWafPolicyResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: DeleteDcdnWafPolicyRequest
         @return: DeleteDcdnWafPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dcdn_waf_policy_with_options_async(request, runtime)
 
     def delete_routine_with_options(
         self,
         request: dcdn_20180115_models.DeleteRoutineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteRoutineResponse:
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DeleteRoutineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteRoutineResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -3396,15 +3354,15 @@
 
     async def delete_routine_with_options_async(
         self,
         request: dcdn_20180115_models.DeleteRoutineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteRoutineResponse:
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DeleteRoutineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteRoutineResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -3430,28 +3388,28 @@
         )
 
     def delete_routine(
         self,
         request: dcdn_20180115_models.DeleteRoutineRequest,
     ) -> dcdn_20180115_models.DeleteRoutineResponse:
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DeleteRoutineRequest
         @return: DeleteRoutineResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_routine_with_options(request, runtime)
 
     async def delete_routine_async(
         self,
         request: dcdn_20180115_models.DeleteRoutineRequest,
     ) -> dcdn_20180115_models.DeleteRoutineResponse:
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DeleteRoutineRequest
         @return: DeleteRoutineResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_routine_with_options_async(request, runtime)
 
@@ -3557,17 +3515,15 @@
 
     def delete_routine_conf_envs_with_options(
         self,
         tmp_req: dcdn_20180115_models.DeleteRoutineConfEnvsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteRoutineConfEnvsResponse:
         """
-        >
-        *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
-        *   You can call this operation up to 100 times per second per account.
+        The ID of the region.
         
         @param tmp_req: DeleteRoutineConfEnvsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteRoutineConfEnvsResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dcdn_20180115_models.DeleteRoutineConfEnvsShrinkRequest()
@@ -3600,17 +3556,15 @@
 
     async def delete_routine_conf_envs_with_options_async(
         self,
         tmp_req: dcdn_20180115_models.DeleteRoutineConfEnvsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DeleteRoutineConfEnvsResponse:
         """
-        >
-        *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
-        *   You can call this operation up to 100 times per second per account.
+        The ID of the region.
         
         @param tmp_req: DeleteRoutineConfEnvsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteRoutineConfEnvsResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dcdn_20180115_models.DeleteRoutineConfEnvsShrinkRequest()
@@ -3642,46 +3596,42 @@
         )
 
     def delete_routine_conf_envs(
         self,
         request: dcdn_20180115_models.DeleteRoutineConfEnvsRequest,
     ) -> dcdn_20180115_models.DeleteRoutineConfEnvsResponse:
         """
-        >
-        *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
-        *   You can call this operation up to 100 times per second per account.
+        The ID of the region.
         
         @param request: DeleteRoutineConfEnvsRequest
         @return: DeleteRoutineConfEnvsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_routine_conf_envs_with_options(request, runtime)
 
     async def delete_routine_conf_envs_async(
         self,
         request: dcdn_20180115_models.DeleteRoutineConfEnvsRequest,
     ) -> dcdn_20180115_models.DeleteRoutineConfEnvsResponse:
         """
-        >
-        *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
-        *   You can call this operation up to 100 times per second per account.
+        The ID of the region.
         
         @param request: DeleteRoutineConfEnvsRequest
         @return: DeleteRoutineConfEnvsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_routine_conf_envs_with_options_async(request, runtime)
 
     def describe_dcdn_acl_fields_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnAclFieldsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnAclFieldsResponse:
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to three times per second per account.
         
         @param request: DescribeDcdnAclFieldsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnAclFieldsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3708,15 +3658,15 @@
 
     async def describe_dcdn_acl_fields_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnAclFieldsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnAclFieldsResponse:
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to three times per second per account.
         
         @param request: DescribeDcdnAclFieldsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnAclFieldsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3742,28 +3692,28 @@
         )
 
     def describe_dcdn_acl_fields(
         self,
         request: dcdn_20180115_models.DescribeDcdnAclFieldsRequest,
     ) -> dcdn_20180115_models.DescribeDcdnAclFieldsResponse:
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to three times per second per account.
         
         @param request: DescribeDcdnAclFieldsRequest
         @return: DescribeDcdnAclFieldsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_acl_fields_with_options(request, runtime)
 
     async def describe_dcdn_acl_fields_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnAclFieldsRequest,
     ) -> dcdn_20180115_models.DescribeDcdnAclFieldsResponse:
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to three times per second per account.
         
         @param request: DescribeDcdnAclFieldsRequest
         @return: DescribeDcdnAclFieldsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_acl_fields_with_options_async(request, runtime)
 
@@ -4105,15 +4055,15 @@
 
     def describe_dcdn_certificate_detail_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnCertificateDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnCertificateDetailResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnCertificateDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnCertificateDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4144,15 +4094,15 @@
 
     async def describe_dcdn_certificate_detail_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnCertificateDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnCertificateDetailResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnCertificateDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnCertificateDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4182,28 +4132,28 @@
         )
 
     def describe_dcdn_certificate_detail(
         self,
         request: dcdn_20180115_models.DescribeDcdnCertificateDetailRequest,
     ) -> dcdn_20180115_models.DescribeDcdnCertificateDetailResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnCertificateDetailRequest
         @return: DescribeDcdnCertificateDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_certificate_detail_with_options(request, runtime)
 
     async def describe_dcdn_certificate_detail_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnCertificateDetailRequest,
     ) -> dcdn_20180115_models.DescribeDcdnCertificateDetailResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnCertificateDetailRequest
         @return: DescribeDcdnCertificateDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_certificate_detail_with_options_async(request, runtime)
 
@@ -4661,22 +4611,18 @@
 
     def describe_dcdn_domain_bps_data_by_layer_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second.
-        - If you do not set the **StartTime** or **EndTime** parameters, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data is available | Data delay |
-        | ---------------- | ---------------------------- | ---------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        #
+        *\
+        *   ****************\
+        ****| -------------- | -------------- | ------\
         
         @param request: DescribeDcdnDomainBpsDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainBpsDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4715,22 +4661,18 @@
 
     async def describe_dcdn_domain_bps_data_by_layer_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second.
-        - If you do not set the **StartTime** or **EndTime** parameters, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data is available | Data delay |
-        | ---------------- | ---------------------------- | ---------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        #
+        *\
+        *   ****************\
+        ****| -------------- | -------------- | ------\
         
         @param request: DescribeDcdnDomainBpsDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainBpsDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4768,42 +4710,34 @@
         )
 
     def describe_dcdn_domain_bps_data_by_layer(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second.
-        - If you do not set the **StartTime** or **EndTime** parameters, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data is available | Data delay |
-        | ---------------- | ---------------------------- | ---------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        #
+        *\
+        *   ****************\
+        ****| -------------- | -------------- | ------\
         
         @param request: DescribeDcdnDomainBpsDataByLayerRequest
         @return: DescribeDcdnDomainBpsDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_bps_data_by_layer_with_options(request, runtime)
 
     async def describe_dcdn_domain_bps_data_by_layer_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second.
-        - If you do not set the **StartTime** or **EndTime** parameters, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data is available | Data delay |
-        | ---------------- | ---------------------------- | ---------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        #
+        *\
+        *   ****************\
+        ****| -------------- | -------------- | ------\
         
         @param request: DescribeDcdnDomainBpsDataByLayerRequest
         @return: DescribeDcdnDomainBpsDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_bps_data_by_layer_with_options_async(request, runtime)
 
@@ -4912,15 +4846,15 @@
         request: dcdn_20180115_models.DescribeDcdnDomainCcActivityLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainCcActivityLogResponse:
         """
         >
         *   If you do not configure the StartTime or EndTime parameter, data collected over the last 24 hours is queried. If you configure both the StartTime and EndTime parameters, data collected within the specified time range is queried.
         *   You can query data collected over the last 30 days.
-        *   You can call this operation up to 50 times per second.
+        *   You can call this operation up to 50 times per second per user.
         
         @param request: DescribeDcdnDomainCcActivityLogRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainCcActivityLogResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4964,15 +4898,15 @@
         request: dcdn_20180115_models.DescribeDcdnDomainCcActivityLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainCcActivityLogResponse:
         """
         >
         *   If you do not configure the StartTime or EndTime parameter, data collected over the last 24 hours is queried. If you configure both the StartTime and EndTime parameters, data collected within the specified time range is queried.
         *   You can query data collected over the last 30 days.
-        *   You can call this operation up to 50 times per second.
+        *   You can call this operation up to 50 times per second per user.
         
         @param request: DescribeDcdnDomainCcActivityLogRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainCcActivityLogResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5015,15 +4949,15 @@
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainCcActivityLogRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainCcActivityLogResponse:
         """
         >
         *   If you do not configure the StartTime or EndTime parameter, data collected over the last 24 hours is queried. If you configure both the StartTime and EndTime parameters, data collected within the specified time range is queried.
         *   You can query data collected over the last 30 days.
-        *   You can call this operation up to 50 times per second.
+        *   You can call this operation up to 50 times per second per user.
         
         @param request: DescribeDcdnDomainCcActivityLogRequest
         @return: DescribeDcdnDomainCcActivityLogResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_cc_activity_log_with_options(request, runtime)
 
@@ -5031,29 +4965,29 @@
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainCcActivityLogRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainCcActivityLogResponse:
         """
         >
         *   If you do not configure the StartTime or EndTime parameter, data collected over the last 24 hours is queried. If you configure both the StartTime and EndTime parameters, data collected within the specified time range is queried.
         *   You can query data collected over the last 30 days.
-        *   You can call this operation up to 50 times per second.
+        *   You can call this operation up to 50 times per second per user.
         
         @param request: DescribeDcdnDomainCcActivityLogRequest
         @return: DescribeDcdnDomainCcActivityLogResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_cc_activity_log_with_options_async(request, runtime)
 
     def describe_dcdn_domain_certificate_info_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainCertificateInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainCertificateInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDcdnDomainCertificateInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainCertificateInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5080,15 +5014,15 @@
 
     async def describe_dcdn_domain_certificate_info_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainCertificateInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainCertificateInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDcdnDomainCertificateInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainCertificateInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5114,28 +5048,28 @@
         )
 
     def describe_dcdn_domain_certificate_info(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainCertificateInfoRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainCertificateInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDcdnDomainCertificateInfoRequest
         @return: DescribeDcdnDomainCertificateInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_certificate_info_with_options(request, runtime)
 
     async def describe_dcdn_domain_certificate_info_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainCertificateInfoRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainCertificateInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDcdnDomainCertificateInfoRequest
         @return: DescribeDcdnDomainCertificateInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_certificate_info_with_options_async(request, runtime)
 
@@ -5461,22 +5395,18 @@
 
     def describe_dcdn_domain_hit_rate_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainHitRateDataResponse:
         """
-        - You can call this operation up to 100 times per second per account.
-        - If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        #
+        *   You can call this operation up to 100 times per second per account.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table. |Time granularity |Maximum time range per query |Historical data available |Data delay | -------------- | -------------- | ------ |5 minutes |3 days |93 days |15 minutes |1 hour |31 days |186 days |4 hours |1 day |366 days |366 days |04:00 on the next day
         
         @param request: DescribeDcdnDomainHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5509,22 +5439,18 @@
 
     async def describe_dcdn_domain_hit_rate_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainHitRateDataResponse:
         """
-        - You can call this operation up to 100 times per second per account.
-        - If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        #
+        *   You can call this operation up to 100 times per second per account.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table. |Time granularity |Maximum time range per query |Historical data available |Data delay | -------------- | -------------- | ------ |5 minutes |3 days |93 days |15 minutes |1 hour |31 days |186 days |4 hours |1 day |366 days |366 days |04:00 on the next day
         
         @param request: DescribeDcdnDomainHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5556,64 +5482,48 @@
         )
 
     def describe_dcdn_domain_hit_rate_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainHitRateDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainHitRateDataResponse:
         """
-        - You can call this operation up to 100 times per second per account.
-        - If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        #
+        *   You can call this operation up to 100 times per second per account.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table. |Time granularity |Maximum time range per query |Historical data available |Data delay | -------------- | -------------- | ------ |5 minutes |3 days |93 days |15 minutes |1 hour |31 days |186 days |4 hours |1 day |366 days |366 days |04:00 on the next day
         
         @param request: DescribeDcdnDomainHitRateDataRequest
         @return: DescribeDcdnDomainHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_hit_rate_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_hit_rate_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainHitRateDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainHitRateDataResponse:
         """
-        - You can call this operation up to 100 times per second per account.
-        - If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        #
+        *   You can call this operation up to 100 times per second per account.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table. |Time granularity |Maximum time range per query |Historical data available |Data delay | -------------- | -------------- | ------ |5 minutes |3 days |93 days |15 minutes |1 hour |31 days |186 days |4 hours |1 day |366 days |366 days |04:00 on the next day
         
         @param request: DescribeDcdnDomainHitRateDataRequest
         @return: DescribeDcdnDomainHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_hit_rate_data_with_options_async(request, runtime)
 
     def describe_dcdn_domain_http_code_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataResponse:
         """
-        If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        * You can call this operation up to 100 times per second per account.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        Queries the total number and proportions of HTTP status codes returned from one or more accelerated domain names. Data is collected every 5 minutes. You can query data in the last 90 days.
         
         @param request: DescribeDcdnDomainHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5650,23 +5560,15 @@
 
     async def describe_dcdn_domain_http_code_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataResponse:
         """
-        If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        * You can call this operation up to 100 times per second per account.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        Queries the total number and proportions of HTTP status codes returned from one or more accelerated domain names. Data is collected every 5 minutes. You can query data in the last 90 days.
         
         @param request: DescribeDcdnDomainHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5702,44 +5604,28 @@
         )
 
     def describe_dcdn_domain_http_code_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataResponse:
         """
-        If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        * You can call this operation up to 100 times per second per account.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        Queries the total number and proportions of HTTP status codes returned from one or more accelerated domain names. Data is collected every 5 minutes. You can query data in the last 90 days.
         
         @param request: DescribeDcdnDomainHttpCodeDataRequest
         @return: DescribeDcdnDomainHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_http_code_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_http_code_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataResponse:
         """
-        If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        * You can call this operation up to 100 times per second per account.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        Queries the total number and proportions of HTTP status codes returned from one or more accelerated domain names. Data is collected every 5 minutes. You can query data in the last 90 days.
         
         @param request: DescribeDcdnDomainHttpCodeDataRequest
         @return: DescribeDcdnDomainHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_http_code_data_with_options_async(request, runtime)
 
@@ -5882,15 +5768,15 @@
     def describe_dcdn_domain_ipa_bps_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataResponse:
         """
         >
-        *   Unit: bit/s.
+        *   The bandwidth is measured in bit/s.
         *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
         *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnDomainIpaBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainIpaBpsDataResponse
         """
@@ -5934,15 +5820,15 @@
     async def describe_dcdn_domain_ipa_bps_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataResponse:
         """
         >
-        *   Unit: bit/s.
+        *   The bandwidth is measured in bit/s.
         *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
         *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnDomainIpaBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainIpaBpsDataResponse
         """
@@ -5985,15 +5871,15 @@
 
     def describe_dcdn_domain_ipa_bps_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataResponse:
         """
         >
-        *   Unit: bit/s.
+        *   The bandwidth is measured in bit/s.
         *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
         *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnDomainIpaBpsDataRequest
         @return: DescribeDcdnDomainIpaBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -6001,15 +5887,15 @@
 
     async def describe_dcdn_domain_ipa_bps_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataResponse:
         """
         >
-        *   Unit: bit/s.
+        *   The bandwidth is measured in bit/s.
         *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
         *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnDomainIpaBpsDataRequest
         @return: DescribeDcdnDomainIpaBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -6138,17 +6024,17 @@
     def describe_dcdn_domain_ipa_traffic_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataResponse:
         """
         >
-        *   If you do not set **StartTime** or **EndTime**, data collected within the last 24 hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        *   The monitoring data is measured in bytes.
-        *   The maximum number of times that users can call this operation per second is 100.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        *   Unit: bytes.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnDomainIpaTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainIpaTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6190,17 +6076,17 @@
     async def describe_dcdn_domain_ipa_traffic_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataResponse:
         """
         >
-        *   If you do not set **StartTime** or **EndTime**, data collected within the last 24 hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        *   The monitoring data is measured in bytes.
-        *   The maximum number of times that users can call this operation per second is 100.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        *   Unit: bytes.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnDomainIpaTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainIpaTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6241,55 +6127,47 @@
 
     def describe_dcdn_domain_ipa_traffic_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataResponse:
         """
         >
-        *   If you do not set **StartTime** or **EndTime**, data collected within the last 24 hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        *   The monitoring data is measured in bytes.
-        *   The maximum number of times that users can call this operation per second is 100.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        *   Unit: bytes.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnDomainIpaTrafficDataRequest
         @return: DescribeDcdnDomainIpaTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_ipa_traffic_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_ipa_traffic_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataResponse:
         """
         >
-        *   If you do not set **StartTime** or **EndTime**, data collected within the last 24 hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        *   The monitoring data is measured in bytes.
-        *   The maximum number of times that users can call this operation per second is 100.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        *   Unit: bytes.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnDomainIpaTrafficDataRequest
         @return: DescribeDcdnDomainIpaTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_ipa_traffic_data_with_options_async(request, runtime)
 
     def describe_dcdn_domain_isp_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIspDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIspDataResponse:
         """
-        >
-        *   You can call this operation up to 100 times per second.
-        *   If **StartTime** is set but **EndTime** is not set, the data within the hour that starts from **StartTime** is queried.
-        *   If **EndTime** is set but **StartTime** is not set, the data within the last hour that precedes **EndTime** is queried.
-        *   You can query data of a domain name or all domain names that belong to your account.
-        *   You can view data that is collected over the last seven days. The interval at which data is queried is based on the time range specified by **StartTime** and **EndTime**.
-        *   **If the time range is shorter than or equal to one hour**, data is queried every minute.
-        *   **If the time range is longer than 1 hour but shorter than or equal to three days**, data is queried every five minutes.
-        *   **If the time range is longer than three days but shorter than or equal to seven days**, data is queried every hour.
+        The end of the time range during which data was queried.
         
         @param request: DescribeDcdnDomainIspDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainIspDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6320,23 +6198,15 @@
 
     async def describe_dcdn_domain_isp_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIspDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIspDataResponse:
         """
-        >
-        *   You can call this operation up to 100 times per second.
-        *   If **StartTime** is set but **EndTime** is not set, the data within the hour that starts from **StartTime** is queried.
-        *   If **EndTime** is set but **StartTime** is not set, the data within the last hour that precedes **EndTime** is queried.
-        *   You can query data of a domain name or all domain names that belong to your account.
-        *   You can view data that is collected over the last seven days. The interval at which data is queried is based on the time range specified by **StartTime** and **EndTime**.
-        *   **If the time range is shorter than or equal to one hour**, data is queried every minute.
-        *   **If the time range is longer than 1 hour but shorter than or equal to three days**, data is queried every five minutes.
-        *   **If the time range is longer than three days but shorter than or equal to seven days**, data is queried every hour.
+        The end of the time range during which data was queried.
         
         @param request: DescribeDcdnDomainIspDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainIspDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6366,60 +6236,43 @@
         )
 
     def describe_dcdn_domain_isp_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIspDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIspDataResponse:
         """
-        >
-        *   You can call this operation up to 100 times per second.
-        *   If **StartTime** is set but **EndTime** is not set, the data within the hour that starts from **StartTime** is queried.
-        *   If **EndTime** is set but **StartTime** is not set, the data within the last hour that precedes **EndTime** is queried.
-        *   You can query data of a domain name or all domain names that belong to your account.
-        *   You can view data that is collected over the last seven days. The interval at which data is queried is based on the time range specified by **StartTime** and **EndTime**.
-        *   **If the time range is shorter than or equal to one hour**, data is queried every minute.
-        *   **If the time range is longer than 1 hour but shorter than or equal to three days**, data is queried every five minutes.
-        *   **If the time range is longer than three days but shorter than or equal to seven days**, data is queried every hour.
+        The end of the time range during which data was queried.
         
         @param request: DescribeDcdnDomainIspDataRequest
         @return: DescribeDcdnDomainIspDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_isp_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_isp_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainIspDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainIspDataResponse:
         """
-        >
-        *   You can call this operation up to 100 times per second.
-        *   If **StartTime** is set but **EndTime** is not set, the data within the hour that starts from **StartTime** is queried.
-        *   If **EndTime** is set but **StartTime** is not set, the data within the last hour that precedes **EndTime** is queried.
-        *   You can query data of a domain name or all domain names that belong to your account.
-        *   You can view data that is collected over the last seven days. The interval at which data is queried is based on the time range specified by **StartTime** and **EndTime**.
-        *   **If the time range is shorter than or equal to one hour**, data is queried every minute.
-        *   **If the time range is longer than 1 hour but shorter than or equal to three days**, data is queried every five minutes.
-        *   **If the time range is longer than three days but shorter than or equal to seven days**, data is queried every hour.
+        The end of the time range during which data was queried.
         
         @param request: DescribeDcdnDomainIspDataRequest
         @return: DescribeDcdnDomainIspDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_isp_data_with_options_async(request, runtime)
 
     def describe_dcdn_domain_log_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainLogResponse:
         """
-        >
-        *   If you specify neither the **StartTime** parameter nor the **EndTime** parameter, the data in the last 24 hours is returned. If you specify the **StartTime** and **EndTime** parameters, the data within the specified time range is returned.
-        *   You can call this operation up to 100 times per second per account.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDcdnDomainLogRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainLogResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6454,17 +6307,16 @@
 
     async def describe_dcdn_domain_log_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainLogResponse:
         """
-        >
-        *   If you specify neither the **StartTime** parameter nor the **EndTime** parameter, the data in the last 24 hours is returned. If you specify the **StartTime** and **EndTime** parameters, the data within the specified time range is returned.
-        *   You can call this operation up to 100 times per second per account.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDcdnDomainLogRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainLogResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6498,32 +6350,30 @@
         )
 
     def describe_dcdn_domain_log(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainLogRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainLogResponse:
         """
-        >
-        *   If you specify neither the **StartTime** parameter nor the **EndTime** parameter, the data in the last 24 hours is returned. If you specify the **StartTime** and **EndTime** parameters, the data within the specified time range is returned.
-        *   You can call this operation up to 100 times per second per account.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDcdnDomainLogRequest
         @return: DescribeDcdnDomainLogResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_log_with_options(request, runtime)
 
     async def describe_dcdn_domain_log_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainLogRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainLogResponse:
         """
-        >
-        *   If you specify neither the **StartTime** parameter nor the **EndTime** parameter, the data in the last 24 hours is returned. If you specify the **StartTime** and **EndTime** parameters, the data within the specified time range is returned.
-        *   You can call this operation up to 100 times per second per account.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDcdnDomainLogRequest
         @return: DescribeDcdnDomainLogResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_log_with_options_async(request, runtime)
 
@@ -6532,15 +6382,15 @@
         request: dcdn_20180115_models.DescribeDcdnDomainMultiUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainMultiUsageDataResponse:
         """
         When you call this operation, take note of the following rules:
         *   If you do not set the StartTime or EndTime parameter, data within the last 10 minutes is queried. You can set both the StartTime and EndTime parameters to specify a time range.
         *   You can specify one or more accelerated domain names. Separate domain names with commas (,).
-        *   You can query data up to the last 90 days.
+        *   You can query data within the last 90 days.
         *   The time range cannot exceed 1 hour.
         
         @param request: DescribeDcdnDomainMultiUsageDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainMultiUsageDataResponse
         """
         UtilClient.validate_model(request)
@@ -6575,15 +6425,15 @@
         request: dcdn_20180115_models.DescribeDcdnDomainMultiUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainMultiUsageDataResponse:
         """
         When you call this operation, take note of the following rules:
         *   If you do not set the StartTime or EndTime parameter, data within the last 10 minutes is queried. You can set both the StartTime and EndTime parameters to specify a time range.
         *   You can specify one or more accelerated domain names. Separate domain names with commas (,).
-        *   You can query data up to the last 90 days.
+        *   You can query data within the last 90 days.
         *   The time range cannot exceed 1 hour.
         
         @param request: DescribeDcdnDomainMultiUsageDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainMultiUsageDataResponse
         """
         UtilClient.validate_model(request)
@@ -6617,15 +6467,15 @@
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainMultiUsageDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainMultiUsageDataResponse:
         """
         When you call this operation, take note of the following rules:
         *   If you do not set the StartTime or EndTime parameter, data within the last 10 minutes is queried. You can set both the StartTime and EndTime parameters to specify a time range.
         *   You can specify one or more accelerated domain names. Separate domain names with commas (,).
-        *   You can query data up to the last 90 days.
+        *   You can query data within the last 90 days.
         *   The time range cannot exceed 1 hour.
         
         @param request: DescribeDcdnDomainMultiUsageDataRequest
         @return: DescribeDcdnDomainMultiUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_multi_usage_data_with_options(request, runtime)
@@ -6634,15 +6484,15 @@
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainMultiUsageDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainMultiUsageDataResponse:
         """
         When you call this operation, take note of the following rules:
         *   If you do not set the StartTime or EndTime parameter, data within the last 10 minutes is queried. You can set both the StartTime and EndTime parameters to specify a time range.
         *   You can specify one or more accelerated domain names. Separate domain names with commas (,).
-        *   You can query data up to the last 90 days.
+        *   You can query data within the last 90 days.
         *   The time range cannot exceed 1 hour.
         
         @param request: DescribeDcdnDomainMultiUsageDataRequest
         @return: DescribeDcdnDomainMultiUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_multi_usage_data_with_options_async(request, runtime)
@@ -6925,15 +6775,15 @@
 
     def describe_dcdn_domain_property_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainPropertyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainPropertyResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        The accelerated domain name that you want to query. You can specify only one domain name in each call.
         
         @param request: DescribeDcdnDomainPropertyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainPropertyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6960,15 +6810,15 @@
 
     async def describe_dcdn_domain_property_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainPropertyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainPropertyResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        The accelerated domain name that you want to query. You can specify only one domain name in each call.
         
         @param request: DescribeDcdnDomainPropertyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainPropertyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6994,28 +6844,28 @@
         )
 
     def describe_dcdn_domain_property(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainPropertyRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainPropertyResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        The accelerated domain name that you want to query. You can specify only one domain name in each call.
         
         @param request: DescribeDcdnDomainPropertyRequest
         @return: DescribeDcdnDomainPropertyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_property_with_options(request, runtime)
 
     async def describe_dcdn_domain_property_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainPropertyRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainPropertyResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        The accelerated domain name that you want to query. You can specify only one domain name in each call.
         
         @param request: DescribeDcdnDomainPropertyRequest
         @return: DescribeDcdnDomainPropertyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_property_with_options_async(request, runtime)
 
@@ -7599,23 +7449,16 @@
 
     def describe_dcdn_domain_real_time_detail_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataResponse:
         """
-        > You can call this operation up to 10 times per second per account.
-        **Time granularity of general data returned by the operation**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        Unless otherwise specified, statistics in the preceding table prevail.
+        The name of the ISP. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the ISP name.
+        If you do not specify a value for this parameter, all ISPs are queried.
         
         @param request: DescribeDcdnDomainRealTimeDetailDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainRealTimeDetailDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -7640,23 +7483,16 @@
 
     async def describe_dcdn_domain_real_time_detail_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataResponse:
         """
-        > You can call this operation up to 10 times per second per account.
-        **Time granularity of general data returned by the operation**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        Unless otherwise specified, statistics in the preceding table prevail.
+        The name of the ISP. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the ISP name.
+        If you do not specify a value for this parameter, all ISPs are queried.
         
         @param request: DescribeDcdnDomainRealTimeDetailDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainRealTimeDetailDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -7680,44 +7516,30 @@
         )
 
     def describe_dcdn_domain_real_time_detail_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataResponse:
         """
-        > You can call this operation up to 10 times per second per account.
-        **Time granularity of general data returned by the operation**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        Unless otherwise specified, statistics in the preceding table prevail.
+        The name of the ISP. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the ISP name.
+        If you do not specify a value for this parameter, all ISPs are queried.
         
         @param request: DescribeDcdnDomainRealTimeDetailDataRequest
         @return: DescribeDcdnDomainRealTimeDetailDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_real_time_detail_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_real_time_detail_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataResponse:
         """
-        > You can call this operation up to 10 times per second per account.
-        **Time granularity of general data returned by the operation**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        Unless otherwise specified, statistics in the preceding table prevail.
+        The name of the ISP. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the ISP name.
+        If you do not specify a value for this parameter, all ISPs are queried.
         
         @param request: DescribeDcdnDomainRealTimeDetailDataRequest
         @return: DescribeDcdnDomainRealTimeDetailDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_real_time_detail_data_with_options_async(request, runtime)
 
@@ -7963,23 +7785,19 @@
 
     def describe_dcdn_domain_real_time_req_hit_rate_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataResponse:
         """
-        - You can call this operation up to 10 times per second per account.
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
-        - If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last hour. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        #
+        *   You can call this operation up to 10 times per second per account.
+        *   The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last hour. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. |Time granularity |Maximum time range per query |Historical data available|Data delay| |---------------|--------| |1 minute|1 hour|7 days|5 minutes| |5 minutes|3 days|93 days|15 minutes| |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDcdnDomainRealTimeReqHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainRealTimeReqHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8004,23 +7822,19 @@
 
     async def describe_dcdn_domain_real_time_req_hit_rate_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataResponse:
         """
-        - You can call this operation up to 10 times per second per account.
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
-        - If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last hour. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        #
+        *   You can call this operation up to 10 times per second per account.
+        *   The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last hour. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. |Time granularity |Maximum time range per query |Historical data available|Data delay| |---------------|--------| |1 minute|1 hour|7 days|5 minutes| |5 minutes|3 days|93 days|15 minutes| |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDcdnDomainRealTimeReqHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainRealTimeReqHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8044,44 +7858,36 @@
         )
 
     def describe_dcdn_domain_real_time_req_hit_rate_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataResponse:
         """
-        - You can call this operation up to 10 times per second per account.
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
-        - If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last hour. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        #
+        *   You can call this operation up to 10 times per second per account.
+        *   The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last hour. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. |Time granularity |Maximum time range per query |Historical data available|Data delay| |---------------|--------| |1 minute|1 hour|7 days|5 minutes| |5 minutes|3 days|93 days|15 minutes| |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDcdnDomainRealTimeReqHitRateDataRequest
         @return: DescribeDcdnDomainRealTimeReqHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_real_time_req_hit_rate_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_real_time_req_hit_rate_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataResponse:
         """
-        - You can call this operation up to 10 times per second per account.
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
-        - If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last hour. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        **Time granularity**The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        #
+        *   You can call this operation up to 10 times per second per account.
+        *   The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last hour. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. |Time granularity |Maximum time range per query |Historical data available|Data delay| |---------------|--------| |1 minute|1 hour|7 days|5 minutes| |5 minutes|3 days|93 days|15 minutes| |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDcdnDomainRealTimeReqHitRateDataRequest
         @return: DescribeDcdnDomainRealTimeReqHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_real_time_req_hit_rate_data_with_options_async(request, runtime)
 
@@ -8319,22 +8125,15 @@
 
     def describe_dcdn_domain_real_time_src_traffic_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataResponse:
         """
-        If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The timestamp of the returned data.
         
         @param request: DescribeDcdnDomainRealTimeSrcTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainRealTimeSrcTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8365,22 +8164,15 @@
 
     async def describe_dcdn_domain_real_time_src_traffic_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataResponse:
         """
-        If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The timestamp of the returned data.
         
         @param request: DescribeDcdnDomainRealTimeSrcTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainRealTimeSrcTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8410,62 +8202,44 @@
         )
 
     def describe_dcdn_domain_real_time_src_traffic_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataResponse:
         """
-        If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The timestamp of the returned data.
         
         @param request: DescribeDcdnDomainRealTimeSrcTrafficDataRequest
         @return: DescribeDcdnDomainRealTimeSrcTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_real_time_src_traffic_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_real_time_src_traffic_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataResponse:
         """
-        If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The timestamp of the returned data.
         
         @param request: DescribeDcdnDomainRealTimeSrcTrafficDataRequest
         @return: DescribeDcdnDomainRealTimeSrcTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_real_time_src_traffic_data_with_options_async(request, runtime)
 
     def describe_dcdn_domain_real_time_traffic_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataResponse:
         """
-        You can call this operation up to 50 times per second per account.
-        **Time granularity**The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        #
+        You can call this operation up to 50 times per second per user.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. |Time granularity |Maximum time range per query |Historical data available|Data delay| |---------------|--------| |1 minute|1 hour|7 days|5 minutes| |5 minutes|3 days|93 days|15 minutes| |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDcdnDomainRealTimeTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainRealTimeTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8496,21 +8270,17 @@
 
     async def describe_dcdn_domain_real_time_traffic_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataResponse:
         """
-        You can call this operation up to 50 times per second per account.
-        **Time granularity**The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        #
+        You can call this operation up to 50 times per second per user.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. |Time granularity |Maximum time range per query |Historical data available|Data delay| |---------------|--------| |1 minute|1 hour|7 days|5 minutes| |5 minutes|3 days|93 days|15 minutes| |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDcdnDomainRealTimeTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainRealTimeTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8540,40 +8310,32 @@
         )
 
     def describe_dcdn_domain_real_time_traffic_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataResponse:
         """
-        You can call this operation up to 50 times per second per account.
-        **Time granularity**The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        #
+        You can call this operation up to 50 times per second per user.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. |Time granularity |Maximum time range per query |Historical data available|Data delay| |---------------|--------| |1 minute|1 hour|7 days|5 minutes| |5 minutes|3 days|93 days|15 minutes| |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDcdnDomainRealTimeTrafficDataRequest
         @return: DescribeDcdnDomainRealTimeTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_real_time_traffic_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_real_time_traffic_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataResponse:
         """
-        You can call this operation up to 50 times per second per account.
-        **Time granularity**The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        #
+        You can call this operation up to 50 times per second per user.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. |Time granularity |Maximum time range per query |Historical data available|Data delay| |---------------|--------| |1 minute|1 hour|7 days|5 minutes| |5 minutes|3 days|93 days|15 minutes| |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDcdnDomainRealTimeTrafficDataRequest
         @return: DescribeDcdnDomainRealTimeTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_real_time_traffic_data_with_options_async(request, runtime)
 
@@ -8787,15 +8549,15 @@
 
     def describe_dcdn_domain_top_refer_visit_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTopReferVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTopReferVisitResponse:
         """
-        *Before you call this operation, take note of the following considerations:**\
+        *Before you call this operation, take note of the following rules:**\
         *   If you do not set the StartTime parameter, the data on the previous day is queried.
         *   You can specify only one domain name.
         
         @param request: DescribeDcdnDomainTopReferVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainTopReferVisitResponse
         """
@@ -8828,15 +8590,15 @@
 
     async def describe_dcdn_domain_top_refer_visit_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTopReferVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTopReferVisitResponse:
         """
-        *Before you call this operation, take note of the following considerations:**\
+        *Before you call this operation, take note of the following rules:**\
         *   If you do not set the StartTime parameter, the data on the previous day is queried.
         *   You can specify only one domain name.
         
         @param request: DescribeDcdnDomainTopReferVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainTopReferVisitResponse
         """
@@ -8868,30 +8630,30 @@
         )
 
     def describe_dcdn_domain_top_refer_visit(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTopReferVisitRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTopReferVisitResponse:
         """
-        *Before you call this operation, take note of the following considerations:**\
+        *Before you call this operation, take note of the following rules:**\
         *   If you do not set the StartTime parameter, the data on the previous day is queried.
         *   You can specify only one domain name.
         
         @param request: DescribeDcdnDomainTopReferVisitRequest
         @return: DescribeDcdnDomainTopReferVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_top_refer_visit_with_options(request, runtime)
 
     async def describe_dcdn_domain_top_refer_visit_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTopReferVisitRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTopReferVisitResponse:
         """
-        *Before you call this operation, take note of the following considerations:**\
+        *Before you call this operation, take note of the following rules:**\
         *   If you do not set the StartTime parameter, the data on the previous day is queried.
         *   You can specify only one domain name.
         
         @param request: DescribeDcdnDomainTopReferVisitRequest
         @return: DescribeDcdnDomainTopReferVisitResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -8899,15 +8661,15 @@
 
     def describe_dcdn_domain_top_url_visit_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitResponse:
         """
-        >  You can only query the data within the last seven days.
+        > You can query data in the last seven days.
         
         @param request: DescribeDcdnDomainTopUrlVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainTopUrlVisitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8938,15 +8700,15 @@
 
     async def describe_dcdn_domain_top_url_visit_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitResponse:
         """
-        >  You can only query the data within the last seven days.
+        > You can query data in the last seven days.
         
         @param request: DescribeDcdnDomainTopUrlVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainTopUrlVisitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8976,50 +8738,42 @@
         )
 
     def describe_dcdn_domain_top_url_visit(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitResponse:
         """
-        >  You can only query the data within the last seven days.
+        > You can query data in the last seven days.
         
         @param request: DescribeDcdnDomainTopUrlVisitRequest
         @return: DescribeDcdnDomainTopUrlVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_top_url_visit_with_options(request, runtime)
 
     async def describe_dcdn_domain_top_url_visit_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitResponse:
         """
-        >  You can only query the data within the last seven days.
+        > You can query data in the last seven days.
         
         @param request: DescribeDcdnDomainTopUrlVisitRequest
         @return: DescribeDcdnDomainTopUrlVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_top_url_visit_with_options_async(request, runtime)
 
     def describe_dcdn_domain_traffic_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTrafficDataResponse:
         """
-        If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        * You can call this operation up to 100 times per second per account.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        Queries the monitoring data of network traffic for one or more accelerated domain names. You can query data in the last 90 days.
         
         @param request: DescribeDcdnDomainTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9056,23 +8810,15 @@
 
     async def describe_dcdn_domain_traffic_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTrafficDataResponse:
         """
-        If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        * You can call this operation up to 100 times per second per account.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        Queries the monitoring data of network traffic for one or more accelerated domain names. You can query data in the last 90 days.
         
         @param request: DescribeDcdnDomainTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9108,44 +8854,28 @@
         )
 
     def describe_dcdn_domain_traffic_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTrafficDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTrafficDataResponse:
         """
-        If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        * You can call this operation up to 100 times per second per account.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        Queries the monitoring data of network traffic for one or more accelerated domain names. You can query data in the last 90 days.
         
         @param request: DescribeDcdnDomainTrafficDataRequest
         @return: DescribeDcdnDomainTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_traffic_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_traffic_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainTrafficDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainTrafficDataResponse:
         """
-        If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
-        * You can call this operation up to 100 times per second per account.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        Queries the monitoring data of network traffic for one or more accelerated domain names. You can query data in the last 90 days.
         
         @param request: DescribeDcdnDomainTrafficDataRequest
         @return: DescribeDcdnDomainTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_traffic_data_with_options_async(request, runtime)
 
@@ -9275,17 +9005,17 @@
 
     def describe_dcdn_domain_uv_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainUvDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainUvDataResponse:
         """
-        *Before you call this operation, pay attention to the following considerations:**\
-        *   If you do not specify the StartTime or EndTime parameter, the data collected within the last 24 hours is queried by default. If you specify the StartTime and EndTime parameters, the data collected within the specified time range is queried.
-        *   You can specify only one accelerated domain or all the accelerated domains under your account.
+        ***\
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can specify only one accelerated domain name or all the accelerated domain names that belong to your Alibaba Cloud account.
         
         @param request: DescribeDcdnDomainUvDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainUvDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9316,17 +9046,17 @@
 
     async def describe_dcdn_domain_uv_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainUvDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainUvDataResponse:
         """
-        *Before you call this operation, pay attention to the following considerations:**\
-        *   If you do not specify the StartTime or EndTime parameter, the data collected within the last 24 hours is queried by default. If you specify the StartTime and EndTime parameters, the data collected within the specified time range is queried.
-        *   You can specify only one accelerated domain or all the accelerated domains under your account.
+        ***\
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can specify only one accelerated domain name or all the accelerated domain names that belong to your Alibaba Cloud account.
         
         @param request: DescribeDcdnDomainUvDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainUvDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9356,32 +9086,32 @@
         )
 
     def describe_dcdn_domain_uv_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainUvDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainUvDataResponse:
         """
-        *Before you call this operation, pay attention to the following considerations:**\
-        *   If you do not specify the StartTime or EndTime parameter, the data collected within the last 24 hours is queried by default. If you specify the StartTime and EndTime parameters, the data collected within the specified time range is queried.
-        *   You can specify only one accelerated domain or all the accelerated domains under your account.
+        ***\
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can specify only one accelerated domain name or all the accelerated domain names that belong to your Alibaba Cloud account.
         
         @param request: DescribeDcdnDomainUvDataRequest
         @return: DescribeDcdnDomainUvDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_uv_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_uv_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainUvDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainUvDataResponse:
         """
-        *Before you call this operation, pay attention to the following considerations:**\
-        *   If you do not specify the StartTime or EndTime parameter, the data collected within the last 24 hours is queried by default. If you specify the StartTime and EndTime parameters, the data collected within the specified time range is queried.
-        *   You can specify only one accelerated domain or all the accelerated domains under your account.
+        ***\
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can specify only one accelerated domain name or all the accelerated domain names that belong to your Alibaba Cloud account.
         
         @param request: DescribeDcdnDomainUvDataRequest
         @return: DescribeDcdnDomainUvDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_uv_data_with_options_async(request, runtime)
 
@@ -9515,21 +9245,17 @@
 
     def describe_dcdn_domain_websocket_http_code_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataResponse:
         """
+        #
         You can call this operation up to 100 times per second per account.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        **Time granularity** The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table. |Time granularity |Maximum time range per query |Historical data available |Data delay | -------------- | -------------- | ------ |5 minutes |3 days |93 days |15 minutes |1 hour |31 days |186 days |4 hours |1 day |366 days |366 days |04:00 on the next day
         
         @param request: DescribeDcdnDomainWebsocketHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainWebsocketHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9566,21 +9292,17 @@
 
     async def describe_dcdn_domain_websocket_http_code_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataResponse:
         """
+        #
         You can call this operation up to 100 times per second per account.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        **Time granularity** The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table. |Time granularity |Maximum time range per query |Historical data available |Data delay | -------------- | -------------- | ------ |5 minutes |3 days |93 days |15 minutes |1 hour |31 days |186 days |4 hours |1 day |366 days |366 days |04:00 on the next day
         
         @param request: DescribeDcdnDomainWebsocketHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainWebsocketHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9616,40 +9338,32 @@
         )
 
     def describe_dcdn_domain_websocket_http_code_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataResponse:
         """
+        #
         You can call this operation up to 100 times per second per account.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        **Time granularity** The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table. |Time granularity |Maximum time range per query |Historical data available |Data delay | -------------- | -------------- | ------ |5 minutes |3 days |93 days |15 minutes |1 hour |31 days |186 days |4 hours |1 day |366 days |366 days |04:00 on the next day
         
         @param request: DescribeDcdnDomainWebsocketHttpCodeDataRequest
         @return: DescribeDcdnDomainWebsocketHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_websocket_http_code_data_with_options(request, runtime)
 
     async def describe_dcdn_domain_websocket_http_code_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataResponse:
         """
+        #
         You can call this operation up to 100 times per second per account.
-        **Time granularity**The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        **Time granularity** The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table. |Time granularity |Maximum time range per query |Historical data available |Data delay | -------------- | -------------- | ------ |5 minutes |3 days |93 days |15 minutes |1 hour |31 days |186 days |4 hours |1 day |366 days |366 days |04:00 on the next day
         
         @param request: DescribeDcdnDomainWebsocketHttpCodeDataRequest
         @return: DescribeDcdnDomainWebsocketHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_websocket_http_code_data_with_options_async(request, runtime)
 
@@ -9803,16 +9517,17 @@
 
     def describe_dcdn_er_usage_data_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnErUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnErUsageDataResponse:
         """
-        >   You can call this operation up to 10 times per second per account.
-        *   The minimum time granularity for a query is one hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
+        # Usage notes
+        *   You can call this operation up to 10 times per second per account.
+        *   The minimum time granularity for a query is 1 hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
         
         @param request: DescribeDcdnErUsageDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnErUsageDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9847,16 +9562,17 @@
 
     async def describe_dcdn_er_usage_data_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnErUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnErUsageDataResponse:
         """
-        >   You can call this operation up to 10 times per second per account.
-        *   The minimum time granularity for a query is one hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
+        # Usage notes
+        *   You can call this operation up to 10 times per second per account.
+        *   The minimum time granularity for a query is 1 hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
         
         @param request: DescribeDcdnErUsageDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnErUsageDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9890,30 +9606,32 @@
         )
 
     def describe_dcdn_er_usage_data(
         self,
         request: dcdn_20180115_models.DescribeDcdnErUsageDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnErUsageDataResponse:
         """
-        >   You can call this operation up to 10 times per second per account.
-        *   The minimum time granularity for a query is one hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
+        # Usage notes
+        *   You can call this operation up to 10 times per second per account.
+        *   The minimum time granularity for a query is 1 hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
         
         @param request: DescribeDcdnErUsageDataRequest
         @return: DescribeDcdnErUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_er_usage_data_with_options(request, runtime)
 
     async def describe_dcdn_er_usage_data_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnErUsageDataRequest,
     ) -> dcdn_20180115_models.DescribeDcdnErUsageDataResponse:
         """
-        >   You can call this operation up to 10 times per second per account.
-        *   The minimum time granularity for a query is one hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
+        # Usage notes
+        *   You can call this operation up to 10 times per second per account.
+        *   The minimum time granularity for a query is 1 hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
         
         @param request: DescribeDcdnErUsageDataRequest
         @return: DescribeDcdnErUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_er_usage_data_with_options_async(request, runtime)
 
@@ -10167,15 +9885,15 @@
 
     def describe_dcdn_ip_info_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnIpInfoResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnIpInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnIpInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10202,15 +9920,15 @@
 
     async def describe_dcdn_ip_info_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnIpInfoResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnIpInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnIpInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10236,28 +9954,28 @@
         )
 
     def describe_dcdn_ip_info(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpInfoRequest,
     ) -> dcdn_20180115_models.DescribeDcdnIpInfoResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnIpInfoRequest
         @return: DescribeDcdnIpInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_ip_info_with_options(request, runtime)
 
     async def describe_dcdn_ip_info_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpInfoRequest,
     ) -> dcdn_20180115_models.DescribeDcdnIpInfoResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnIpInfoRequest
         @return: DescribeDcdnIpInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_ip_info_with_options_async(request, runtime)
 
@@ -10475,15 +10193,16 @@
 
     def describe_dcdn_ipa_service_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpaServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnIpaServiceResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
         @param request: DescribeDcdnIpaServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnIpaServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10512,15 +10231,16 @@
 
     async def describe_dcdn_ipa_service_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpaServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnIpaServiceResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
         @param request: DescribeDcdnIpaServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnIpaServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10548,42 +10268,50 @@
         )
 
     def describe_dcdn_ipa_service(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpaServiceRequest,
     ) -> dcdn_20180115_models.DescribeDcdnIpaServiceResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
         @param request: DescribeDcdnIpaServiceRequest
         @return: DescribeDcdnIpaServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_ipa_service_with_options(request, runtime)
 
     async def describe_dcdn_ipa_service_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpaServiceRequest,
     ) -> dcdn_20180115_models.DescribeDcdnIpaServiceResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
         @param request: DescribeDcdnIpaServiceRequest
         @return: DescribeDcdnIpaServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_ipa_service_with_options_async(request, runtime)
 
     def describe_dcdn_ipa_user_domains_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpaUserDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnIpaUserDomainsResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The status of the domain name. Valid values:
+        *   **online**: enabled
+        *   **offline**: disabled
+        *   **configuring**: configuring
+        *   **configure_failed**: configuration failed
+        *   **checking**: reviewing
+        *   **check_failed**: review failed
         
         @param request: DescribeDcdnIpaUserDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnIpaUserDomainsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10630,15 +10358,21 @@
 
     async def describe_dcdn_ipa_user_domains_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpaUserDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnIpaUserDomainsResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The status of the domain name. Valid values:
+        *   **online**: enabled
+        *   **offline**: disabled
+        *   **configuring**: configuring
+        *   **configure_failed**: configuration failed
+        *   **checking**: reviewing
+        *   **check_failed**: review failed
         
         @param request: DescribeDcdnIpaUserDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnIpaUserDomainsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10684,28 +10418,40 @@
         )
 
     def describe_dcdn_ipa_user_domains(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpaUserDomainsRequest,
     ) -> dcdn_20180115_models.DescribeDcdnIpaUserDomainsResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The status of the domain name. Valid values:
+        *   **online**: enabled
+        *   **offline**: disabled
+        *   **configuring**: configuring
+        *   **configure_failed**: configuration failed
+        *   **checking**: reviewing
+        *   **check_failed**: review failed
         
         @param request: DescribeDcdnIpaUserDomainsRequest
         @return: DescribeDcdnIpaUserDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_ipa_user_domains_with_options(request, runtime)
 
     async def describe_dcdn_ipa_user_domains_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnIpaUserDomainsRequest,
     ) -> dcdn_20180115_models.DescribeDcdnIpaUserDomainsResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The status of the domain name. Valid values:
+        *   **online**: enabled
+        *   **offline**: disabled
+        *   **configuring**: configuring
+        *   **configure_failed**: configuration failed
+        *   **checking**: reviewing
+        *   **check_failed**: review failed
         
         @param request: DescribeDcdnIpaUserDomainsRequest
         @return: DescribeDcdnIpaUserDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_ipa_user_domains_with_options_async(request, runtime)
 
@@ -10877,17 +10623,15 @@
 
     def describe_dcdn_refresh_quota_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshQuotaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshQuotaResponse:
         """
-        >
-        *   You can call the **RefreshDcdnObjectCaches** operation to refresh content and call the **PreloadDcdnObjectCaches** operation to prefetch content.
-        *   You can call this operation up to 20 times per second.
+        The remaining number of URLs that can be prefetched each day.
         
         @param request: DescribeDcdnRefreshQuotaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnRefreshQuotaResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10916,17 +10660,15 @@
 
     async def describe_dcdn_refresh_quota_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshQuotaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshQuotaResponse:
         """
-        >
-        *   You can call the **RefreshDcdnObjectCaches** operation to refresh content and call the **PreloadDcdnObjectCaches** operation to prefetch content.
-        *   You can call this operation up to 20 times per second.
+        The remaining number of URLs that can be prefetched each day.
         
         @param request: DescribeDcdnRefreshQuotaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnRefreshQuotaResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10954,32 +10696,28 @@
         )
 
     def describe_dcdn_refresh_quota(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshQuotaRequest,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshQuotaResponse:
         """
-        >
-        *   You can call the **RefreshDcdnObjectCaches** operation to refresh content and call the **PreloadDcdnObjectCaches** operation to prefetch content.
-        *   You can call this operation up to 20 times per second.
+        The remaining number of URLs that can be prefetched each day.
         
         @param request: DescribeDcdnRefreshQuotaRequest
         @return: DescribeDcdnRefreshQuotaResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_refresh_quota_with_options(request, runtime)
 
     async def describe_dcdn_refresh_quota_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshQuotaRequest,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshQuotaResponse:
         """
-        >
-        *   You can call the **RefreshDcdnObjectCaches** operation to refresh content and call the **PreloadDcdnObjectCaches** operation to prefetch content.
-        *   You can call this operation up to 20 times per second.
+        The remaining number of URLs that can be prefetched each day.
         
         @param request: DescribeDcdnRefreshQuotaRequest
         @return: DescribeDcdnRefreshQuotaResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_refresh_quota_with_options_async(request, runtime)
 
@@ -10987,15 +10725,15 @@
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshTaskByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshTaskByIdResponse:
         """
         >
         *   You can query data within the last three days.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnRefreshTaskByIdRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnRefreshTaskByIdResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11024,15 +10762,15 @@
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshTaskByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshTaskByIdResponse:
         """
         >
         *   You can query data within the last three days.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnRefreshTaskByIdRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnRefreshTaskByIdResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11060,48 +10798,48 @@
     def describe_dcdn_refresh_task_by_id(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshTaskByIdRequest,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshTaskByIdResponse:
         """
         >
         *   You can query data within the last three days.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnRefreshTaskByIdRequest
         @return: DescribeDcdnRefreshTaskByIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_refresh_task_by_id_with_options(request, runtime)
 
     async def describe_dcdn_refresh_task_by_id_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshTaskByIdRequest,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshTaskByIdResponse:
         """
         >
         *   You can query data within the last three days.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnRefreshTaskByIdRequest
         @return: DescribeDcdnRefreshTaskByIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_refresh_task_by_id_with_options_async(request, runtime)
 
     def describe_dcdn_refresh_tasks_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshTasksResponse:
         """
-        >
-        *   You can query the refresh or prefetch tasks by ID or URL.
-        *   You can set both **TaskId** and **ObjectPath** in a request. If you do not set **TaskId** or **ObjectPath**, the data in the last 3 days on the first page is returned. By default, a maximum of 20 entries can be displayed on each page.
-        *   If you specify **DomainName** or **Status**, you must also specify **ObjectType**.
-        *   You can call this operation up to 10 times per second per account.
+        The type of the task.
+        *   **file**: URL-based refresh
+        *   **directory**: directory-based refresh
+        *   **preload**: URL-based prefetch
+        If you set the **DomainName** or **Status** parameter, you must also set this parameter.
         
         @param request: DescribeDcdnRefreshTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnRefreshTasksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11148,19 +10886,19 @@
 
     async def describe_dcdn_refresh_tasks_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshTasksResponse:
         """
-        >
-        *   You can query the refresh or prefetch tasks by ID or URL.
-        *   You can set both **TaskId** and **ObjectPath** in a request. If you do not set **TaskId** or **ObjectPath**, the data in the last 3 days on the first page is returned. By default, a maximum of 20 entries can be displayed on each page.
-        *   If you specify **DomainName** or **Status**, you must also specify **ObjectType**.
-        *   You can call this operation up to 10 times per second per account.
+        The type of the task.
+        *   **file**: URL-based refresh
+        *   **directory**: directory-based refresh
+        *   **preload**: URL-based prefetch
+        If you set the **DomainName** or **Status** parameter, you must also set this parameter.
         
         @param request: DescribeDcdnRefreshTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnRefreshTasksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11206,50 +10944,51 @@
         )
 
     def describe_dcdn_refresh_tasks(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshTasksRequest,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshTasksResponse:
         """
-        >
-        *   You can query the refresh or prefetch tasks by ID or URL.
-        *   You can set both **TaskId** and **ObjectPath** in a request. If you do not set **TaskId** or **ObjectPath**, the data in the last 3 days on the first page is returned. By default, a maximum of 20 entries can be displayed on each page.
-        *   If you specify **DomainName** or **Status**, you must also specify **ObjectType**.
-        *   You can call this operation up to 10 times per second per account.
+        The type of the task.
+        *   **file**: URL-based refresh
+        *   **directory**: directory-based refresh
+        *   **preload**: URL-based prefetch
+        If you set the **DomainName** or **Status** parameter, you must also set this parameter.
         
         @param request: DescribeDcdnRefreshTasksRequest
         @return: DescribeDcdnRefreshTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_refresh_tasks_with_options(request, runtime)
 
     async def describe_dcdn_refresh_tasks_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnRefreshTasksRequest,
     ) -> dcdn_20180115_models.DescribeDcdnRefreshTasksResponse:
         """
-        >
-        *   You can query the refresh or prefetch tasks by ID or URL.
-        *   You can set both **TaskId** and **ObjectPath** in a request. If you do not set **TaskId** or **ObjectPath**, the data in the last 3 days on the first page is returned. By default, a maximum of 20 entries can be displayed on each page.
-        *   If you specify **DomainName** or **Status**, you must also specify **ObjectType**.
-        *   You can call this operation up to 10 times per second per account.
+        The type of the task.
+        *   **file**: URL-based refresh
+        *   **directory**: directory-based refresh
+        *   **preload**: URL-based prefetch
+        If you set the **DomainName** or **Status** parameter, you must also set this parameter.
         
         @param request: DescribeDcdnRefreshTasksRequest
         @return: DescribeDcdnRefreshTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_refresh_tasks_with_options_async(request, runtime)
 
     def describe_dcdn_region_and_isp_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnRegionAndIspRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnRegionAndIspResponse:
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        ****\
         
         @param request: DescribeDcdnRegionAndIspRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnRegionAndIspResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11278,15 +11017,16 @@
 
     async def describe_dcdn_region_and_isp_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnRegionAndIspRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnRegionAndIspResponse:
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        ****\
         
         @param request: DescribeDcdnRegionAndIspRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnRegionAndIspResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11314,28 +11054,30 @@
         )
 
     def describe_dcdn_region_and_isp(
         self,
         request: dcdn_20180115_models.DescribeDcdnRegionAndIspRequest,
     ) -> dcdn_20180115_models.DescribeDcdnRegionAndIspResponse:
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        ****\
         
         @param request: DescribeDcdnRegionAndIspRequest
         @return: DescribeDcdnRegionAndIspResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_region_and_isp_with_options(request, runtime)
 
     async def describe_dcdn_region_and_isp_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnRegionAndIspRequest,
     ) -> dcdn_20180115_models.DescribeDcdnRegionAndIspResponse:
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        ****\
         
         @param request: DescribeDcdnRegionAndIspRequest
         @return: DescribeDcdnRegionAndIspResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_region_and_isp_with_options_async(request, runtime)
 
@@ -11565,15 +11307,15 @@
 
     def describe_dcdn_slsrealtime_log_delivery_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnSLSRealtimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnSLSRealtimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11600,15 +11342,15 @@
 
     async def describe_dcdn_slsrealtime_log_delivery_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnSLSRealtimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnSLSRealtimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11634,28 +11376,28 @@
         )
 
     def describe_dcdn_slsrealtime_log_delivery(
         self,
         request: dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryRequest,
     ) -> dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnSLSRealtimeLogDeliveryRequest
         @return: DescribeDcdnSLSRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_slsrealtime_log_delivery_with_options(request, runtime)
 
     async def describe_dcdn_slsrealtime_log_delivery_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryRequest,
     ) -> dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnSLSRealtimeLogDeliveryRequest
         @return: DescribeDcdnSLSRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_slsrealtime_log_delivery_with_options_async(request, runtime)
 
@@ -11873,15 +11615,15 @@
 
     def describe_dcdn_sec_func_info_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnSecFuncInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnSecFuncInfoResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnSecFuncInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnSecFuncInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11910,15 +11652,15 @@
 
     async def describe_dcdn_sec_func_info_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnSecFuncInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnSecFuncInfoResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnSecFuncInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnSecFuncInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11946,41 +11688,41 @@
         )
 
     def describe_dcdn_sec_func_info(
         self,
         request: dcdn_20180115_models.DescribeDcdnSecFuncInfoRequest,
     ) -> dcdn_20180115_models.DescribeDcdnSecFuncInfoResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnSecFuncInfoRequest
         @return: DescribeDcdnSecFuncInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_sec_func_info_with_options(request, runtime)
 
     async def describe_dcdn_sec_func_info_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnSecFuncInfoRequest,
     ) -> dcdn_20180115_models.DescribeDcdnSecFuncInfoResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnSecFuncInfoRequest
         @return: DescribeDcdnSecFuncInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_sec_func_info_with_options_async(request, runtime)
 
     def describe_dcdn_sec_spec_info_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnSecSpecInfoResponse:
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnSecSpecInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnSecSpecInfoResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -12000,15 +11742,15 @@
         )
 
     async def describe_dcdn_sec_spec_info_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnSecSpecInfoResponse:
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDcdnSecSpecInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnSecSpecInfoResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -12025,37 +11767,37 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnSecSpecInfoResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dcdn_sec_spec_info(self) -> dcdn_20180115_models.DescribeDcdnSecSpecInfoResponse:
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
         @return: DescribeDcdnSecSpecInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_sec_spec_info_with_options(runtime)
 
     async def describe_dcdn_sec_spec_info_async(self) -> dcdn_20180115_models.DescribeDcdnSecSpecInfoResponse:
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
         @return: DescribeDcdnSecSpecInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_sec_spec_info_with_options_async(runtime)
 
     def describe_dcdn_service_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnServiceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12084,15 +11826,15 @@
 
     async def describe_dcdn_service_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnServiceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12120,28 +11862,28 @@
         )
 
     def describe_dcdn_service(
         self,
         request: dcdn_20180115_models.DescribeDcdnServiceRequest,
     ) -> dcdn_20180115_models.DescribeDcdnServiceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnServiceRequest
         @return: DescribeDcdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_service_with_options(request, runtime)
 
     async def describe_dcdn_service_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnServiceRequest,
     ) -> dcdn_20180115_models.DescribeDcdnServiceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnServiceRequest
         @return: DescribeDcdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_service_with_options_async(request, runtime)
 
@@ -12407,15 +12149,15 @@
 
     def describe_dcdn_top_domains_by_flow_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnTopDomainsByFlowRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnTopDomainsByFlowResponse:
         """
-        *Before you call this operation, pay attention to the following considerations:**If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
+        \\\\*Before you call this operation, pay attention to the following considerations:\\*\\* If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
         
         @param request: DescribeDcdnTopDomainsByFlowRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnTopDomainsByFlowResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12446,15 +12188,15 @@
 
     async def describe_dcdn_top_domains_by_flow_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnTopDomainsByFlowRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnTopDomainsByFlowResponse:
         """
-        *Before you call this operation, pay attention to the following considerations:**If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
+        \\\\*Before you call this operation, pay attention to the following considerations:\\*\\* If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
         
         @param request: DescribeDcdnTopDomainsByFlowRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnTopDomainsByFlowResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12484,28 +12226,28 @@
         )
 
     def describe_dcdn_top_domains_by_flow(
         self,
         request: dcdn_20180115_models.DescribeDcdnTopDomainsByFlowRequest,
     ) -> dcdn_20180115_models.DescribeDcdnTopDomainsByFlowResponse:
         """
-        *Before you call this operation, pay attention to the following considerations:**If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
+        \\\\*Before you call this operation, pay attention to the following considerations:\\*\\* If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
         
         @param request: DescribeDcdnTopDomainsByFlowRequest
         @return: DescribeDcdnTopDomainsByFlowResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_top_domains_by_flow_with_options(request, runtime)
 
     async def describe_dcdn_top_domains_by_flow_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnTopDomainsByFlowRequest,
     ) -> dcdn_20180115_models.DescribeDcdnTopDomainsByFlowResponse:
         """
-        *Before you call this operation, pay attention to the following considerations:**If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
+        \\\\*Before you call this operation, pay attention to the following considerations:\\*\\* If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
         
         @param request: DescribeDcdnTopDomainsByFlowRequest
         @return: DescribeDcdnTopDomainsByFlowResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_top_domains_by_flow_with_options_async(request, runtime)
 
@@ -13343,15 +13085,16 @@
 
     def describe_dcdn_user_resource_package_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnUserResourcePackageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnUserResourcePackageResponse:
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        **The maximum number of times that each user can call this operation per second is 30.
         
         @param request: DescribeDcdnUserResourcePackageRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnUserResourcePackageResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13382,15 +13125,16 @@
 
     async def describe_dcdn_user_resource_package_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnUserResourcePackageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnUserResourcePackageResponse:
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        **The maximum number of times that each user can call this operation per second is 30.
         
         @param request: DescribeDcdnUserResourcePackageRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnUserResourcePackageResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13420,28 +13164,30 @@
         )
 
     def describe_dcdn_user_resource_package(
         self,
         request: dcdn_20180115_models.DescribeDcdnUserResourcePackageRequest,
     ) -> dcdn_20180115_models.DescribeDcdnUserResourcePackageResponse:
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        **The maximum number of times that each user can call this operation per second is 30.
         
         @param request: DescribeDcdnUserResourcePackageRequest
         @return: DescribeDcdnUserResourcePackageResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_user_resource_package_with_options(request, runtime)
 
     async def describe_dcdn_user_resource_package_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnUserResourcePackageRequest,
     ) -> dcdn_20180115_models.DescribeDcdnUserResourcePackageResponse:
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        **The maximum number of times that each user can call this operation per second is 30.
         
         @param request: DescribeDcdnUserResourcePackageRequest
         @return: DescribeDcdnUserResourcePackageResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_user_resource_package_with_options_async(request, runtime)
 
@@ -13551,15 +13297,15 @@
 
     def describe_dcdn_user_sec_drop_by_minute_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        The domain name.
         
         @param request: DescribeDcdnUserSecDropByMinuteRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnUserSecDropByMinuteResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13602,15 +13348,15 @@
 
     async def describe_dcdn_user_sec_drop_by_minute_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        The domain name.
         
         @param request: DescribeDcdnUserSecDropByMinuteRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnUserSecDropByMinuteResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13652,41 +13398,41 @@
         )
 
     def describe_dcdn_user_sec_drop_by_minute(
         self,
         request: dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteRequest,
     ) -> dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        The domain name.
         
         @param request: DescribeDcdnUserSecDropByMinuteRequest
         @return: DescribeDcdnUserSecDropByMinuteResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_user_sec_drop_by_minute_with_options(request, runtime)
 
     async def describe_dcdn_user_sec_drop_by_minute_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteRequest,
     ) -> dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        The domain name.
         
         @param request: DescribeDcdnUserSecDropByMinuteRequest
         @return: DescribeDcdnUserSecDropByMinuteResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_user_sec_drop_by_minute_with_options_async(request, runtime)
 
     def describe_dcdn_user_tags_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnUserTagsResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDcdnUserTagsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnUserTagsResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -13706,15 +13452,15 @@
         )
 
     async def describe_dcdn_user_tags_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnUserTagsResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDcdnUserTagsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnUserTagsResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -13731,24 +13477,24 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnUserTagsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dcdn_user_tags(self) -> dcdn_20180115_models.DescribeDcdnUserTagsResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 100.
+        The ID of the request.
         
         @return: DescribeDcdnUserTagsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_user_tags_with_options(runtime)
 
     async def describe_dcdn_user_tags_async(self) -> dcdn_20180115_models.DescribeDcdnUserTagsResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 100.
+        The ID of the request.
         
         @return: DescribeDcdnUserTagsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_user_tags_with_options_async(runtime)
 
     def describe_dcdn_verify_content_with_options(
@@ -13953,16 +13699,15 @@
 
     def describe_dcdn_waf_domain_detail_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafDomainDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafDomainDetailResponse:
         """
-        # Usage notes
-        You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
         @param request: DescribeDcdnWafDomainDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafDomainDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13989,16 +13734,15 @@
 
     async def describe_dcdn_waf_domain_detail_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafDomainDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafDomainDetailResponse:
         """
-        # Usage notes
-        You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
         @param request: DescribeDcdnWafDomainDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafDomainDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14024,30 +13768,28 @@
         )
 
     def describe_dcdn_waf_domain_detail(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafDomainDetailRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafDomainDetailResponse:
         """
-        # Usage notes
-        You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
         @param request: DescribeDcdnWafDomainDetailRequest
         @return: DescribeDcdnWafDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_domain_detail_with_options(request, runtime)
 
     async def describe_dcdn_waf_domain_detail_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafDomainDetailRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafDomainDetailResponse:
         """
-        # Usage notes
-        You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
         @param request: DescribeDcdnWafDomainDetailRequest
         @return: DescribeDcdnWafDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_waf_domain_detail_with_options_async(request, runtime)
 
@@ -14261,15 +14003,15 @@
 
     def describe_dcdn_waf_geo_info_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafGeoInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafGeoInfoResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDcdnWafGeoInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafGeoInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14296,15 +14038,15 @@
 
     async def describe_dcdn_waf_geo_info_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafGeoInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafGeoInfoResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDcdnWafGeoInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafGeoInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14330,43 +14072,43 @@
         )
 
     def describe_dcdn_waf_geo_info(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafGeoInfoRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafGeoInfoResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDcdnWafGeoInfoRequest
         @return: DescribeDcdnWafGeoInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_geo_info_with_options(request, runtime)
 
     async def describe_dcdn_waf_geo_info_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafGeoInfoRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafGeoInfoResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDcdnWafGeoInfoRequest
         @return: DescribeDcdnWafGeoInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_waf_geo_info_with_options_async(request, runtime)
 
     def describe_dcdn_waf_logs_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafLogsResponse:
         """
         >
-        *   If you do not set StartTime or EndTime, data collected in the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         *   The log data is collected every hour.
         *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnWafLogsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafLogsResponse
         """
@@ -14404,15 +14146,15 @@
     async def describe_dcdn_waf_logs_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafLogsResponse:
         """
         >
-        *   If you do not set StartTime or EndTime, data collected in the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         *   The log data is collected every hour.
         *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnWafLogsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafLogsResponse
         """
@@ -14449,15 +14191,15 @@
 
     def describe_dcdn_waf_logs(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafLogsRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafLogsResponse:
         """
         >
-        *   If you do not set StartTime or EndTime, data collected in the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         *   The log data is collected every hour.
         *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnWafLogsRequest
         @return: DescribeDcdnWafLogsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -14465,15 +14207,15 @@
 
     async def describe_dcdn_waf_logs_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafLogsRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafLogsResponse:
         """
         >
-        *   If you do not set StartTime or EndTime, data collected in the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         *   The log data is collected every hour.
         *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnWafLogsRequest
         @return: DescribeDcdnWafLogsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -14585,15 +14327,15 @@
 
     def describe_dcdn_waf_policy_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafPolicyResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDcdnWafPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14620,15 +14362,15 @@
 
     async def describe_dcdn_waf_policy_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafPolicyResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDcdnWafPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14654,42 +14396,42 @@
         )
 
     def describe_dcdn_waf_policy(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafPolicyRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafPolicyResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDcdnWafPolicyRequest
         @return: DescribeDcdnWafPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_policy_with_options(request, runtime)
 
     async def describe_dcdn_waf_policy_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafPolicyRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafPolicyResponse:
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDcdnWafPolicyRequest
         @return: DescribeDcdnWafPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_waf_policy_with_options_async(request, runtime)
 
     def describe_dcdn_waf_policy_domains_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafPolicyDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafPolicyDomainsResponse:
         """
-        >You can call this operation up to 20 times per second per account.
+        The number of domain names returned per page, which is the same as the PageSize parameter in request parameters.
         
         @param request: DescribeDcdnWafPolicyDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafPolicyDomainsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14720,15 +14462,15 @@
 
     async def describe_dcdn_waf_policy_domains_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafPolicyDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnWafPolicyDomainsResponse:
         """
-        >You can call this operation up to 20 times per second per account.
+        The number of domain names returned per page, which is the same as the PageSize parameter in request parameters.
         
         @param request: DescribeDcdnWafPolicyDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnWafPolicyDomainsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14758,28 +14500,28 @@
         )
 
     def describe_dcdn_waf_policy_domains(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafPolicyDomainsRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafPolicyDomainsResponse:
         """
-        >You can call this operation up to 20 times per second per account.
+        The number of domain names returned per page, which is the same as the PageSize parameter in request parameters.
         
         @param request: DescribeDcdnWafPolicyDomainsRequest
         @return: DescribeDcdnWafPolicyDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_policy_domains_with_options(request, runtime)
 
     async def describe_dcdn_waf_policy_domains_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnWafPolicyDomainsRequest,
     ) -> dcdn_20180115_models.DescribeDcdnWafPolicyDomainsResponse:
         """
-        >You can call this operation up to 20 times per second per account.
+        The number of domain names returned per page, which is the same as the PageSize parameter in request parameters.
         
         @param request: DescribeDcdnWafPolicyDomainsRequest
         @return: DescribeDcdnWafPolicyDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_waf_policy_domains_with_options_async(request, runtime)
 
@@ -15834,15 +15576,15 @@
         return await self.describe_routine_with_options_async(request, runtime)
 
     def describe_routine_canary_envs_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeRoutineCanaryEnvsResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        The canary release environments that are supported by the edge routine.
         
         @param request: DescribeRoutineCanaryEnvsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRoutineCanaryEnvsResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -15862,15 +15604,15 @@
         )
 
     async def describe_routine_canary_envs_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeRoutineCanaryEnvsResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        The canary release environments that are supported by the edge routine.
         
         @param request: DescribeRoutineCanaryEnvsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRoutineCanaryEnvsResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -15887,37 +15629,37 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeRoutineCanaryEnvsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_routine_canary_envs(self) -> dcdn_20180115_models.DescribeRoutineCanaryEnvsResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        The canary release environments that are supported by the edge routine.
         
         @return: DescribeRoutineCanaryEnvsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_routine_canary_envs_with_options(runtime)
 
     async def describe_routine_canary_envs_async(self) -> dcdn_20180115_models.DescribeRoutineCanaryEnvsResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        The canary release environments that are supported by the edge routine.
         
         @return: DescribeRoutineCanaryEnvsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_routine_canary_envs_with_options_async(runtime)
 
     def describe_routine_code_revision_with_options(
         self,
         request: dcdn_20180115_models.DescribeRoutineCodeRevisionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeRoutineCodeRevisionResponse:
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRoutineCodeRevisionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRoutineCodeRevisionResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -15946,15 +15688,15 @@
 
     async def describe_routine_code_revision_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeRoutineCodeRevisionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeRoutineCodeRevisionResponse:
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRoutineCodeRevisionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRoutineCodeRevisionResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -15982,28 +15724,28 @@
         )
 
     def describe_routine_code_revision(
         self,
         request: dcdn_20180115_models.DescribeRoutineCodeRevisionRequest,
     ) -> dcdn_20180115_models.DescribeRoutineCodeRevisionResponse:
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRoutineCodeRevisionRequest
         @return: DescribeRoutineCodeRevisionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_routine_code_revision_with_options(request, runtime)
 
     async def describe_routine_code_revision_async(
         self,
         request: dcdn_20180115_models.DescribeRoutineCodeRevisionRequest,
     ) -> dcdn_20180115_models.DescribeRoutineCodeRevisionResponse:
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRoutineCodeRevisionRequest
         @return: DescribeRoutineCodeRevisionResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_routine_code_revision_with_options_async(request, runtime)
 
@@ -16157,15 +15899,16 @@
 
     def describe_user_dcdn_ipa_status_with_options(
         self,
         request: dcdn_20180115_models.DescribeUserDcdnIpaStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeUserDcdnIpaStatusResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
         @param request: DescribeUserDcdnIpaStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserDcdnIpaStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16194,15 +15937,16 @@
 
     async def describe_user_dcdn_ipa_status_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeUserDcdnIpaStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeUserDcdnIpaStatusResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
         @param request: DescribeUserDcdnIpaStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserDcdnIpaStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16230,42 +15974,44 @@
         )
 
     def describe_user_dcdn_ipa_status(
         self,
         request: dcdn_20180115_models.DescribeUserDcdnIpaStatusRequest,
     ) -> dcdn_20180115_models.DescribeUserDcdnIpaStatusResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
         @param request: DescribeUserDcdnIpaStatusRequest
         @return: DescribeUserDcdnIpaStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_dcdn_ipa_status_with_options(request, runtime)
 
     async def describe_user_dcdn_ipa_status_async(
         self,
         request: dcdn_20180115_models.DescribeUserDcdnIpaStatusRequest,
     ) -> dcdn_20180115_models.DescribeUserDcdnIpaStatusResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
         @param request: DescribeUserDcdnIpaStatusRequest
         @return: DescribeUserDcdnIpaStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_dcdn_ipa_status_with_options_async(request, runtime)
 
     def describe_user_dcdn_status_with_options(
         self,
         request: dcdn_20180115_models.DescribeUserDcdnStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeUserDcdnStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeUserDcdnStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserDcdnStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16292,15 +16038,15 @@
 
     async def describe_user_dcdn_status_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeUserDcdnStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeUserDcdnStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeUserDcdnStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserDcdnStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16326,42 +16072,42 @@
         )
 
     def describe_user_dcdn_status(
         self,
         request: dcdn_20180115_models.DescribeUserDcdnStatusRequest,
     ) -> dcdn_20180115_models.DescribeUserDcdnStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeUserDcdnStatusRequest
         @return: DescribeUserDcdnStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_dcdn_status_with_options(request, runtime)
 
     async def describe_user_dcdn_status_async(
         self,
         request: dcdn_20180115_models.DescribeUserDcdnStatusRequest,
     ) -> dcdn_20180115_models.DescribeUserDcdnStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeUserDcdnStatusRequest
         @return: DescribeUserDcdnStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_dcdn_status_with_options_async(request, runtime)
 
     def describe_user_er_status_with_options(
         self,
         request: dcdn_20180115_models.DescribeUserErStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeUserErStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeUserErStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserErStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16388,15 +16134,15 @@
 
     async def describe_user_er_status_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeUserErStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeUserErStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeUserErStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserErStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16422,42 +16168,42 @@
         )
 
     def describe_user_er_status(
         self,
         request: dcdn_20180115_models.DescribeUserErStatusRequest,
     ) -> dcdn_20180115_models.DescribeUserErStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeUserErStatusRequest
         @return: DescribeUserErStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_er_status_with_options(request, runtime)
 
     async def describe_user_er_status_async(
         self,
         request: dcdn_20180115_models.DescribeUserErStatusRequest,
     ) -> dcdn_20180115_models.DescribeUserErStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeUserErStatusRequest
         @return: DescribeUserErStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_er_status_with_options_async(request, runtime)
 
     def describe_user_logservice_status_with_options(
         self,
         request: dcdn_20180115_models.DescribeUserLogserviceStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeUserLogserviceStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeUserLogserviceStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserLogserviceStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16486,15 +16232,15 @@
 
     async def describe_user_logservice_status_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeUserLogserviceStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeUserLogserviceStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeUserLogserviceStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserLogserviceStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16522,28 +16268,28 @@
         )
 
     def describe_user_logservice_status(
         self,
         request: dcdn_20180115_models.DescribeUserLogserviceStatusRequest,
     ) -> dcdn_20180115_models.DescribeUserLogserviceStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeUserLogserviceStatusRequest
         @return: DescribeUserLogserviceStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_logservice_status_with_options(request, runtime)
 
     async def describe_user_logservice_status_async(
         self,
         request: dcdn_20180115_models.DescribeUserLogserviceStatusRequest,
     ) -> dcdn_20180115_models.DescribeUserLogserviceStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeUserLogserviceStatusRequest
         @return: DescribeUserLogserviceStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_logservice_status_with_options_async(request, runtime)
 
@@ -16935,16 +16681,17 @@
 
     def modify_dcdn_waf_policy_with_options(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.ModifyDcdnWafPolicyResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: ModifyDcdnWafPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDcdnWafPolicyResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -16975,16 +16722,17 @@
 
     async def modify_dcdn_waf_policy_with_options_async(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.ModifyDcdnWafPolicyResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: ModifyDcdnWafPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDcdnWafPolicyResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -17014,50 +16762,44 @@
         )
 
     def modify_dcdn_waf_policy(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafPolicyRequest,
     ) -> dcdn_20180115_models.ModifyDcdnWafPolicyResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: ModifyDcdnWafPolicyRequest
         @return: ModifyDcdnWafPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dcdn_waf_policy_with_options(request, runtime)
 
     async def modify_dcdn_waf_policy_async(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafPolicyRequest,
     ) -> dcdn_20180115_models.ModifyDcdnWafPolicyResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
         @param request: ModifyDcdnWafPolicyRequest
         @return: ModifyDcdnWafPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dcdn_waf_policy_with_options_async(request, runtime)
 
     def modify_dcdn_waf_policy_domains_with_options(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafPolicyDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.ModifyDcdnWafPolicyDomainsResponse:
-        """
-        >   You can call this operation up to 20 times per second.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
-        
-        @param request: ModifyDcdnWafPolicyDomainsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDcdnWafPolicyDomainsResponse
-        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.bind_domains):
             body['BindDomains'] = request.bind_domains
         if not UtilClient.is_unset(request.method):
             body['Method'] = request.method
         if not UtilClient.is_unset(request.policy_id):
@@ -17084,22 +16826,14 @@
         )
 
     async def modify_dcdn_waf_policy_domains_with_options_async(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafPolicyDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.ModifyDcdnWafPolicyDomainsResponse:
-        """
-        >   You can call this operation up to 20 times per second.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
-        
-        @param request: ModifyDcdnWafPolicyDomainsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyDcdnWafPolicyDomainsResponse
-        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.bind_domains):
             body['BindDomains'] = request.bind_domains
         if not UtilClient.is_unset(request.method):
             body['Method'] = request.method
         if not UtilClient.is_unset(request.policy_id):
@@ -17125,45 +16859,32 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dcdn_waf_policy_domains(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafPolicyDomainsRequest,
     ) -> dcdn_20180115_models.ModifyDcdnWafPolicyDomainsResponse:
-        """
-        >   You can call this operation up to 20 times per second.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
-        
-        @param request: ModifyDcdnWafPolicyDomainsRequest
-        @return: ModifyDcdnWafPolicyDomainsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dcdn_waf_policy_domains_with_options(request, runtime)
 
     async def modify_dcdn_waf_policy_domains_async(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafPolicyDomainsRequest,
     ) -> dcdn_20180115_models.ModifyDcdnWafPolicyDomainsResponse:
-        """
-        >   You can call this operation up to 20 times per second.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
-        
-        @param request: ModifyDcdnWafPolicyDomainsRequest
-        @return: ModifyDcdnWafPolicyDomainsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dcdn_waf_policy_domains_with_options_async(request, runtime)
 
     def modify_dcdn_waf_rule_with_options(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.ModifyDcdnWafRuleResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
+        #
+        *   You can call this operation up to 20 times per second.
         *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
         *   You must configure at least one of the **RuleStatus**, **RuleName** and **RuleConfig** parameters.
         
         @param request: ModifyDcdnWafRuleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDcdnWafRuleResponse
         """
@@ -17198,15 +16919,16 @@
 
     async def modify_dcdn_waf_rule_with_options_async(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.ModifyDcdnWafRuleResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
+        #
+        *   You can call this operation up to 20 times per second.
         *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
         *   You must configure at least one of the **RuleStatus**, **RuleName** and **RuleConfig** parameters.
         
         @param request: ModifyDcdnWafRuleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDcdnWafRuleResponse
         """
@@ -17240,30 +16962,32 @@
         )
 
     def modify_dcdn_waf_rule(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafRuleRequest,
     ) -> dcdn_20180115_models.ModifyDcdnWafRuleResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
+        #
+        *   You can call this operation up to 20 times per second.
         *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
         *   You must configure at least one of the **RuleStatus**, **RuleName** and **RuleConfig** parameters.
         
         @param request: ModifyDcdnWafRuleRequest
         @return: ModifyDcdnWafRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dcdn_waf_rule_with_options(request, runtime)
 
     async def modify_dcdn_waf_rule_async(
         self,
         request: dcdn_20180115_models.ModifyDcdnWafRuleRequest,
     ) -> dcdn_20180115_models.ModifyDcdnWafRuleResponse:
         """
-        >   You can call this operation up to 20 times per second per account.
+        #
+        *   You can call this operation up to 20 times per second.
         *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
         *   You must configure at least one of the **RuleStatus**, **RuleName** and **RuleConfig** parameters.
         
         @param request: ModifyDcdnWafRuleRequest
         @return: ModifyDcdnWafRuleResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -17379,25 +17103,25 @@
 
     def preload_dcdn_object_caches_with_options(
         self,
         request: dcdn_20180115_models.PreloadDcdnObjectCachesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.PreloadDcdnObjectCachesResponse:
         """
-        # Usage notes
+        #
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
-        *   Dynamic Route for CDN (DCDN) supports POST requests in which parameters are sent as a form.
+        *   Dynamic Content Delivery Network (DCDN) supports POST requests in which parameters are sent as a form.
         *   By default, each Alibaba Cloud account can submit up to 1,000 URLs per day. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase your daily quota. Alibaba Cloud reviews your application and then increases the quota accordingly.
-        *   Each Alibaba Cloud account can submit up to 100 URLs in a request.
+        *   You can specify at most 100 URLs in each prefetch request.
         *   The prefetch queue of each Alibaba Cloud account can contain up to 50,000 URLs. DCDN executes prefetch tasks based on the time at which you submit the URLs.
         *   You can call this operation up to 15 times per second per account.
-        # Precautions
-        *   After a refresh task is submitted and executed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks take 5 to 30 minutes to complete. A task with a smaller average file size takes less time.
-        *   To allow Resource Access Management (RAM) users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
+        # Usage notes
+        *   After a refresh task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks require 5 to 30 minutes to complete. A task with a smaller average file size requires less time.
+        *   To allow RAM users to perform this operation, you need to first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
         
         @param request: PreloadDcdnObjectCachesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: PreloadDcdnObjectCachesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -17434,25 +17158,25 @@
 
     async def preload_dcdn_object_caches_with_options_async(
         self,
         request: dcdn_20180115_models.PreloadDcdnObjectCachesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.PreloadDcdnObjectCachesResponse:
         """
-        # Usage notes
+        #
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
-        *   Dynamic Route for CDN (DCDN) supports POST requests in which parameters are sent as a form.
+        *   Dynamic Content Delivery Network (DCDN) supports POST requests in which parameters are sent as a form.
         *   By default, each Alibaba Cloud account can submit up to 1,000 URLs per day. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase your daily quota. Alibaba Cloud reviews your application and then increases the quota accordingly.
-        *   Each Alibaba Cloud account can submit up to 100 URLs in a request.
+        *   You can specify at most 100 URLs in each prefetch request.
         *   The prefetch queue of each Alibaba Cloud account can contain up to 50,000 URLs. DCDN executes prefetch tasks based on the time at which you submit the URLs.
         *   You can call this operation up to 15 times per second per account.
-        # Precautions
-        *   After a refresh task is submitted and executed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks take 5 to 30 minutes to complete. A task with a smaller average file size takes less time.
-        *   To allow Resource Access Management (RAM) users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
+        # Usage notes
+        *   After a refresh task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks require 5 to 30 minutes to complete. A task with a smaller average file size requires less time.
+        *   To allow RAM users to perform this operation, you need to first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
         
         @param request: PreloadDcdnObjectCachesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: PreloadDcdnObjectCachesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -17488,62 +17212,62 @@
         )
 
     def preload_dcdn_object_caches(
         self,
         request: dcdn_20180115_models.PreloadDcdnObjectCachesRequest,
     ) -> dcdn_20180115_models.PreloadDcdnObjectCachesResponse:
         """
-        # Usage notes
+        #
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
-        *   Dynamic Route for CDN (DCDN) supports POST requests in which parameters are sent as a form.
+        *   Dynamic Content Delivery Network (DCDN) supports POST requests in which parameters are sent as a form.
         *   By default, each Alibaba Cloud account can submit up to 1,000 URLs per day. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase your daily quota. Alibaba Cloud reviews your application and then increases the quota accordingly.
-        *   Each Alibaba Cloud account can submit up to 100 URLs in a request.
+        *   You can specify at most 100 URLs in each prefetch request.
         *   The prefetch queue of each Alibaba Cloud account can contain up to 50,000 URLs. DCDN executes prefetch tasks based on the time at which you submit the URLs.
         *   You can call this operation up to 15 times per second per account.
-        # Precautions
-        *   After a refresh task is submitted and executed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks take 5 to 30 minutes to complete. A task with a smaller average file size takes less time.
-        *   To allow Resource Access Management (RAM) users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
+        # Usage notes
+        *   After a refresh task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks require 5 to 30 minutes to complete. A task with a smaller average file size requires less time.
+        *   To allow RAM users to perform this operation, you need to first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
         
         @param request: PreloadDcdnObjectCachesRequest
         @return: PreloadDcdnObjectCachesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.preload_dcdn_object_caches_with_options(request, runtime)
 
     async def preload_dcdn_object_caches_async(
         self,
         request: dcdn_20180115_models.PreloadDcdnObjectCachesRequest,
     ) -> dcdn_20180115_models.PreloadDcdnObjectCachesResponse:
         """
-        # Usage notes
+        #
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
-        *   Dynamic Route for CDN (DCDN) supports POST requests in which parameters are sent as a form.
+        *   Dynamic Content Delivery Network (DCDN) supports POST requests in which parameters are sent as a form.
         *   By default, each Alibaba Cloud account can submit up to 1,000 URLs per day. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase your daily quota. Alibaba Cloud reviews your application and then increases the quota accordingly.
-        *   Each Alibaba Cloud account can submit up to 100 URLs in a request.
+        *   You can specify at most 100 URLs in each prefetch request.
         *   The prefetch queue of each Alibaba Cloud account can contain up to 50,000 URLs. DCDN executes prefetch tasks based on the time at which you submit the URLs.
         *   You can call this operation up to 15 times per second per account.
-        # Precautions
-        *   After a refresh task is submitted and executed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks take 5 to 30 minutes to complete. A task with a smaller average file size takes less time.
-        *   To allow Resource Access Management (RAM) users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
+        # Usage notes
+        *   After a refresh task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks require 5 to 30 minutes to complete. A task with a smaller average file size requires less time.
+        *   To allow RAM users to perform this operation, you need to first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
         
         @param request: PreloadDcdnObjectCachesRequest
         @return: PreloadDcdnObjectCachesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.preload_dcdn_object_caches_with_options_async(request, runtime)
 
     def publish_dcdn_staging_config_to_production_with_options(
         self,
         request: dcdn_20180115_models.PublishDcdnStagingConfigToProductionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.PublishDcdnStagingConfigToProductionResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: PublishDcdnStagingConfigToProductionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: PublishDcdnStagingConfigToProductionResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -17572,15 +17296,15 @@
 
     async def publish_dcdn_staging_config_to_production_with_options_async(
         self,
         request: dcdn_20180115_models.PublishDcdnStagingConfigToProductionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.PublishDcdnStagingConfigToProductionResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: PublishDcdnStagingConfigToProductionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: PublishDcdnStagingConfigToProductionResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -17608,42 +17332,42 @@
         )
 
     def publish_dcdn_staging_config_to_production(
         self,
         request: dcdn_20180115_models.PublishDcdnStagingConfigToProductionRequest,
     ) -> dcdn_20180115_models.PublishDcdnStagingConfigToProductionResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: PublishDcdnStagingConfigToProductionRequest
         @return: PublishDcdnStagingConfigToProductionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.publish_dcdn_staging_config_to_production_with_options(request, runtime)
 
     async def publish_dcdn_staging_config_to_production_async(
         self,
         request: dcdn_20180115_models.PublishDcdnStagingConfigToProductionRequest,
     ) -> dcdn_20180115_models.PublishDcdnStagingConfigToProductionResponse:
         """
-        >  The maximum number of times that users can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: PublishDcdnStagingConfigToProductionRequest
         @return: PublishDcdnStagingConfigToProductionResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.publish_dcdn_staging_config_to_production_with_options_async(request, runtime)
 
     def publish_routine_code_revision_with_options(
         self,
         tmp_req: dcdn_20180115_models.PublishRoutineCodeRevisionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.PublishRoutineCodeRevisionResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param tmp_req: PublishRoutineCodeRevisionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: PublishRoutineCodeRevisionResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dcdn_20180115_models.PublishRoutineCodeRevisionShrinkRequest()
@@ -17678,15 +17402,15 @@
 
     async def publish_routine_code_revision_with_options_async(
         self,
         tmp_req: dcdn_20180115_models.PublishRoutineCodeRevisionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.PublishRoutineCodeRevisionResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param tmp_req: PublishRoutineCodeRevisionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: PublishRoutineCodeRevisionResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dcdn_20180115_models.PublishRoutineCodeRevisionShrinkRequest()
@@ -17720,28 +17444,28 @@
         )
 
     def publish_routine_code_revision(
         self,
         request: dcdn_20180115_models.PublishRoutineCodeRevisionRequest,
     ) -> dcdn_20180115_models.PublishRoutineCodeRevisionResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: PublishRoutineCodeRevisionRequest
         @return: PublishRoutineCodeRevisionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.publish_routine_code_revision_with_options(request, runtime)
 
     async def publish_routine_code_revision_async(
         self,
         request: dcdn_20180115_models.PublishRoutineCodeRevisionRequest,
     ) -> dcdn_20180115_models.PublishRoutineCodeRevisionResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: PublishRoutineCodeRevisionRequest
         @return: PublishRoutineCodeRevisionResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.publish_routine_code_revision_with_options_async(request, runtime)
 
@@ -17829,23 +17553,25 @@
 
     def refresh_dcdn_object_caches_with_options(
         self,
         request: dcdn_20180115_models.RefreshDcdnObjectCachesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.RefreshDcdnObjectCachesResponse:
         """
-        Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests in which parameters are sent as a form.
+        #
+        *   DCDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
-        *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to apply for an increased upper limit. Alibaba Cloud will review your application and then increase the quota accordingly.
+        *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. DCDN evaluates your application based on your workloads.
         *   You can specify up to 1,000 URLs or 100 directories that you want to refresh in each request.
-        *   You can refresh a maximum of 1,000 URLs per minute for each domain name.
+        *   You can refresh up to 1,000 URLs per minute for each domain name.
         *   You can call this operation up to 30 times per second per account.
-        - After a refresh task is submitted and completed, your resources that are stored on CDN POPs are removed. When a POP receives a request your resources, the request is redirected to the origin server to retrieve the resources. Then, the resources are returned to the client and cached on the POP. If you frequently run refresh tasks, more requests will be redirected back to the origin server for resources, which result in high bandwidth costs and undue pressure on the origin server.
-        - A refresh task takes effect five to six minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
-        - If you want to use Resource Access Management (RAM) users to refresh or prefetch resources, you must acquire the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/to-grant-the-ram-users-refresh-and-preheating-permissions).
+        # Precautions
+        *   After a refresh task is submitted and completed, your resources that are stored on DCDN POPs are removed. When a POP receives a request to your resources, the request is redirected to the origin server to retrieve the resources. Then, the resources are returned to the client and cached on the POP. If you frequently run refresh tasks, more requests will be redirected back to the origin server for resources, which result in high bandwidth costs and undue pressure on the origin server.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
+        *   If you want to use RAM users to refresh or prefetch resources, you need to obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
         
         @param request: RefreshDcdnObjectCachesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RefreshDcdnObjectCachesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -17878,23 +17604,25 @@
 
     async def refresh_dcdn_object_caches_with_options_async(
         self,
         request: dcdn_20180115_models.RefreshDcdnObjectCachesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.RefreshDcdnObjectCachesResponse:
         """
-        Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests in which parameters are sent as a form.
+        #
+        *   DCDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
-        *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to apply for an increased upper limit. Alibaba Cloud will review your application and then increase the quota accordingly.
+        *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. DCDN evaluates your application based on your workloads.
         *   You can specify up to 1,000 URLs or 100 directories that you want to refresh in each request.
-        *   You can refresh a maximum of 1,000 URLs per minute for each domain name.
+        *   You can refresh up to 1,000 URLs per minute for each domain name.
         *   You can call this operation up to 30 times per second per account.
-        - After a refresh task is submitted and completed, your resources that are stored on CDN POPs are removed. When a POP receives a request your resources, the request is redirected to the origin server to retrieve the resources. Then, the resources are returned to the client and cached on the POP. If you frequently run refresh tasks, more requests will be redirected back to the origin server for resources, which result in high bandwidth costs and undue pressure on the origin server.
-        - A refresh task takes effect five to six minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
-        - If you want to use Resource Access Management (RAM) users to refresh or prefetch resources, you must acquire the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/to-grant-the-ram-users-refresh-and-preheating-permissions).
+        # Precautions
+        *   After a refresh task is submitted and completed, your resources that are stored on DCDN POPs are removed. When a POP receives a request to your resources, the request is redirected to the origin server to retrieve the resources. Then, the resources are returned to the client and cached on the POP. If you frequently run refresh tasks, more requests will be redirected back to the origin server for resources, which result in high bandwidth costs and undue pressure on the origin server.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
+        *   If you want to use RAM users to refresh or prefetch resources, you need to obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
         
         @param request: RefreshDcdnObjectCachesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RefreshDcdnObjectCachesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -17926,58 +17654,62 @@
         )
 
     def refresh_dcdn_object_caches(
         self,
         request: dcdn_20180115_models.RefreshDcdnObjectCachesRequest,
     ) -> dcdn_20180115_models.RefreshDcdnObjectCachesResponse:
         """
-        Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests in which parameters are sent as a form.
+        #
+        *   DCDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
-        *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to apply for an increased upper limit. Alibaba Cloud will review your application and then increase the quota accordingly.
+        *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. DCDN evaluates your application based on your workloads.
         *   You can specify up to 1,000 URLs or 100 directories that you want to refresh in each request.
-        *   You can refresh a maximum of 1,000 URLs per minute for each domain name.
+        *   You can refresh up to 1,000 URLs per minute for each domain name.
         *   You can call this operation up to 30 times per second per account.
-        - After a refresh task is submitted and completed, your resources that are stored on CDN POPs are removed. When a POP receives a request your resources, the request is redirected to the origin server to retrieve the resources. Then, the resources are returned to the client and cached on the POP. If you frequently run refresh tasks, more requests will be redirected back to the origin server for resources, which result in high bandwidth costs and undue pressure on the origin server.
-        - A refresh task takes effect five to six minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
-        - If you want to use Resource Access Management (RAM) users to refresh or prefetch resources, you must acquire the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/to-grant-the-ram-users-refresh-and-preheating-permissions).
+        # Precautions
+        *   After a refresh task is submitted and completed, your resources that are stored on DCDN POPs are removed. When a POP receives a request to your resources, the request is redirected to the origin server to retrieve the resources. Then, the resources are returned to the client and cached on the POP. If you frequently run refresh tasks, more requests will be redirected back to the origin server for resources, which result in high bandwidth costs and undue pressure on the origin server.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
+        *   If you want to use RAM users to refresh or prefetch resources, you need to obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
         
         @param request: RefreshDcdnObjectCachesRequest
         @return: RefreshDcdnObjectCachesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.refresh_dcdn_object_caches_with_options(request, runtime)
 
     async def refresh_dcdn_object_caches_async(
         self,
         request: dcdn_20180115_models.RefreshDcdnObjectCachesRequest,
     ) -> dcdn_20180115_models.RefreshDcdnObjectCachesResponse:
         """
-        Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests in which parameters are sent as a form.
+        #
+        *   DCDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
-        *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to apply for an increased upper limit. Alibaba Cloud will review your application and then increase the quota accordingly.
+        *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. DCDN evaluates your application based on your workloads.
         *   You can specify up to 1,000 URLs or 100 directories that you want to refresh in each request.
-        *   You can refresh a maximum of 1,000 URLs per minute for each domain name.
+        *   You can refresh up to 1,000 URLs per minute for each domain name.
         *   You can call this operation up to 30 times per second per account.
-        - After a refresh task is submitted and completed, your resources that are stored on CDN POPs are removed. When a POP receives a request your resources, the request is redirected to the origin server to retrieve the resources. Then, the resources are returned to the client and cached on the POP. If you frequently run refresh tasks, more requests will be redirected back to the origin server for resources, which result in high bandwidth costs and undue pressure on the origin server.
-        - A refresh task takes effect five to six minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
-        - If you want to use Resource Access Management (RAM) users to refresh or prefetch resources, you must acquire the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/to-grant-the-ram-users-refresh-and-preheating-permissions).
+        # Precautions
+        *   After a refresh task is submitted and completed, your resources that are stored on DCDN POPs are removed. When a POP receives a request to your resources, the request is redirected to the origin server to retrieve the resources. Then, the resources are returned to the client and cached on the POP. If you frequently run refresh tasks, more requests will be redirected back to the origin server for resources, which result in high bandwidth costs and undue pressure on the origin server.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
+        *   If you want to use RAM users to refresh or prefetch resources, you need to obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~445051~~).
         
         @param request: RefreshDcdnObjectCachesRequest
         @return: RefreshDcdnObjectCachesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.refresh_dcdn_object_caches_with_options_async(request, runtime)
 
     def rollback_dcdn_staging_config_with_options(
         self,
         request: dcdn_20180115_models.RollbackDcdnStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.RollbackDcdnStagingConfigResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The ID of the request.
         
         @param request: RollbackDcdnStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RollbackDcdnStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -18004,15 +17736,15 @@
 
     async def rollback_dcdn_staging_config_with_options_async(
         self,
         request: dcdn_20180115_models.RollbackDcdnStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.RollbackDcdnStagingConfigResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The ID of the request.
         
         @param request: RollbackDcdnStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RollbackDcdnStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -18038,42 +17770,42 @@
         )
 
     def rollback_dcdn_staging_config(
         self,
         request: dcdn_20180115_models.RollbackDcdnStagingConfigRequest,
     ) -> dcdn_20180115_models.RollbackDcdnStagingConfigResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The ID of the request.
         
         @param request: RollbackDcdnStagingConfigRequest
         @return: RollbackDcdnStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.rollback_dcdn_staging_config_with_options(request, runtime)
 
     async def rollback_dcdn_staging_config_async(
         self,
         request: dcdn_20180115_models.RollbackDcdnStagingConfigRequest,
     ) -> dcdn_20180115_models.RollbackDcdnStagingConfigResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The ID of the request.
         
         @param request: RollbackDcdnStagingConfigRequest
         @return: RollbackDcdnStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.rollback_dcdn_staging_config_with_options_async(request, runtime)
 
     def set_dcdn_domain_certificate_with_options(
         self,
         request: dcdn_20180115_models.SetDcdnDomainCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.SetDcdnDomainCertificateResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The name of the certificate.
         
         @param request: SetDcdnDomainCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetDcdnDomainCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -18118,15 +17850,15 @@
 
     async def set_dcdn_domain_certificate_with_options_async(
         self,
         request: dcdn_20180115_models.SetDcdnDomainCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.SetDcdnDomainCertificateResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The name of the certificate.
         
         @param request: SetDcdnDomainCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetDcdnDomainCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -18170,28 +17902,28 @@
         )
 
     def set_dcdn_domain_certificate(
         self,
         request: dcdn_20180115_models.SetDcdnDomainCertificateRequest,
     ) -> dcdn_20180115_models.SetDcdnDomainCertificateResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The name of the certificate.
         
         @param request: SetDcdnDomainCertificateRequest
         @return: SetDcdnDomainCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_dcdn_domain_certificate_with_options(request, runtime)
 
     async def set_dcdn_domain_certificate_async(
         self,
         request: dcdn_20180115_models.SetDcdnDomainCertificateRequest,
     ) -> dcdn_20180115_models.SetDcdnDomainCertificateResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        The name of the certificate.
         
         @param request: SetDcdnDomainCertificateRequest
         @return: SetDcdnDomainCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_dcdn_domain_certificate_with_options_async(request, runtime)
 
@@ -18409,15 +18141,15 @@
 
     def set_dcdn_user_config_with_options(
         self,
         request: dcdn_20180115_models.SetDcdnUserConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.SetDcdnUserConfigResponse:
         """
-        >  You can call this operation up to 30 times per second.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetDcdnUserConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetDcdnUserConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -18452,15 +18184,15 @@
 
     async def set_dcdn_user_config_with_options_async(
         self,
         request: dcdn_20180115_models.SetDcdnUserConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.SetDcdnUserConfigResponse:
         """
-        >  You can call this operation up to 30 times per second.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetDcdnUserConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetDcdnUserConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -18494,28 +18226,28 @@
         )
 
     def set_dcdn_user_config(
         self,
         request: dcdn_20180115_models.SetDcdnUserConfigRequest,
     ) -> dcdn_20180115_models.SetDcdnUserConfigResponse:
         """
-        >  You can call this operation up to 30 times per second.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetDcdnUserConfigRequest
         @return: SetDcdnUserConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_dcdn_user_config_with_options(request, runtime)
 
     async def set_dcdn_user_config_async(
         self,
         request: dcdn_20180115_models.SetDcdnUserConfigRequest,
     ) -> dcdn_20180115_models.SetDcdnUserConfigResponse:
         """
-        >  You can call this operation up to 30 times per second.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetDcdnUserConfigRequest
         @return: SetDcdnUserConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_dcdn_user_config_with_options_async(request, runtime)
 
@@ -18633,17 +18365,18 @@
 
     def start_dcdn_domain_with_options(
         self,
         request: dcdn_20180115_models.StartDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.StartDcdnDomainResponse:
         """
-        >
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *\
+        ****\
+        *\
+        *\
         
         @param request: StartDcdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartDcdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -18674,17 +18407,18 @@
 
     async def start_dcdn_domain_with_options_async(
         self,
         request: dcdn_20180115_models.StartDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.StartDcdnDomainResponse:
         """
-        >
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *\
+        ****\
+        *\
+        *\
         
         @param request: StartDcdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartDcdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -18714,53 +18448,46 @@
         )
 
     def start_dcdn_domain(
         self,
         request: dcdn_20180115_models.StartDcdnDomainRequest,
     ) -> dcdn_20180115_models.StartDcdnDomainResponse:
         """
-        >
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *\
+        ****\
+        *\
+        *\
         
         @param request: StartDcdnDomainRequest
         @return: StartDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.start_dcdn_domain_with_options(request, runtime)
 
     async def start_dcdn_domain_async(
         self,
         request: dcdn_20180115_models.StartDcdnDomainRequest,
     ) -> dcdn_20180115_models.StartDcdnDomainResponse:
         """
-        >
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *\
+        ****\
+        *\
+        *\
         
         @param request: StartDcdnDomainRequest
         @return: StartDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.start_dcdn_domain_with_options_async(request, runtime)
 
     def start_dcdn_ipa_domain_with_options(
         self,
         request: dcdn_20180115_models.StartDcdnIpaDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.StartDcdnIpaDomainResponse:
-        """
-        >
-        *   The maximum number of times that users can call this operation per second is 20.
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        
-        @param request: StartDcdnIpaDomainRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StartDcdnIpaDomainResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.security_token):
@@ -18785,23 +18512,14 @@
         )
 
     async def start_dcdn_ipa_domain_with_options_async(
         self,
         request: dcdn_20180115_models.StartDcdnIpaDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.StartDcdnIpaDomainResponse:
-        """
-        >
-        *   The maximum number of times that users can call this operation per second is 20.
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        
-        @param request: StartDcdnIpaDomainRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StartDcdnIpaDomainResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.security_token):
@@ -18825,37 +18543,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_dcdn_ipa_domain(
         self,
         request: dcdn_20180115_models.StartDcdnIpaDomainRequest,
     ) -> dcdn_20180115_models.StartDcdnIpaDomainResponse:
-        """
-        >
-        *   The maximum number of times that users can call this operation per second is 20.
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        
-        @param request: StartDcdnIpaDomainRequest
-        @return: StartDcdnIpaDomainResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.start_dcdn_ipa_domain_with_options(request, runtime)
 
     async def start_dcdn_ipa_domain_async(
         self,
         request: dcdn_20180115_models.StartDcdnIpaDomainRequest,
     ) -> dcdn_20180115_models.StartDcdnIpaDomainResponse:
-        """
-        >
-        *   The maximum number of times that users can call this operation per second is 20.
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        
-        @param request: StartDcdnIpaDomainRequest
-        @return: StartDcdnIpaDomainResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.start_dcdn_ipa_domain_with_options_async(request, runtime)
 
     def stop_dcdn_domain_with_options(
         self,
         request: dcdn_20180115_models.StopDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
@@ -19649,15 +19351,15 @@
 
     def update_dcdn_slsrealtime_log_delivery_with_options(
         self,
         request: dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UpdateDcdnSLSRealtimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDcdnSLSRealtimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -19696,15 +19398,15 @@
 
     async def update_dcdn_slsrealtime_log_delivery_with_options_async(
         self,
         request: dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UpdateDcdnSLSRealtimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDcdnSLSRealtimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -19742,42 +19444,42 @@
         )
 
     def update_dcdn_slsrealtime_log_delivery(
         self,
         request: dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryRequest,
     ) -> dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UpdateDcdnSLSRealtimeLogDeliveryRequest
         @return: UpdateDcdnSLSRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_dcdn_slsrealtime_log_delivery_with_options(request, runtime)
 
     async def update_dcdn_slsrealtime_log_delivery_async(
         self,
         request: dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryRequest,
     ) -> dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UpdateDcdnSLSRealtimeLogDeliveryRequest
         @return: UpdateDcdnSLSRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_dcdn_slsrealtime_log_delivery_with_options_async(request, runtime)
 
     def update_dcdn_sub_task_with_options(
         self,
         request: dcdn_20180115_models.UpdateDcdnSubTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.UpdateDcdnSubTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        The ID of the request.
         
         @param request: UpdateDcdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDcdnSubTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -19810,15 +19512,15 @@
 
     async def update_dcdn_sub_task_with_options_async(
         self,
         request: dcdn_20180115_models.UpdateDcdnSubTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.UpdateDcdnSubTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        The ID of the request.
         
         @param request: UpdateDcdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDcdnSubTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -19850,42 +19552,42 @@
         )
 
     def update_dcdn_sub_task(
         self,
         request: dcdn_20180115_models.UpdateDcdnSubTaskRequest,
     ) -> dcdn_20180115_models.UpdateDcdnSubTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        The ID of the request.
         
         @param request: UpdateDcdnSubTaskRequest
         @return: UpdateDcdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_dcdn_sub_task_with_options(request, runtime)
 
     async def update_dcdn_sub_task_async(
         self,
         request: dcdn_20180115_models.UpdateDcdnSubTaskRequest,
     ) -> dcdn_20180115_models.UpdateDcdnSubTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        The ID of the request.
         
         @param request: UpdateDcdnSubTaskRequest
         @return: UpdateDcdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_dcdn_sub_task_with_options_async(request, runtime)
 
     def update_dcdn_user_real_time_delivery_field_with_options(
         self,
         request: dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UpdateDcdnUserRealTimeDeliveryFieldRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDcdnUserRealTimeDeliveryFieldResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -19910,15 +19612,15 @@
 
     async def update_dcdn_user_real_time_delivery_field_with_options_async(
         self,
         request: dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UpdateDcdnUserRealTimeDeliveryFieldRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDcdnUserRealTimeDeliveryFieldResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -19942,28 +19644,28 @@
         )
 
     def update_dcdn_user_real_time_delivery_field(
         self,
         request: dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldRequest,
     ) -> dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UpdateDcdnUserRealTimeDeliveryFieldRequest
         @return: UpdateDcdnUserRealTimeDeliveryFieldResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_dcdn_user_real_time_delivery_field_with_options(request, runtime)
 
     async def update_dcdn_user_real_time_delivery_field_async(
         self,
         request: dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldRequest,
     ) -> dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UpdateDcdnUserRealTimeDeliveryFieldRequest
         @return: UpdateDcdnUserRealTimeDeliveryFieldResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_dcdn_user_real_time_delivery_field_with_options_async(request, runtime)
```

### Comparing `alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115/models.py` & `alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,41 +225,43 @@
         protocol: str = None,
         resource_group_id: str = None,
         scope: str = None,
         security_token: str = None,
         sources: str = None,
         top_level_domain: str = None,
     ):
-        # The URL that is used to check the accessibility of the origin server.
+        # The URL that is used for health checks.
         self.check_url = check_url
         # The domain name to be added to IPA.
         # 
         # A wildcard domain that starts with a period (.) is supported, such as .example.com.
         self.domain_name = domain_name
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The protocol. Valid values:
         # 
         # *   **udp**\
         # *   **tcp**\
         # 
-        # >  Example: `{"protocol":"udp"}`.
+        # **\
+        # 
+        # **Description** For example: `{"protocol":"udp"}`.
         self.protocol = protocol
         # The ID of the resource group. If you do not specify a value for this parameter, the system automatically assigns the ID of the default resource group.
         self.resource_group_id = resource_group_id
-        # The acceleration region. Valid values:
+        # The acceleration region. Default value: domestic. Valid values:
         # 
         # *   **domestic**: Chinese mainland
-        # *   **overseas**: global (excluding the Chinese mainland)
+        # *   **overseas**: outside the Chinese mainland
         # *   **global**: global
         self.scope = scope
         self.security_token = security_token
         # The information about the addresses of origin servers.
         self.sources = sources
-        # The top-level domain name.
+        # The top-level domain.
         self.top_level_domain = top_level_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -395,32 +397,55 @@
         owner_id: int = None,
         resource_group_id: str = None,
         scope: str = None,
         security_token: str = None,
         sources: str = None,
         top_level_domain: str = None,
     ):
-        # The URL that is used to check whether the origin server can be accessed.
+        # The following table describes the fields in the Sources parameter.
+        # 
+        # | Field | Type | Required | Description |
+        # | ----- | ---- | -------- | ----------- |
+        # | type | String | Yes | The type of the origin server. Valid values: **ipaddr**: the IP address  
+        # 
+        # **domain**: the domain name  
+        # 
+        # **oss**: the endpoint of an Object Storage Service (OSS) bucket  
+        # 
+        # **fc_domain**: the domain name of Function Compute |
+        # | content | String | Yes | The address of the origin server. You can specify an IP address or a domain name. |
+        # | port | Integer | No | The port. Valid values: **80**: the default port  
+        # 
+        # **443**: the HTTPS port  
+        # 
+        # A custom port |
+        # | priority | String | No | The priority of the origin server if multiple origin servers are specified. Default value: 20. Valid values: **20**: the primary origin server  
+        # 
+        # **30**: the secondary origin server |
+        # | weight | String | No | The weight of the origin server if multiple origin servers are specified. Valid values: 0 to 100. Default value: 10. |
         self.check_url = check_url
-        # You can add up to 50 domain names to DCDN for each of your Alibaba Cloud account. Separate multiple domain names with commas (,).
+        # The top-level domain name.
         self.domain_name = domain_name
         self.owner_account = owner_account
         self.owner_id = owner_id
-        # The ID of the resource group. If you do not specify a value for this parameter, the system automatically assigns the ID of the default resource group.
+        # The ID of the request.
         self.resource_group_id = resource_group_id
-        # The accelerated region. Default value: domestic. Valid values:
-        # 
-        # *   domestic: Chinese mainland
-        # *   overseas: global (excluding the Chinese mainland)
-        # *   global: global
+        # Adds one or more domain names to Dynamic Route for CDN (DCDN).
         self.scope = scope
         self.security_token = security_token
-        # The information about the addresses of origin servers.
+        # **Prerequisites**:
+        # 
+        # *   The [DCDN service is activated](~~64926~~).
+        # *   Internet Content Provider (ICP) filing is complete for the accelerated domain names.
+        # 
+        # > 
+        # *   If the content of the origin server is not stored on Alibaba Cloud, the content must be reviewed. After you submit the request, the review is complete by the end of the following business day.
+        # *   The maximum number of domain names configured at a time is 50.
+        # *   The maximum number of times that each user can call this operation per second is 30.
         self.sources = sources
-        # The top-level domain name.
         self.top_level_domain = top_level_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -472,15 +497,14 @@
 
 
 class BatchAddDcdnDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -545,17 +569,1050 @@
 
 class BatchCreateDcdnWafRulesRequest(TeaModel):
     def __init__(
         self,
         policy_id: int = None,
         rule_configs: str = None,
     ):
-        # The ID of the protection policy.
-        self.policy_id = policy_id
         # The configurations of the protection rule.
+        self.policy_id = policy_id
+        # ## Description of the RuleConfigs parameter
+        # 
+        # - RuleConfigs is a list slice, in which each struct represents a rule.
+        # - The fields in the RuleConfigs parameter vary based on the type of the protection policy whose ID is specified by the PolicyId parameter.
+        # 
+        # 
+        # ## Scenario 1:web RegEx protection (waf_group)
+        # 
+        # | Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | status | String | No | on | Specifies whether to enable the protection rule. Valid values: on and off. Default value: on. |
+        # | action | String | Yes | block | Specifies the action of the rule. Valid values: block and monitor. |
+        # Sample code for waf_group
+        # 
+        # ```
+        # // You can configure only one rule for a protection policy of the waf_group type. 
+        # [
+        #   {
+        #     "status": "on",
+        #     "action": "block"
+        #   }
+        # ]
+        # ```
+        # 
+        # ## Scenario 2: custom rules (custom_acl)
+        # 
+        # | Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | name | string | Yes | acl_1 | The name of the protection rule. The name can be up to 64 characters in length and can contain letters, digits, and underscores (_). |
+        # | status | string | No | on | Valid values: on and off. Default value: on. |
+        # | conditions | Condition | Yes | [ {"key": "URI", "subKey": "","opValue": "contain",  "values": "/login.php" }] | The trigger condition. For more information, see **Table 1 Fields in the Conditions parameter**. |
+        # | ccStatus | string | Yes | off | Specifies whether to enable rate limiting. Valid values: on and off. |
+        # | rateLimit | RateLimit | No | { "target": "Header", "subKey": "User-Agent", "interval": 5, "threshold": 2, "ttl": 1800} | The rules of rate limiting. If you set ccStatus to on, you must configure this parameter. For more information, see **Table 2 Fields in the rateLimit parameter**. |
+        # | effect | string | No | service | The effective scope of the rate limiting blacklist. If you set ccStatus to on, you must configure this parameter. Valid values: rule (takes effect for the current rule) and service (takes effect globally). |
+        # | action | string | Yes | deny | The action of the rule. Valid values: deny, js (JavaScript verification), and monitor. |
+        # Table 1 Fields in the Conditions parameter
+        # 
+        # | Field | Type | Required | Example | Description |
+        # | ----- | ---- | -------- | ------- | ----------- |
+        # | Key | string | Yes | Query String Parameter | The match field. For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # | subKey | string | No | action | The match subfield. For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # | opValue | String | Yes | eq | The logical symbol. For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # | values | String | No | js | The match content. Separate multiple values with commas (,). For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # Table 2 Fields in the rateLimit parameter
+        # 
+        # | Field | Type | Required | Example | Description |
+        # | ----- | ---- | -------- | ------- | ----------- |
+        # | target | string | Yes | Header | The statistical field of rate limiting. IP: calculates the frequency at which requests are sent from a specified IP address. Header: calculates the frequency of requests that contain the specified header. Query String Parameter: calculates the frequency of requests that contain the specified parameter. Cookie Name: calculates the frequency of requests that contain the specified cookie. Session: calculates the frequency of requests that are transmitted over a specified session. |
+        # | subKey | string | No | User-Agent | The subfield of the target field. If you set target to Header, Query String Parameter, or Cookie Name, you must configure subKey. |
+        # | Interval | Integer | Yes | 5 | The statistical interval. Valid values: 5 to 1800. Unit: seconds. |
+        # | threshold | Integer | Yes | 2 | The trigger threshold of rate limiting. Valid values: 2 to 500000. Unit: requests. |
+        # | ttl | Integer | Yes | 1800 | The validity period of the blacklist. Valid values: 60 to 86400. Unit: seconds. |
+        # | status | RateLimitStatus | No | {"code": "404", "ratio": 10} | The information about the HTTP status code. For more information, see **Table 3 Fields in the RateLimitStatus parameter**. |
+        # Table 3 Fields in the RateLimitStatus parameter
+        # 
+        # | Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | codet | string | Yes | 404 | The HTTP status code returned. |
+        # | ratio | Integer | No | 10 | The percentage of HTTP status codes. Valid values: 1 to 100. You can configure only one of the ratio and count fields. |
+        # | count | Integer | No | 10 | The number of times that the HTTP status code that was returned. Valid values: 2 to 50000. You can configure only one of the ratio and count fields. |
+        # Sample code for custom_acl
+        # 
+        # ```
+        # [
+        #   // Access control
+        #   {
+        #     "name": "acl_1",
+        #     "status": "off",
+        #     "conditions":
+        #     [
+        #       {
+        #         "key": "Query String Parameter",
+        #         "subKey": "action",
+        #         "opValue": "eq",
+        #         "values": "js"
+        #       }
+        #     ],
+        #     "ccStatus": "off",
+        #     "action": "js"
+        #   },
+        #   // Rate limiting
+        #   {
+        #     "name": "cc_1",
+        #     "status": "on",
+        #   	"conditions": 
+        #     [
+        #       {
+        #         "key": "URI",
+        #         "subKey": "",
+        #         "opValue": "contain",
+        #         "values": "/login.php"
+        #       },
+        #       {
+        #         "key": "IP",
+        #         "subKey": "",
+        #         "opValue": "ip-contain",
+        #         "values": "192.168.0.1/24"
+        #       }
+        #     ],
+        #     "ccStatus": "on",
+        #     "ratelimit":
+        #     {
+        #       "target": "Header",
+        #       "subKey": "User-Agent",
+        #       "interval": 5,
+        #       "threshold": 2,
+        #       "ttl": 1800,
+        #       "status":
+        #       {
+        #         "code": "404",
+        #         "ratio": 10
+        #       }
+        #     },
+        #     "effect": "service",
+        #     "action": "deny"
+        #   }
+        # ]
+        # ```
+        # 
+        # ## Scenario 3: whitelist (whitelist)
+        # 
+        # | Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | name | string | Yes | on | The name of the protection rule. The name can be up to 64 characters in length and can contain letters, digits, and underscores (_). |
+        # | status | string | No | on | Specifies whether to enable the protection rule. Default value: on. Valid values: on and off. off: disables the multiplexing feature for ports. |
+        # | conditions | Condition | Yes | [{ "key": "Http-Method","subKey": "","opValue": "match-one", "values": "GET,POST,DELETE" }] | The trigger condition of the rule. For more information, see **Table 1 Fields in the Conditions parameter**. |
+        # | tags | String | Yes | [ "waf_group",  "custom_acl"] | The types of the protection policies. |
+        # | regularTypes | String | No | [  [ "sqli", "xss","code_exec", "crlf", "lfilei",  "rfilei", "webshell","vvip", "other"] | The type of the regular expression. If the value of the tags field contains waf_group, you can specify this field. Valid values: ["sqli", "xss", "code_exec", "crlf", "lfilei", "rfilei", "webshell", "vvip", and "other"]. |
+        # | regularRules | String | No | [   "100001", "100002", "100003"] | The regular expression. If the value of the tags field contains waf_group, you can specify this field. You can configure only regularRules or regularTypes. The value must be a string that consists of six digits. |
+        # Sample code for whitelist:
+        # 
+        # ```
+        # [
+        #   // Skip all protection policies.
+        #   {
+        #     "name": "wl_all",
+        #     "status": "on",
+        #     "conditions":
+        #     [
+        #       {
+        #         "key": "Http-Method",
+        #         "subKey": "",
+        #         "opValue": "match-one",
+        #         "values": "GET,POST,DELETE"
+        #       }
+        #     ],
+        #     "tags":
+        #     [
+        #       "waf_group",
+        #       "custom_acl",
+        #       "ip_blacklist",
+        #       "region_block"
+        #     ]
+        #   },
+        #   // Skip the ID of the rule that is specified in waf_group.
+        #   {
+        #     "name": "wl_waf_id",
+        #     "status": "off",
+        #     "conditions":
+        #     [
+        #       {
+        #         "key": "Cookie Name",
+        #         "subKey": "cdn-sec",
+        #         "opValue": "prefix-match",
+        #         "values": "a7sdsa9dsa8d8sa"
+        #       },
+        #       {
+        #         "key": "Referer",
+        #         "subKey": "",
+        #         "opValue": "none",
+        #         "values": ""
+        #       }
+        #     ],
+        #     "tags":
+        #     [
+        #       "waf_group"
+        #     ],
+        #     "regularRules":
+        #     [
+        #       "100001",
+        #       "100002",
+        #       "100003"
+        #     ]
+        #   },
+        #   {
+        #   // Skip the type of rules that is specified in waf_group.
+        #     "name": "wl_waf_type",
+        #     "status": "on",
+        #     "conditions":
+        #     [
+        #       {
+        #         "key": "Query String",
+        #         "subKey": "",
+        #         "opValue": "exists",
+        #         "values": ""
+        #       }
+        #     ],
+        #     "tags":
+        #     [
+        #       "waf_group"
+        #     ],
+        #     "regularTypes":
+        #     [
+        #       "sqli",
+        #       "xss",
+        #       "code_exec",
+        #       "crlf",
+        #       "lfilei",
+        #       "rfilei",
+        #       "webshell",
+        #       "vvip",
+        #       "other"
+        #     ]
+        #   },
+        #   // Skip custom rules.
+        #   {
+        #     "name": "wl_custom_acl",
+        #     "status": "on",
+        #     "conditions":
+        #     [
+        #       {
+        #         "key": "Http-Method",
+        #         "subKey": "",
+        #         "opValue": "match-one",
+        #         "values": "GET,POST,DELETE"
+        #       }
+        #     ],
+        #     "tags":
+        #     [
+        #       "custom_acl"
+        #     ]
+        #   },
+        #   // Skip IP addresses in the blacklist.
+        #   {
+        #     "name": "wl_ip_blacklist",
+        #     "status": "on",
+        #     "conditions":
+        #     [
+        #       {
+        #         "key": "Http-Method",
+        #         "subKey": "",
+        #         "opValue": "match-one",
+        #         "values": "GET,POST,DELETE"
+        #       }
+        #     ],
+        #     "tags":
+        #     [
+        #       "ip_blacklist"
+        #     ]
+        #   },
+        #   // Skip the region blocking
+        #   {
+        #     "name": "wl_region_block",
+        #     "status": "on",
+        #     "conditions":
+        #     [
+        #       {
+        #         "key": "Http-Method",
+        #         "subKey": "",
+        #         "opValue": "match-one",
+        #         "values": "GET,POST,DELETE"
+        #       }
+        #     ],
+        #     "tags":
+        #     [
+        #       "region_block"
+        #     ]
+        #   }
+        # ]
+        # ```
+        # 
+        # ## Scenario 4:IP address blacklist (ip_blacklist)
+        # 
+        # | Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | name | string | Yes | ipblacklist | The name of the protection rule. The name can be up to 64 characters in length and can contain letters, digits, and underscores (_). |
+        # | status | string | No | on | Specifies whether to enable the protection rule. Valid values: on and off. Default value: on. |
+        # | remoteAddr | []String | Yes | ["192.168.0.1","10.10.10.10/24","::1","abcd::abcd","BCDE::BCDE"] | Filter by IP address. For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # | action | string | Yes | deny | The action of the rule. Valid values: deny and monitor. |
+        # Sample code for ipblacklist:
+        # 
+        # ```
+        # [
+        #     {
+        #     "name": "ipblacklist",
+        #     "status": "on",
+        #     "remoteAddr": ["192.168.0.1","10.10.10.10/24","::1","abcd::abcd","BCDE::BCDE"],
+        #     "action": "deny"
+        #   }
+        # ]
+        # ```
+        # 
+        # ## Protection scenario 5: region blocking (region_block)
+        # 
+        # | Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | status | string | No | on | Specifies whether to enable the protection rule. Valid values: on and off. Default value: on. |
+        # | cnRegionList | string | No | 110000,TW,MO | The blocked regions in the Chinese mainland, separated by commas (,). For more information about the regions that can be blocked, see [DescribeDcdnWafGeoInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/describe-dcdn-waf-geo-info). |
+        # | otherRegionList | string | No | JP,GB | Blocked regions outside the Chinese mainland, separated by commas (,). For more information about the regions that can be blocked, see [DescribeDcdnWafGeoInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/describe-dcdn-waf-geo-info). |
+        # | action | string | Yes | deny | The action of the rule. Valid values: deny and monitor. |
+        # >  You must specify at least one of the ProcessId or ProcessName parameters.  Sample code for region_block:
+        # 
+        # ```
+        # [
+        #     {
+        #     "status": "on",
+        #     "cnRegionList": "110000,TW,MO",
+        #     "otherRegionList": "JP,GB",
+        #     "action": "deny"
+        #   }
+        # ]
+        # ```
+        # 
+        # ## Scenario 6: Bot management (bot)
+        # 
+        # **Rule template**All rules have the four parameters in the following table. For more information, see the rule classification.  
+        # 
+        # | Parameter | Type | Required | Description |
+        # | --------- | ---- | -------- | ----------- |
+        # | type | String | Yes | The type of the rule. For more information, see the rule classification. |
+        # | status | String | Yes | The status of the rule. Valid values: on and off. |
+        # | config | TargetType | No | Rule configuration. For more information, see Rule classification. |
+        # | action | String | No | Rule actions. For more information, see Rule classification. |
+        # **Rule category 1: protection target type**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | target_type | The type of the rule. Set the value to target_type. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Set the value to on. |
+        # | config | TargetType | No | {"target":"app"} | The configuration of the rule. Format:
+        # 
+        # (Required) target: the type of the protection target. Valid values: web (web pages and browsers) and app (apps). |
+        # | action | String | No | Empty | The action of the rule, which is not involved here. Leave the value empty. |
+        # Configuration example of the protection target type:
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"target_type",
+        #     "status":"on",
+        #     "config":{"target":"app"},
+        #     "action":""
+        #   }
+        # ]
+        # ```
+        # **Rule classification 2: Web SDK integration**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | web_sdk | The type of the rule. Set the value to web_sdk. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Set the value to on. |
+        # | config | WebSdk | No | {"mode":"automatic","crossDomain":"example.com"} | The configuration of the rule. Format:
+        # 
+        # (Required) mode : the integration mode of the Web SDK. Valid values: automatic and manual.  
+        # 
+        # (Optional) crossDomain: cross-domain resource calling. This parameter takes effect only when the value of mode is automatic. |
+        # | action | String | No | Empty | The action of the rule, which is not involved here. Leave the value empty. |
+        # Configuration example of Web SDK integration:
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"web_sdk",
+        #     "status":"on",
+        #     "config":{"mode":"automatic","crossDomain":"example.com"},
+        #     "action":""
+        #   }
+        # ]
+        # ```
+        # **Rule classification 3: protection target characteristics**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | traffic_feature | The type of the rule. Set the value to traffic_feature. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Set the value to on. |
+        # | config | TrafficFeature | Yes | {"conditions":[{"key":"Header","subKey":"User-Agent","opValue":"contain","values":"Chrome"},{"key":"IP","subKey":"","opValue":"ip-contain","values":"192.168.0.1/24"}]} | The configuration of the rule. For more information, see **condition**. |
+        # | action | String | No | Empty | The action of the rule, which is not involved here. Leave the value empty. |
+        # **condition** (match condition) 
+        # 
+        # | Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | key | String | Yes | Header | The match field. For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # | subKey | String | No | User-Agent | The match subfield. For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # | opValue | String | Yes | contain | The operator. For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # | values | String | No | Chrome | The match content. Separate multiple values with commas (,). For more information, see [DescribeDcdnWafFilterInfo](https://www.alibabacloud.com/help/en/dynamic-route-for-cdn/latest/obtain-the-matching-conditions-of-custom-protection-rules). |
+        # Configuration example of protection target characteristics:
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"traffic_feature",
+        #     "status":"on",
+        #     "config":{"conditions":[{"key":"Header","subKey":"User-Agent","opValue":"contain","values":"Chrome"},{"key":"IP","subKey":"","opValue":"ip-contain","values":"192.168.0.1/24"}]},
+        #     "action":""
+        #   }
+        # ]
+        # ```
+        # **Rule classification 4: legitimate Bot management**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | intelligence_crawler | The type of the rule. Set the value to intelligence_crawler. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Set the value to on. |
+        # | config | IntelligenceCrawler | No | {"name":"intelligence_crawler_baidu"} | The configuration of the rule. For more information, see **name (spider whitelist)**. |
+        # | action | String | Yes | bypass | The action of the rule. Set the value to bypass. |
+        # **name (spider whitelist)**| Value | Description |
+        # | ----- | ----------- |
+        # | intelligence_crawler_all | Whitelist for authorized search engines, such as Google, Bing, Baidu, Sogou, 360, and Yandex. |
+        # | intelligence_crawler_baidu | Baidu spider whitelist |
+        # | intelligence_crawler_sogou | Sogou spider whitelist |
+        # | intelligence_crawler_360 | 360 spider whitelist |
+        # | intelligence_crawler_google | Google spider whitelist |
+        # | intelligence_crawler_bing | Bing spider whitelist |
+        # | intelligence_crawler_yandex | Yandex spider whitelist |
+        # Configuration example of legitimate Bot management:
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"intelligence_crawler",
+        #     "status":"on",
+        #     "config":{"name":"intelligence_crawler_baidu"},
+        #     "action":"bypass"
+        #   },
+        #   {
+        #     "type":"intelligence_crawler",
+        #     "status":"on",
+        #     "config":{"name":"intelligence_crawler_google"},
+        #     "action":"bypass"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 5: script-based Bot block (JavaScript)**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | js | The type of the rule. Set the value to js. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | Js | No | Empty | The configuration of the rule, which is not involved here. Leave the value empty. |
+        # | action | String | Yes | js | The action of the rule. Set the value to js (JavaScript verification). |
+        # Configuration example of script-based Bot block (JavaScript)
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"js",
+        #     "status":"on",
+        #     "config":{},
+        #     "action":"js"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 6: advanced Bot defense (dynamic token-based authentication)**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | sigchl | The type of the rule. Set the value to sigchl. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | Sigchl | No | {"sigchl":["sig","replay","driver"]} | The configuration of the rule. Format:
+        # 
+        # (Required) sigchl : signature-based verification for request data. Valid values: sig (signature verification exception),replay (signature timestamp exception), and driver(WebDriver attack). |
+        # | action | String | Yes | sigchl | The action of the rule. Set the value to sigchl (block). |
+        # Configuration example of advanced Bot defense (dynamic token-based authentication):
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"sigchl",
+        #     "status":"on",
+        #     "config":{"sigchl":["sig","replay","driver"]},
+        #     "action":"sigchl"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 7: intelligent protection**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | algorithm | The type of the rule. Set the value to algorithm. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | Algorithm | No | Empty | The configuration of the rule, which is not involved here. Leave the value empty. |
+        # | action | String | Yes | captcha | The action of the rule. Valid values: monitor and captcha. |
+        # Configuration example of intelligent protection:
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"algorithm",
+        #     "status":"on",
+        #     "config":{},
+        #     "action":"captcha"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 8: IP address throttling**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | custom_cc_ip | The type of the rule. Set the value to custom_cc_ip. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | CustomCcIp | Yes | {"interval":20,"target":"IP","threshold":50,"ttl":2800} | The configuration of the rule. For more information, see **Fields in the config parameter of IP address throttling**. |
+        # | action | String | Yes | monitor | The action of the rule. Valid values: deny, monitor, and captcha (only for web). |
+        # **Fields in the config parameter of IP address throttling**| Field | Type | Required | Example | Description |
+        # | ----- | ---- | -------- | ------- | ----------- |
+        # | target | String | Yes | IP | The statistical field of rate limiting. Set the value to IP. |
+        # | subKey | String | No | Empty | The subfield of the target field, which is not involved here. Leave the value empty. |
+        # | Interval | Integer | Yes | 20 | The statistical interval. Valid values: 5 to 1800. Unit: seconds. |
+        # | threshold | Integer | Yes | 50 | The trigger threshold of rate limiting. Valid values: 2 to 50000. Unit: calls. |
+        # | ttl | Integer | Yes | 2800 | The validity period of the blacklist. Valid values: 60 to 86400. Unit: seconds. |
+        # Configuration example of IP address throttling
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"custom_cc_ip",
+        #     "status":"on",
+        #     "config":{"interval":20,"target":"IP","threshold":50,"ttl":2800},
+        #     "action":"monitor"
+        #   },
+        #   {
+        #     "type":"custom_cc_ip",
+        #     "status":"on",
+        #     "config":{"interval":10,"target":"IP","threshold":30,"ttl":1800},
+        #     "action":"monitor"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 9: device throttling**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | custom_cc_dev | The type of the rule. Set the value to custom_cc_dev. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | CustomCcDev | Yes | {"interval":20,"target":"Header","subKey":"aliwaf_wxbb_umid","threshold":50,"ttl":2800} | The configuration of the rule. For more information, see **Fields in the config parameter of device throttling**. |
+        # | action | String | Yes | monitor | The action of the rule. Valid values: deny and monitor. |
+        # **Fields in the config parameter of device throttling**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | target | String | Yes | Header | The statistical field of rate limiting. Set the value to Header. |
+        # | subKey | String | No | aliwaf_wxbb_umid | The subfield of the target field. Set the value to aliwaf_wxbb_umid. |
+        # | Interval | Integer | Yes | 20 | The statistical interval. Valid values: 5 to 1800. Unit: seconds. |
+        # | threshold | Integer | Yes | 50 | The trigger threshold of rate limiting. Valid values: 2 to 50000. Unit: calls. |
+        # | ttl | Integer | Yes | 2800 | The validity period of the blacklist. Valid values: 60 to 86400. Unit: seconds. |
+        # Configuration example of device throttling
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"custom_cc_dev",
+        #     "status":"on",
+        #     "config":{"interval":20,"target":"Header","subKey":"aliwaf_wxbb_umid","threshold":50,"ttl":2800},
+        #     "action":"monitor"
+        #   },
+        #   {
+        #     "type":"custom_cc_dev",
+        #     "status":"on",
+        #     "config":{"interval":20,"target":"Header","subKey":"aliwaf_wxbb_umid","threshold":50,"ttl":2800},
+        #     "action":"deny"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 10: custom session-based throttling**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | custom_cc | The type of the rule. Set the value to custom_cc. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | CustomCcIp | Yes | {"interval":10,"target":"Query String Parameter","subKey":"arg","threshold":30,"ttl":1800} | The configuration of the rule. For more information, see **Fields in the config parameter of custom session-based throttling**. |
+        # | action | String | Yes | monitor | The action of the rule. Valid values: deny, monitor, and captcha (only for web). |
+        # **Fields in the config parameter of custom session-based throttling**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | target | String | Yes | Query String Parameter | The statistical fields for frequency control. Valid values: Header, calculates the frequency of requests that contain the specified header; Query String Parameter, calculates the frequency of requests that contain the specified parameter; Cookie Name, calculates the frequency of requests that contain the specified cookie; and Session, calculates the frequency of requests that are transmitted over a specified session. |
+        # | subKey | String | No | arg | The subfield of the target field. You can customize the value. |
+        # | Interval | Integer | Yes | 10 | The statistical interval. Valid values: 5 to 1800. Unit: seconds. |
+        # | threshold | Integer | Yes | 30 | The trigger threshold of rate limiting. Valid values: 2 to 50000. Unit: calls. |
+        # | ttl | Integer | Yes | 2800 | The validity period of the blacklist. Valid values: 60 to 86400. Unit: seconds. |
+        # Configuration example of custom session-based throttling
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"custom_cc",
+        #     "status":"on",
+        #     "config":{"interval":10,"target":"Query String Parameter","subKey":"arg","threshold":30,"ttl":1800},
+        #     "action":"deny"
+        #   },
+        #   {
+        #     "type":"custom_cc",
+        #     "status":"on",
+        #     "config":{"interval":10,"target":"Query String Parameter","subKey":"arg","threshold":30,"ttl":1800},
+        #     "action":"captcha"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 11: Bot threat intelligence library**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | intelligence | The type of the rule. Set the value to intelligence. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | Intelligence | No | Empty | The configuration of the rule, which is not involved here. Leave the value empty. |
+        # | action | String | Yes | captcha | The action of the rule. Valid values: monitor and captcha. |
+        # Configuration example of bot threat intelligence library:
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"intelligence",
+        #     "status":"on",
+        #     "config":{},
+        #     "action":"captcha"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 12: data center blacklist**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | intelligence_idc | The type of the rule. Set the value to intelligence_idc. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | IntelligenceIdc | Yes | {"name":"intelligence_idc_alibaba"} | The configuration of the rule. For more information, see **Values of name**. |
+        # | action | String | Yes | captcha | The action of the rule. Valid values: deny, monitor, and captcha. |
+        # **Values of name**| Value | Description |
+        # | ----- | ----------- |
+        # | intelligence_idc_alibaba | Data center IP address library-Alibaba Cloud |
+        # | intelligence_idc_tencent | Data center IP address library-Tencent Cloud |
+        # | intelligence_idc_mtyun | Data center IP address library-Meituan Open Services |
+        # | intelligence_idc_vnet | Data center IP address library-21Vianet |
+        # | intelligence_idc_other | Data center IP address library-Others |
+        # Configuration example of data center blacklist
+        # 
+        # ```
+        # [
+        #   {
+        #     "type":"intelligence_idc",
+        #     "status":"on",
+        #     "config":{"name":"intelligence_idc_alibaba"},
+        #     "action":"captcha"
+        #   },
+        #   {
+        #     "type":"intelligence_idc",
+        #     "status":"on",
+        #     "config":{"name":"intelligence_idc_tencent"},
+        #     "action":"captcha"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 13: fake spider blocking**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | intelligence_fake_crawler | The type of the rule. Set the value to intelligence_fake_crawler. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Valid values: on and off. |
+        # | config | IntelligenceFakeCrawler | No | Empty | The configuration of the rule, which is not involved here. Leave the value empty. |
+        # | action | String | Yes | deny | The action of the rule. Set the value to deny. |
+        # Configuration example of fake spider blocking:
+        # 
+        # ```
+        # [
+        #   {
+        #     "type": "intelligence_fake_crawler",
+        #     "status": "on",
+        #     "config":{},
+        #     "action": "deny"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 14: Bot characteristic detection**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | app_sdk | The type of the rule. Set the value to app_sdk. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Set the value to on. |
+        # | config | AppSdk | Yes | {"featureAbnormal":["simulator","proxy","root","debugged","hook","virtual","antiReplay","signInvalid"],"customSignStatus":"on","customSign":{"key":"header","value":"ua"}} | The configuration of the rule. For more information, see **Fields in the config parameter of Bot characteristic detection**. |
+        # | action | String | Yes | monitor | The action of the rule. Valid values: deny and monitor. |
+        # **Fields in the config parameter of Bot characteristic detection**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | featureAbnormal | []String | Yes | simulator | signInvalid: The app signature is invalid. 
+        # 
+        # antiReplay: The signature expired. 
+        # 
+        # simulator: Uses a simulator.
+        # 
+        # proxy: Uses a proxy.
+        # 
+        # root: Root device.
+        # 
+        # debugged: The debugging mode. 
+        # 
+        # hook: The app is hooked. 
+        # 
+        # virtual : Multiboxing. |
+        # | customSignStatus | String | No | on | Specifies whether to enable the custom signature field. Valid values: on and off. |
+        # | customSign | CustomSign | No | {"key":"header","value":"ua"} | The custom signature field. Format:  
+        # 
+        #   (Required) key : the name of the field. Valid values: header, arg, and cookie.  
+        # 
+        #  (Required) value: the value of the field. |
+        # Configuration example of Bot characteristic detection:
+        # 
+        # ```
+        # [
+        #   {
+        #     "type": "app_sdk",
+        #     "status": "on",
+        #     "config": {"featureAbnormal":["simulator","proxy","root","debugged","hook","virtual","antiReplay","signInvalid"],"customSignStatus":"on","customSign":{"key":"header","value":"ua"}},
+        #     "action": "monitor"
+        #   }
+        # ]
+        # ```
+        # **Rule classification 15: advanced protection (secondary packaging detection)**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | type | String | Yes | app_package | The type of the rule. Set the value to app_package. |
+        # | status | String | Yes | on | Specifies whether to enable the rule. Set the value to on. |
+        # | config | AppPackage | No | {"packageSigns":[{"name":"aaaaa","sign":"bbbb"},{"name":"cccc","sign":"dddd"}]} | The configuration of the rule. For more information, see **Fields in the packageSigns parameter**. |
+        # | action | String | Yes | monitor | The action of the rule. Valid values: deny and monitor. |
+        # **Fields in the packageSigns parameter**| Parameter | Type | Required | Example | Description |
+        # | --------- | ---- | -------- | ------- | ----------- |
+        # | name | String | Yes | aaaaa | The valid package name. |
+        # | sign | String | No | bbbb | The signature of the package. |
+        # Configuration examples of advanced protection (secondary packaging detection):
+        # 
+        # ```
+        # [
+        #   {
+        #     "type": "app_package",
+        #     "status": "on",
+        #     "config": {"packageSigns":[{"name":"aaaaa","sign":"bbbb"},{"name":"cccc","sign":"dddd"}]},
+        #     "action": "deny"
+        #   }
+        # ]
+        # ```
+        # **Configuration example of Bot management and web page/browser protection**```
+        # [
+        #     {
+        #         "type": "target_type",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "target": "web"
+        #         },
+        #         "action": ""
+        #     },
+        #     {
+        #         "type": "web_sdk",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "mode": "automatic",
+        #             "crossDomain": "example.com"
+        #         },
+        #         "action": ""
+        #     },
+        #     {
+        #         "type": "traffic_feature",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "conditions":
+        #             [
+        #                 {
+        #                     "key": "Header",
+        #                     "subKey": "User-Agent",
+        #                     "opValue": "contain",
+        #                     "values": "Chrome"
+        #                 },
+        #                 {
+        #                     "key": "IP",
+        #                     "subKey": "",
+        #                     "opValue": "ip-contain",
+        #                     "values": "192.168.0.1/24"
+        #                 }
+        #             ]
+        #         },
+        #         "action": ""
+        #     },
+        #     {
+        #         "type": "intelligence_crawler",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "name": "intelligence_crawler_baidu"
+        #         },
+        #         "action": "bypass"
+        #     },
+        #     {
+        #         "type": "intelligence_crawler",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "name": "intelligence_crawler_google"
+        #         },
+        #         "action": "bypass"
+        #     },
+        #     {
+        #         "type": "js",
+        #         "status": "on",
+        #         "config":
+        #         {},
+        #         "action": "js"
+        #     },
+        #     {
+        #         "type": "sigchl",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "sigchl":
+        #             [
+        #                 "sig",
+        #                 "replay",
+        #                 "driver"
+        #             ]
+        #         },
+        #         "action": "sigchl"
+        #     },
+        #     {
+        #         "type": "algorithm",
+        #         "status": "on",
+        #         "config":
+        #         {},
+        #         "action": "captcha"
+        #     },
+        #     {
+        #         "type": "custom_cc_ip",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 20,
+        #             "target": "IP",
+        #             "threshold": 50,
+        #             "ttl": 2800
+        #         },
+        #         "action": "monitor"
+        #     },
+        #     {
+        #         "type": "custom_cc_ip",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 10,
+        #             "target": "IP",
+        #             "threshold": 30,
+        #             "ttl": 1800
+        #         },
+        #         "action": "monitor"
+        #     },
+        #     {
+        #         "type": "custom_cc",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 10,
+        #             "target": "Query String Parameter",
+        #             "subKey": "arg",
+        #             "threshold": 30,
+        #             "ttl": 1800
+        #         },
+        #         "action": "deny"
+        #     },
+        #     {
+        #         "type": "custom_cc",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 10,
+        #             "target": "Query String Parameter",
+        #             "subKey": "arg",
+        #             "threshold": 30,
+        #             "ttl": 1800
+        #         },
+        #         "action": "captcha"
+        #     },
+        #     {
+        #         "type": "intelligence",
+        #         "status": "on",
+        #         "config":
+        #         {},
+        #         "action": "captcha"
+        #     },
+        #     {
+        #         "type": "intelligence_idc",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "name": "intelligence_idc_alibaba"
+        #         },
+        #         "action": "captcha"
+        #     },
+        #     {
+        #         "type": "intelligence_idc",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "name": "intelligence_idc_tencent"
+        #         },
+        #         "action": "captcha"
+        #     },
+        #     {
+        #         "type": "intelligence_fake_crawler",
+        #         "status": "on",
+        #         "config":
+        #         {},
+        #         "action": "deny"
+        #     }
+        # ]
+        # ```
+        # **Configuration example of Bot management and app protection**```
+        # json
+        # [
+        #     {
+        #         "type": "target_type",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "target": "app"
+        #         },
+        #         "action": ""
+        #     },
+        #     {
+        #         "type": "traffic_feature",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "conditions":
+        #             [
+        #                 {
+        #                     "key": "Header",
+        #                     "subKey": "User-Agent",
+        #                     "opValue": "contain",
+        #                     "values": "Chrome"
+        #                 },
+        #                 {
+        #                     "key": "IP",
+        #                     "subKey": "",
+        #                     "opValue": "ip-contain",
+        #                     "values": "192.168.0.1/24"
+        #                 }
+        #             ]
+        #         },
+        #         "action": ""
+        #     },
+        #     {
+        #         "type": "custom_cc_ip",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 20,
+        #             "target": "IP",
+        #             "threshold": 50,
+        #             "ttl": 2800
+        #         },
+        #         "action": "monitor"
+        #     },
+        #     {
+        #         "type": "custom_cc_ip",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 10,
+        #             "target": "IP",
+        #             "threshold": 30,
+        #             "ttl": 1800
+        #         },
+        #         "action": "monitor"
+        #     },
+        #     {
+        #         "type": "custom_cc_dev",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 20,
+        #             "target": "Header",
+        #             "subKey": "aliwaf_wxbb_umid",
+        #             "threshold": 50,
+        #             "ttl": 2800
+        #         },
+        #         "action": "monitor"
+        #     },
+        #     {
+        #         "type": "custom_cc_dev",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 20,
+        #             "target": "Header",
+        #             "subKey": "aliwaf_wxbb_umid",
+        #             "threshold": 50,
+        #             "ttl": 2800
+        #         },
+        #         "action": "deny"
+        #     },
+        #     {
+        #         "type": "custom_cc",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 10,
+        #             "target": "Query String Parameter",
+        #             "subKey": "arg",
+        #             "threshold": 30,
+        #             "ttl": 1800
+        #         },
+        #         "action": "monitor"
+        #     },
+        #     {
+        #         "type": "custom_cc",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "interval": 10,
+        #             "target": "Query String Parameter",
+        #             "subKey": "arg",
+        #             "threshold": 30,
+        #             "ttl": 1800
+        #         },
+        #         "action": "deny"
+        #     },
+        #     {
+        #         "type": "app_sdk",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "featureAbnormal":
+        #             [
+        #                 "simulator",
+        #                 "proxy",
+        #                 "root",
+        #                 "debugged",
+        #                 "hook",
+        #                 "virtual",
+        #                 "antiReplay",
+        #                 "signInvalid"
+        #             ],
+        #             "customSignStatus": "on",
+        #             "customSign":
+        #             {
+        #                 "key": "header",
+        #                 "value": "ua"
+        #             }
+        #         },
+        #         "action": "monitor"
+        #     },
+        #     {
+        #         "type": "app_package",
+        #         "status": "on",
+        #         "config":
+        #         {
+        #             "packageSigns":
+        #             [
+        #                 {
+        #                     "name": "aaaaa",
+        #                     "sign": "bbbb"
+        #                 },
+        #                 {
+        #                     "name": "cccc",
+        #                     "sign": "dddd"
+        #                 }
+        #             ]
+        #         },
+        #         "action": "deny"
+        #     }
+        # ]
+        # ```
         self.rule_configs = rule_configs
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -607,17 +1664,16 @@
 
 class BatchCreateDcdnWafRulesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         rule_ids: BatchCreateDcdnWafRulesResponseBodyRuleIds = None,
     ):
-        # The ID of the request.
+        # Creates Web Application Firewall (WAF) protection rules.
         self.request_id = request_id
-        # The IDs of created rules.
         self.rule_ids = rule_ids
 
     def validate(self):
         if self.rule_ids:
             self.rule_ids.validate()
 
     def to_map(self):
@@ -1027,31 +2083,31 @@
         security_token: str = None,
     ):
         # The name of the certificate.
         self.cert_name = cert_name
         # The type of the certificate. Valid values:
         # 
         # *   **upload**: a custom certificate that you upload.
-        # *   **cas**: a certificate that is purchased from Alibaba Cloud SSL Certificates Service
+        # *   **cas**: a certificate that is acquired through Certificate Management Service.
         self.cert_type = cert_type
-        # The name of the accelerated domain for which you want to configure the HTTPS certificate. The accelerated domain must have HTTPS acceleration enabled. You can specify multiple domain names and separate them with commas (,).
+        # The accelerated domain name for which you want to configure the HTTPS certificate. The accelerated domain must have HTTPS acceleration enabled. You can specify multiple domain names and separate them with commas (,).
         # 
-        # >  You can configure up to 10 domain names at a time.
+        # > You can configure up to 10 domain names in each request.
         self.domain_name = domain_name
         self.owner_id = owner_id
         # The ID of the region.
         self.region = region
         # The private key. This parameter is required only if you enable the certificate.
         self.sslpri = sslpri
         # Specifies whether to enable the HTTPS certificate. Valid values:
         # 
-        # *   **on:**\
-        # *   **off**\
+        # *   \*\*on\*\*: enables the HTTPS certificate.
+        # *   **off**: does not enable the HTTPS certificate.
         # 
-        # The default value is **off**.
+        # This is the default value.
         self.sslprotocol = sslprotocol
         # The content of the certificate. This parameter is required only if you enable the certificate.
         self.sslpub = sslpub
         self.security_token = security_token
 
     def validate(self):
         pass
@@ -1332,17 +2388,15 @@
         functions: str = None,
         owner_account: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
         # The domain names accelerated by IPA. Separate multiple domain names with commas (,).
         self.domain_names = domain_names
-        # The list of features.
-        # 
-        #     [{"functionArgs":[{"argName":"Parameter name","argValue":"Parameter value"}],"functionName":"Feature name"}]
+        # The list of features. `[{"functionArgs":[{"argName":"parameter name","argValue":"parameter value"}],"functionName":"feature name"}]`
         self.functions = functions
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
@@ -1459,15 +2513,15 @@
         defense_status: str = None,
         domain_names: str = None,
     ):
         # Specifies the header that records the IP address to be obtained. If the default header is selected, the value of this parameter is empty. If a custom header is selected, the value of this parameter is the value specified by the user. Separate multiple values with commas (,). You can specify a maximum of five values.
         self.client_ip_tag = client_ip_tag
         # The protection status of the domain name. Valid values: on, off, and empty string.
         # 
-        # *   When you add a domain name, the value of this parameter is **on**, and the value of ClientIpTag takes effect.
+        # *   When you add a domain name, the value of this parameter is **on**, and the value of ClientIpTag takes effect, which is empty if the default header is selected and is the value specified by the user if a custom header is selected.
         # *   When you delete a domain name, the value of this parameter is **off**, and the value of ClientIpTag does not take effect.
         # *   When you only modify the value of ClientIpTag, the value of DefenseStatus is an empty string.
         self.defense_status = defense_status
         # The protected domain names for which you want to change the protection status. You can specify up to 50 domain names. Separate multiple domain names with commas (,).
         self.domain_names = domain_names
 
     def validate(self):
@@ -1825,25 +2879,18 @@
         self,
         deliver: str = None,
         domain_name: str = None,
         name: str = None,
         reports: str = None,
         schedule: str = None,
     ):
-        # The method that is used to send operations reports. Operations reports are sent to you only by email. The settings must be escaped in JSON.
         self.deliver = deliver
-        # The domain names to be tracked. Separate multiple domain names with commas (,). You can specify up to 500 domain names. If you want to specify more than 500 domain names, [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex).
-        # 
-        # > If you do not specify a domain name, the tracking task is created for all domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
-        # The name of the tracking task.
         self.name = name
-        # The operations reports that are tracked by the task. The data must be escaped in JSON.
         self.reports = reports
-        # The parameters that specify the time interval at which the tracking task sends operations reports. The settings must be escaped in JSON.
         self.schedule = schedule
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1880,17 +2927,15 @@
 
 class CreateDcdnDeliverTaskResponseBody(TeaModel):
     def __init__(
         self,
         deliver_id: str = None,
         request_id: str = None,
     ):
-        # The ID of the tracking task.
         self.deliver_id = deliver_id
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1967,15 +3012,15 @@
         slslog_store: str = None,
         slsproject: str = None,
         slsregion: str = None,
         sampling_rate: str = None,
     ):
         # The type of the collected logs. Default value: cdn_log_access_l1. Valid values:
         # 
-        # *   **cdn_log_access_l1**: access logs of L1 Dynamic Route for CDN (DCDN) points of presence (POPs)
+        # *   **cdn_log_access_l1**: access logs of Dynamic Content Delivery Network (DCDN) points of presence (POPs)
         # *   **cdn_log_origin**: back-to-origin logs
         # *   **cdn_log_er**: EdgeRoutine logs
         self.business_type = business_type
         # The data center. Valid values:
         # 
         # *   cn: China
         # *   sg: Singapore
@@ -2448,19 +3493,22 @@
 class CreateRoutineRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         env_conf: Dict[str, Any] = None,
         name: str = None,
     ):
-        # The description of the routine.
-        self.description = description
         # The configurations of the specified environment.
-        self.env_conf = env_conf
+        self.description = description
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        self.env_conf = env_conf
+        # > 
+        # *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
+        # *   This operation creates a routine that contains only production and staging environments.
+        # *   You can call this operation up to 100 times per second.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2490,19 +3538,22 @@
 class CreateRoutineShrinkRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         env_conf_shrink: str = None,
         name: str = None,
     ):
-        # The description of the routine.
-        self.description = description
         # The configurations of the specified environment.
-        self.env_conf_shrink = env_conf_shrink
+        self.description = description
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        self.env_conf_shrink = env_conf_shrink
+        # > 
+        # *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
+        # *   This operation creates a routine that contains only production and staging environments.
+        # *   You can call this operation up to 100 times per second.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2610,22 +3661,18 @@
 
 class CreateSlrAndSlsProjectRequest(TeaModel):
     def __init__(
         self,
         business_type: str = None,
         region: str = None,
     ):
-        # The type of the collected logs. Default value: cdn_log_access_l1. Valid values:
-        # 
-        # *   **cdn_log_access_l1**: access logs of L1 Dynamic Route for CDN (DCDN) points of presence (POPs)
-        # *   **cdn_log_origin**: back-to-origin logs
-        # *   **cdn_log_er**: EdgeRoutine logs
+        # *   ****\
+        # *   ****\
+        # *   ****\
         self.business_type = business_type
-        # The region where Log Service resides. Valid values:
-        # 
         # *   **cn-hangzhou**\
         # *   **cn-shanghai**\
         # *   **cn-qingdao**\
         # *   **cn-beijing**\
         # *   **cn-zhangjiakou**\
         # *   **cn-shenzhen**\
         # *   **eu-central-1**\
@@ -2662,21 +3709,17 @@
     def __init__(
         self,
         end_point: str = None,
         log_store: str = None,
         project: str = None,
         region: str = None,
     ):
-        # The endpoint of Log Service.
         self.end_point = end_point
-        # The Logstore of Log Service.
         self.log_store = log_store
-        # The project of Log Service.
         self.project = project
-        # The region where Log Service resides.
         self.region = region
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2709,17 +3752,15 @@
 
 class CreateSlrAndSlsProjectResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         sls_info: CreateSlrAndSlsProjectResponseBodySlsInfo = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
-        # The information about Log Service.
         self.sls_info = sls_info
 
     def validate(self):
         if self.sls_info:
             self.sls_info.validate()
 
     def to_map(self):
@@ -2891,15 +3932,14 @@
     def __init__(
         self,
         domain_name: str = None,
         owner_account: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The accelerated domain name to be deleted. You can specify only one domain name.
         self.domain_name = domain_name
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
@@ -2934,15 +3974,14 @@
 
 
 class DeleteDcdnDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3129,15 +4168,15 @@
         config_id: str = None,
         domain_name: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the configuration. You can call the [DescribeDcdnDomainConfigs](~~130625~~) operation to query configuration IDs.
         self.config_id = config_id
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -3244,15 +4283,15 @@
 
 class DeleteDcdnKvRequest(TeaModel):
     def __init__(
         self,
         key: str = None,
         namespace: str = None,
     ):
-        # The name of the key that you want to delete.
+        # The ID of the request.
         self.key = key
         # The namespace that you specify when you call the PutDcdnKvNamespace operation.
         self.namespace = namespace
 
     def validate(self):
         pass
 
@@ -3278,15 +4317,15 @@
 
 
 class DeleteDcdnKvResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The name of the key to delete.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3891,15 +4930,15 @@
 
 class DeleteRoutineResponseBody(TeaModel):
     def __init__(
         self,
         content: Dict[str, Any] = None,
         request_id: str = None,
     ):
-        # Returns ""Status": "OK"".
+        # The message returned, such as ""Status": "OK"".
         self.content = content
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -4084,17 +5123,19 @@
 
 class DeleteRoutineConfEnvsRequest(TeaModel):
     def __init__(
         self,
         envs: Dict[str, Any] = None,
         name: str = None,
     ):
-        # The custom canary release environments that you want to delete.
-        self.envs = envs
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        self.envs = envs
+        # > 
+        # *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
+        # *   You can call this operation up to 100 times per second per account.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4119,17 +5160,19 @@
 
 class DeleteRoutineConfEnvsShrinkRequest(TeaModel):
     def __init__(
         self,
         envs_shrink: str = None,
         name: str = None,
     ):
-        # The custom canary release environments that you want to delete.
-        self.envs_shrink = envs_shrink
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        self.envs_shrink = envs_shrink
+        # > 
+        # *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
+        # *   You can call this operation up to 100 times per second per account.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4263,15 +5306,15 @@
 
 
 class DescribeDcdnAclFieldsResponseBodyContent(TeaModel):
     def __init__(
         self,
         fields: str = None,
     ):
-        # The rules and policies that were configured. The JSON string must be decoded.
+        # The rules and policies that were configured. The JSON string is decoded.
         self.fields = fields
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4292,15 +5335,15 @@
 
 class DescribeDcdnAclFieldsResponseBody(TeaModel):
     def __init__(
         self,
         content: List[DescribeDcdnAclFieldsResponseBodyContent] = None,
         request_id: str = None,
     ):
-        # The details about the rules.
+        # Details about the rules.
         self.content = content
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.content:
             for k in self.content:
@@ -5963,39 +7006,24 @@
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         layer: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify multiple domain names and separate them with commas (,). You can specify up to 500 domain names in each request. The query results of multiple domain names are aggregated.
-        # 
-        # If you do not specify a domain name, data of all domain names is queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # **\
         # 
-        # >  The end time must be later than the start time.
+        # ****\
         self.end_time = end_time
-        # The time interval between the data entries to return. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
+        # ****\
         self.interval = interval
-        # The name of the Internet service provider (ISP). You can call the DescribeDcdnRegionAndIsp operation to query the ISP name. If you do not specify a value for this parameter, all ISPs are queried.
         self.isp_name_en = isp_name_en
-        # The layer at which you want to query the bandwidth data. The network layer supports IPv4 and IPv6. The application layer supports http, https, and quic. You can also set the value to all.
-        # 
-        # Default value: all.
         self.layer = layer
-        # The name of the region. You can call the DescribeDcdnRegionAndIsp operation to query the region name. If you do not specify a value for this parameter, all regions are queried.
         self.location_name_en = location_name_en
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The minimum data granularity is 5 minutes.
-        # 
-        # If you do not set this parameter, data in the last 24 hours is queried.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6049,19 +7077,16 @@
         traffic_value: str = None,
         value: str = None,
     ):
         self.dynamic_traffic_value = dynamic_traffic_value
         self.dynamic_value = dynamic_value
         self.static_traffic_value = static_traffic_value
         self.static_value = static_value
-        # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The total amount of network traffic. Unit: bytes.
         self.traffic_value = traffic_value
-        # The total bandwidth. Unit: bit/s.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6142,19 +7167,16 @@
 class DescribeDcdnDomainBpsDataByLayerResponseBody(TeaModel):
     def __init__(
         self,
         bps_data_interval: DescribeDcdnDomainBpsDataByLayerResponseBodyBpsDataInterval = None,
         data_interval: str = None,
         request_id: str = None,
     ):
-        # The bandwidth returned at each time interval.
         self.bps_data_interval = bps_data_interval
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.bps_data_interval:
             self.bps_data_interval.validate()
 
     def to_map(self):
@@ -6491,29 +7513,29 @@
         # 
         # If you leave this parameter empty, the data of all domain names is queried.
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The end time must be later than the start time.
         self.end_time = end_time
-        # The number of the page to return. Default value: **1**.
+        # The page number of the returned page. Default value: **1**.
         self.page_number = page_number
         # The number of entries to return on each page. Default value: **30**.
         self.page_size = page_size
-        # The name of the rule. Valid values
+        # The name of the rule.
         # 
         # *   default_normal in normal mode
         # *   default_attack in emergency mode
         # *   A custom rule name in custom mode. Example: test2.
         # 
         # If you leave this parameter empty, all events that triggered rate limiting are queried.
         self.rule_name = rule_name
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The resolution of the queried data is 5 minutes.
+        # The minimum data granularity is 5 minutes.
         # 
         # If you leave this parameter empty, the data collected over the last 24 hours is queried.
         self.start_time = start_time
         # The object that triggered rate limiting.
         # 
         # If you leave this parameter empty, all events that triggered rate limiting are queried.
         self.trigger_object = trigger_object
@@ -6583,15 +7605,15 @@
     ):
         # The action that was triggered.
         self.action = action
         # The accelerated domain name.
         self.domain_name = domain_name
         # The name of the rule that was triggered.
         self.rule_name = rule_name
-        # The timestamp of the data.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
         # The object that triggered rate limiting.
         self.trigger_object = trigger_object
         # The period of time during which rate limiting remains effective.
         self.ttl = ttl
         # The value of the object that triggered rate limiting.
         self.value = value
@@ -6749,15 +7771,15 @@
 
 
 class DescribeDcdnDomainCertificateInfoRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each request.
+        # The certificate information of the domain name.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6788,53 +7810,48 @@
         cert_region: str = None,
         cert_type: str = None,
         domain_name: str = None,
         sslprotocol: str = None,
         sslpub: str = None,
         status: str = None,
     ):
-        # The domain name that matches the certificate.
+        # The certificate authority (CA) that issued the certificate.
         self.cert_domain_name = cert_domain_name
-        # The expiration time of the certificate.
+        # The status of HTTPS. Valid values:
+        # 
+        # *   **on**: enabled
+        # *   **off**: disabled
         self.cert_expire_time = cert_expire_time
+        # The type of the certificate. Valid values:
+        # 
+        # *   **free**: a free certificate
+        # *   **cas**: a certificate that is purchased from Alibaba Cloud SSL Certificates Service
+        # *   **upload**: a certificate that is uploaded by the user
         self.cert_id = cert_id
-        # The validity period of the certificate. Unit: **months** or **years**.
+        # The public key of the certificate.
         self.cert_life = cert_life
-        # The name of the certificate.
+        # The accelerated domain name.
         self.cert_name = cert_name
-        # The certificate authority (CA) that issued the certificate.
+        # >  The maximum number of times that each user can call this operation per second is 100.
         self.cert_org = cert_org
+        # The expiration time of the certificate.
         self.cert_region = cert_region
+        # The name of the certificate.
+        self.cert_type = cert_type
+        # The domain name that matches the certificate.
+        self.domain_name = domain_name
+        # The domain name that matches the certificate.
+        self.sslprotocol = sslprotocol
         # The type of the certificate. Valid values:
         # 
         # *   **free**: a free certificate
         # *   **cas**: a certificate that is purchased from Alibaba Cloud SSL Certificates Service
         # *   **upload**: a certificate that is uploaded by the user
-        self.cert_type = cert_type
-        # The accelerated domain name.
-        self.domain_name = domain_name
-        # The status of HTTPS. Valid values:
-        # 
-        # *   **on**: enabled
-        # *   **off**: disabled
-        self.sslprotocol = sslprotocol
-        # The public key of the certificate.
         self.sslpub = sslpub
-        # The status of the certificate. Valid values:
-        # 
-        # *   **success**: The certificate has taken effect.
-        # *   **checking**: The system is checking whether the domain name is using Dynamic Route for CDN (DCDN).
-        # *   **cname_error**: The domain name is not using DCDN.
-        # *   **domain_invalid**: The domain name contains invalid characters.
-        # *   **unsupport_wildcard**: The wildcard domain name is not supported.
-        # *   **applying**: Certificate application is in progress.
-        # *   **get_token_timeout**: The certificate application request has timed out.
-        # *   **check_token_timeout**: The verification has timed out.
-        # *   **get_cert_timeout**: The request to obtain the certificate has timed out.
-        # *   **failed**: The certificate application request failed.
+        # The expiration time of the certificate.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6934,17 +7951,28 @@
 
 class DescribeDcdnDomainCertificateInfoResponseBody(TeaModel):
     def __init__(
         self,
         cert_infos: DescribeDcdnDomainCertificateInfoResponseBodyCertInfos = None,
         request_id: str = None,
     ):
-        # The certificate information of the domain name.
+        # The validity period of the certificate. Unit: **months** or **years**.
         self.cert_infos = cert_infos
-        # The ID of the request.
+        # The status of the certificate. Valid values:
+        # 
+        # *   **success**: The certificate has taken effect.
+        # *   **checking**: The system is checking whether the domain name is using Dynamic Route for CDN (DCDN).
+        # *   **cname_error**: The domain name is not using DCDN.
+        # *   **domain_invalid**: The domain name contains invalid characters.
+        # *   **unsupport_wildcard**: The wildcard domain name is not supported.
+        # *   **applying**: Certificate application is in progress.
+        # *   **get_token_timeout**: The certificate application request has timed out.
+        # *   **check_token_timeout**: The verification has timed out.
+        # *   **get_cert_timeout**: The request to obtain the certificate has timed out.
+        # *   **failed**: The certificate application request failed.
         self.request_id = request_id
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
 
     def to_map(self):
@@ -7834,23 +8862,23 @@
         interval: str = None,
         start_time: str = None,
     ):
         # The accelerated domain name. You can specify only one domain name.
         # 
         # If you do not specify a value for this parameter, all domain names are queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time needs to be in UTC.
         # 
-        # The end time must be later than the start time.
+        # The end time needs to be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries to return. Unit: seconds.
+        # The time granularity for a query. Unit: seconds.
         # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time needs to be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7888,15 +8916,15 @@
         req_hit_rate: float = None,
         time_stamp: str = None,
     ):
         # The byte hit ratio.
         self.byte_hit_rate = byte_hit_rate
         # The request hit ratio.
         self.req_hit_rate = req_hit_rate
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8073,37 +9101,19 @@
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         self.domain_name = domain_name
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time granularity for a query. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The name of the ISP.
-        # 
-        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en
-        # The name of the region.
-        # 
-        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8145,19 +9155,16 @@
 class DescribeDcdnDomainHttpCodeDataResponseBodyDataPerIntervalDataModuleHttpCodeDataPerIntervalHttpCodeDataModule(TeaModel):
     def __init__(
         self,
         code: int = None,
         count: float = None,
         proportion: float = None,
     ):
-        # The HTTP status code returned.
         self.code = code
-        # The total number of entries.
         self.count = count
-        # The proportion of the HTTP status code.
         self.proportion = proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8221,17 +9228,15 @@
 
 class DescribeDcdnDomainHttpCodeDataResponseBodyDataPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         http_code_data_per_interval: DescribeDcdnDomainHttpCodeDataResponseBodyDataPerIntervalDataModuleHttpCodeDataPerInterval = None,
         time_stamp: str = None,
     ):
-        # The proportions of the HTTP status codes.
         self.http_code_data_per_interval = http_code_data_per_interval
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp
 
     def validate(self):
         if self.http_code_data_per_interval:
             self.http_code_data_per_interval.validate()
 
     def to_map(self):
@@ -8297,25 +9302,19 @@
         data_interval: str = None,
         data_per_interval: DescribeDcdnDomainHttpCodeDataResponseBodyDataPerInterval = None,
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The proportions of HTTP status codes at each time interval.
         self.data_per_interval = data_per_interval
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.data_per_interval:
             self.data_per_interval.validate()
 
     def to_map(self):
@@ -8649,48 +9648,48 @@
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
         time_merge: str = None,
     ):
         # The accelerated domain name.
         # 
-        # Separate multiple domain names with commas (,). If you do not specify a value for this parameter, all accelerated domain names are queried.
+        # Separate multiple domain names with commas (,). If you leave this parameter empty, all accelerated domain names are queried.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # Specify whether to implement padding with zeros. Valid values:
+        # Specifies whether to implement padding with zeros. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.fix_time_gap = fix_time_gap
-        # The time granularity for a query. Unit: seconds.
+        # The time granularity of data entries. Unit: seconds.
         # 
-        # The value varies based on the values of the **StartTime** and **EndTime** parameters. Valid values:
+        # The time granularity varies with the time range specified by **StartTime** and **EndTime**.
         # 
-        # *   If the time range between StartTime and EndTime is less than 3 days, the valid values are **300**, **3600**, and **86400**. If you do not specify a value for this parameter, **300** is used.
-        # *   If the time range between StartTime and EndTime is from 3 to 31 days (31 days excluded), the valid values are **3600** and **86400**. Default value: **3600**.
+        # *   If the time range between StartTime and EndTime is less than 3 days, the valid values are **300**, **3600**, and **86400**. If you leave this parameter empty, **300** is used.
+        # *   If the time range between StartTime and EndTime is greater than or equal to 3 days and less than 31 days, the valid values are **3600** and **86400**. Default value: **3600**.
         # *   If the time range between StartTime and EndTime is 31 days or longer, the valid value is **86400**. Default value: **86400**.
         self.interval = interval
         # The name of the Internet service provider (ISP).
         # 
         # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en
         # The name of the region.
         # 
         # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
-        # Specifies whether to automatically set the interval. If you set **TimeMerge** to **1**, the value of the **Interval** parameter is automatically assigned based on the **startTime** and **endTime** parameters. You can set either this parameter or the **Interval** parameter.
+        # Specifies whether to automatically set the interval. If you set **TimeMerge** to **1**, the value of the **Interval** parameter is automatically assigned based on the **startTime** and **endTime** parameters. You can specify either this parameter or the **Interval** parameter.
         self.time_merge = time_merge
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8815,15 +9814,15 @@
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
     ):
         # The bandwidth data returned at each interval.
         self.bps_data_per_interval = bps_data_per_interval
-        # The time interval at which data is collected. Unit: seconds.
+        # The time interval at which data was collected. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
         # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
@@ -9156,50 +10155,50 @@
         fix_time_gap: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
         time_merge: str = None,
     ):
-        # The name of the accelerated domain name.
+        # The accelerated domain name.
         # 
-        # You can specify one or more accelerated domain names. Separate them with commas (,). By default, all accelerated domain names that belong to your Alibaba Cloud account are queried.
+        # Separate multiple domain names with commas (,). If you do not specify a value for this parameter, data for all accelerated domain names is queried.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
-        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
         # Specify whether to implement padding with zeros. Valid values:
         # 
-        # *   **true**: Yes
-        # *   **false**: No
+        # *   **true**\
+        # *   **false**\
         self.fix_time_gap = fix_time_gap
-        # The time interval between the data entries returned. Unit: seconds.
+        # The time granularity of data entries. Unit: seconds.
         # 
-        # The valid values vary based on the values of the **StartTime** and **EndTime** parameters. Valid values:
+        # The time granularity varies with the time range specified by **StartTime** and **EndTime**.
         # 
-        # *   If the time range between StartTime and EndTime is less than 3 days, valid values are **300**, **3600**, and **86400**. Default value: **300**.
-        # *   If the time range between StartTime and EndTime is from 3 to 31 days (31 days excluded), valid values are **3600** and **86400**. Default value: **3600**.
+        # *   If the time range between StartTime and EndTime is less than 3 days, the valid values are **300**, **3600**, and **86400**. If you do not specify a value for this parameter, **300** is used.
+        # *   If the time range between StartTime and EndTime is greater than or equal to 3 days and less than 31 days, the valid values are **3600** and **86400**. Default value: **3600**.
         # *   If the time range between StartTime and EndTime is 31 days or longer, the valid value is **86400**. Default value: **86400**.
         self.interval = interval
-        # The name of the Internet service provider (ISP) for Dynamic Route for CDN (DCDN).
+        # The name of the Internet service provider (ISP).
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~207199~~) operation to query the most recent ISP list. If you do not specify an ISP, all ISPs are queried.
+        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en
         # The name of the region.
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~207199~~) operation to query the most recent region list. If you do not specify a region, all regions are queried.
+        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en
         # The beginning of the time range to query.
         # 
-        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
-        # Specify whether to automatically calculate the value of the **Interval** parameter. If you set the **TimeMerge** parameter to **1**, the value of the **Interval** parameter is automatically assigned based on the **StartTime** and **EndTime** parameters. You can set this parameter or the **Interval** parameter.
+        # Specifies whether to automatically calculate the value of the **interval**. If the **timeMerge** parameter is set to **1**, the value of **inteval** is calculated based on **StartTime** and **EndTime**. You can set either this parameter or the **interval** parameter.
         self.time_merge = time_merge
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9250,15 +10249,15 @@
     def __init__(
         self,
         ipa_traffic: float = None,
         time_stamp: str = None,
     ):
         # The total amount of network traffic.
         self.ipa_traffic = ipa_traffic
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9326,21 +10325,21 @@
         start_time: str = None,
         traffic_data_per_interval: DescribeDcdnDomainIpaTrafficDataResponseBodyTrafficDataPerInterval = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
-        # The monitoring data of network traffic that was collected at each interval.
+        # The network traffic that was collected at each interval.
         self.traffic_data_per_interval = traffic_data_per_interval
 
     def validate(self):
         if self.traffic_data_per_interval:
             self.traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -9428,23 +10427,19 @@
 class DescribeDcdnDomainIspDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each request.
-        # 
-        # If you do not specify an accelerated domain name, the data of all accelerated domain names that belong to your account is queried.
+        # The beginning of the time range during which data was queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # The accelerated domain name.
         self.end_time = end_time
-        # The beginning of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9482,35 +10477,43 @@
         isp: str = None,
         isp_ename: str = None,
         proportion: str = None,
         qps: str = None,
         total_bytes: str = None,
         total_query: str = None,
     ):
-        # The average response size. Unit: bytes.
+        # The proportion of network traffic. For example, a value of 90 indicates that 90% of network traffic was coming from the specified ISP.
         self.avg_object_size = avg_object_size
-        # The average response speed. Unit: byte/ms.
+        # The name of the ISP.
         self.avg_response_rate = avg_response_rate
-        # The average response time. Unit: milliseconds.
-        self.avg_response_time = avg_response_time
         # The bandwidth.
+        self.avg_response_time = avg_response_time
+        # The information about the ISP.
         self.bps = bps
-        # The proportion of network traffic. For example, a value of 90 indicates that 90% of network traffic was coming from the specified ISP.
+        # The total amount of network traffic.
         self.bytes_proportion = bytes_proportion
-        # The information about the ISP.
-        self.isp = isp
         # The name of the ISP.
+        self.isp = isp
+        # > 
+        # *   You can call this operation up to 100 times per second.
+        # *   If **StartTime** is set but **EndTime** is not set, the data within the hour that starts from **StartTime** is queried.
+        # *   If **EndTime** is set but **StartTime** is not set, the data within the last hour that precedes **EndTime** is queried.
+        # *   You can query data of a domain name or all domain names that belong to your account.
+        # *   You can view data that is collected over the last seven days. The interval at which data is queried is based on the time range specified by **StartTime** and **EndTime**.
+        #     *   **If the time range is shorter than or equal to one hour**, data is queried every minute.
+        #     *   **If the time range is longer than 1 hour but shorter than or equal to three days**, data is queried every five minutes.
+        #     *   **If the time range is longer than three days but shorter than or equal to seven days**, data is queried every hour.
         self.isp_ename = isp_ename
-        # The proportion of requests.
+        # The information about the ISP.
         self.proportion = proportion
-        # The number of queries per second.
+        # The average response time. Unit: milliseconds.
         self.qps = qps
-        # The total amount of network traffic.
+        # The average response size. Unit: bytes.
         self.total_bytes = total_bytes
-        # The total number of requests.
+        # The proportion of requests.
         self.total_query = total_query
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9610,25 +10613,25 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         value: DescribeDcdnDomainIspDataResponseBodyValue = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
+        # The total amount of network traffic.
         self.data_interval = data_interval
-        # The accelerated domain name.
+        # The total number of requests.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
+        # The time interval between the data entries returned. Unit: seconds.
         self.end_time = end_time
-        # The ID of the request.
+        # The number of queries per second.
         self.request_id = request_id
-        # The beginning of the time range during which data was queried.
-        self.start_time = start_time
         # The access statistics by ISP.
+        self.start_time = start_time
+        # The average response speed. Unit: byte/ms.
         self.value = value
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -9718,33 +10721,27 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         page_number: int = None,
         page_size: int = None,
         start_time: str = None,
     ):
-        # The accelerated domain name that you want to query. You can specify only one domain name in each call.
-        self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # >  The end time must be later than the start time.
+        self.domain_name = domain_name
+        # The total number of entries returned on the current page.
         self.end_time = end_time
-        # The number of the page to return. Pages start from page **1**.
-        # 
-        # Default value: **1**.
+        # The ID of the request.
         self.page_number = page_number
-        # The number of entries to return on each page.
-        # 
-        # Valid values: **1** to **1000**. Default value: **300**. Maximum value: **1000**.
+        # The domain name.
         self.page_size = page_size
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The log information. The log information is indicated by the DomainLogDetail parameter.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9784,25 +10781,25 @@
         self,
         end_time: str = None,
         log_name: str = None,
         log_path: str = None,
         log_size: int = None,
         start_time: str = None,
     ):
-        # The end of the time range during which data was queried.
-        self.end_time = end_time
-        # The name of the log file.
-        self.log_name = log_name
         # The path of the log file.
         # 
         # Take note of the Expires field (expiration timestamp) in the response parameter LogPath. If the log download URL expires, you must obtain it again. For more information, see [LogPath field](~~31952~~).
+        self.end_time = end_time
+        # The number of entries returned per page.
+        self.log_name = log_name
+        # The total number of entries returned.
         self.log_path = log_path
-        # The size of the log file. Unit: bytes.
+        # The page information. The page information is indicated by the PageInfoDetail parameter.
         self.log_size = log_size
-        # The beginning of the time range during which data was queried.
+        # The page number of the returned page.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9875,19 +10872,21 @@
 class DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailPageInfos(TeaModel):
     def __init__(
         self,
         page_index: int = None,
         page_size: int = None,
         total: int = None,
     ):
-        # The page number of the returned page.
+        # The end of the time range during which data was queried.
         self.page_index = page_index
-        # The number of entries returned per page.
+        # The number of entries to return on each page.
+        # 
+        # Valid values: **1** to **1000**. Default value: **300**. Maximum value: **1000**.
         self.page_size = page_size
-        # The total number of entries returned.
+        # The total number of entries returned on the current page.
         self.total = total
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9917,19 +10916,21 @@
 class DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetail(TeaModel):
     def __init__(
         self,
         log_count: int = None,
         log_infos: DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailLogInfos = None,
         page_infos: DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailPageInfos = None,
     ):
-        # The total number of entries returned on the current page.
+        # The beginning of the time range during which data was queried.
         self.log_count = log_count
-        # The log information. The log information is indicated by the LogInfoDetail parameter.
+        # The name of the log file.
         self.log_infos = log_infos
-        # The page information. The page information is indicated by the PageInfoDetail parameter.
+        # > 
+        # *   If you specify neither the **StartTime** parameter nor the **EndTime** parameter, the data in the last 24 hours is returned. If you specify the **StartTime** and **EndTime** parameters, the data within the specified time range is returned.
+        # *   You can call this operation up to 100 times per second per account.
         self.page_infos = page_infos
 
     def validate(self):
         if self.log_infos:
             self.log_infos.validate()
         if self.page_infos:
             self.page_infos.validate()
@@ -9999,19 +11000,19 @@
 class DescribeDcdnDomainLogResponseBody(TeaModel):
     def __init__(
         self,
         domain_log_details: DescribeDcdnDomainLogResponseBodyDomainLogDetails = None,
         domain_name: str = None,
         request_id: str = None,
     ):
-        # The log information. The log information is indicated by the DomainLogDetail parameter.
+        # The size of the log file. Unit: bytes.
         self.domain_log_details = domain_log_details
-        # The domain name.
+        # The log information. The log information is indicated by the LogInfoDetail parameter.
         self.domain_name = domain_name
-        # The ID of the request.
+        # The end of the time range during which data was queried.
         self.request_id = request_id
 
     def validate(self):
         if self.domain_log_details:
             self.domain_log_details.validate()
 
     def to_map(self):
@@ -10093,24 +11094,24 @@
     ):
         # If this parameter is not set, data of all your accelerated domain names is queried.
         # 
         # You can specify one or more accelerated domain names. Separate domain names with commas (,).
         self.domain_name = domain_name
         # The end time must be later than the start time.
         # 
-        # *   Specify the time in the ISO 8601 standard
-        # *   in the YYYY-MM-DDThh:mm:ssZ format. The time is displayed in UTC.
+        # *   Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format.
+        # *   The time must be in UTC.
         # *   You must set both the start time and the end time.
         self.end_time = end_time
         # The beginning of the time range to query.
         # 
-        # *   Specify the time in the ISO 8601 standard
-        # *   in the yyyy-MM-ddTHH:mm:ssZ format . The time must be in UTC.
-        # *   The minimum time interval at which data is collected is 5 minutes.
-        # *   If you do not specify a start time, data within the last 24 hours is queried.
+        # *   Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format.
+        # *   The time must be in UTC.
+        # *   The minimum data granularity is 5 minutes.
+        # *   If you do not set this parameter, data in the last 24 hours is queried.
         # *   You must set both the start time and the end time.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -10142,19 +11143,19 @@
     def __init__(
         self,
         domain: str = None,
         request: int = None,
         time_stamp: str = None,
         type: str = None,
     ):
-        # The accelerated domain name.
+        # The domain name.
         self.domain = domain
         # The number of requests.
         self.request = request
-        # The timestamp of the data entry.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
         # The type of the requests. Valid values: StaticHttps, DynamicHttps, DynamicHttp, StaticQuic, and DynamicQuic.
         self.type = type
 
     def validate(self):
         pass
 
@@ -10227,21 +11228,21 @@
         self,
         area: str = None,
         bps: float = None,
         domain: str = None,
         time_stamp: str = None,
         type: str = None,
     ):
-        # The name of the district.
+        # The name of the region.
         self.area = area
         # The number of bits per second.
         self.bps = bps
-        # The accelerated domain name.
+        # The domain name.
         self.domain = domain
-        # The timestamp of the data entry.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
         # The type of the network traffic. Valid values: Simple, IPA, and WebSocket.
         self.type = type
 
     def validate(self):
         pass
 
@@ -10318,21 +11319,21 @@
         self,
         end_time: str = None,
         request_id: str = None,
         request_per_interval: DescribeDcdnDomainMultiUsageDataResponseBodyRequestPerInterval = None,
         start_time: str = None,
         traffic_per_interval: DescribeDcdnDomainMultiUsageDataResponseBodyTrafficPerInterval = None,
     ):
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
         # The information about requests collected every 5 minutes.
         self.request_per_interval = request_per_interval
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # The statistics of network traffic collected every 5 minutes.
         self.traffic_per_interval = traffic_per_interval
 
     def validate(self):
         if self.request_per_interval:
             self.request_per_interval.validate()
@@ -10939,15 +11940,15 @@
 
 
 class DescribeDcdnDomainPropertyRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
     ):
-        # The accelerated domain name that you want to query. You can specify only one domain name in each call.
+        # The ID of the request.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10969,22 +11970,22 @@
 class DescribeDcdnDomainPropertyResponseBody(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         protocol: str = None,
         request_id: str = None,
     ):
-        # The accelerated domain name that is queried.
-        self.domain_name = domain_name
         # The name of the protocol. Valid values:
         # 
         # *   **udp**: User Datagram Protocol (UDP)
         # *   **tcp**: Transmission Control Protocol (TCP)
+        self.domain_name = domain_name
+        # >  The maximum number of times that users can call this operation per second is 10.
         self.protocol = protocol
-        # The ID of the request.
+        # The accelerated domain name that is queried.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11058,15 +12059,15 @@
 class DescribeDcdnDomainPvDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The name of the accelerated domain. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
@@ -11101,15 +12102,15 @@
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The consumed network traffic.
+        # The number of PVs.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11173,25 +12174,25 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         pv_data_interval: DescribeDcdnDomainPvDataResponseBodyPvDataInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The data collection interval. Unit: second.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The name of the accelerated domain for which the data was returned.
+        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which the data was collected.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The number of PVs at each interval.
         self.pv_data_interval = pv_data_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range during which the data was collected.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.pv_data_interval:
             self.pv_data_interval.validate()
 
     def to_map(self):
@@ -11602,39 +12603,33 @@
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         layer: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify multiple domain names and separate them with commas (,). You can specify up to 500 domain names in each request. The query results of multiple domain names are aggregated.
-        # 
-        # If you do not specify a domain name, data of all domain names is queried.
+        # The QPS returned at each time interval.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # The number of queries per second outside the Chinese mainland.
         self.end_time = end_time
-        # The time interval between the data entries to return. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
+        # The layer at which the data was collected.
         self.interval = interval
-        # The name of the ISP. You can call the DescribeDcdnRegionAndIsp operation to query the ISP name. If you do not specify a value for this parameter, all ISPs are queried.
-        self.isp_name_en = isp_name_en
-        # The layers at which you want to query the QPS. The network layer supports IPv4 and IPv6. The application layer supports http, https, and quic. You can also set the value to all.
-        # 
-        # Default value: all.
-        self.layer = layer
-        # The name of the region. You can call the DescribeDcdnRegionAndIsp operation to query the region name. If you do not specify a value for this parameter, all regions are queried.
-        self.location_name_en = location_name_en
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The minimum data granularity is 5 minutes.
         # 
         # If you do not set this parameter, data in the last 24 hours is queried.
+        self.isp_name_en = isp_name_en
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  The end time must be later than the start time.
+        self.layer = layer
+        # The accelerated domain name.
+        self.location_name_en = location_name_en
+        # The number of requests in the Chinese mainland.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11684,27 +12679,31 @@
         acc_overseas_value: str = None,
         acc_value: str = None,
         domestic_value: str = None,
         overseas_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The number of requests in the Chinese mainland.
-        self.acc_domestic_value = acc_domestic_value
         # The number of requests outside the Chinese mainland.
+        self.acc_domestic_value = acc_domestic_value
+        # The beginning of the time range during which data was queried.
         self.acc_overseas_value = acc_overseas_value
-        # The total number of requests.
-        self.acc_value = acc_value
         # The number of queries per second in the Chinese mainland.
+        self.acc_value = acc_value
+        # The time interval between the data entries returned. Unit: seconds.
         self.domestic_value = domestic_value
-        # The number of queries per second outside the Chinese mainland.
+        # The total number of queries per second.
         self.overseas_value = overseas_value
-        # The timestamp of the data returned.
+        # The time interval between the data entries to return. Unit: seconds.
+        # 
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
         self.time_stamp = time_stamp
-        # The total number of queries per second.
+        # The accelerated domain name. You can specify multiple domain names and separate them with commas (,). You can specify up to 500 domain names in each request. The query results of multiple domain names are aggregated.
+        # 
+        # If you do not specify a domain name, data of all domain names is queried.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11789,27 +12788,29 @@
         domain_name: str = None,
         end_time: str = None,
         layer: str = None,
         qps_data_interval: DescribeDcdnDomainQpsDataByLayerResponseBodyQpsDataInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
+        # The end of the time range during which data was queried.
         self.data_interval = data_interval
-        # The accelerated domain name.
+        # The name of the ISP. You can call the DescribeDcdnRegionAndIsp operation to query the ISP name. If you do not specify a value for this parameter, all ISPs are queried.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
+        # The layers at which you want to query the QPS. The network layer supports IPv4 and IPv6. The application layer supports http, https, and quic. You can also set the value to all.
+        # 
+        # Default value: all.
         self.end_time = end_time
-        # The layer at which the data was collected.
+        # The operation that you want to perform. Set the value to **DescribeDcdnDomainQpsDataByLayer**.
         self.layer = layer
-        # The QPS returned at each time interval.
+        # The name of the region. You can call the DescribeDcdnRegionAndIsp operation to query the region name. If you do not specify a value for this parameter, all regions are queried.
         self.qps_data_interval = qps_data_interval
-        # The ID of the request.
+        # The timestamp of the data returned.
         self.request_id = request_id
-        # The beginning of the time range during which data was queried.
+        # The total number of requests.
         self.start_time = start_time
 
     def validate(self):
         if self.qps_data_interval:
             self.qps_data_interval.validate()
 
     def to_map(self):
@@ -12308,47 +13309,45 @@
         field: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         merge: str = None,
         merge_loc_isp: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
+        # Specifies whether to return a summary value of **LocationNameEn** and **IspNameEn**. Valid values:
+        # 
+        # *   **true**: yes
+        # *   **false**: no
+        # 
+        # The default value is **false**.
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # > The end time must be later than the start time, and the maximum time range to query is 10 minutes.
         self.end_time = end_time
-        # The type of the information that you want to query. Separate multiple types with commas (,). Valid values:
-        # 
-        # *   **qps**: queries per second
-        # *   **bps**: bandwidth
-        # *   **http_code**: HTTP status code
-        self.field = field
-        # The name of the ISP. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the ISP name.
-        # 
-        # If you do not specify a value for this parameter, all ISPs are queried.
-        self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the region name.
-        # 
-        # If you do not specify a value for this parameter, all regions are queried.
-        self.location_name_en = location_name_en
         # Specifies whether to return a summary value. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
         # 
         # The default value is **false**.
-        self.merge = merge
-        # Specifies whether to return a summary value of **LocationNameEn** and **IspNameEn**. Valid values:
+        self.field = field
+        # The information returned.
+        self.isp_name_en = isp_name_en
+        # The type of the information that you want to query. Separate multiple types with commas (,). Valid values:
         # 
-        # *   **true**: yes
-        # *   **false**: no
+        # *   **qps**: queries per second
+        # *   **bps**: bandwidth
+        # *   **http_code**: HTTP status code
+        self.location_name_en = location_name_en
+        # The ID of the request.
+        self.merge = merge
+        # The name of the region. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the region name.
         # 
-        # The default value is **false**.
+        # If you do not specify a value for this parameter, all regions are queried.
         self.merge_loc_isp = merge_loc_isp
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -12399,17 +13398,17 @@
 
 class DescribeDcdnDomainRealTimeDetailDataResponseBody(TeaModel):
     def __init__(
         self,
         data: str = None,
         request_id: str = None,
     ):
-        # The information returned.
+        # DescribeDcdnDomainRealTimeDetailData
         self.data = data
-        # The ID of the request.
+        # Queries traffic data and the number of visits of each ISP in each region. Data is collected every minute. The maximum time range to query for this operation is 10 minutes.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13029,15 +14028,15 @@
         end_time: str = None,
         start_time: str = None,
     ):
         # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The end time must be later than the start time.
+        # The end time needs to be later than the start time.
         self.end_time = end_time
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -13070,15 +14069,15 @@
     def __init__(
         self,
         req_hit_rate: float = None,
         time_stamp: str = None,
     ):
         # The request hit ratio.
         self.req_hit_rate = req_hit_rate
-        # The timestamp of the data returned. The time follows the ISO 8601 standard. The time is displayed in UTC.
+        # The timestamp of the data returned. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13138,15 +14137,15 @@
 
 class DescribeDcdnDomainRealTimeReqHitRateDataResponseBody(TeaModel):
     def __init__(
         self,
         data: DescribeDcdnDomainRealTimeReqHitRateDataResponseBodyData = None,
         request_id: str = None,
     ):
-        # The list of request hit ratios.
+        # The list of byte hit ratios.
         self.data = data
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -13772,21 +14771,16 @@
 class DescribeDcdnDomainRealTimeSrcTrafficDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
         self.end_time = end_time
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13815,17 +14809,15 @@
 
 class DescribeDcdnDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The traffic value at each time interval.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13889,27 +14881,19 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         real_time_src_traffic_data_per_interval: DescribeDcdnDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
         self.data_interval = data_interval
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The amount of origin traffic returned at each time interval. Unit: bytes.
         self.real_time_src_traffic_data_per_interval = real_time_src_traffic_data_per_interval
-        # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_src_traffic_data_per_interval:
             self.real_time_src_traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -14001,19 +14985,19 @@
         end_time: str = None,
         start_time: str = None,
     ):
         # The accelerated domain name. You can specify one or more domain names and separate them with commas (,).
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. The end time must be later than the start time.
         # 
-        # >  If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
+        # > If you do not specify StartTime or EndTime, data within the last hour is queried. If you specify both StartTime and EndTime, data within the specified time range is queried.
         self.end_time = end_time
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
+        # > If you do not specify StartTime or EndTime, data within the last hour is queried. If you specify both StartTime and EndTime, data within the specified time range is queried.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14044,17 +15028,17 @@
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The amount of back-to-origin network traffic.
+        # The traffic value at each time interval.
         # 
-        # >  The network traffic is measured in bytes.
+        # > The network traffic is measured in bytes.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14118,23 +15102,23 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         real_time_traffic_data_per_interval: DescribeDcdnDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
+        # The time interval between the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600 (1 hour). For more information, see **Description**.
+        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
         # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The amount of back-to-origin network traffic returned at each interval.
+        # The amount of back-to-origin traffic returned at each interval.
         self.real_time_traffic_data_per_interval = real_time_traffic_data_per_interval
         # The ID of the request.
         self.request_id = request_id
         # The beginning of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
@@ -14726,26 +15710,26 @@
         self,
         domain_name: str = None,
         sort_by: str = None,
         start_time: str = None,
     ):
         # The accelerated domain name. You can specify only one domain name.
         self.domain_name = domain_name
-        # The method that is used to sort the web pages. Valid values:
+        # The method that is used to arrange the returned application information. Valid values:
         # 
-        # *   **traf**: by network traffic.
-        # *   **pv**: by the number of visits.
+        # *   **traf**: by network traffic
+        # *   **pv**: by the number of visits
         # 
-        # Default value**: pv**.
+        # Default value: **pv**.
         self.sort_by = sort_by
         # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # To query the data on a specified day, use the yyyy-MM-ddT16:00:00Z format.
         # 
-        # If you do not specify this parameter, data collected within the last 24 hours is queried by default.
+        # If you leave this parameter empty, data collected in the last 24 hours is queried.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14777,23 +15761,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         refer_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The network traffic. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of the network traffic.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
         # The complete referenced URL.
         self.refer_detail = refer_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of the visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14871,15 +15855,15 @@
         start_time: str = None,
         top_refer_list: DescribeDcdnDomainTopReferVisitResponseBodyTopReferList = None,
     ):
         # The accelerated domain name.
         self.domain_name = domain_name
         # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which the data is collected.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # The list of frequently referenced URLs returned.
         self.top_refer_list = top_refer_list
 
     def validate(self):
         if self.top_refer_list:
             self.top_refer_list.validate()
@@ -14961,30 +15945,30 @@
 class DescribeDcdnDomainTopUrlVisitRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         sort_by: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
-        # The method that is used to sort the web pages. Valid values:
+        # The sorting method. Valid values:
         # 
-        # *   **traf**: by network traffic.
-        # *   **pv**: by the number of visits.
+        # *   **traf**: by network traffic
+        # *   **pv**: by the number of visits
         # 
-        # Default value: **pv**.
+        # Default value: **pv**\
         self.sort_by = sort_by
         # The start of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the YYYY-MM-DDThh:mm:ssZ format. The time must be in UTC.
         # 
         # To query the data on a specified day, use the format: yyyy-MM-ddT16:00:00Z.
         # 
-        # >  If you do not set this parameter, the data within the last 24 hours is queried.
+        # > If you do not specify this parameter, the data in the last 24 hours is queried.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15016,23 +16000,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15107,19 +16091,19 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
         # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
@@ -15198,23 +16182,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15289,23 +16273,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15380,23 +16364,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15476,19 +16460,19 @@
         url_200list: DescribeDcdnDomainTopUrlVisitResponseBodyUrl200List = None,
         url_300list: DescribeDcdnDomainTopUrlVisitResponseBodyUrl300List = None,
         url_400list: DescribeDcdnDomainTopUrlVisitResponseBodyUrl400List = None,
         url_500list: DescribeDcdnDomainTopUrlVisitResponseBodyUrl500List = None,
     ):
         # A list of frequently requested URLs.
         self.all_url_list = all_url_list
-        # The accelerated domain name for which the data was returned.
+        # The accelerated domain name.
         self.domain_name = domain_name
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range during which the data was collected.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # A list of URLs for which 2xx status codes were returned.
         self.url_200list = url_200list
         # A list of URLs for which 3xx status codes were returned.
         self.url_300list = url_300list
         # A list of URLs for which 4xx status codes were returned.
         self.url_400list = url_400list
@@ -15607,39 +16591,19 @@
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name.
-        # 
-        # Separate multiple domain names with commas (,). If you do not specify a value for this parameter, all accelerated domain names are queried.
         self.domain_name = domain_name
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time granularity for a query. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The name of the Internet service provider (ISP).
-        # 
-        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en
-        # The name of the region.
-        # 
-        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15684,25 +16648,19 @@
         dynamic_http_traffic: float = None,
         dynamic_https_traffic: float = None,
         static_http_traffic: float = None,
         static_https_traffic: float = None,
         time_stamp: str = None,
         traffic: float = None,
     ):
-        # The network traffic that was consumed to deliver dynamic content over HTTP.
         self.dynamic_http_traffic = dynamic_http_traffic
-        # The network traffic that was consumed to deliver dynamic content over HTTPS.
         self.dynamic_https_traffic = dynamic_https_traffic
-        # The network traffic that was consumed to deliver static content over HTTP.
         self.static_http_traffic = static_http_traffic
-        # The network traffic that was consumed to deliver static content over HTTPS.
         self.static_https_traffic = static_https_traffic
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The total amount of network traffic.
         self.traffic = traffic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15782,25 +16740,19 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         traffic_data_per_interval: DescribeDcdnDomainTrafficDataResponseBodyTrafficDataPerInterval = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range during which data was queried.
         self.start_time = start_time
-        # The network traffic returned at each time interval. Unit: bytes.
         self.traffic_data_per_interval = traffic_data_per_interval
 
     def validate(self):
         if self.traffic_data_per_interval:
             self.traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -16205,17 +17157,17 @@
 class DescribeDcdnDomainUvDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The name of the accelerated domain. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         # 
-        # By default, all the accelerated domains are queried.
+        # If you do not specify a domain name, this operation queries UV data of all accelerated domain names in your account.
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The end time must be later than the start time.
         self.end_time = end_time
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
@@ -16324,23 +17276,23 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         uv_data_interval: DescribeDcdnDomainUvDataResponseBodyUvDataInterval = None,
     ):
-        # The data collection interval. Unit: second.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The name of the accelerated domain for which the data was returned.
+        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which the data was collected.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range during which the data was collected.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # The number of UVs at each interval.
         self.uv_data_interval = uv_data_interval
 
     def validate(self):
         if self.uv_data_interval:
             self.uv_data_interval.validate()
@@ -16689,37 +17641,37 @@
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
+        # The accelerated domain name. You can specify multiple accelerated domain names and separate them with commas (,).
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries to return. Unit: seconds.
+        # The time granularity for a query. Unit: seconds.
         # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
         # The name of the Internet service provider (ISP).
         # 
         # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en
         # The name of the region.
         # 
         # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16761,17 +17713,17 @@
 class DescribeDcdnDomainWebsocketHttpCodeDataResponseBodyHttpCodeDataPerIntervalDataModuleWebsocketHttpCodeHttpCodeDataModule(TeaModel):
     def __init__(
         self,
         code: int = None,
         count: float = None,
         proportion: float = None,
     ):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code
-        # The total number of times that the HTTP status code was returned.
+        # The total number of entries returned.
         self.count = count
         # The proportion of the HTTP status code.
         self.proportion = proportion
 
     def validate(self):
         pass
 
@@ -16837,17 +17789,17 @@
 
 class DescribeDcdnDomainWebsocketHttpCodeDataResponseBodyHttpCodeDataPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         websocket_http_code: DescribeDcdnDomainWebsocketHttpCodeDataResponseBodyHttpCodeDataPerIntervalDataModuleWebsocketHttpCode = None,
     ):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The information about the HTTP status codes.
+        # The proportions of the HTTP status codes.
         self.websocket_http_code = websocket_http_code
 
     def validate(self):
         if self.websocket_http_code:
             self.websocket_http_code.validate()
 
     def to_map(self):
@@ -16919,19 +17871,19 @@
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
         # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The HTTP status codes.
+        # The HTTP status code.
         self.http_code_data_per_interval = http_code_data_per_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range during which data was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.http_code_data_per_interval:
             self.http_code_data_per_interval.validate()
 
     def to_map(self):
@@ -17279,27 +18231,27 @@
         routine_id: str = None,
         spec: str = None,
         split_by: str = None,
         start_time: str = None,
     ):
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The ID of the ER.
+        # The ID of the routine.
         self.routine_id = routine_id
-        # The specification of the ER. Valid values:
+        # The specification of the routine. Valid values:
         # 
         # *   5ms
         # *   50ms
         # *   100ms
         self.spec = spec
-        # Specifies how the results are grouped. If you set this parameter to routine, the returned results are grouped based on the ER ID. If you set this parameter to spec, the returned results are grouped based on the ER specification.
+        # Specifies how the results are grouped. If you set this parameter to routine, the returned results are grouped based on the routine ID. If you set this parameter to spec, the returned results are grouped based on the routine specification.
         # 
-        # >  If you leave this parameter empty, the returned results are not grouped.
+        # > If you leave this parameter empty, the returned results are not grouped.
         self.split_by = split_by
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -17340,19 +18292,19 @@
     def __init__(
         self,
         er_acc: int = None,
         routine: str = None,
         spec: str = None,
         time_stamp: str = None,
     ):
-        # The number of ER requests.
+        # The number of requests.
         self.er_acc = er_acc
-        # The ID of the ER. This parameter is returned only when SplitBy is set to routine.
+        # The ID of the routine. This parameter is returned only when SplitBy is set to routine.
         self.routine = routine
-        # The specification of the ER. This parameter is returned only when SplitBy is set to spec.
+        # The specification of the routine. This parameter is returned only when SplitBy is set to spec.
         self.spec = spec
         # The timestamp of the returned data.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
@@ -17426,19 +18378,19 @@
         end_time: str = None,
         er_acc_data: DescribeDcdnErUsageDataResponseBodyErAccData = None,
         request_id: str = None,
         start_time: str = None,
     ):
         # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The list of the returned data.
+        # The list of the data returned.
         self.er_acc_data = er_acc_data
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range during which data was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.er_acc_data:
             self.er_acc_data.validate()
 
     def to_map(self):
@@ -17803,19 +18755,28 @@
 class DescribeDcdnHttpsDomainListRequest(TeaModel):
     def __init__(
         self,
         keyword: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
-        # The keyword used for search.
+        # The status of the certificate. Valid values:
+        # 
+        # *   **ok**: The certificate is working as expected.
+        # *   **mismatch**: The certificate does not match the specified domain name.
+        # *   **expired**: The certificate has expired.
+        # *   **expire_soon**: The certificate is about to expire.
         self.keyword = keyword
-        # The number of pages to return. Valid values: **1 to 100000**.
+        # The total number of entries returned.
         self.page_number = page_number
-        # The number of entries to return on each page. Valid values: **1 to 500**. Default value: **20**.
+        # The type of the certificate. Valid values:
+        # 
+        # *   **free**: A free certificate.
+        # *   **cas**: A certificate that is purchased through Alibaba Cloud SSL Certificates Service.
+        # *   **upload**: A user-uploaded certificate.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17850,38 +18811,29 @@
         cert_name: str = None,
         cert_start_time: str = None,
         cert_status: str = None,
         cert_type: str = None,
         cert_update_time: str = None,
         domain_name: str = None,
     ):
-        # The returned primary domain name of the certificate.
+        # The certificate information about the domain name.
         self.cert_common_name = cert_common_name
-        # The time when the certificate expires.
-        self.cert_expire_time = cert_expire_time
         # The name of the certificate.
+        self.cert_expire_time = cert_expire_time
+        # The accelerated domain name for which the certificate information was queried.
         self.cert_name = cert_name
-        # The time when the certificate became effective.
+        # The time when the certificate expires.
         self.cert_start_time = cert_start_time
-        # The status of the certificate. Valid values:
-        # 
-        # *   **ok**: The certificate is working as expected.
-        # *   **mismatch**: The certificate does not match the specified domain name.
-        # *   **expired**: The certificate has expired.
-        # *   **expire_soon**: The certificate is about to expire.
+        # The number of pages to return. Valid values: **1 to 100000**.
         self.cert_status = cert_status
-        # The type of the certificate. Valid values:
-        # 
-        # *   **free**: A free certificate.
-        # *   **cas**: A certificate that is purchased through Alibaba Cloud SSL Certificates Service.
-        # *   **upload**: A user-uploaded certificate.
+        # The operation that you want to perform. Set the value to **DescribeDcdnHttpsDomainList**.
         self.cert_type = cert_type
-        # The time when the certificate was updated.
+        # The keyword used for search.
         self.cert_update_time = cert_update_time
-        # The accelerated domain name for which the certificate information was queried.
+        # The time when the certificate was updated.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17966,19 +18918,19 @@
 class DescribeDcdnHttpsDomainListResponseBody(TeaModel):
     def __init__(
         self,
         cert_infos: DescribeDcdnHttpsDomainListResponseBodyCertInfos = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The certificate information about the domain name.
+        # The time when the certificate became effective.
         self.cert_infos = cert_infos
-        # The ID of the request.
+        # The returned primary domain name of the certificate.
         self.request_id = request_id
-        # The total number of entries returned.
+        # The number of entries to return on each page. Valid values: **1 to 500**. Default value: **20**.
         self.total_count = total_count
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
 
     def to_map(self):
@@ -18085,26 +19037,26 @@
         dcdn_ip: str = None,
         isp: str = None,
         isp_ename: str = None,
         region: str = None,
         region_ename: str = None,
         request_id: str = None,
     ):
-        # Indicates whether the specified IP address is assigned to an Alibaba Cloud DCDN node.
+        # Indicates whether the specified IP address is assigned to an Alibaba Cloud DCDN POP.
         # 
-        # *   True: The specified IP address is assigned to an Alibaba Cloud DCDN node.
-        # *   False: The specified IP address is not assigned to an Alibaba Cloud DCDN node.
+        # *   True
+        # *   False
         self.dcdn_ip = dcdn_ip
-        # The Internet service provider (ISP) to which the specified IP address belongs.
+        # The ISP to which the specified IP address belongs.
         self.isp = isp
-        # The name of the ISP.
+        # The name of the Internet service provider (ISP).
         self.isp_ename = isp_ename
-        # The region to which the specified IP address belongs.
+        # The Chinese name of the region.
         self.region = region
-        # The name of the region.
+        # The English name of the region.
         self.region_ename = region_ename
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -18193,17 +19145,17 @@
     def __init__(
         self,
         domain_name: str = None,
         function_names: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The accelerated domain names. Separate multiple domain names with commas (,).
+        # The accelerated domain name. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
-        # The name of the feature. Only the protogw value is supported, which indicates IP Application Accelerator (IPA).
+        # The name of the feature. Set the value to protogw, which indicates IP Application Accelerator (IPA).
         self.function_names = function_names
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -18856,15 +19808,15 @@
 
 
 class DescribeDcdnIpaServiceResponseBodyOperationLocksLockReason(TeaModel):
     def __init__(
         self,
         lock_reason: str = None,
     ):
-        # The reason why the IPA service was locked. A value of **financial** indicates that your account has an overdue payment.
+        # The reason why the instance is locked. For example, a value of **financial** indicates that an overdue payment exists.
         self.lock_reason = lock_reason
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18929,37 +19881,37 @@
         operation_locks: DescribeDcdnIpaServiceResponseBodyOperationLocks = None,
         request_id: str = None,
     ):
         # The time when the change of the billing method starts to take effect. The time is in GMT. This time appears on the frontend only when it is later than the current time.
         self.changing_affect_time = changing_affect_time
         # The new billing method to take effect. Valid values:
         # 
-        # *   **PayByTraffic**\
-        # *   **PayByBandwidth**\
-        # *   **PayByBandwidth95**\
-        # *   **PayByBandwidth_monthavg**\
-        # *   **PayByBandwidth_month4th**\
-        # *   **PayByBandwidth_monthday95avg**\
-        # *   **PayByBandwidth_nighthalf95**\
+        # *   **PayByTraffic**: pay-by-data-transfer
+        # *   **PayByBandwidth**: pay-by-bandwidth
+        # *   **PayByBandwidth95**: pay-by-95th percentile bandwidth
+        # *   **PayByBandwidth_monthavg**: pay-by-monthly average bandwidth
+        # *   **PayByBandwidth_month4th**: pay-by-fourth peak bandwidth per month
+        # *   **PayByBandwidth_monthday95avg**: pay-by-monthly average 95th percentile bandwidth
+        # *   **PayByBandwidth_nighthalf95**: pay-by-95th percentile bandwidth (50% off during nighttime)
         self.changing_charge_type = changing_charge_type
         # The ID of the instance.
         self.instance_id = instance_id
-        # The current billing method. Valid values:
+        # The billing method of the instance. Valid values:
         # 
-        # *   **PayByTraffic**\
-        # *   **PayByBandwidth**\
-        # *   **PayByBandwidth95**\
-        # *   **PayByBandwidth_monthavg**\
-        # *   **PayByBandwidth_month4th**\
-        # *   **PayByBandwidth_monthday95avg**\
-        # *   **PayByBandwidth_nighthalf95**\
+        # *   **PayByTraffic**: pay-by-data-transfer
+        # *   **PayByBandwidth**: pay-by-bandwidth
+        # *   **PayByBandwidth95**: pay-by-95th percentile bandwidth
+        # *   **PayByBandwidth_monthavg**: pay-by-monthly average bandwidth
+        # *   **PayByBandwidth_month4th**: pay-by-fourth peak bandwidth per month
+        # *   **PayByBandwidth_monthday95avg**: pay-by-monthly average 95th percentile bandwidth
+        # *   **PayByBandwidth_nighthalf95**: pay-by-95th percentile bandwidth (50% off during nighttime)
         self.internet_charge_type = internet_charge_type
-        # The time when the IPA service was activated. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mmZ format.
+        # The time when the DCDN service was activated. The time follows the ISO 8601 standard.
         self.opening_time = opening_time
-        # The lock status of the IPA service.
+        # The lock status of secure DCDN.
         self.operation_locks = operation_locks
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.operation_locks:
             self.operation_locks.validate()
@@ -19052,17 +20004,17 @@
 
 class DescribeDcdnIpaUserDomainsRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The tag key. Valid values of N: 1 to 20. You can call the TagDcdnResources operation to set a tag for a domain name.
+        # The array that consists of multiple PageData parameters. The details about each accelerated domain name are included in a separate PageData parameter.
         self.key = key
-        # The tag value. Valid values of N: 1 to 20.
+        # The time when the accelerated domain name was added to Alibaba Cloud Dynamic Route for CDN (DCDN).
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19096,55 +20048,45 @@
         func_id: str = None,
         owner_id: int = None,
         page_number: int = None,
         page_size: int = None,
         resource_group_id: str = None,
         tag: List[DescribeDcdnIpaUserDomainsRequestTag] = None,
     ):
-        # Specifies whether to display domain names that are under review, failed the review, or failed to be configured. Valid values:
-        # 
-        # *   **true**\
-        # *   **false**\
+        # The tag key. Valid values of N: 1 to 20. You can call the TagDcdnResources operation to set a tag for a domain name.
         self.check_domain_show = check_domain_show
-        # The domain name that is used as a keyword to filter domain names. Fuzzy match is supported.
+        # The ID of the resource group.
         self.domain_name = domain_name
-        # The search method. Default value: full_match. Valid values:
-        # 
-        # *   **fuzzy_match**: fuzzy match
-        # *   **pre_match**: prefix match
-        # *   **suf_match**: suffix match
-        # *   **full_match**: exact match
-        self.domain_search_type = domain_search_type
-        # The status of the domain name. Valid values:
-        # 
-        # *   **online**: enabled
-        # *   **offline**: disabled
-        # *   **configuring**: configuring
-        # *   **configure_failed**: configuration failed
-        # *   **checking**: reviewing
-        # *   **check_failed**: review failed
-        self.domain_status = domain_status
         # The status of the feature.
         # 
         # *   config: The feature is enabled.
         # *   unconfig: The feature is not enabled.
-        self.func_filter = func_filter
+        self.domain_search_type = domain_search_type
         # The ID of the feature. For example, a value of 7 specifies the feature of configuring an expiration rule for a specific directory. For more information about feature IDs, see [Parameters for configuring features for domain names](~~410622~~).
+        self.domain_status = domain_status
+        # The number of the returned page.
+        self.func_filter = func_filter
+        # The ID of the request.
         self.func_id = func_id
         self.owner_id = owner_id
-        # The number of the page to return. Valid values: **1** to **100000**.
+        # Specifies whether to display domain names that are under review, failed the review, or failed to be configured. Valid values:
         # 
-        # Default value: **1**.
+        # *   **true**\
+        # *   **false**\
         self.page_number = page_number
-        # The number of domain names to return on each page. Default value: **20**. Maximum value: **500**.
+        # The search method. Default value: full_match. Valid values:
         # 
-        # Valid values: an integer from **1** to **500**.
+        # *   **fuzzy_match**: fuzzy match
+        # *   **pre_match**: prefix match
+        # *   **suf_match**: suffix match
+        # *   **full_match**: exact match
         self.page_size = page_size
-        # The ID of the resource group.
+        # The tag value. Valid values of N: 1 to 20.
         self.resource_group_id = resource_group_id
+        # The number of domain names returned per page.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -19216,23 +20158,20 @@
         self,
         content: str = None,
         port: int = None,
         priority: str = None,
         type: str = None,
         weight: str = None,
     ):
-        # The address of the origin server.
         self.content = content
-        # The port of the origin server.
         self.port = port
-        # The priority of the origin server.
         self.priority = priority
-        # The type of the origin server.
+        # Queries information about all domain names that are accelerated by IPA in your account.
+        #                   Fuzzy search and filtering by domain name status are supported.
         self.type = type
-        # The weight of the origin server if multiple origin servers have been specified.
         self.weight = weight
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19312,43 +20251,33 @@
         gmt_created: str = None,
         gmt_modified: str = None,
         resource_group_id: str = None,
         sslprotocol: str = None,
         sandbox: str = None,
         sources: DescribeDcdnIpaUserDomainsResponseBodyDomainsPageDataSources = None,
     ):
-        # The CNAME assigned to the accelerated domain name.
+        # The priority of the origin server.
         self.cname = cname
-        # The reason why the accelerated domain name failed the review.
+        # The time when the accelerated domain name was modified.
         self.description = description
-        # The accelerated domain name.
+        # The address of the origin server.
         self.domain_name = domain_name
-        # The status of the accelerated domain name. Valid values:
-        # 
-        # *   **online**: enabled
-        # *   **offline**: disabled
-        # *   **configuring**: configuring
-        # *   **configure_failed**: configuration failed
-        # *   **checking**: reviewing
-        # *   **check_failed**: review failed
+        # The weight of the origin server if multiple origin servers have been specified.
         self.domain_status = domain_status
-        # The time when the accelerated domain name was added to Alibaba Cloud Dynamic Route for CDN (DCDN).
+        # The CNAME assigned to the accelerated domain name.
         self.gmt_created = gmt_created
-        # The time when the accelerated domain name was modified.
+        # The port of the origin server.
         self.gmt_modified = gmt_modified
-        # The ID of the resource group.
+        # The information about the origin server.
         self.resource_group_id = resource_group_id
-        # The status of HTTPS.
-        # 
-        # *   **on**\
-        # *   **off**\
+        # The accelerated domain name.
         self.sslprotocol = sslprotocol
-        # Indicates whether the accelerated domain name was in a sandbox.
+        # The type of the origin server.
         self.sandbox = sandbox
-        # The information about the origin server.
+        # >  You can call this operation up to 30 times per second per account.
         self.sources = sources
 
     def validate(self):
         if self.sources:
             self.sources.validate()
 
     def to_map(self):
@@ -19445,23 +20374,33 @@
         self,
         domains: DescribeDcdnIpaUserDomainsResponseBodyDomains = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The array that consists of multiple PageData parameters. The details about each accelerated domain name are included in a separate PageData parameter.
+        # The status of the accelerated domain name. Valid values:
+        # 
+        # *   **online**: enabled
+        # *   **offline**: disabled
+        # *   **configuring**: configuring
+        # *   **configure_failed**: configuration failed
+        # *   **checking**: reviewing
+        # *   **check_failed**: review failed
         self.domains = domains
-        # The number of the returned page.
+        # The status of HTTPS.
+        # 
+        # *   **on**\
+        # *   **off**\
         self.page_number = page_number
-        # The number of domain names returned per page.
+        # The ID of the resource group.
         self.page_size = page_size
-        # The ID of the request.
+        # The reason why the accelerated domain name failed the review.
         self.request_id = request_id
-        # The total number of domain names returned.
+        # Indicates whether the accelerated domain name was in a sandbox.
         self.total_count = total_count
 
     def validate(self):
         if self.domains:
             self.domains.validate()
 
     def to_map(self):
@@ -19885,37 +20824,39 @@
         preload_remain: str = None,
         regex_quota: str = None,
         regex_remain: str = None,
         request_id: str = None,
         url_quota: str = None,
         url_remain: str = None,
     ):
-        # The maximum number of URLs that can be blocked.
+        # The ID of the request.
         self.block_quota = block_quota
-        # The remaining number of URLs that can be blocked each day.
+        # The remaining number of URLs that can be refreshed each day.
         self.block_remain = block_remain
-        # The maximum number of directories that can be refreshed each day.
+        # > 
+        # *   You can call the **RefreshDcdnObjectCaches** operation to refresh content and call the **PreloadDcdnObjectCaches** operation to prefetch content.
+        # *   You can call this operation up to 20 times per second.
         self.dir_quota = dir_quota
-        # The remaining number of directories that can be refreshed each day.
+        # The maximum number of URLs that can be prefetched each day.
         self.dir_remain = dir_remain
         self.ignore_params_quota = ignore_params_quota
         self.ignore_params_remain = ignore_params_remain
-        # The maximum number of URLs that can be prefetched each day.
+        # The maximum number of URLs that can be blocked.
         self.preload_quota = preload_quota
-        # The remaining number of URLs that can be prefetched each day.
+        # The maximum number of directories that can be refreshed each day.
         self.preload_remain = preload_remain
-        # The maximum number of URLs or directories that can be refreshed by using regular expressions each day.
+        # The maximum number of URLs that can be refreshed each day.
         self.regex_quota = regex_quota
-        # The remaining number of URLs or directories that can be refreshed by using regular expressions each day.
+        # The remaining number of directories that can be refreshed each day.
         self.regex_remain = regex_remain
-        # The ID of the request.
-        self.request_id = request_id
         # The maximum number of URLs that can be refreshed each day.
+        self.request_id = request_id
+        # The remaining number of URLs that can be blocked each day.
         self.url_quota = url_quota
-        # The remaining number of URLs that can be refreshed each day.
+        # The maximum number of URLs or directories that can be refreshed by using regular expressions each day.
         self.url_remain = url_remain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20027,20 +20968,20 @@
 
 
 class DescribeDcdnRefreshTaskByIdRequest(TeaModel):
     def __init__(
         self,
         task_id: str = None,
     ):
-        # The ID of the task that you want to query. You can query task IDs by performing the following operations:
+        # The ID of the task that you want to query. The following signature algorithms require different message digest algorithms:
         # 
         # *   Perform the [RefreshDcdnObjectCaches](~~130620~~) operation to query refresh task IDs.
         # *   Perform the [PreloadDcdnObjectCaches](~~130636~~) operation to query prefetch task IDs.
         # 
-        # >  You can specify at most 10 task IDs in each call. Separate IDs with commas (,).
+        # > You can specify at most 10 task IDs in each call. Separate IDs with commas (,).
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20066,38 +21007,38 @@
         description: str = None,
         object_path: str = None,
         object_type: str = None,
         process: str = None,
         status: str = None,
         task_id: str = None,
     ):
-        # The time when the task was created. The time follows the ISO 8601 standard in the YYYY-MM-DDThh:mm:ssZ format. The time is displayed in UTC.
+        # The time when the task was created. The time follows the ISO8601 standard in the YYYY-MM-DDThh:mmZ format. The time is displayed in UTC.
         self.creation_time = creation_time
         # The error returned when the refresh or prefetch task failed. Valid values:
         # 
         # *   **Internal Error**: An internal error occurred.
         # *   **Origin Timeout**: The response from the origin server timed out.
-        # *   **Origin Return StatusCode 5XX**: The origin server returned an HTTP 5xx status code.
+        # *   **Origin Return StatusCode 5XX**: The origin server returned a 5XX error.
         self.description = description
         # The path of the refresh or prefetch object.
         self.object_path = object_path
         # The type of the refresh or prefetch task. Valid values:
         # 
         # *   **file**: refreshes an individual file.
-        # *   **directory**: refreshes files under a specified directory.
+        # *   **directory**: refreshes files under the specified directory.
         # *   **preload**: prefetches an individual file.
         self.object_type = object_type
         # The progress of the task, in percentage.
         self.process = process
         # The status of the task. Valid values:
         # 
-        # *   **Complete**: The task has completed.
+        # *   **Complete**: The task is complete.
         # *   **Pending**: The task is pending.
-        # *   **Refreshing**: The task is in progress.
-        # *   **Failed**: The task has failed.
+        # *   **Refreshing**: The task is running.
+        # *   **Failed**: The task failed.
         self.status = status
         # The ID of the task.
         self.task_id = task_id
 
     def validate(self):
         pass
 
@@ -20247,45 +21188,39 @@
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         start_time: str = None,
         status: str = None,
         task_id: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each request.
-        self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # > The end time must be later than the start time.
+        # >  The end time must be later than the start time.
+        self.domain_name = domain_name
+        # The number of tasks.
         self.end_time = end_time
-        # The path of the object. The path is used as a condition for exact matching.
-        self.object_path = object_path
-        # The type of the task.
-        # 
-        # *   **file**: URL-based refresh
-        # *   **directory**: directory-based refresh
-        # *   **preload**: URL-based prefetch
+        # The status of the task.
         # 
-        # If you set **DomainName** or **Status**, you must also set this parameter.
+        # *   **Complete**: The task has completed.
+        # *   **Refreshing**: The task is in progress.
+        # *   **Failed**: The task failed.
+        self.object_path = object_path
+        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.object_type = object_type
         self.owner_id = owner_id
-        # The number of the page to return. Valid values: **1** to **100000**.
-        self.page_number = page_number
         # The number of entries to return on each page. Default value: **20**. Maximum value: **50**. Valid values: **1** to **50**.
+        self.page_number = page_number
+        # The page number of the returned page.
         self.page_size = page_size
         self.security_token = security_token
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The number of entries returned per page.
         self.start_time = start_time
-        # The status of the task.
-        # 
-        # *   **Complete**: The task is complete.
-        # *   **Refreshing**: The task is in progress.
-        # *   **Failed**: The task failed.
+        # The ID of the request.
         self.status = status
-        # The ID of the task. A task ID is assigned when you create a refresh or prefetch task.
+        # The accelerated domain name. You can specify only one domain name in each call.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20351,39 +21286,43 @@
         description: str = None,
         object_path: str = None,
         object_type: str = None,
         process: str = None,
         status: str = None,
         task_id: str = None,
     ):
-        # The time when the task was created. The time is displayed in UTC.
+        # The URL of the object to be refreshed.
         self.creation_time = creation_time
-        # The type of error returned when the refresh or prefetch task has failed.
-        # 
-        # *   **InternalError**: An internal error occurred.
-        # *   **OriginTimeout**: The response from the origin server timed out.
-        # *   **OriginReturn StatusCode 5XX**: The origin server returned a 5XX error.
-        self.description = description
-        # The URL of the object refreshed.
-        self.object_path = object_path
         # The type of the task.
         # 
         # *   **file**: URL-based refresh
         # *   **path**: directory-based refresh
         # *   **preload**: URL-based prefetch
-        self.object_type = object_type
-        # The progress of the task in percentage.
-        self.process = process
+        self.description = description
         # The status of the task.
         # 
-        # *   **Complete**: The task is complete.
+        # *   **Complete**: The task has completed.
         # *   **Refreshing**: The task is in progress.
         # *   **Failed**: The task failed.
-        self.status = status
+        self.object_path = object_path
         # The ID of the task.
+        self.object_type = object_type
+        # > 
+        # *   You can query the status information by task ID or URL.
+        # *   You can set both the **TaskId** parameter and the **ObjectPath** parameter to query. If you set neither the **TaskId** parameter nor the **ObjectPath** parameter, the data in the last 3 days on the first page is returned. By default, a maximum of 20 entries can be displayed on each page.
+        # *   If you specify the **DomainName** or **Status** parameter, you must also specify the **ObjectType** parameter.
+        # *   You can call this operation up to 10 times per second per account.
+        self.process = process
+        # The type of error returned when the refresh or prefetch task has failed.
+        # 
+        # *   **InternalError**: An internal error occurred.
+        # *   **OriginTimeout**: The response from the origin server timed out.
+        # *   **OriginReturn StatusCode 5XX**: The origin server returned a 5XX error.
+        self.status = status
+        # The URL of the object to be refreshed.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20466,23 +21405,31 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         tasks: DescribeDcdnRefreshTasksResponseBodyTasks = None,
         total_count: int = None,
     ):
-        # The page number of the returned page.
+        # The status of the task.
+        # 
+        # *   **Complete**: The task has completed.
+        # *   **Refreshing**: The task is in progress.
+        # *   **Failed**: The task failed.
         self.page_number = page_number
-        # The number of entries returned per page.
+        # The time when the task was created. The time is displayed in UTC.
         self.page_size = page_size
-        # The ID of the request.
-        self.request_id = request_id
         # Details about tasks.
+        self.request_id = request_id
+        # The progress of the task, in percentage.
         self.tasks = tasks
-        # The number of tasks.
+        # The type of the task.
+        # 
+        # *   **file**: URL-based refresh
+        # *   **path**: directory-based refresh
+        # *   **preload**: URL-based prefetch
         self.total_count = total_count
 
     def validate(self):
         if self.tasks:
             self.tasks.validate()
 
     def to_map(self):
@@ -20598,17 +21545,15 @@
 
 class DescribeDcdnRegionAndIspResponseBodyIspsIsp(TeaModel):
     def __init__(
         self,
         name_en: str = None,
         name_zh: str = None,
     ):
-        # The English name of the ISP.
         self.name_en = name_en
-        # The Chinese name of the ISP.
         self.name_zh = name_zh
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20668,17 +21613,15 @@
 
 class DescribeDcdnRegionAndIspResponseBodyRegionsRegion(TeaModel):
     def __init__(
         self,
         name_en: str = None,
         name_zh: str = None,
     ):
-        # The English name of the region.
         self.name_en = name_en
-        # The Chinese name of the region.
         self.name_zh = name_zh
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20739,19 +21682,16 @@
 class DescribeDcdnRegionAndIspResponseBody(TeaModel):
     def __init__(
         self,
         isps: DescribeDcdnRegionAndIspResponseBodyIsps = None,
         regions: DescribeDcdnRegionAndIspResponseBodyRegions = None,
         request_id: str = None,
     ):
-        # The list of ISPs.
         self.isps = isps
-        # The list of regions.
         self.regions = regions
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.isps:
             self.isps.validate()
         if self.regions:
             self.regions.validate()
@@ -21134,38 +22074,38 @@
         slsregion: str = None,
         sampling_rate: str = None,
         status: str = None,
         type: str = None,
     ):
         # The type of the collected logs. Default value: cdn_log_access_l1. Valid values:
         # 
-        # *   **cdn_log_access_l1**: access logs of Dynamic Route for CDN (DCDN) points of presence (POPs)
+        # *   **cdn_log_access_l1**: access logs of Dynamic Content Delivery Network (DCDN) points of presence (POPs)
         # *   **cdn_log_origin**: back-to-origin logs
         # *   **cdn_log_er**: EdgeRoutine logs
         self.business_type = business_type
         # The region from which logs were collected.
         self.data_center = data_center
         # The domain names from which logs were collected. You can specify one or more domain names. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
         # The name of the field. For more information about fields in real-time log entries, see [Fields in a real-time log](~~324199~~).
         self.field_name = field_name
-        # The name of the Log Service project
+        # The name of the project.
         self.project_name = project_name
         # The name of the Logstore.
         self.slslog_store = slslog_store
-        # The name of the Log Service project.
+        # The name of the log file.
         self.slsproject = slsproject
         # The region to which logs were delivered.
         self.slsregion = slsregion
         # The sampling rate.
         self.sampling_rate = sampling_rate
         # The status of real-time logs.
         # 
-        # *   **success**: The transcoded stream is uploaded.
-        # *   **fail**: The transcoded stream fails to be uploaded.
+        # *   **success**\
+        # *   **fail**\
         self.status = status
         # The type of log delivery. Only **SLS_POST** is supported.
         self.type = type
 
     def validate(self):
         pass
 
@@ -21762,15 +22702,15 @@
         self.content = content
         # The description of HTTP responses.
         self.description = description
         # The HTTP status code.
         self.http_status = http_status
         # The ID of the request.
         self.request_id = request_id
-        # The return value for HTTP requests.
+        # The return value for HTTP requests. Valid values:
         # 
         # *   0: OK.
         # *   Values other than 0: an error.
         self.ret_code = ret_code
 
     def validate(self):
         if self.content:
@@ -22073,15 +23013,15 @@
 
 
 class DescribeDcdnServiceResponseBodyOperationLocksLockReason(TeaModel):
     def __init__(
         self,
         lock_reason: str = None,
     ):
-        # The reason why the service was locked. For example, a value of financial indicates that an overdue payment exists.
+        # The reason why the instance is locked. For example, a value of financial indicates that an overdue payment exists.
         self.lock_reason = lock_reason
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22145,41 +23085,41 @@
         opening_time: str = None,
         operation_locks: DescribeDcdnServiceResponseBodyOperationLocks = None,
         request_id: str = None,
         websocket_changing_time: str = None,
         websocket_changing_type: str = None,
         websocket_type: str = None,
     ):
-        # The start time when the next billing method takes effect. The time is displayed in UTC.
+        # The time when the renewed secure DCDN takes effect. The time is displayed in UTC.
         self.changing_affect_time = changing_affect_time
-        # The next billing method that takes effect. Valid values:
+        # The new metering method for DCDN. Valid values:
         # 
-        # *   **PayByTraffic**: traffic
-        # *   **PayByBandwidth**: bandwidth
-        # *   **PayByBandwidth95**: 95th percentile bandwidth
-        # *   **PayByBandwidth_monthavg**: monthly average bandwidth
-        # *   **PayByBandwidth_month4th**: the fourth peak bandwidth in each month
-        # *   **PayByBandwidth_monthday95avg**: monthly average 95th percentile bandwidth
-        # *   **PayByBandwidth_nighthalf95**: 95th percentile bandwidth of half idle bandwidth in the nighttime
+        # *   **PayByTraffic**: pay-by-data-transfer
+        # *   **PayByBandwidth**: pay-by-bandwidth
+        # *   **PayByBandwidth95**: pay-by-95th percentile bandwidth
+        # *   **PayByBandwidth_monthavg**: pay-by-monthly average bandwidth
+        # *   **PayByBandwidth_month4th**: pay-by-fourth peak bandwidth per month
+        # *   **PayByBandwidth_monthday95avg**: pay-by-monthly average 95th percentile bandwidth
+        # *   **PayByBandwidth_nighthalf95**: pay-by-95th percentile bandwidth (50% off during nighttime)
         self.changing_charge_type = changing_charge_type
         # The ID of the instance.
         self.instance_id = instance_id
-        # The current billing method. Valid values:
+        # The current metering method. Valid values:
         # 
-        # *   **PayByTraffic**: traffic
-        # *   **PayByBandwidth**: bandwidth
-        # *   **PayByBandwidth95**: 95th percentile bandwidth
-        # *   **PayByBandwidth_monthavg**: monthly average bandwidth
-        # *   **PayByBandwidth_month4th**: the fourth peak bandwidth in each month
-        # *   **PayByBandwidth_monthday95avg**: monthly average 95th percentile bandwidth
-        # *   **PayByBandwidth_nighthalf95**: 95th percentile bandwidth of half idle bandwidth in the nighttime
+        # *   **PayByTraffic**: pay-by-data-transfer
+        # *   **PayByBandwidth**: pay-by-bandwidth
+        # *   **PayByBandwidth95**: pay-by-95th percentile bandwidth
+        # *   **PayByBandwidth_monthavg**: pay-by-monthly average bandwidth
+        # *   **PayByBandwidth_month4th**: pay-by-fourth peak bandwidth per month
+        # *   **PayByBandwidth_monthday95avg**: pay-by-monthly average 95th percentile bandwidth
+        # *   **PayByBandwidth_nighthalf95**: pay-by-95th percentile bandwidth (50% off during nighttime)
         self.internet_charge_type = internet_charge_type
         # The time when the DCDN service was activated. The time follows the ISO 8601 standard.
         self.opening_time = opening_time
-        # The lock status of the DCDN service.
+        # The lock status of secure DCDN.
         self.operation_locks = operation_locks
         # The ID of the request.
         self.request_id = request_id
         # The time when the changes of the WebSocket configuration take effect. The value is the same as that of the ChangingAffectTime parameter. This parameter can be displayed in the console only if the specified time is later than the current time.
         self.websocket_changing_time = websocket_changing_time
         # The next effective billing method of WebSocket. Valid values: **websockettraffic** and **websocketbps**. A value of websockettraffic indicates that you are billed based on the traffic volume. A value of websocketbps indicates that you are billed based on the bandwidth.
         self.websocket_changing_type = websocket_changing_type
@@ -22771,27 +23711,27 @@
         max_bps: int = None,
         max_bps_time: str = None,
         rank: int = None,
         total_access: int = None,
         total_traffic: str = None,
         traffic_percent: str = None,
     ):
-        # The name of the accelerated domain.
+        # The domain name.
         self.domain_name = domain_name
-        # The peak bandwidth.
+        # The peak bandwidth value.
         self.max_bps = max_bps
         # The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         self.max_bps_time = max_bps_time
-        # The ranking of the domains.
+        # The ranking of the accelerated domain name.
         self.rank = rank
-        # The number of visits to the URL that was queried.
+        # The number of visits to the URL.
         self.total_access = total_access
-        # The total amount of network traffic.
+        # The total volume of traffic.
         self.total_traffic = total_traffic
-        # The proportion of the network traffic that was consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.traffic_percent = traffic_percent
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22879,19 +23819,19 @@
         start_time: str = None,
         top_domains: DescribeDcdnTopDomainsByFlowResponseBodyTopDomains = None,
     ):
         # The total number of accelerated domains under your account.
         self.domain_count = domain_count
         # The total number of accelerated domains that are in the **Enabled** state under your account.
         self.domain_online_count = domain_online_count
-        # The end of the time range during which the data was collected.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range during which the data was collected.
+        # The beginning of the time range during which data was queried.
         self.start_time = start_time
         # The top N domain names ranked by network traffic.
         self.top_domains = top_domains
 
     def validate(self):
         if self.top_domains:
             self.top_domains.validate()
@@ -23279,23 +24219,19 @@
     def __init__(
         self,
         end_time: str = None,
         start_time: str = None,
     ):
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard
-        # 
-        # in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end time must be later than the start time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard
-        # 
-        # in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23326,34 +24262,34 @@
         dimension: str = None,
         end_time: str = None,
         product: str = None,
         start_time: str = None,
     ):
         # The metering method. Valid values:
         # 
-        # *   **hour_flow**: pay by data transfer per hour
-        # *   **day_bandwidth**: pay by bandwidth per day
-        # *   **month\_95**: pay by 95th percentile
+        # *   **hour_flow**: pay by hourly traffic
+        # *   **day_bandwidth**: pay by daily bandwidth
+        # *   **month\_95**: pay by monthly 95th percentile
         # *   **month_avg_day_bandwidth**: pay by average daily peak bandwidth per month
         # *   **month\_4th_day_bandwidth**: pay by 4th peak bandwidth per month
         # *   **month_avg_day\_95**: pay by average daily 95th percentile per month
-        # *   **month\_95\_night_half**: pay by 95th percentile (50 % off during nighttime)
+        # *   **month\_95\_night_half**: pay by 95th percentile (50% off during nighttime)
         # *   **hour_vas**: pay by value-added service per month
         # *   **quic_hour_count**: pay by QUIC request per hour
         # *   **hour_count**: pay by request per hour
-        # *   **rtlog_count_day**: pay by real-time log entry
+        # *   **rtlog_count_day**: pay by the number of real-time logs per day
         self.bill_type = bill_type
         # The billing cycle.
         self.billing_cycle = billing_cycle
         # The dimension. Valid values:
         # 
         # *   **flow**: network traffic and bandwidth
         # *   **vas**: value-added services (HTTPS and requests for dynamic content)
         # *   **websocket**: WebSocket
-        # *   **quic**: the number of QUIC requests
+        # *   **quic**: QUIC requests
         # *   **rtlog2sls**: log entries delivered to Log Service in real time
         self.dimension = dimension
         # The time when the metering method ends.
         self.end_time = end_time
         # The name of the service.
         self.product = product
         # The time when the metering method takes effect.
@@ -24299,15 +25235,15 @@
         # The accelerated domain name.
         self.domain_name = domain_name
         # Specifies whether the feature that is specified by the FuncId parameter is enabled. Valid values:
         # 
         # *   **config**: enabled
         # *   **unconfig**: not enabled
         self.func_filter = func_filter
-        # The ID of the feature. For more information about how to query feature IDs, see [Feature settings for a domain name](~~410622~~). For example, the ID of the origin host feature (set_req_host_header) is 18.
+        # The ID of the feature. For more information about how to query feature IDs, see [Parameters for configuring features for domain names](~~410622~~). For example, the ID of the origin host feature (set_req_host_header) is 18.
         self.func_id = func_id
         # The number of the page to return. Default value: **1**. Valid values: **1 to 100000**.
         self.page_number = page_number
         # The number of entries to return on each page. Default value: **20**. Valid values: **1 to 500**.
         self.page_size = page_size
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
@@ -24461,22 +25397,22 @@
         self.cname = cname
         # The reason why the accelerated domain name failed the review.
         self.description = description
         # The accelerated domain name.
         self.domain_name = domain_name
         # The status of the accelerated domain name. Valid values:
         # 
-        # *   **online**: enabled
-        # *   **offline**: disabled
-        # *   **configuring**: configuring
-        # *   **configure_failed**: configuration failed
-        # *   **checking**: reviewing
-        # *   **check_failed**: failed the review
+        # *   **online**\
+        # *   **offline**\
+        # *   **configuring**\
+        # *   **configure_failed**\
+        # *   **checking**\
+        # *   **check_failed**\
         self.domain_status = domain_status
-        # The time when the accelerated domain name was added.
+        # The time when the accelerated domain name was added to Dynamic Content Delivery Network (DCDN).
         self.gmt_created = gmt_created
         # The time when the accelerated domain name was modified.
         self.gmt_modified = gmt_modified
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         # Indicates whether the accelerated domain name was in a sandbox.
         self.sandbox = sandbox
@@ -24586,21 +25522,21 @@
         self,
         domains: DescribeDcdnUserDomainsByFuncResponseBodyDomains = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The detailed information about each accelerated domain name. The returned information is displayed in the format that is specified by the PageData parameter.
+        # The array that consists of multiple PageData parameters. The details about each accelerated domain name are included in a separate PageData parameter.
         self.domains = domains
-        # The page number of the returned page.
+        # The number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
         # The total number of domain names returned.
         self.total_count = total_count
 
     def validate(self):
         if self.domains:
             self.domains.validate()
@@ -25053,16 +25989,16 @@
         security_token: str = None,
         status: str = None,
     ):
         self.owner_id = owner_id
         self.security_token = security_token
         # The status of the resource plan. Valid values:
         # 
-        # *   **valid**: The resource plan is valid.
-        # *   **closed**: The resource plan is expired.
+        # *   **valid**: valid
+        # *   **closed**: expired
         # *   If you leave this parameter empty, all resource plans are queried.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -25108,29 +26044,29 @@
         # The remaining quota of the resource plan.
         # 
         # *   The unit for traffic: bytes.
         # *   The unit for requests: count.
         self.curr_capacity = curr_capacity
         # The name of the resource plan.
         self.display_name = display_name
-        # The time when the resource plan expires. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The expiration time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time
         # The total quota of the resource plan.
         # 
         # *   The unit for traffic: bytes.
         # *   The unit for requests: count.
         self.init_capacity = init_capacity
         # The ID of the resource plan.
         self.instance_id = instance_id
-        # The time when the resource plan takes effect. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The validation time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
         # The status of the resource plan. Valid values:
         # 
-        # *   **valid**: The resource plan is valid.
-        # *   **closed**: The resource package is expired.
+        # *   **valid**: valid
+        # *   **closed**: expired
         self.status = status
         # The name of the template.
         self.template_name = template_name
 
     def validate(self):
         pass
 
@@ -25457,33 +26393,33 @@
         object: str = None,
         page_number: int = None,
         page_size: int = None,
         rule_name: str = None,
         sec_func: str = None,
         start_time: str = None,
     ):
-        # The domain name.
+        # The number of the page to return. Pages start from page 1.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0. Example: 2006-01-02T15:05:04Z.
-        # 
-        # >  The end time must be later than the start time.
+        # The ID of the request.
         self.end_time = end_time
-        # The language. Valid values: en and zh. Default value: en
+        # The number of the returned page.
         self.lang = lang
-        # The object that triggered the rule.
+        # The number of entries to return on each page. Maximum value: 100.
         self.object = object
-        # The number of the page to return. Pages start from page 1.
+        # The total number of entries returned.
         self.page_number = page_number
-        # The number of entries to return on each page. Maximum value: 100.
+        # The description of HTTP responses.
         self.page_size = page_size
-        # The rule that was triggered.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0. Example: 2006-01-02T15:05:04Z.
+        # 
+        # >  The end time must be later than the start time.
         self.rule_name = rule_name
-        # The name of the security feature.
-        self.sec_func = sec_func
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0. Example: 2006-01-02T15:04:04Z.
+        self.sec_func = sec_func
+        # The language. Valid values: en and zh. Default value: en
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25540,25 +26476,25 @@
         domain: str = None,
         drops: int = None,
         object: str = None,
         rule_name: str = None,
         sec_func: str = None,
         tm_str: str = None,
     ):
-        # The domain name.
+        # The security feature that blocked the packets.
         self.domain = domain
-        # The number of packets blocked within 5 minutes.
+        # >  The maximum number of times that users can call this operation per second is 50.
         self.drops = drops
-        # The object that triggered the rule.
+        # The total number of entries returned.
         self.object = object
-        # The rule that is triggered.
+        # The total number of entries returned.
         self.rule_name = rule_name
-        # The security feature that blocked the packets.
+        # The array returned.
         self.sec_func = sec_func
-        # The beginning of the time range that was queried. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is in UTC+0.
+        # The rule that is triggered.
         self.tm_str = tm_str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25604,27 +26540,27 @@
         len: int = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         rows: List[DescribeDcdnUserSecDropByMinuteResponseBodyRows] = None,
         total_count: int = None,
     ):
-        # The description of HTTP responses.
-        self.description = description
         # The total number of entries returned.
+        self.description = description
+        # The array returned.
         self.len = len
-        # The number of the returned page.
+        # The domain name.
         self.page_number = page_number
-        # The number of entries returned on each page.
+        # The beginning of the time range that was queried. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is in UTC+0.
         self.page_size = page_size
-        # The ID of the request.
+        # The number of entries returned on each page.
         self.request_id = request_id
-        # The array returned.
+        # The object that triggered the rule.
         self.rows = rows
-        # The total number of entries returned.
+        # The number of packets blocked within 5 minutes.
         self.total_count = total_count
 
     def validate(self):
         if self.rows:
             for k in self.rows:
                 if k:
                     k.validate()
@@ -25721,17 +26657,16 @@
 
 class DescribeDcdnUserTagsResponseBodyTags(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: List[str] = None,
     ):
-        # The key of the returned tag.
-        self.key = key
         # The value of the returned tag.
+        self.key = key
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25756,17 +26691,17 @@
 
 class DescribeDcdnUserTagsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tags: List[DescribeDcdnUserTagsResponseBodyTags] = None,
     ):
-        # The ID of the request.
-        self.request_id = request_id
         # The tags.
+        self.request_id = request_id
+        # The key of the returned tag.
         self.tags = tags
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -26154,15 +27089,15 @@
 
 
 class DescribeDcdnWafDomainDetailRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each request. Exact match is supported.
+        # The types of the protection policies.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26184,23 +27119,16 @@
 class DescribeDcdnWafDomainDetailResponseBodyDomainDefenseScenes(TeaModel):
     def __init__(
         self,
         defense_scene: str = None,
         policy_id: int = None,
         policy_ids: str = None,
     ):
-        # The type of the protection policy. Valid values:
-        # 
-        # *   waf_group: basic web protection
-        # *   custom_acl: custom protection
-        # *   whitelist: IP address whitelist
         self.defense_scene = defense_scene
-        # The ID of the protection policy. If multiple IDs exist, only one ID is returned.
         self.policy_id = policy_id
-        # The IDs of the protection policies. Multiple IDs are separated by commas (,).
         self.policy_ids = policy_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26229,17 +27157,15 @@
 
 class DescribeDcdnWafDomainDetailResponseBodyDomain(TeaModel):
     def __init__(
         self,
         defense_scenes: List[DescribeDcdnWafDomainDetailResponseBodyDomainDefenseScenes] = None,
         domain_name: str = None,
     ):
-        # The types of the protection policies.
         self.defense_scenes = defense_scenes
-        # The accelerated domain name.
         self.domain_name = domain_name
 
     def validate(self):
         if self.defense_scenes:
             for k in self.defense_scenes:
                 if k:
                     k.validate()
@@ -26272,17 +27198,21 @@
 
 class DescribeDcdnWafDomainDetailResponseBody(TeaModel):
     def __init__(
         self,
         domain: DescribeDcdnWafDomainDetailResponseBodyDomain = None,
         request_id: str = None,
     ):
-        # The information about the accelerated domain name.
+        # The IDs of the protection policies. Multiple IDs are separated by commas (,).
         self.domain = domain
-        # The ID of the request.
+        # The type of the protection policy. Valid values:
+        # 
+        # *   waf_group: basic web protection
+        # *   custom_acl: custom protection
+        # *   whitelist: IP address whitelist
         self.request_id = request_id
 
     def validate(self):
         if self.domain:
             self.domain.validate()
 
     def to_map(self):
@@ -27126,25 +28056,25 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         page_number: int = None,
         page_size: int = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
-        # The end of the time range to query the logs.
+        # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time
-        # The number of the page to return. Valid values: positive integers.
+        # The number of the page to return. Valid values: an integer greater than 0.
         self.page_number = page_number
         # The number of entries to return on each page. Default value: **300**. Valid values: **1 to 1000**.
         self.page_size = page_size
-        # The beginning of the time range to query the logs.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -27289,15 +28219,15 @@
     ):
         # The WAF domain name.
         self.domain_name = domain_name
         # The total number of entries returned on the current page.
         self.log_count = log_count
         # The log information.
         self.log_infos = log_infos
-        # The page information. The page information is indicated by the PageInfoDetail parameter.
+        # The page information.
         self.page_infos = page_infos
 
     def validate(self):
         if self.log_infos:
             for k in self.log_infos:
                 if k:
                     k.validate()
@@ -27341,15 +28271,15 @@
 
 class DescribeDcdnWafLogsResponseBody(TeaModel):
     def __init__(
         self,
         domain_log_details: List[DescribeDcdnWafLogsResponseBodyDomainLogDetails] = None,
         request_id: str = None,
     ):
-        # Details about domain logs.
+        # Details about logs returned.
         self.domain_log_details = domain_log_details
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.domain_log_details:
             for k in self.domain_log_details:
@@ -27695,15 +28625,15 @@
         policy_type: str = None,
         rule_configs: str = None,
         rule_count: int = None,
     ):
         # The type of the protection policy. Valid values:
         # 
         # *   waf_group: basic web protection
-        # *   custom_acl: custom
+        # *   custom_acl: custom protection
         # *   whitelist: whitelist
         self.defense_scene = defense_scene
         # The number of domain names that use the protection policy.
         self.domain_count = domain_count
         # The time when the protection policy was modified. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.gmt_modified = gmt_modified
         # The ID of the protection policy.
@@ -27713,18 +28643,18 @@
         # The status of the protection policy. Valid values:
         # 
         # *   on
         # *   off
         self.policy_status = policy_status
         # Indicates whether the current policy is the default policy. Valid values:
         # 
-        # *   default: The current policy is the default policy.
-        # *   custom: The current policy is not the default policy.
+        # *   default
+        # *   custom
         self.policy_type = policy_type
-        # The protection rule configurations corresponding to the protection policy. The configurations only support Bot management. For more information, see [Configure protection rules](~~423350~~).
+        # The protection rule configurations that are defined in the protection policy. The configurations only support bot management. For more information, see [Configure protection rules](~~423350~~).
         self.rule_configs = rule_configs
         # The number of protection rules in the protection policy.
         self.rule_count = rule_count
 
     def validate(self):
         pass
 
@@ -27861,19 +28791,19 @@
 class DescribeDcdnWafPolicyDomainsRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         policy_id: int = None,
     ):
-        # The number of the page to return. Valid values: **1** to **100000**. Default value: **1**.
+        # The page number of the returned page, which is the same as the PageNumber parameter in request parameters.
         self.page_number = page_number
-        # The number of domain names to return per page. Valid values: an integer from **1** to **500**. Default value: **20**.
+        # The total number of domain names returned.
         self.page_size = page_size
-        # The ID of the protection policy. You can specify only one ID in each request.
+        # The ID of the request.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27933,21 +28863,21 @@
         self,
         domains: List[DescribeDcdnWafPolicyDomainsResponseBodyDomains] = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The accelerated domain names.
+        # The ID of the protection policy. You can specify only one ID in each request.
         self.domains = domains
-        # The page number of the returned page, which is the same as the PageNumber parameter in request parameters.
+        # >You can call this operation up to 20 times per second per account.
         self.page_number = page_number
-        # The number of domain names returned per page, which is the same as the PageSize parameter in request parameters.
+        # The accelerated domain names.
         self.page_size = page_size
-        # The ID of the request.
+        # The accelerated domain name that was protected by the specified protection policy.
         self.request_id = request_id
         # The total number of domain names returned.
         self.total_count = total_count
 
     def validate(self):
         if self.domains:
             for k in self.domains:
@@ -28500,19 +29430,19 @@
         self,
         page_number: int = None,
         page_size: int = None,
         query_args: str = None,
     ):
         # The number of the page to return. Valid values: **1** to **100000**. Default value: **1**.
         self.page_number = page_number
-        # The number of protection rules to return per page. Valid values: an integer from **1** to **500**. Default value: **20**.
+        # The number of protection rules to return per page. Valid values: integers from **1** to **500**. Default value: **20**.
         self.page_size = page_size
-        # The query conditions. The value is a string in the JSON format: `QueryArgs={"PolicyIds":"The range of protection policy IDs","RuleIds":"The range of protection rule IDs","RuleNameLike":"The name of the protection rule","DomainNames":"The protected domain names","DefenseScenes":"waf_group","RuleStatus":"on","OrderBy":"GmtModified","Desc":"false"}`
+        # The query conditions. The value needs to be a JSON string in the following format: `QueryArgs={"PolicyIds":"The range of protection policy IDs","RuleIds":"The range of protection rule IDs","RuleNameLike":"The name of the protection rule","DomainNames":"The protected domain names","DefenseScenes":"waf_group","RuleStatus":"on","OrderBy":"GmtModified","Desc":"false"}`.
         # 
-        # >  If you do not specify this parameter, all protection rules are queried.
+        # > If you do not specify this parameter, all protection rules are queried.
         self.query_args = query_args
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28546,27 +29476,27 @@
         gmt_modified: str = None,
         policy_id: int = None,
         rule_config: str = None,
         rule_id: int = None,
         rule_name: str = None,
         rule_status: str = None,
     ):
-        # The type of the protection policy, which is the same as the DefenseScenes field in the QueryArgs parameter.
+        # The type of the protection policy. The value of this parameter is the same as that of the DefenseScene field in QueryArgst.
         self.defense_scene = defense_scene
-        # The modification time. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The time when the protection policy was last modified. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.gmt_modified = gmt_modified
         # The ID of the protection policy.
         self.policy_id = policy_id
         # The configuration information about the protection rule.
         self.rule_config = rule_config
         # The ID of the protection rule.
         self.rule_id = rule_id
         # The name of the protection rule.
         self.rule_name = rule_name
-        # The status of the protection rule, which is the same as the RuleStatus field in the QueryArgs parameter.
+        # The status of the protection rule. The value of this parameter is the same as that of the RuleStatus field in QueryArgst.
         self.rule_status = rule_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28614,17 +29544,17 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         rules: List[DescribeDcdnWafRulesResponseBodyRules] = None,
         total_count: int = None,
     ):
-        # The page number of the returned page, which is the same as the PageNumber parameter in request parameters.
+        # The page number of the returned page. The value of this parameter is the same as that of the PageNumber parameter in the request.
         self.page_number = page_number
-        # The number of protection rules returned per page, which is the same as the PageSize parameter in request parameters.
+        # The number of protection rules returned per page. The value of this parameter is the same as that of the PageSize parameter in the request.
         self.page_size = page_size
         # The ID of the request.
         self.request_id = request_id
         # The information about the protection rule.
         self.rules = rules
         # The total number of protection rules.
         self.total_count = total_count
@@ -30300,15 +31230,15 @@
 
 
 class DescribeRoutineRequest(TeaModel):
     def __init__(
         self,
         name: str = None,
     ):
-        # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        # The metadata of the routine. The next table describes the fields.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30329,17 +31259,17 @@
 
 class DescribeRoutineResponseBody(TeaModel):
     def __init__(
         self,
         content: Dict[str, Any] = None,
         request_id: str = None,
     ):
-        # The metadata of the routine. The next table describes the fields.
-        self.content = content
         # The ID of the request.
+        self.content = content
+        # The operation that you want to perform. Set the value to **DescribeRoutine**.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30408,17 +31338,17 @@
 
 class DescribeRoutineCanaryEnvsResponseBody(TeaModel):
     def __init__(
         self,
         content: Dict[str, Any] = None,
         request_id: str = None,
     ):
-        # The canary release environments that are supported by the edge routine.
-        self.content = content
         # The ID of the region.
+        self.content = content
+        # The operation that you want to perform. Set the value to **DescribeRoutineCanaryEnvs**.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30522,15 +31452,15 @@
 
 class DescribeRoutineCodeRevisionResponseBody(TeaModel):
     def __init__(
         self,
         content: Dict[str, Any] = None,
         request_id: str = None,
     ):
-        # The JavaScript code returned.
+        # The information about the JavaScript code version.
         self.content = content
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -30797,17 +31727,17 @@
         in_debt: bool = None,
         in_debt_overdue: bool = None,
         on_service: bool = None,
         request_id: str = None,
     ):
         # Indicates whether the IPA service is activated.
         self.enabled = enabled
-        # Indicates whether your IPA service has overdue payments.
+        # Indicates whether you have overdue payments.
         self.in_debt = in_debt
-        # Indicates whether an overdue bill has been paid within a specified period.
+        # Indicates whether the grace period for your overdue payments expired.
         self.in_debt_overdue = in_debt_overdue
         # Indicates whether the IPA service is available. The IPA service is available when no payment is overdue.
         self.on_service = on_service
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
@@ -30924,17 +31854,17 @@
         in_debt: bool = None,
         in_debt_overdue: bool = None,
         on_service: bool = None,
         request_id: str = None,
     ):
         # Indicates whether the DCDN service is activated.
         self.enabled = enabled
-        # Indicates whether the DCDN service has overdue payments.
+        # Indicates whether your account has overdue payments.
         self.in_debt = in_debt
-        # Indicates whether an overdue bill has been paid within the specified period.
+        # Indicates whether the grace period for your overdue payments expired.
         self.in_debt_overdue = in_debt_overdue
         # Indicates whether the service is available.
         self.on_service = on_service
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
@@ -31051,31 +31981,31 @@
         in_debt: bool = None,
         in_debt_overdue: bool = None,
         on_service: bool = None,
         request_id: str = None,
     ):
         # Indicates whether ER is activated.
         # 
-        # *   true: activated
-        # *   false: not activated
+        # *   true
+        # *   false
         self.enabled = enabled
         # Indicates whether ER has an overdue payment.
         # 
-        # *   true: has an overdue payment
-        # *   false: does not have an overdue payment
+        # *   true
+        # *   false
         self.in_debt = in_debt
         # Indicates whether an overdue payment of ER has passed the grace period.
         # 
-        # *   true: has passed the grace period
-        # *   false: has not passed the grace period
+        # *   true
+        # *   false
         self.in_debt_overdue = in_debt_overdue
         # Indicates whether ER is available.
         # 
-        # *   true: available
-        # *   false: unavailable
+        # *   true
+        # *   false
         self.on_service = on_service
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -31196,31 +32126,31 @@
         in_debt: bool = None,
         in_debt_overdue: bool = None,
         on_service: bool = None,
         request_id: str = None,
     ):
         # Indicates whether Log Service is activated.
         # 
-        # *   true: activated
-        # *   false: not activated
+        # *   true
+        # *   false
         self.enabled = enabled
         # Indicates whether your Log Service has overdue payments.
         # 
-        # *   true: Your Log Service has overdue payments.
-        # *   false: Your Log Service does not have overdue payments.
+        # *   true
+        # *   false
         self.in_debt = in_debt
-        # Indicates whether the overdue payments of Log Service have passed the grace period.
+        # Indicates whether an overdue payment of your Log Service has passed the grace period.
         # 
-        # *   true: The overdue payments of Log Service have passed the grace period.
-        # *   false: The overdue payments of Log Service have not passed the grace period.
+        # *   true
+        # *   false
         self.in_debt_overdue = in_debt_overdue
         # Indicates whether Log Service is available.
         # 
-        # *   true: available
-        # *   false: unavailable
+        # *   true
+        # *   false
         self.on_service = on_service
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -31480,17 +32410,17 @@
 
 class GetDcdnKvRequest(TeaModel):
     def __init__(
         self,
         key: str = None,
         namespace: str = None,
     ):
-        # The name of the key that you want to query.
-        self.key = key
         # The name of the namespace.
+        self.key = key
+        # Queries the value of the key in a key-value pair.
         self.namespace = namespace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31515,17 +32445,17 @@
 
 class GetDcdnKvResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         value: str = None,
     ):
-        # The ID of the request.
-        self.request_id = request_id
         # The value of the key.
+        self.request_id = request_id
+        # The name of the key that you want to query.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31982,22 +32912,22 @@
         policy_name: str = None,
         policy_status: str = None,
     ):
         # The ID of the protection policy that you want to modify. You can specify only one ID in each request.
         self.policy_id = policy_id
         # The new name of the protection policy.
         # 
-        # >  You must specify PolicyName or PolicyStatus.
+        # > You must specify PolicyName or PolicyStatus.
         self.policy_name = policy_name
         # The new status of the protection policy. Valid values:
         # 
         # *   **on**\
         # *   **off**\
         # 
-        # >  You must specify PolicyName or PolicyStatus.
+        # > You must specify PolicyName or PolicyStatus.
         self.policy_status = policy_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32100,24 +33030,17 @@
     def __init__(
         self,
         bind_domains: str = None,
         method: int = None,
         policy_id: int = None,
         unbind_domains: str = None,
     ):
-        # The domain names that you want to bind to the protection policy. You can specify up to 50 domain names. Separate multiple domain names with commas (,).
-        # 
-        # > You can configure only one of the **BindDomains** and **UnbindDomains** parameters.
         self.bind_domains = bind_domains
         self.method = method
-        # The ID of the protection policy. You can specify only one ID in each request.
         self.policy_id = policy_id
-        # The domain names that you want to unbind from the protection policy. You can specify up to 50 domain names. Separate multiple domain names with commas (,).
-        # 
-        # > You can configure only one of the **BindDomains** and **UnbindDomains** parameters.
         self.unbind_domains = unbind_domains
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32149,15 +33072,14 @@
 
 
 class ModifyDcdnWafPolicyDomainsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32226,15 +33148,15 @@
         rule_config: str = None,
         rule_id: int = None,
         rule_name: str = None,
         rule_status: str = None,
     ):
         # The new configurations of the protection rule.
         # 
-        # >  After you modify the configurations of the protection rule, the previous configurations are overwritten.
+        # > After you modify the configurations of the protection rule, the previous configurations are overwritten.
         self.rule_config = rule_config
         # The ID of the protection rule. You can specify only one ID in each request.
         self.rule_id = rule_id
         # The new name of the protection rule.
         self.rule_name = rule_name
         # The new status of the protection rule. Valid values:
         # 
@@ -32478,26 +33400,26 @@
         owner_id: int = None,
         security_token: str = None,
         with_header: str = None,
     ):
         # The acceleration region in which you want to prefetch content. If you do not specify a region, the value overseas is used.
         # 
         # *   **domestic**: Chinese mainland
-        # *   **overseas**: global (excluding the Chinese mainland)
+        # *   **overseas**: outside the Chinese mainland
         self.area = area
-        # Specifies whether to prefetch content to POPs. Default value: false. Valid values:
+        # Specifies whether to prefetch content to POPs. Valid values:
         # 
-        # *   **true**: prefetches content to POPs that include L2 POPs.
+        # *   **true**: prefetches content to nodes that include L2 DCDN nodes.
         # *   **false**: prefetches content to L2 POPs or L3 POPs.
         self.l_2preload = l_2preload
         # The path of the content that you want to prefetch. Separate multiple URLs with line feed characters (\n) or a pair of carriage return and line feed characters (\r\n).
         self.object_path = object_path
         self.owner_id = owner_id
         self.security_token = security_token
-        # The custom header for prefetch in JSON format.
+        # The custom header for prefetch in the JSON format.
         self.with_header = with_header
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32617,15 +33539,15 @@
 
 class PublishDcdnStagingConfigToProductionRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         function_name: str = None,
     ):
-        # The name of the accelerated domain. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
         # The name of the feature.
         self.function_name = function_name
 
     def validate(self):
         pass
 
@@ -32728,16 +33650,18 @@
         envs: Dict[str, Any] = None,
         name: str = None,
         select_code_revision: str = None,
     ):
         # The environment to which you want to publish the code.
         # 
         # > 
+        # 
         # *   production: the name of the environment, including the environment name (SpecName) and the domain name whitelist (AllowedHosts).
-        # *   presetCanary: **You can add canary release environments based on your business requirements. This parameter is optional.
+        # 
+        # *   Preset_Canary_xx: You can add canary release environments based on your business requirements. This parameter is optional.
         self.envs = envs
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
         self.name = name
         # The version of the routine code that you want to publish.
         self.select_code_revision = select_code_revision
 
     def validate(self):
@@ -32774,16 +33698,18 @@
         envs_shrink: str = None,
         name: str = None,
         select_code_revision: str = None,
     ):
         # The environment to which you want to publish the code.
         # 
         # > 
+        # 
         # *   production: the name of the environment, including the environment name (SpecName) and the domain name whitelist (AllowedHosts).
-        # *   presetCanary: **You can add canary release environments based on your business requirements. This parameter is optional.
+        # 
+        # *   Preset_Canary_xx: You can add canary release environments based on your business requirements. This parameter is optional.
         self.envs_shrink = envs_shrink
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
         self.name = name
         # The version of the routine code that you want to publish.
         self.select_code_revision = select_code_revision
 
     def validate(self):
@@ -32818,15 +33744,15 @@
     def __init__(
         self,
         content: Dict[str, Any] = None,
         request_id: str = None,
     ):
         # The version of the routine code that is published to the specified environment.
         self.content = content
-        # The ID of the region.
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32896,19 +33822,19 @@
 class PutDcdnKvRequest(TeaModel):
     def __init__(
         self,
         key: str = None,
         namespace: str = None,
         value: str = None,
     ):
-        # The name of the key. The name can be up to 512 characters in length, and cannot contain spaces.
+        # The length of the key.
         self.key = key
-        # The name of the namespace.
-        self.namespace = namespace
         # The content of the key. The maximum size is 2 MB (2 x 1000 x 1000 bytes).
+        self.namespace = namespace
+        # The content of the key. If the value exceeds 256 characters in length, the first 100 characters and the last 100 characters are retained and other characters are discarded.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32938,19 +33864,17 @@
 class PutDcdnKvResponseBody(TeaModel):
     def __init__(
         self,
         length: int = None,
         request_id: str = None,
         value: str = None,
     ):
-        # The length of the key.
-        self.length = length
         # The ID of the request.
+        self.length = length
         self.request_id = request_id
-        # The content of the key. If the value exceeds 256 characters in length, the first 100 characters and the last 100 characters are retained and other characters are discarded.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33027,15 +33951,15 @@
         object_path: str = None,
         object_type: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
         # The path of the objects that you want to refresh. Separate multiple URLs with line feed characters (\n) or a pair of carriage return and line feed characters (\r\n).
         self.object_path = object_path
-        # The refresh type. Default value: File. Valid values:
+        # The refresh type. Valid values:
         # 
         # *   **File**: URL
         # *   **Directory**: directory
         self.object_type = object_type
         self.owner_id = owner_id
         self.security_token = security_token
 
@@ -33151,15 +34075,15 @@
 
 
 class RollbackDcdnStagingConfigRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # >  You can call this operation up to 30 times per second per account.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33179,15 +34103,15 @@
 
 
 class RollbackDcdnStagingConfigResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The accelerated domain name. You can specify only one domain name in each call.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33260,43 +34184,41 @@
         owner_id: int = None,
         region: str = None,
         sslpri: str = None,
         sslprotocol: str = None,
         sslpub: str = None,
         security_token: str = None,
     ):
-        # The name of the certificate.
+        # Specifies whether to enable the SSL certificate. Default value: off. Valid values:
+        # 
+        # *   **on**: enables the SSL certificate.
+        # *   **off**: disables the SSL certificate.
         self.cert_name = cert_name
+        # The content of the certificate. This parameter is required only if you enable the SSL certificate.
+        self.cert_type = cert_type
         # The type of the certificate.
         # 
         # *   **upload**: a user-uploaded SSL certificate.
         # *   **cas**: a certificate that is acquired through SSL Certificates Service.
         # *   **free**: a free certificate.
         # 
         # > 
         # *   If the value of the CertType parameter is **cas**, the **SSLPri** parameter is not required.
         # *   If the value of the CertType parameter is **free**, the **SSLPri** and **SSLPub** parameters are not required.
-        self.cert_type = cert_type
-        # The accelerated domain name. You can specify only one domain name.
-        # 
-        # HTTPS acceleration must be enabled for the accelerated domain name.
         self.domain_name = domain_name
-        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information about the existing certificate that uses the same name.
+        # >  You can call this operation up to 30 times per second per account.
         self.force_set = force_set
         self.owner_id = owner_id
-        # The region. Default value: ch-hangzhou.
+        # The ID of the request.
         self.region = region
-        # The private key. This parameter is required only if you enable the SSL certificate.
+        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information about the existing certificate that uses the same name.
         self.sslpri = sslpri
-        # Specifies whether to enable the SSL certificate. Default value: off. Valid values:
-        # 
-        # *   **on**: enables the SSL certificate.
-        # *   **off**: disables the SSL certificate.
+        # The private key. This parameter is required only if you enable the SSL certificate.
         self.sslprotocol = sslprotocol
-        # The content of the certificate. This parameter is required only if you enable the SSL certificate.
+        # The region. Default value: ch-hangzhou.
         self.sslpub = sslpub
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -33353,15 +34275,15 @@
 
 
 class SetDcdnDomainCertificateResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The private key. This parameter is required only if you enable the SSL certificate.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33696,15 +34618,15 @@
         self,
         configs: str = None,
         function_id: int = None,
         owner_account: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The configuration parameters of the features.
+        # The configuration parameters of the feature.
         self.configs = configs
         # The ID of the feature.
         self.function_id = function_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.security_token = security_token
 
@@ -33821,20 +34743,17 @@
         self,
         subdomains: Dict[str, Any] = None,
     ):
         # The parameters of the subdomain.
         # 
         # The parameters are in the following format:
         # 
-        # ```
-        # 
-        # Subdomains: [
-        #     "subdomain-test"
-        # ]
-        # ```
+        #     Subdomains: [
+        #         "subdomain-test"
+        #     ]
         self.subdomains = subdomains
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33858,20 +34777,17 @@
         self,
         subdomains_shrink: str = None,
     ):
         # The parameters of the subdomain.
         # 
         # The parameters are in the following format:
         # 
-        # ```
-        # 
-        # Subdomains: [
-        #     "subdomain-test"
-        # ]
-        # ```
+        #     Subdomains: [
+        #         "subdomain-test"
+        #     ]
         self.subdomains_shrink = subdomains_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33972,15 +34888,14 @@
 class StartDcdnDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The name of the accelerated domain to be enabled. You can specify only one domain name.
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -34010,15 +34925,14 @@
 
 
 class StartDcdnDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34084,15 +34998,14 @@
 class StartDcdnIpaDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The name of the accelerated domain to be enabled. You can specify only one accelerated domain name at a time.
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -34122,15 +35035,14 @@
 
 
 class StartDcdnIpaDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34829,23 +35741,23 @@
         domain_name: str = None,
         owner_id: int = None,
         resource_group_id: str = None,
         security_token: str = None,
         sources: str = None,
         top_level_domain: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The top-level domain name.
         self.domain_name = domain_name
         self.owner_id = owner_id
-        # The ID of the resource group.
+        # The ID of the request.
         self.resource_group_id = resource_group_id
         self.security_token = security_token
-        # The information about the addresses of origin servers.
+        # The accelerated domain name. You can specify only one domain name in each call.
         self.sources = sources
-        # The top-level domain name.
+        # The operation that you want to perform. Set the value to **UpdateDcdnDomain**.
         self.top_level_domain = top_level_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34885,15 +35797,15 @@
 
 
 class UpdateDcdnDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The information about the addresses of origin servers.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -35099,23 +36011,23 @@
         # 
         # *   **cn**: Chinese mainland
         # *   **sg**: Singapore
         # *   **in**: India
         # *   **eu**: Europe
         # *   **us**: United States
         self.data_center = data_center
-        # The domain names. You can specify one or more domain names. Separate multiple domain names with commas (,).
+        # The domain names from which logs were collected. You can specify one or more domain names. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
-        # The name of the real-time log delivery project.
+        # The name of the project.
         self.project_name = project_name
         # The name of the Logstore.
         self.slslog_store = slslog_store
-        # The name of the Log Service project.
+        # The name of the log file.
         self.slsproject = slsproject
-        # The region to which logs are delivered.
+        # The region to which logs were delivered.
         self.slsregion = slsregion
         # The sampling rate.
         self.sampling_rate = sampling_rate
 
     def validate(self):
         pass
 
@@ -35166,17 +36078,17 @@
         desc: str = None,
         domain_name: str = None,
         region: str = None,
         status: str = None,
     ):
         # The description of the returned result.
         self.desc = desc
-        # The domain name for which the real-time log delivery project was updated.
+        # The domain name.
         self.domain_name = domain_name
-        # The region from which logs were collected.
+        # The name of the region.
         self.region = region
         # Indicates whether the real-time log delivery project was successfully updated. Valid values:
         # 
         # *   **success**\
         # *   **fail**\
         self.status = status
 
@@ -35334,19 +36246,17 @@
         domain_name: str = None,
         end_time: str = None,
         report_ids: str = None,
         start_time: str = None,
     ):
         # The domain names that you want to include in the operations report. If you do not specify a domain name, all domain names that belong to your Alibaba Cloud account are included.
         self.domain_name = domain_name
-        # The end time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time
-        # The IDs of operations reports that you want to update. Separate IDs with commas (,). You can call the [DescribeDcdnSubList](~~270075~~) operation to query report IDs.
+        # The operation that you want to perform. Set the value to **UpdateDcdnSubTask**.
         self.report_ids = report_ids
-        # The start time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -35378,15 +36288,14 @@
 
 
 class UpdateDcdnSubTaskResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -35597,15 +36506,15 @@
 
 class UploadRoutineCodeResponseBody(TeaModel):
     def __init__(
         self,
         content: Dict[str, Any] = None,
         request_id: str = None,
     ):
-        # The content returned that includes the code version number and information about code upload.
+        # The content returned, such as the code version number and information about the code upload.
         self.content = content
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_dcdn20180115-1.1.7/alibabacloud_dcdn20180115.egg-info/PKG-INFO` & `alibabacloud_dcdn20180115-1.1.8/alibabacloud_dcdn20180115.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dcdn20180115
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115-1.1.7/setup.py` & `alibabacloud_dcdn20180115-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dcdn20180115.
 
-Created on 19/05/2023
+Created on 22/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dcdn20180115"
 NAME = "alibabacloud_dcdn20180115" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dcdn (20180115) SDK Library for Python"
```

