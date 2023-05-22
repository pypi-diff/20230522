# Comparing `tmp/alibabacloud_dcdn20180115_py2-1.1.7.tar.gz` & `tmp/alibabacloud_dcdn20180115_py2-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dcdn20180115_py2-1.1.7.tar", last modified: Fri May 19 01:37:32 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dcdn20180115_py2-1.1.8.tar", last modified: Mon May 22 10:55:11 2023, max compression
```

## Comparing `alibabacloud_dcdn20180115_py2-1.1.7.tar` & `alibabacloud_dcdn20180115_py2-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/
--rw-r--r--   0 root         (0) root         (0)     1837 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115/__init__.py
--rw-r--r--   0 root         (0) root         (0)   394725 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115/client.py
--rw-r--r--   0 root         (0) root         (0)  1230479 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-19 01:37:32.000000 alibabacloud_dcdn20180115_py2-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2023-05-19 01:37:31.000000 alibabacloud_dcdn20180115_py2-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   377676 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/client.py
+-rw-r--r--   0 root         (0) root         (0)  1271965 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/setup.py
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/ChangeLog.md` & `alibabacloud_dcdn20180115_py2-1.1.8/ChangeLog.md`

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

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/LICENSE` & `alibabacloud_dcdn20180115_py2-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/PKG-INFO` & `alibabacloud_dcdn20180115_py2-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dcdn20180115_py2
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/README-CN.md` & `alibabacloud_dcdn20180115_py2-1.1.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/README.md` & `alibabacloud_dcdn20180115_py2-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115/client.py` & `alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
     def add_dcdn_ipa_domain_with_options(self, request, runtime):
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
@@ -216,33 +216,27 @@
 
     def add_dcdn_ipa_domain(self, request):
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
 
     def batch_add_dcdn_domain_with_options(self, request, runtime):
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
@@ -284,33 +278,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.BatchAddDcdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_add_dcdn_domain(self, request):
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
 
     def batch_create_dcdn_waf_rules_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
 
         @param request: BatchCreateDcdnWafRulesRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BatchCreateDcdnWafRulesResponse
@@ -338,15 +326,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.BatchCreateDcdnWafRulesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_create_dcdn_waf_rules(self, request):
         """
-        >  You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
 
         @param request: BatchCreateDcdnWafRulesRequest
 
         @return: BatchCreateDcdnWafRulesResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -410,16 +398,17 @@
         @return: BatchDeleteDcdnDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_delete_dcdn_domain_configs_with_options(request, runtime)
 
     def batch_delete_dcdn_waf_rules_with_options(self, request, runtime):
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        # Usage notes
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
 
         @param request: BatchDeleteDcdnWafRulesRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BatchDeleteDcdnWafRulesResponse
@@ -445,16 +434,17 @@
         return TeaCore.from_map(
             dcdn_20180115_models.BatchDeleteDcdnWafRulesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_delete_dcdn_waf_rules(self, request):
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
@@ -506,15 +496,15 @@
         @return: BatchModifyDcdnWafRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_modify_dcdn_waf_rules_with_options(request, runtime)
 
     def batch_set_dcdn_domain_certificate_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 10 times per second per account.
+        > You can call this operation up to 10 times per second per account.
         
 
         @param request: BatchSetDcdnDomainCertificateRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BatchSetDcdnDomainCertificateResponse
@@ -556,15 +546,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.BatchSetDcdnDomainCertificateResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_set_dcdn_domain_certificate(self, request):
         """
-        >  You can call this operation up to 10 times per second per account.
+        > You can call this operation up to 10 times per second per account.
         
 
         @param request: BatchSetDcdnDomainCertificateRequest
 
         @return: BatchSetDcdnDomainCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -622,15 +612,15 @@
         @return: BatchSetDcdnDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_set_dcdn_domain_configs_with_options(request, runtime)
 
     def batch_set_dcdn_ipa_domain_configs_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: BatchSetDcdnIpaDomainConfigsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BatchSetDcdnIpaDomainConfigsResponse
@@ -664,28 +654,29 @@
         return TeaCore.from_map(
             dcdn_20180115_models.BatchSetDcdnIpaDomainConfigsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_set_dcdn_ipa_domain_configs(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: BatchSetDcdnIpaDomainConfigsRequest
 
         @return: BatchSetDcdnIpaDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_set_dcdn_ipa_domain_configs_with_options(request, runtime)
 
     def batch_set_dcdn_waf_domain_configs_with_options(self, request, runtime):
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
 
         @param request: BatchSetDcdnWafDomainConfigsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BatchSetDcdnWafDomainConfigsResponse
@@ -715,16 +706,17 @@
         return TeaCore.from_map(
             dcdn_20180115_models.BatchSetDcdnWafDomainConfigsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_set_dcdn_waf_domain_configs(self, request):
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
@@ -822,15 +814,15 @@
         @return: CommitStagingRoutineCodeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.commit_staging_routine_code_with_options(request, runtime)
 
     def create_dcdn_deliver_task_with_options(self, request, runtime):
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
 
         @param request: CreateDcdnDeliverTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateDcdnDeliverTaskResponse
@@ -864,27 +856,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.CreateDcdnDeliverTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_dcdn_deliver_task(self, request):
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
 
         @param request: CreateDcdnDeliverTaskRequest
 
         @return: CreateDcdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dcdn_deliver_task_with_options(request, runtime)
 
     def create_dcdn_slsreal_time_log_delivery_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: CreateDcdnSLSRealTimeLogDeliveryRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateDcdnSLSRealTimeLogDeliveryResponse
@@ -924,15 +916,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.CreateDcdnSLSRealTimeLogDeliveryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_dcdn_slsreal_time_log_delivery(self, request):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: CreateDcdnSLSRealTimeLogDeliveryRequest
 
         @return: CreateDcdnSLSRealTimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1052,18 +1044,15 @@
         @return: CreateDcdnWafPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dcdn_waf_policy_with_options(request, runtime)
 
     def create_routine_with_options(self, tmp_req, runtime):
         """
-        >
-        *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
-        *   This operation creates a routine that contains only production and staging environments.
-        *   You can call this operation up to 100 times per second.
+        The message returned, such as ""Status": "OK"".
         
 
         @param tmp_req: CreateRoutineRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateRoutineResponse
@@ -1097,30 +1086,28 @@
         return TeaCore.from_map(
             dcdn_20180115_models.CreateRoutineResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_routine(self, request):
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
 
     def create_slr_and_sls_project_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 100 times per second per account.
+        *\
+        ****\
         
 
         @param request: CreateSlrAndSlsProjectRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateSlrAndSlsProjectResponse
@@ -1148,15 +1135,16 @@
         return TeaCore.from_map(
             dcdn_20180115_models.CreateSlrAndSlsProjectResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_slr_and_sls_project(self, request):
         """
-        >  You can call this operation up to 100 times per second per account.
+        *\
+        ****\
         
 
         @param request: CreateSlrAndSlsProjectRequest
 
         @return: CreateSlrAndSlsProjectResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1208,18 +1196,19 @@
         @return: DeleteDcdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_deliver_task_with_options(request, runtime)
 
     def delete_dcdn_domain_with_options(self, request, runtime):
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
@@ -1251,18 +1240,19 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DeleteDcdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_dcdn_domain(self, request):
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
@@ -1324,15 +1314,15 @@
         @return: DeleteDcdnIpaDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_ipa_domain_with_options(request, runtime)
 
     def delete_dcdn_ipa_specific_config_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
 
         @param request: DeleteDcdnIpaSpecificConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteDcdnIpaSpecificConfigResponse
@@ -1364,35 +1354,25 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DeleteDcdnIpaSpecificConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_dcdn_ipa_specific_config(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
 
         @param request: DeleteDcdnIpaSpecificConfigRequest
 
         @return: DeleteDcdnIpaSpecificConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_ipa_specific_config_with_options(request, runtime)
 
     def delete_dcdn_kv_with_options(self, request, runtime):
-        """
-        >  You can call this operation up to 50 times per second per account.
-        
-
-        @param request: DeleteDcdnKvRequest
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: DeleteDcdnKvResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key):
             query['Key'] = request.key
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         req = open_api_models.OpenApiRequest(
@@ -1411,22 +1391,14 @@
         )
         return TeaCore.from_map(
             dcdn_20180115_models.DeleteDcdnKvResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_dcdn_kv(self, request):
-        """
-        >  You can call this operation up to 50 times per second per account.
-        
-
-        @param request: DeleteDcdnKvRequest
-
-        @return: DeleteDcdnKvResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_kv_with_options(request, runtime)
 
     def delete_dcdn_real_time_log_project_with_options(self, request, runtime):
         """
         >  You can call this operation up to 100 times per second per account.
         
@@ -1574,15 +1546,15 @@
         @return: DeleteDcdnSpecificStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_specific_staging_config_with_options(request, runtime)
 
     def delete_dcdn_sub_task_with_options(self, runtime):
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to 3 times per second per account.
         
 
         @param request: DeleteDcdnSubTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteDcdnSubTaskResponse
@@ -1602,26 +1574,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DeleteDcdnSubTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_dcdn_sub_task(self):
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to 3 times per second per account.
         
 
         @return: DeleteDcdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dcdn_sub_task_with_options(runtime)
 
     def delete_dcdn_waf_policy_with_options(self, request, runtime):
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
 
         @param request: DeleteDcdnWafPolicyRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteDcdnWafPolicyResponse
@@ -1647,28 +1620,29 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DeleteDcdnWafPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_dcdn_waf_policy(self, request):
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
 
     def delete_routine_with_options(self, request, runtime):
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DeleteRoutineRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteRoutineResponse
@@ -1694,15 +1668,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DeleteRoutineResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_routine(self, request):
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DeleteRoutineRequest
 
         @return: DeleteRoutineResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1754,17 +1728,15 @@
         @return: DeleteRoutineCodeRevisionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_routine_code_revision_with_options(request, runtime)
 
     def delete_routine_conf_envs_with_options(self, tmp_req, runtime):
         """
-        >
-        *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
-        *   You can call this operation up to 100 times per second per account.
+        The ID of the region.
         
 
         @param tmp_req: DeleteRoutineConfEnvsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteRoutineConfEnvsResponse
@@ -1796,29 +1768,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DeleteRoutineConfEnvsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_routine_conf_envs(self, request):
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
 
     def describe_dcdn_acl_fields_with_options(self, request, runtime):
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to three times per second per account.
         
 
         @param request: DescribeDcdnAclFieldsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnAclFieldsResponse
@@ -1844,15 +1814,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnAclFieldsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_acl_fields(self, request):
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to three times per second per account.
         
 
         @param request: DescribeDcdnAclFieldsRequest
 
         @return: DescribeDcdnAclFieldsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2018,15 +1988,15 @@
         @return: DescribeDcdnBlockedRegionsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_blocked_regions_with_options(request, runtime)
 
     def describe_dcdn_certificate_detail_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDcdnCertificateDetailRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnCertificateDetailResponse
@@ -2056,15 +2026,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnCertificateDetailResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_certificate_detail(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDcdnCertificateDetailRequest
 
         @return: DescribeDcdnCertificateDetailResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2286,22 +2256,18 @@
         @return: DescribeDcdnDomainBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_bps_data_with_options(request, runtime)
 
     def describe_dcdn_domain_bps_data_by_layer_with_options(self, request, runtime):
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
@@ -2339,22 +2305,18 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainBpsDataByLayerResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_bps_data_by_layer(self, request):
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
@@ -2409,15 +2371,15 @@
         return self.describe_dcdn_domain_by_certificate_with_options(request, runtime)
 
     def describe_dcdn_domain_cc_activity_log_with_options(self, request, runtime):
         """
         >
         *   If you do not configure the StartTime or EndTime parameter, data collected over the last 24 hours is queried. If you configure both the StartTime and EndTime parameters, data collected within the specified time range is queried.
         *   You can query data collected over the last 30 days.
-        *   You can call this operation up to 50 times per second.
+        *   You can call this operation up to 50 times per second per user.
         
 
         @param request: DescribeDcdnDomainCcActivityLogRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnDomainCcActivityLogResponse
@@ -2460,27 +2422,27 @@
         )
 
     def describe_dcdn_domain_cc_activity_log(self, request):
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
 
     def describe_dcdn_domain_certificate_info_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: DescribeDcdnDomainCertificateInfoRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnDomainCertificateInfoResponse
@@ -2506,15 +2468,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainCertificateInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_certificate_info(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: DescribeDcdnDomainCertificateInfoRequest
 
         @return: DescribeDcdnDomainCertificateInfoResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2672,22 +2634,18 @@
         @return: DescribeDcdnDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_detail_with_options(request, runtime)
 
     def describe_dcdn_domain_hit_rate_data_with_options(self, request, runtime):
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
@@ -2719,42 +2677,30 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainHitRateDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_hit_rate_data(self, request):
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
 
     def describe_dcdn_domain_http_code_data_with_options(self, request, runtime):
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
@@ -2790,23 +2736,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainHttpCodeDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_http_code_data(self, request):
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
@@ -2877,15 +2815,15 @@
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_http_code_data_by_layer_with_options(request, runtime)
 
     def describe_dcdn_domain_ipa_bps_data_with_options(self, request, runtime):
         """
         >
-        *   Unit: bit/s.
+        *   The bandwidth is measured in bit/s.
         *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
         *   You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeDcdnDomainIpaBpsDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -2928,15 +2866,15 @@
             dcdn_20180115_models.DescribeDcdnDomainIpaBpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_ipa_bps_data(self, request):
         """
         >
-        *   Unit: bit/s.
+        *   The bandwidth is measured in bit/s.
         *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the last 24 hours. If you set both the **StartTime** and **EndTime** parameters, the request returns the data collected within the specified time range.
         *   You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeDcdnDomainIpaBpsDataRequest
 
         @return: DescribeDcdnDomainIpaBpsDataResponse
@@ -3001,17 +2939,17 @@
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_ipa_conn_data_with_options(request, runtime)
 
     def describe_dcdn_domain_ipa_traffic_data_with_options(self, request, runtime):
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
@@ -3052,37 +2990,29 @@
             dcdn_20180115_models.DescribeDcdnDomainIpaTrafficDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_ipa_traffic_data(self, request):
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
 
     def describe_dcdn_domain_isp_data_with_options(self, request, runtime):
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
@@ -3112,37 +3042,28 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainIspDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_isp_data(self, request):
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
 
     def describe_dcdn_domain_log_with_options(self, request, runtime):
         """
-        >
-        *   If you specify neither the **StartTime** parameter nor the **EndTime** parameter, the data in the last 24 hours is returned. If you specify the **StartTime** and **EndTime** parameters, the data within the specified time range is returned.
-        *   You can call this operation up to 100 times per second per account.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
 
         @param request: DescribeDcdnDomainLogRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnDomainLogResponse
@@ -3176,32 +3097,31 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainLogResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_log(self, request):
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
 
     def describe_dcdn_domain_multi_usage_data_with_options(self, request, runtime):
         """
         When you call this operation, take note of the following rules:
         *   If you do not set the StartTime or EndTime parameter, data within the last 10 minutes is queried. You can set both the StartTime and EndTime parameters to specify a time range.
         *   You can specify one or more accelerated domain names. Separate domain names with commas (,).
-        *   You can query data up to the last 90 days.
+        *   You can query data within the last 90 days.
         *   The time range cannot exceed 1 hour.
         
 
         @param request: DescribeDcdnDomainMultiUsageDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
@@ -3235,15 +3155,15 @@
         )
 
     def describe_dcdn_domain_multi_usage_data(self, request):
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
@@ -3382,15 +3302,15 @@
         @return: DescribeDcdnDomainOriginTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_origin_traffic_data_with_options(request, runtime)
 
     def describe_dcdn_domain_property_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        The accelerated domain name that you want to query. You can specify only one domain name in each call.
         
 
         @param request: DescribeDcdnDomainPropertyRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnDomainPropertyResponse
@@ -3416,15 +3336,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainPropertyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_property(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 10.
+        The accelerated domain name that you want to query. You can specify only one domain name in each call.
         
 
         @param request: DescribeDcdnDomainPropertyRequest
 
         @return: DescribeDcdnDomainPropertyResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -3702,23 +3622,16 @@
         @return: DescribeDcdnDomainRealTimeByteHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_real_time_byte_hit_rate_data_with_options(request, runtime)
 
     def describe_dcdn_domain_real_time_detail_data_with_options(self, request, runtime):
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
@@ -3742,23 +3655,16 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainRealTimeDetailDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_real_time_detail_data(self, request):
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
@@ -3878,23 +3784,19 @@
         @return: DescribeDcdnDomainRealTimeQpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_real_time_qps_data_with_options(request, runtime)
 
     def describe_dcdn_domain_real_time_req_hit_rate_data_with_options(self, request, runtime):
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
@@ -3918,23 +3820,19 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainRealTimeReqHitRateDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_real_time_req_hit_rate_data(self, request):
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
@@ -4050,22 +3948,15 @@
         @return: DescribeDcdnDomainRealTimeSrcHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_real_time_src_http_code_data_with_options(request, runtime)
 
     def describe_dcdn_domain_real_time_src_traffic_data_with_options(self, request, runtime):
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
@@ -4095,40 +3986,29 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainRealTimeSrcTrafficDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_real_time_src_traffic_data(self, request):
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
 
     def describe_dcdn_domain_real_time_traffic_data_with_options(self, request, runtime):
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
@@ -4158,21 +4038,17 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainRealTimeTrafficDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_real_time_traffic_data(self, request):
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
@@ -4276,15 +4152,15 @@
         @return: DescribeDcdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_staging_config_with_options(request, runtime)
 
     def describe_dcdn_domain_top_refer_visit_with_options(self, request, runtime):
         """
-        *Before you call this operation, take note of the following considerations:**\
+        *Before you call this operation, take note of the following rules:**\
         *   If you do not set the StartTime parameter, the data on the previous day is queried.
         *   You can specify only one domain name.
         
 
         @param request: DescribeDcdnDomainTopReferVisitRequest
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -4316,29 +4192,29 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainTopReferVisitResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_top_refer_visit(self, request):
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
 
     def describe_dcdn_domain_top_url_visit_with_options(self, request, runtime):
         """
-        >  You can only query the data within the last seven days.
+        > You can query data in the last seven days.
         
 
         @param request: DescribeDcdnDomainTopUrlVisitRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnDomainTopUrlVisitResponse
@@ -4368,35 +4244,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainTopUrlVisitResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_top_url_visit(self, request):
         """
-        >  You can only query the data within the last seven days.
+        > You can query data in the last seven days.
         
 
         @param request: DescribeDcdnDomainTopUrlVisitRequest
 
         @return: DescribeDcdnDomainTopUrlVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_top_url_visit_with_options(request, runtime)
 
     def describe_dcdn_domain_traffic_data_with_options(self, request, runtime):
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
@@ -4432,23 +4300,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainTrafficDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_traffic_data(self, request):
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
@@ -4512,17 +4372,17 @@
         @return: DescribeDcdnDomainUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_usage_data_with_options(request, runtime)
 
     def describe_dcdn_domain_uv_data_with_options(self, request, runtime):
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
@@ -4552,17 +4412,17 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainUvDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_uv_data(self, request):
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
@@ -4628,21 +4488,17 @@
         @return: DescribeDcdnDomainWebsocketBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_websocket_bps_data_with_options(request, runtime)
 
     def describe_dcdn_domain_websocket_http_code_data_with_options(self, request, runtime):
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
@@ -4678,21 +4534,17 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainWebsocketHttpCodeDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_websocket_http_code_data(self, request):
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
@@ -4768,16 +4620,17 @@
         @return: DescribeDcdnDomainWebsocketTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_websocket_traffic_data_with_options(request, runtime)
 
     def describe_dcdn_er_usage_data_with_options(self, request, runtime):
         """
-        >   You can call this operation up to 10 times per second per account.
-        *   The minimum time granularity for a query is one hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
+        # Usage notes
+        *   You can call this operation up to 10 times per second per account.
+        *   The minimum time granularity for a query is 1 hour. The maximum time span for a query is 24 hours. The time period within which historical data is available for a query is 366 days.
         
 
         @param request: DescribeDcdnErUsageDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnErUsageDataResponse
@@ -4811,16 +4664,17 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnErUsageDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_er_usage_data(self, request):
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
@@ -4932,15 +4786,15 @@
         @return: DescribeDcdnHttpsDomainListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_https_domain_list_with_options(request, runtime)
 
     def describe_dcdn_ip_info_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeDcdnIpInfoRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnIpInfoResponse
@@ -4966,15 +4820,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnIpInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_ip_info(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeDcdnIpInfoRequest
 
         @return: DescribeDcdnIpInfoResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -5080,15 +4934,16 @@
         @return: DescribeDcdnIpaDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_ipa_domain_detail_with_options(request, runtime)
 
     def describe_dcdn_ipa_service_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
 
         @param request: DescribeDcdnIpaServiceRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnIpaServiceResponse
@@ -5116,27 +4971,34 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnIpaServiceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_ipa_service(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
 
         @param request: DescribeDcdnIpaServiceRequest
 
         @return: DescribeDcdnIpaServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_ipa_service_with_options(request, runtime)
 
     def describe_dcdn_ipa_user_domains_with_options(self, request, runtime):
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
@@ -5182,15 +5044,21 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnIpaUserDomainsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_ipa_user_domains(self, request):
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
@@ -5268,17 +5136,15 @@
         @return: DescribeDcdnRealTimeDeliveryFieldResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_real_time_delivery_field_with_options(request, runtime)
 
     def describe_dcdn_refresh_quota_with_options(self, request, runtime):
         """
-        >
-        *   You can call the **RefreshDcdnObjectCaches** operation to refresh content and call the **PreloadDcdnObjectCaches** operation to prefetch content.
-        *   You can call this operation up to 20 times per second.
+        The remaining number of URLs that can be prefetched each day.
         
 
         @param request: DescribeDcdnRefreshQuotaRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnRefreshQuotaResponse
@@ -5306,31 +5172,29 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnRefreshQuotaResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_refresh_quota(self, request):
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
 
     def describe_dcdn_refresh_task_by_id_with_options(self, request, runtime):
         """
         >
         *   You can query data within the last three days.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        *   You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDcdnRefreshTaskByIdRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnRefreshTaskByIdResponse
@@ -5358,31 +5222,31 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_refresh_task_by_id(self, request):
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
 
     def describe_dcdn_refresh_tasks_with_options(self, request, runtime):
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
@@ -5428,31 +5292,32 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnRefreshTasksResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_refresh_tasks(self, request):
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
 
     def describe_dcdn_region_and_isp_with_options(self, request, runtime):
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        ****\
         
 
         @param request: DescribeDcdnRegionAndIspRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnRegionAndIspResponse
@@ -5480,15 +5345,16 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnRegionAndIspResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_region_and_isp(self, request):
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        ****\
         
 
         @param request: DescribeDcdnRegionAndIspRequest
 
         @return: DescribeDcdnRegionAndIspResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -5600,15 +5466,15 @@
         @return: DescribeDcdnReportListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_report_list_with_options(request, runtime)
 
     def describe_dcdn_slsrealtime_log_delivery_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeDcdnSLSRealtimeLogDeliveryRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnSLSRealtimeLogDeliveryResponse
@@ -5634,15 +5500,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnSLSRealtimeLogDeliveryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_slsrealtime_log_delivery(self, request):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeDcdnSLSRealtimeLogDeliveryRequest
 
         @return: DescribeDcdnSLSRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -5748,15 +5614,15 @@
         @return: DescribeDcdnSMCertificateListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_smcertificate_list_with_options(request, runtime)
 
     def describe_dcdn_sec_func_info_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeDcdnSecFuncInfoRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnSecFuncInfoResponse
@@ -5784,27 +5650,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnSecFuncInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_sec_func_info(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeDcdnSecFuncInfoRequest
 
         @return: DescribeDcdnSecFuncInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_sec_func_info_with_options(request, runtime)
 
     def describe_dcdn_sec_spec_info_with_options(self, runtime):
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeDcdnSecSpecInfoRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnSecSpecInfoResponse
@@ -5824,25 +5690,25 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnSecSpecInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_sec_spec_info(self):
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
 
         @return: DescribeDcdnSecSpecInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_sec_spec_info_with_options(runtime)
 
     def describe_dcdn_service_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDcdnServiceRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnServiceResponse
@@ -5870,15 +5736,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnServiceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_service(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDcdnServiceRequest
 
         @return: DescribeDcdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -6012,15 +5878,15 @@
         @return: DescribeDcdnTagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_tag_resources_with_options(request, runtime)
 
     def describe_dcdn_top_domains_by_flow_with_options(self, request, runtime):
         """
-        *Before you call this operation, pay attention to the following considerations:**If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
+        \\\\*Before you call this operation, pay attention to the following considerations:\\*\\* If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
         
 
         @param request: DescribeDcdnTopDomainsByFlowRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnTopDomainsByFlowResponse
@@ -6050,15 +5916,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnTopDomainsByFlowResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_top_domains_by_flow(self, request):
         """
-        *Before you call this operation, pay attention to the following considerations:**If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
+        \\\\*Before you call this operation, pay attention to the following considerations:\\*\\* If you do not specify the StartTime and EndTime parameters, the data within the current month is queried by default. If you specify the StartTime and EndTime parameters, the data within the specified time range is queried.
         
 
         @param request: DescribeDcdnTopDomainsByFlowRequest
 
         @return: DescribeDcdnTopDomainsByFlowResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -6460,15 +6326,16 @@
         @return: DescribeDcdnUserRealTimeDeliveryFieldResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_user_real_time_delivery_field_with_options(request, runtime)
 
     def describe_dcdn_user_resource_package_with_options(self, request, runtime):
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        **The maximum number of times that each user can call this operation per second is 30.
         
 
         @param request: DescribeDcdnUserResourcePackageRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnUserResourcePackageResponse
@@ -6498,15 +6365,16 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnUserResourcePackageResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_user_resource_package(self, request):
         """
-        > You can call this operation up to 30 times per second per account.
+        *\
+        **The maximum number of times that each user can call this operation per second is 30.
         
 
         @param request: DescribeDcdnUserResourcePackageRequest
 
         @return: DescribeDcdnUserResourcePackageResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -6560,15 +6428,15 @@
         @return: DescribeDcdnUserSecDropResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_user_sec_drop_with_options(request, runtime)
 
     def describe_dcdn_user_sec_drop_by_minute_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        The domain name.
         
 
         @param request: DescribeDcdnUserSecDropByMinuteRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnUserSecDropByMinuteResponse
@@ -6610,27 +6478,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnUserSecDropByMinuteResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_user_sec_drop_by_minute(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 50.
+        The domain name.
         
 
         @param request: DescribeDcdnUserSecDropByMinuteRequest
 
         @return: DescribeDcdnUserSecDropByMinuteResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_user_sec_drop_by_minute_with_options(request, runtime)
 
     def describe_dcdn_user_tags_with_options(self, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: DescribeDcdnUserTagsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnUserTagsResponse
@@ -6650,15 +6518,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnUserTagsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_user_tags(self):
         """
-        >  The maximum number of times that users can call this operation per second is 100.
+        The ID of the request.
         
 
         @return: DescribeDcdnUserTagsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_user_tags_with_options(runtime)
 
@@ -6756,16 +6624,15 @@
         @return: DescribeDcdnWafDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_domain_with_options(request, runtime)
 
     def describe_dcdn_waf_domain_detail_with_options(self, request, runtime):
         """
-        # Usage notes
-        You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
 
         @param request: DescribeDcdnWafDomainDetailRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnWafDomainDetailResponse
@@ -6791,16 +6658,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnWafDomainDetailResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_waf_domain_detail(self, request):
         """
-        # Usage notes
-        You can call this operation up to 20 times per second per account.
+        The ID of the request.
         
 
         @param request: DescribeDcdnWafDomainDetailRequest
 
         @return: DescribeDcdnWafDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -6904,15 +6770,15 @@
         @return: DescribeDcdnWafFilterInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_filter_info_with_options(request, runtime)
 
     def describe_dcdn_waf_geo_info_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeDcdnWafGeoInfoRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnWafGeoInfoResponse
@@ -6938,28 +6804,28 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnWafGeoInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_waf_geo_info(self, request):
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeDcdnWafGeoInfoRequest
 
         @return: DescribeDcdnWafGeoInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_geo_info_with_options(request, runtime)
 
     def describe_dcdn_waf_logs_with_options(self, request, runtime):
         """
         >
-        *   If you do not set StartTime or EndTime, data collected in the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         *   The log data is collected every hour.
         *   You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeDcdnWafLogsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -6996,15 +6862,15 @@
             dcdn_20180115_models.DescribeDcdnWafLogsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_waf_logs(self, request):
         """
         >
-        *   If you do not set StartTime or EndTime, data collected in the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         *   The log data is collected every hour.
         *   You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeDcdnWafLogsRequest
 
         @return: DescribeDcdnWafLogsResponse
@@ -7060,15 +6926,15 @@
         @return: DescribeDcdnWafPoliciesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_policies_with_options(request, runtime)
 
     def describe_dcdn_waf_policy_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeDcdnWafPolicyRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnWafPolicyResponse
@@ -7094,27 +6960,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnWafPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_waf_policy(self, request):
         """
-        >  You can call this operation up to 20 times per second per account.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeDcdnWafPolicyRequest
 
         @return: DescribeDcdnWafPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_waf_policy_with_options(request, runtime)
 
     def describe_dcdn_waf_policy_domains_with_options(self, request, runtime):
         """
-        >You can call this operation up to 20 times per second per account.
+        The number of domain names returned per page, which is the same as the PageSize parameter in request parameters.
         
 
         @param request: DescribeDcdnWafPolicyDomainsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnWafPolicyDomainsResponse
@@ -7144,15 +7010,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnWafPolicyDomainsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_waf_policy_domains(self, request):
         """
-        >You can call this operation up to 20 times per second per account.
+        The number of domain names returned per page, which is the same as the PageSize parameter in request parameters.
         
 
         @param request: DescribeDcdnWafPolicyDomainsRequest
 
         @return: DescribeDcdnWafPolicyDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -7652,15 +7518,15 @@
         @return: DescribeRoutineResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_routine_with_options(request, runtime)
 
     def describe_routine_canary_envs_with_options(self, runtime):
         """
-        >  You can call this operation up to 100 times per second per account.
+        The canary release environments that are supported by the edge routine.
         
 
         @param request: DescribeRoutineCanaryEnvsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeRoutineCanaryEnvsResponse
@@ -7680,25 +7546,25 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeRoutineCanaryEnvsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_routine_canary_envs(self):
         """
-        >  You can call this operation up to 100 times per second per account.
+        The canary release environments that are supported by the edge routine.
         
 
         @return: DescribeRoutineCanaryEnvsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_routine_canary_envs_with_options(runtime)
 
     def describe_routine_code_revision_with_options(self, request, runtime):
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeRoutineCodeRevisionRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeRoutineCodeRevisionResponse
@@ -7726,15 +7592,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeRoutineCodeRevisionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_routine_code_revision(self, request):
         """
-        >  The call frequency of the API is no more than 100 queries per second.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeRoutineCodeRevisionRequest
 
         @return: DescribeRoutineCodeRevisionResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -7814,15 +7680,16 @@
         @return: DescribeRoutineUserInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_routine_user_info_with_options(runtime)
 
     def describe_user_dcdn_ipa_status_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
 
         @param request: DescribeUserDcdnIpaStatusRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeUserDcdnIpaStatusResponse
@@ -7850,27 +7717,28 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeUserDcdnIpaStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_user_dcdn_ipa_status(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 20.
+        *\
+        **The maximum number of times that each user can call this operation per second is 20.
         
 
         @param request: DescribeUserDcdnIpaStatusRequest
 
         @return: DescribeUserDcdnIpaStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_dcdn_ipa_status_with_options(request, runtime)
 
     def describe_user_dcdn_status_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeUserDcdnStatusRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeUserDcdnStatusResponse
@@ -7896,27 +7764,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeUserDcdnStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_user_dcdn_status(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeUserDcdnStatusRequest
 
         @return: DescribeUserDcdnStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_dcdn_status_with_options(request, runtime)
 
     def describe_user_er_status_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeUserErStatusRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeUserErStatusResponse
@@ -7942,27 +7810,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeUserErStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_user_er_status(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeUserErStatusRequest
 
         @return: DescribeUserErStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_er_status_with_options(request, runtime)
 
     def describe_user_logservice_status_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeUserLogserviceStatusRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeUserLogserviceStatusResponse
@@ -7990,15 +7858,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeUserLogserviceStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_user_logservice_status(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeUserLogserviceStatusRequest
 
         @return: DescribeUserLogserviceStatusResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -8182,16 +8050,17 @@
         @return: ModifyDCdnDomainSchdmByPropertyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dcdn_domain_schdm_by_property_with_options(request, runtime)
 
     def modify_dcdn_waf_policy_with_options(self, request, runtime):
         """
-        >   You can call this operation up to 20 times per second per account.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
+        #
+        *   You can call this operation up to 20 times per second per account.
+        *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
 
         @param request: ModifyDcdnWafPolicyRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ModifyDcdnWafPolicyResponse
@@ -8221,37 +8090,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.ModifyDcdnWafPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_dcdn_waf_policy(self, request):
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
 
     def modify_dcdn_waf_policy_domains_with_options(self, request, runtime):
-        """
-        >   You can call this operation up to 20 times per second.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
-        
-
-        @param request: ModifyDcdnWafPolicyDomainsRequest
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: ModifyDcdnWafPolicyDomainsResponse
-        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.bind_domains):
             body['BindDomains'] = request.bind_domains
         if not UtilClient.is_unset(request.method):
             body['Method'] = request.method
         if not UtilClient.is_unset(request.policy_id):
@@ -8274,29 +8133,21 @@
         )
         return TeaCore.from_map(
             dcdn_20180115_models.ModifyDcdnWafPolicyDomainsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_dcdn_waf_policy_domains(self, request):
-        """
-        >   You can call this operation up to 20 times per second.
-        *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
-        
-
-        @param request: ModifyDcdnWafPolicyDomainsRequest
-
-        @return: ModifyDcdnWafPolicyDomainsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dcdn_waf_policy_domains_with_options(request, runtime)
 
     def modify_dcdn_waf_rule_with_options(self, request, runtime):
         """
-        >   You can call this operation up to 20 times per second per account.
+        #
+        *   You can call this operation up to 20 times per second.
         *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
         *   You must configure at least one of the **RuleStatus**, **RuleName** and **RuleConfig** parameters.
         
 
         @param request: ModifyDcdnWafRuleRequest
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -8330,15 +8181,16 @@
         return TeaCore.from_map(
             dcdn_20180115_models.ModifyDcdnWafRuleResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_dcdn_waf_rule(self, request):
         """
-        >   You can call this operation up to 20 times per second per account.
+        #
+        *   You can call this operation up to 20 times per second.
         *   Alibaba Cloud Dynamic Route for CDN (DCDN) supports POST requests.
         *   You must configure at least one of the **RuleStatus**, **RuleName** and **RuleConfig** parameters.
         
 
         @param request: ModifyDcdnWafRuleRequest
 
         @return: ModifyDcdnWafRuleResponse
@@ -8396,25 +8248,25 @@
         @return: OpenDcdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.open_dcdn_service_with_options(request, runtime)
 
     def preload_dcdn_object_caches_with_options(self, request, runtime):
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
@@ -8450,37 +8302,37 @@
         return TeaCore.from_map(
             dcdn_20180115_models.PreloadDcdnObjectCachesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def preload_dcdn_object_caches(self, request):
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
 
     def publish_dcdn_staging_config_to_production_with_options(self, request, runtime):
         """
-        >  The maximum number of times that users can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: PublishDcdnStagingConfigToProductionRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: PublishDcdnStagingConfigToProductionResponse
@@ -8508,27 +8360,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.PublishDcdnStagingConfigToProductionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def publish_dcdn_staging_config_to_production(self, request):
         """
-        >  The maximum number of times that users can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: PublishDcdnStagingConfigToProductionRequest
 
         @return: PublishDcdnStagingConfigToProductionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.publish_dcdn_staging_config_to_production_with_options(request, runtime)
 
     def publish_routine_code_revision_with_options(self, tmp_req, runtime):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param tmp_req: PublishRoutineCodeRevisionRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: PublishRoutineCodeRevisionResponse
@@ -8562,15 +8414,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.PublishRoutineCodeRevisionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def publish_routine_code_revision(self, request):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: PublishRoutineCodeRevisionRequest
 
         @return: PublishRoutineCodeRevisionResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -8608,23 +8460,25 @@
 
     def put_dcdn_kv(self, request):
         runtime = util_models.RuntimeOptions()
         return self.put_dcdn_kv_with_options(request, runtime)
 
     def refresh_dcdn_object_caches_with_options(self, request, runtime):
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
@@ -8656,35 +8510,37 @@
         return TeaCore.from_map(
             dcdn_20180115_models.RefreshDcdnObjectCachesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def refresh_dcdn_object_caches(self, request):
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
 
     def rollback_dcdn_staging_config_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 30 times per second per account.
+        The ID of the request.
         
 
         @param request: RollbackDcdnStagingConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: RollbackDcdnStagingConfigResponse
@@ -8710,27 +8566,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.RollbackDcdnStagingConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def rollback_dcdn_staging_config(self, request):
         """
-        >  You can call this operation up to 30 times per second per account.
+        The ID of the request.
         
 
         @param request: RollbackDcdnStagingConfigRequest
 
         @return: RollbackDcdnStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.rollback_dcdn_staging_config_with_options(request, runtime)
 
     def set_dcdn_domain_certificate_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 30 times per second per account.
+        The name of the certificate.
         
 
         @param request: SetDcdnDomainCertificateRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: SetDcdnDomainCertificateResponse
@@ -8774,15 +8630,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.SetDcdnDomainCertificateResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_dcdn_domain_certificate(self, request):
         """
-        >  You can call this operation up to 30 times per second per account.
+        The name of the certificate.
         
 
         @param request: SetDcdnDomainCertificateRequest
 
         @return: SetDcdnDomainCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -8888,15 +8744,15 @@
         @return: SetDcdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_dcdn_domain_staging_config_with_options(request, runtime)
 
     def set_dcdn_user_config_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 30 times per second.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: SetDcdnUserConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: SetDcdnUserConfigResponse
@@ -8930,15 +8786,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.SetDcdnUserConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_dcdn_user_config(self, request):
         """
-        >  You can call this operation up to 30 times per second.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: SetDcdnUserConfigRequest
 
         @return: SetDcdnUserConfigResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -8996,17 +8852,18 @@
         @return: SetRoutineSubdomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_routine_subdomain_with_options(request, runtime)
 
     def start_dcdn_domain_with_options(self, request, runtime):
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
@@ -9036,39 +8893,28 @@
         return TeaCore.from_map(
             dcdn_20180115_models.StartDcdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def start_dcdn_domain(self, request):
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
 
     def start_dcdn_ipa_domain_with_options(self, request, runtime):
-        """
-        >
-        *   The maximum number of times that users can call this operation per second is 20.
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        
-
-        @param request: StartDcdnIpaDomainRequest
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: StartDcdnIpaDomainResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.security_token):
@@ -9089,24 +8935,14 @@
         )
         return TeaCore.from_map(
             dcdn_20180115_models.StartDcdnIpaDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def start_dcdn_ipa_domain(self, request):
-        """
-        >
-        *   The maximum number of times that users can call this operation per second is 20.
-        *   If an accelerated domain is in an invalid state or your account has an overdue payment, the accelerated domain cannot be enabled.
-        
-
-        @param request: StartDcdnIpaDomainRequest
-
-        @return: StartDcdnIpaDomainResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.start_dcdn_ipa_domain_with_options(request, runtime)
 
     def stop_dcdn_domain_with_options(self, request, runtime):
         """
         *\
         ****\
@@ -9486,15 +9322,15 @@
         @return: UpdateDcdnIpaDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_dcdn_ipa_domain_with_options(request, runtime)
 
     def update_dcdn_slsrealtime_log_delivery_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: UpdateDcdnSLSRealtimeLogDeliveryRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateDcdnSLSRealtimeLogDeliveryResponse
@@ -9532,27 +9368,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.UpdateDcdnSLSRealtimeLogDeliveryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_dcdn_slsrealtime_log_delivery(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: UpdateDcdnSLSRealtimeLogDeliveryRequest
 
         @return: UpdateDcdnSLSRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_dcdn_slsrealtime_log_delivery_with_options(request, runtime)
 
     def update_dcdn_sub_task_with_options(self, request, runtime):
         """
-        >  You can call this operation up to three times per second per account.
+        The ID of the request.
         
 
         @param request: UpdateDcdnSubTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateDcdnSubTaskResponse
@@ -9584,27 +9420,27 @@
         return TeaCore.from_map(
             dcdn_20180115_models.UpdateDcdnSubTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_dcdn_sub_task(self, request):
         """
-        >  You can call this operation up to three times per second per account.
+        The ID of the request.
         
 
         @param request: UpdateDcdnSubTaskRequest
 
         @return: UpdateDcdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_dcdn_sub_task_with_options(request, runtime)
 
     def update_dcdn_user_real_time_delivery_field_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: UpdateDcdnUserRealTimeDeliveryFieldRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateDcdnUserRealTimeDeliveryFieldResponse
@@ -9628,15 +9464,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.UpdateDcdnUserRealTimeDeliveryFieldResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_dcdn_user_real_time_delivery_field(self, request):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: UpdateDcdnUserRealTimeDeliveryFieldRequest
 
         @return: UpdateDcdnUserRealTimeDeliveryFieldResponse
         """
         runtime = util_models.RuntimeOptions()
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115/models.py` & `alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,41 +190,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddDcdnIpaDomainRequest(TeaModel):
     def __init__(self, check_url=None, domain_name=None, owner_account=None, owner_id=None, protocol=None,
                  resource_group_id=None, scope=None, security_token=None, sources=None, top_level_domain=None):
-        # The URL that is used to check the accessibility of the origin server.
+        # The URL that is used for health checks.
         self.check_url = check_url  # type: str
         # The domain name to be added to IPA.
         # 
         # A wildcard domain that starts with a period (.) is supported, such as .example.com.
         self.domain_name = domain_name  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         # The protocol. Valid values:
         # 
         # *   **udp**\
         # *   **tcp**\
         # 
-        # >  Example: `{"protocol":"udp"}`.
+        # **\
+        # 
+        # **Description** For example: `{"protocol":"udp"}`.
         self.protocol = protocol  # type: str
         # The ID of the resource group. If you do not specify a value for this parameter, the system automatically assigns the ID of the default resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The acceleration region. Valid values:
+        # The acceleration region. Default value: domestic. Valid values:
         # 
         # *   **domestic**: Chinese mainland
-        # *   **overseas**: global (excluding the Chinese mainland)
+        # *   **overseas**: outside the Chinese mainland
         # *   **global**: global
         self.scope = scope  # type: str
         self.security_token = security_token  # type: str
         # The information about the addresses of origin servers.
         self.sources = sources  # type: str
-        # The top-level domain name.
+        # The top-level domain.
         self.top_level_domain = top_level_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddDcdnIpaDomainRequest, self).to_map()
@@ -342,32 +344,55 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchAddDcdnDomainRequest(TeaModel):
     def __init__(self, check_url=None, domain_name=None, owner_account=None, owner_id=None, resource_group_id=None,
                  scope=None, security_token=None, sources=None, top_level_domain=None):
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
         self.check_url = check_url  # type: str
-        # You can add up to 50 domain names to DCDN for each of your Alibaba Cloud account. Separate multiple domain names with commas (,).
+        # The top-level domain name.
         self.domain_name = domain_name  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
-        # The ID of the resource group. If you do not specify a value for this parameter, the system automatically assigns the ID of the default resource group.
+        # The ID of the request.
         self.resource_group_id = resource_group_id  # type: str
-        # The accelerated region. Default value: domestic. Valid values:
-        # 
-        # *   domestic: Chinese mainland
-        # *   overseas: global (excluding the Chinese mainland)
-        # *   global: global
+        # Adds one or more domain names to Dynamic Route for CDN (DCDN).
         self.scope = scope  # type: str
         self.security_token = security_token  # type: str
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
         self.sources = sources  # type: str
-        # The top-level domain name.
         self.top_level_domain = top_level_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchAddDcdnDomainRequest, self).to_map()
@@ -416,15 +441,14 @@
         if m.get('TopLevelDomain') is not None:
             self.top_level_domain = m.get('TopLevelDomain')
         return self
 
 
 class BatchAddDcdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchAddDcdnDomainResponseBody, self).to_map()
@@ -480,17 +504,1050 @@
             temp_model = BatchAddDcdnDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchCreateDcdnWafRulesRequest(TeaModel):
     def __init__(self, policy_id=None, rule_configs=None):
-        # The ID of the protection policy.
-        self.policy_id = policy_id  # type: long
         # The configurations of the protection rule.
+        self.policy_id = policy_id  # type: long
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
         self.rule_configs = rule_configs  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchCreateDcdnWafRulesRequest, self).to_map()
@@ -535,17 +1592,16 @@
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class BatchCreateDcdnWafRulesResponseBody(TeaModel):
     def __init__(self, request_id=None, rule_ids=None):
-        # The ID of the request.
+        # Creates Web Application Firewall (WAF) protection rules.
         self.request_id = request_id  # type: str
-        # The IDs of created rules.
         self.rule_ids = rule_ids  # type: BatchCreateDcdnWafRulesResponseBodyRuleIds
 
     def validate(self):
         if self.rule_ids:
             self.rule_ids.validate()
 
     def to_map(self):
@@ -903,31 +1959,31 @@
     def __init__(self, cert_name=None, cert_type=None, domain_name=None, owner_id=None, region=None, sslpri=None,
                  sslprotocol=None, sslpub=None, security_token=None):
         # The name of the certificate.
         self.cert_name = cert_name  # type: str
         # The type of the certificate. Valid values:
         # 
         # *   **upload**: a custom certificate that you upload.
-        # *   **cas**: a certificate that is purchased from Alibaba Cloud SSL Certificates Service
+        # *   **cas**: a certificate that is acquired through Certificate Management Service.
         self.cert_type = cert_type  # type: str
-        # The name of the accelerated domain for which you want to configure the HTTPS certificate. The accelerated domain must have HTTPS acceleration enabled. You can specify multiple domain names and separate them with commas (,).
+        # The accelerated domain name for which you want to configure the HTTPS certificate. The accelerated domain must have HTTPS acceleration enabled. You can specify multiple domain names and separate them with commas (,).
         # 
-        # >  You can configure up to 10 domain names at a time.
+        # > You can configure up to 10 domain names in each request.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         # The ID of the region.
         self.region = region  # type: str
         # The private key. This parameter is required only if you enable the certificate.
         self.sslpri = sslpri  # type: str
         # Specifies whether to enable the HTTPS certificate. Valid values:
         # 
-        # *   **on:**\
-        # *   **off**\
+        # *   \*\*on\*\*: enables the HTTPS certificate.
+        # *   **off**: does not enable the HTTPS certificate.
         # 
-        # The default value is **off**.
+        # This is the default value.
         self.sslprotocol = sslprotocol  # type: str
         # The content of the certificate. This parameter is required only if you enable the certificate.
         self.sslpub = sslpub  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
@@ -1178,17 +2234,15 @@
         return self
 
 
 class BatchSetDcdnIpaDomainConfigsRequest(TeaModel):
     def __init__(self, domain_names=None, functions=None, owner_account=None, owner_id=None, security_token=None):
         # The domain names accelerated by IPA. Separate multiple domain names with commas (,).
         self.domain_names = domain_names  # type: str
-        # The list of features.
-        # 
-        #     [{"functionArgs":[{"argName":"Parameter name","argValue":"Parameter value"}],"functionName":"Feature name"}]
+        # The list of features. `[{"functionArgs":[{"argName":"parameter name","argValue":"parameter value"}],"functionName":"feature name"}]`
         self.functions = functions  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
@@ -1292,15 +2346,15 @@
 
 class BatchSetDcdnWafDomainConfigsRequest(TeaModel):
     def __init__(self, client_ip_tag=None, defense_status=None, domain_names=None):
         # Specifies the header that records the IP address to be obtained. If the default header is selected, the value of this parameter is empty. If a custom header is selected, the value of this parameter is the value specified by the user. Separate multiple values with commas (,). You can specify a maximum of five values.
         self.client_ip_tag = client_ip_tag  # type: str
         # The protection status of the domain name. Valid values: on, off, and empty string.
         # 
-        # *   When you add a domain name, the value of this parameter is **on**, and the value of ClientIpTag takes effect.
+        # *   When you add a domain name, the value of this parameter is **on**, and the value of ClientIpTag takes effect, which is empty if the default header is selected and is the value specified by the user if a custom header is selected.
         # *   When you delete a domain name, the value of this parameter is **off**, and the value of ClientIpTag does not take effect.
         # *   When you only modify the value of ClientIpTag, the value of DefenseStatus is an empty string.
         self.defense_status = defense_status  # type: str
         # The protected domain names for which you want to change the protection status. You can specify up to 50 domain names. Separate multiple domain names with commas (,).
         self.domain_names = domain_names  # type: str
 
     def validate(self):
@@ -1615,25 +2669,18 @@
             temp_model = CommitStagingRoutineCodeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateDcdnDeliverTaskRequest(TeaModel):
     def __init__(self, deliver=None, domain_name=None, name=None, reports=None, schedule=None):
-        # The method that is used to send operations reports. Operations reports are sent to you only by email. The settings must be escaped in JSON.
         self.deliver = deliver  # type: str
-        # The domain names to be tracked. Separate multiple domain names with commas (,). You can specify up to 500 domain names. If you want to specify more than 500 domain names, [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex).
-        # 
-        # > If you do not specify a domain name, the tracking task is created for all domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
-        # The name of the tracking task.
         self.name = name  # type: str
-        # The operations reports that are tracked by the task. The data must be escaped in JSON.
         self.reports = reports  # type: str
-        # The parameters that specify the time interval at which the tracking task sends operations reports. The settings must be escaped in JSON.
         self.schedule = schedule  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateDcdnDeliverTaskRequest, self).to_map()
@@ -1666,17 +2713,15 @@
         if m.get('Schedule') is not None:
             self.schedule = m.get('Schedule')
         return self
 
 
 class CreateDcdnDeliverTaskResponseBody(TeaModel):
     def __init__(self, deliver_id=None, request_id=None):
-        # The ID of the tracking task.
         self.deliver_id = deliver_id  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateDcdnDeliverTaskResponseBody, self).to_map()
@@ -1739,15 +2784,15 @@
 
 
 class CreateDcdnSLSRealTimeLogDeliveryRequest(TeaModel):
     def __init__(self, business_type=None, data_center=None, domain_name=None, project_name=None, slslog_store=None,
                  slsproject=None, slsregion=None, sampling_rate=None):
         # The type of the collected logs. Default value: cdn_log_access_l1. Valid values:
         # 
-        # *   **cdn_log_access_l1**: access logs of L1 Dynamic Route for CDN (DCDN) points of presence (POPs)
+        # *   **cdn_log_access_l1**: access logs of Dynamic Content Delivery Network (DCDN) points of presence (POPs)
         # *   **cdn_log_origin**: back-to-origin logs
         # *   **cdn_log_er**: EdgeRoutine logs
         self.business_type = business_type  # type: str
         # The data center. Valid values:
         # 
         # *   cn: China
         # *   sg: Singapore
@@ -2170,19 +3215,22 @@
             temp_model = CreateDcdnWafPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateRoutineRequest(TeaModel):
     def __init__(self, description=None, env_conf=None, name=None):
-        # The description of the routine.
-        self.description = description  # type: str
         # The configurations of the specified environment.
-        self.env_conf = env_conf  # type: dict[str, any]
+        self.description = description  # type: str
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        self.env_conf = env_conf  # type: dict[str, any]
+        # > 
+        # *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
+        # *   This operation creates a routine that contains only production and staging environments.
+        # *   You can call this operation up to 100 times per second.
         self.name = name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateRoutineRequest, self).to_map()
@@ -2207,19 +3255,22 @@
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
 class CreateRoutineShrinkRequest(TeaModel):
     def __init__(self, description=None, env_conf_shrink=None, name=None):
-        # The description of the routine.
-        self.description = description  # type: str
         # The configurations of the specified environment.
-        self.env_conf_shrink = env_conf_shrink  # type: str
+        self.description = description  # type: str
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        self.env_conf_shrink = env_conf_shrink  # type: str
+        # > 
+        # *   The parameters must comply with the rules of EnvConf. The description of a routine cannot exceed 50 characters in length.
+        # *   This operation creates a routine that contains only production and staging environments.
+        # *   You can call this operation up to 100 times per second.
         self.name = name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateRoutineShrinkRequest, self).to_map()
@@ -2314,22 +3365,18 @@
             temp_model = CreateRoutineResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateSlrAndSlsProjectRequest(TeaModel):
     def __init__(self, business_type=None, region=None):
-        # The type of the collected logs. Default value: cdn_log_access_l1. Valid values:
-        # 
-        # *   **cdn_log_access_l1**: access logs of L1 Dynamic Route for CDN (DCDN) points of presence (POPs)
-        # *   **cdn_log_origin**: back-to-origin logs
-        # *   **cdn_log_er**: EdgeRoutine logs
+        # *   ****\
+        # *   ****\
+        # *   ****\
         self.business_type = business_type  # type: str
-        # The region where Log Service resides. Valid values:
-        # 
         # *   **cn-hangzhou**\
         # *   **cn-shanghai**\
         # *   **cn-qingdao**\
         # *   **cn-beijing**\
         # *   **cn-zhangjiakou**\
         # *   **cn-shenzhen**\
         # *   **eu-central-1**\
@@ -2360,21 +3407,17 @@
         if m.get('Region') is not None:
             self.region = m.get('Region')
         return self
 
 
 class CreateSlrAndSlsProjectResponseBodySlsInfo(TeaModel):
     def __init__(self, end_point=None, log_store=None, project=None, region=None):
-        # The endpoint of Log Service.
         self.end_point = end_point  # type: str
-        # The Logstore of Log Service.
         self.log_store = log_store  # type: str
-        # The project of Log Service.
         self.project = project  # type: str
-        # The region where Log Service resides.
         self.region = region  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateSlrAndSlsProjectResponseBodySlsInfo, self).to_map()
@@ -2403,17 +3446,15 @@
         if m.get('Region') is not None:
             self.region = m.get('Region')
         return self
 
 
 class CreateSlrAndSlsProjectResponseBody(TeaModel):
     def __init__(self, request_id=None, sls_info=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The information about Log Service.
         self.sls_info = sls_info  # type: CreateSlrAndSlsProjectResponseBodySlsInfo
 
     def validate(self):
         if self.sls_info:
             self.sls_info.validate()
 
     def to_map(self):
@@ -2563,15 +3604,14 @@
             temp_model = DeleteDcdnDeliverTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteDcdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_account=None, owner_id=None, security_token=None):
-        # The accelerated domain name to be deleted. You can specify only one domain name.
         self.domain_name = domain_name  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
@@ -2603,15 +3643,14 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DeleteDcdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteDcdnDomainResponseBody, self).to_map()
@@ -2773,15 +3812,15 @@
         return self
 
 
 class DeleteDcdnIpaSpecificConfigRequest(TeaModel):
     def __init__(self, config_id=None, domain_name=None, owner_id=None, security_token=None):
         # The ID of the configuration. You can call the [DescribeDcdnDomainConfigs](~~130625~~) operation to query configuration IDs.
         self.config_id = config_id  # type: str
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -2876,15 +3915,15 @@
             temp_model = DeleteDcdnIpaSpecificConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteDcdnKvRequest(TeaModel):
     def __init__(self, key=None, namespace=None):
-        # The name of the key that you want to delete.
+        # The ID of the request.
         self.key = key  # type: str
         # The namespace that you specify when you call the PutDcdnKvNamespace operation.
         self.namespace = namespace  # type: str
 
     def validate(self):
         pass
 
@@ -2907,15 +3946,15 @@
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
         return self
 
 
 class DeleteDcdnKvResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The name of the key to delete.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteDcdnKvResponseBody, self).to_map()
@@ -3450,15 +4489,15 @@
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
 class DeleteRoutineResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # Returns ""Status": "OK"".
+        # The message returned, such as ""Status": "OK"".
         self.content = content  # type: dict[str, any]
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -3621,17 +4660,19 @@
             temp_model = DeleteRoutineCodeRevisionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteRoutineConfEnvsRequest(TeaModel):
     def __init__(self, envs=None, name=None):
-        # The custom canary release environments that you want to delete.
-        self.envs = envs  # type: dict[str, any]
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        self.envs = envs  # type: dict[str, any]
+        # > 
+        # *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
+        # *   You can call this operation up to 100 times per second per account.
         self.name = name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteRoutineConfEnvsRequest, self).to_map()
@@ -3652,17 +4693,19 @@
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
 class DeleteRoutineConfEnvsShrinkRequest(TeaModel):
     def __init__(self, envs_shrink=None, name=None):
-        # The custom canary release environments that you want to delete.
-        self.envs_shrink = envs_shrink  # type: str
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        self.envs_shrink = envs_shrink  # type: str
+        # > 
+        # *   This operation deletes only custom preset canary release environments. You cannot delete production or staging environments.
+        # *   You can call this operation up to 100 times per second per account.
         self.name = name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteRoutineConfEnvsShrinkRequest, self).to_map()
@@ -3781,15 +4824,15 @@
         if m.get('Lang') is not None:
             self.lang = m.get('Lang')
         return self
 
 
 class DescribeDcdnAclFieldsResponseBodyContent(TeaModel):
     def __init__(self, fields=None):
-        # The rules and policies that were configured. The JSON string must be decoded.
+        # The rules and policies that were configured. The JSON string is decoded.
         self.fields = fields  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnAclFieldsResponseBodyContent, self).to_map()
@@ -3806,15 +4849,15 @@
         if m.get('Fields') is not None:
             self.fields = m.get('Fields')
         return self
 
 
 class DescribeDcdnAclFieldsResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The details about the rules.
+        # Details about the rules.
         self.content = content  # type: list[DescribeDcdnAclFieldsResponseBodyContent]
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.content:
             for k in self.content:
@@ -5288,39 +6331,24 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainBpsDataByLayerRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, layer=None,
                  location_name_en=None, start_time=None):
-        # The accelerated domain name. You can specify multiple domain names and separate them with commas (,). You can specify up to 500 domain names in each request. The query results of multiple domain names are aggregated.
-        # 
-        # If you do not specify a domain name, data of all domain names is queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # **\
         # 
-        # >  The end time must be later than the start time.
+        # ****\
         self.end_time = end_time  # type: str
-        # The time interval between the data entries to return. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
+        # ****\
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP). You can call the DescribeDcdnRegionAndIsp operation to query the ISP name. If you do not specify a value for this parameter, all ISPs are queried.
         self.isp_name_en = isp_name_en  # type: str
-        # The layer at which you want to query the bandwidth data. The network layer supports IPv4 and IPv6. The application layer supports http, https, and quic. You can also set the value to all.
-        # 
-        # Default value: all.
         self.layer = layer  # type: str
-        # The name of the region. You can call the DescribeDcdnRegionAndIsp operation to query the region name. If you do not specify a value for this parameter, all regions are queried.
         self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The minimum data granularity is 5 minutes.
-        # 
-        # If you do not set this parameter, data in the last 24 hours is queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainBpsDataByLayerRequest, self).to_map()
@@ -5366,19 +6394,16 @@
 class DescribeDcdnDomainBpsDataByLayerResponseBodyBpsDataIntervalDataModule(TeaModel):
     def __init__(self, dynamic_traffic_value=None, dynamic_value=None, static_traffic_value=None,
                  static_value=None, time_stamp=None, traffic_value=None, value=None):
         self.dynamic_traffic_value = dynamic_traffic_value  # type: str
         self.dynamic_value = dynamic_value  # type: str
         self.static_traffic_value = static_traffic_value  # type: str
         self.static_value = static_value  # type: str
-        # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The total amount of network traffic. Unit: bytes.
         self.traffic_value = traffic_value  # type: str
-        # The total bandwidth. Unit: bit/s.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainBpsDataByLayerResponseBodyBpsDataIntervalDataModule, self).to_map()
@@ -5451,19 +6476,16 @@
                 temp_model = DescribeDcdnDomainBpsDataByLayerResponseBodyBpsDataIntervalDataModule()
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainBpsDataByLayerResponseBody(TeaModel):
     def __init__(self, bps_data_interval=None, data_interval=None, request_id=None):
-        # The bandwidth returned at each time interval.
         self.bps_data_interval = bps_data_interval  # type: DescribeDcdnDomainBpsDataByLayerResponseBodyBpsDataInterval
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.bps_data_interval:
             self.bps_data_interval.validate()
 
     def to_map(self):
@@ -5760,29 +6782,29 @@
         # 
         # If you leave this parameter empty, the data of all domain names is queried.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The number of the page to return. Default value: **1**.
+        # The page number of the returned page. Default value: **1**.
         self.page_number = page_number  # type: long
         # The number of entries to return on each page. Default value: **30**.
         self.page_size = page_size  # type: long
-        # The name of the rule. Valid values
+        # The name of the rule.
         # 
         # *   default_normal in normal mode
         # *   default_attack in emergency mode
         # *   A custom rule name in custom mode. Example: test2.
         # 
         # If you leave this parameter empty, all events that triggered rate limiting are queried.
         self.rule_name = rule_name  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The resolution of the queried data is 5 minutes.
+        # The minimum data granularity is 5 minutes.
         # 
         # If you leave this parameter empty, the data collected over the last 24 hours is queried.
         self.start_time = start_time  # type: str
         # The object that triggered rate limiting.
         # 
         # If you leave this parameter empty, all events that triggered rate limiting are queried.
         self.trigger_object = trigger_object  # type: str
@@ -5844,15 +6866,15 @@
                  value=None):
         # The action that was triggered.
         self.action = action  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The name of the rule that was triggered.
         self.rule_name = rule_name  # type: str
-        # The timestamp of the data.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
         # The object that triggered rate limiting.
         self.trigger_object = trigger_object  # type: str
         # The period of time during which rate limiting remains effective.
         self.ttl = ttl  # type: long
         # The value of the object that triggered rate limiting.
         self.value = value  # type: str
@@ -5995,15 +7017,15 @@
             temp_model = DescribeDcdnDomainCcActivityLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainCertificateInfoRequest(TeaModel):
     def __init__(self, domain_name=None):
-        # The accelerated domain name. You can specify only one domain name in each request.
+        # The certificate information of the domain name.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainCertificateInfoRequest, self).to_map()
@@ -6022,53 +7044,48 @@
         return self
 
 
 class DescribeDcdnDomainCertificateInfoResponseBodyCertInfosCertInfo(TeaModel):
     def __init__(self, cert_domain_name=None, cert_expire_time=None, cert_id=None, cert_life=None, cert_name=None,
                  cert_org=None, cert_region=None, cert_type=None, domain_name=None, sslprotocol=None, sslpub=None,
                  status=None):
-        # The domain name that matches the certificate.
+        # The certificate authority (CA) that issued the certificate.
         self.cert_domain_name = cert_domain_name  # type: str
-        # The expiration time of the certificate.
+        # The status of HTTPS. Valid values:
+        # 
+        # *   **on**: enabled
+        # *   **off**: disabled
         self.cert_expire_time = cert_expire_time  # type: str
+        # The type of the certificate. Valid values:
+        # 
+        # *   **free**: a free certificate
+        # *   **cas**: a certificate that is purchased from Alibaba Cloud SSL Certificates Service
+        # *   **upload**: a certificate that is uploaded by the user
         self.cert_id = cert_id  # type: str
-        # The validity period of the certificate. Unit: **months** or **years**.
+        # The public key of the certificate.
         self.cert_life = cert_life  # type: str
-        # The name of the certificate.
+        # The accelerated domain name.
         self.cert_name = cert_name  # type: str
-        # The certificate authority (CA) that issued the certificate.
+        # >  The maximum number of times that each user can call this operation per second is 100.
         self.cert_org = cert_org  # type: str
+        # The expiration time of the certificate.
         self.cert_region = cert_region  # type: str
+        # The name of the certificate.
+        self.cert_type = cert_type  # type: str
+        # The domain name that matches the certificate.
+        self.domain_name = domain_name  # type: str
+        # The domain name that matches the certificate.
+        self.sslprotocol = sslprotocol  # type: str
         # The type of the certificate. Valid values:
         # 
         # *   **free**: a free certificate
         # *   **cas**: a certificate that is purchased from Alibaba Cloud SSL Certificates Service
         # *   **upload**: a certificate that is uploaded by the user
-        self.cert_type = cert_type  # type: str
-        # The accelerated domain name.
-        self.domain_name = domain_name  # type: str
-        # The status of HTTPS. Valid values:
-        # 
-        # *   **on**: enabled
-        # *   **off**: disabled
-        self.sslprotocol = sslprotocol  # type: str
-        # The public key of the certificate.
         self.sslpub = sslpub  # type: str
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
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainCertificateInfoResponseBodyCertInfosCertInfo, self).to_map()
@@ -6161,17 +7178,28 @@
                 temp_model = DescribeDcdnDomainCertificateInfoResponseBodyCertInfosCertInfo()
                 self.cert_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainCertificateInfoResponseBody(TeaModel):
     def __init__(self, cert_infos=None, request_id=None):
-        # The certificate information of the domain name.
+        # The validity period of the certificate. Unit: **months** or **years**.
         self.cert_infos = cert_infos  # type: DescribeDcdnDomainCertificateInfoResponseBodyCertInfos
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
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
 
     def to_map(self):
@@ -6960,23 +7988,23 @@
 
 class DescribeDcdnDomainHitRateDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, start_time=None):
         # The accelerated domain name. You can specify only one domain name.
         # 
         # If you do not specify a value for this parameter, all domain names are queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time needs to be in UTC.
         # 
-        # The end time must be later than the start time.
+        # The end time needs to be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries to return. Unit: seconds.
+        # The time granularity for a query. Unit: seconds.
         # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time needs to be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainHitRateDataRequest, self).to_map()
@@ -7009,15 +8037,15 @@
 
 class DescribeDcdnDomainHitRateDataResponseBodyHitRatePerIntervalDataModule(TeaModel):
     def __init__(self, byte_hit_rate=None, req_hit_rate=None, time_stamp=None):
         # The byte hit ratio.
         self.byte_hit_rate = byte_hit_rate  # type: float
         # The request hit ratio.
         self.req_hit_rate = req_hit_rate  # type: float
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainHitRateDataResponseBodyHitRatePerIntervalDataModule, self).to_map()
@@ -7172,37 +8200,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainHttpCodeDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, location_name_en=None,
                  start_time=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time granularity for a query. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The name of the ISP.
-        # 
-        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region.
-        # 
-        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainHttpCodeDataRequest, self).to_map()
@@ -7239,19 +8249,16 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainHttpCodeDataResponseBodyDataPerIntervalDataModuleHttpCodeDataPerIntervalHttpCodeDataModule(TeaModel):
     def __init__(self, code=None, count=None, proportion=None):
-        # The HTTP status code returned.
         self.code = code  # type: int
-        # The total number of entries.
         self.count = count  # type: float
-        # The proportion of the HTTP status code.
         self.proportion = proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainHttpCodeDataResponseBodyDataPerIntervalDataModuleHttpCodeDataPerIntervalHttpCodeDataModule, self).to_map()
@@ -7308,17 +8315,15 @@
                 temp_model = DescribeDcdnDomainHttpCodeDataResponseBodyDataPerIntervalDataModuleHttpCodeDataPerIntervalHttpCodeDataModule()
                 self.http_code_data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainHttpCodeDataResponseBodyDataPerIntervalDataModule(TeaModel):
     def __init__(self, http_code_data_per_interval=None, time_stamp=None):
-        # The proportions of the HTTP status codes.
         self.http_code_data_per_interval = http_code_data_per_interval  # type: DescribeDcdnDomainHttpCodeDataResponseBodyDataPerIntervalDataModuleHttpCodeDataPerInterval
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         if self.http_code_data_per_interval:
             self.http_code_data_per_interval.validate()
 
     def to_map(self):
@@ -7374,25 +8379,19 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainHttpCodeDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, data_per_interval=None, domain_name=None, end_time=None, request_id=None,
                  start_time=None):
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The proportions of HTTP status codes at each time interval.
         self.data_per_interval = data_per_interval  # type: DescribeDcdnDomainHttpCodeDataResponseBodyDataPerInterval
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.data_per_interval:
             self.data_per_interval.validate()
 
     def to_map(self):
@@ -7686,48 +8685,48 @@
 
 
 class DescribeDcdnDomainIpaBpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, fix_time_gap=None, interval=None, isp_name_en=None,
                  location_name_en=None, start_time=None, time_merge=None):
         # The accelerated domain name.
         # 
-        # Separate multiple domain names with commas (,). If you do not specify a value for this parameter, all accelerated domain names are queried.
+        # Separate multiple domain names with commas (,). If you leave this parameter empty, all accelerated domain names are queried.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # Specify whether to implement padding with zeros. Valid values:
+        # Specifies whether to implement padding with zeros. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.fix_time_gap = fix_time_gap  # type: str
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
         self.interval = interval  # type: str
         # The name of the Internet service provider (ISP).
         # 
         # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en  # type: str
         # The name of the region.
         # 
         # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
-        # Specifies whether to automatically set the interval. If you set **TimeMerge** to **1**, the value of the **Interval** parameter is automatically assigned based on the **startTime** and **endTime** parameters. You can set either this parameter or the **Interval** parameter.
+        # Specifies whether to automatically set the interval. If you set **TimeMerge** to **1**, the value of the **Interval** parameter is automatically assigned based on the **startTime** and **endTime** parameters. You can specify either this parameter or the **Interval** parameter.
         self.time_merge = time_merge  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainIpaBpsDataRequest, self).to_map()
@@ -7838,15 +8837,15 @@
 
 
 class DescribeDcdnDomainIpaBpsDataResponseBody(TeaModel):
     def __init__(self, bps_data_per_interval=None, data_interval=None, domain_name=None, end_time=None,
                  request_id=None, start_time=None):
         # The bandwidth data returned at each interval.
         self.bps_data_per_interval = bps_data_per_interval  # type: DescribeDcdnDomainIpaBpsDataResponseBodyBpsDataPerInterval
-        # The time interval at which data is collected. Unit: seconds.
+        # The time interval at which data was collected. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
@@ -8140,50 +9139,50 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainIpaTrafficDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, fix_time_gap=None, interval=None, isp_name_en=None,
                  location_name_en=None, start_time=None, time_merge=None):
-        # The name of the accelerated domain name.
+        # The accelerated domain name.
         # 
-        # You can specify one or more accelerated domain names. Separate them with commas (,). By default, all accelerated domain names that belong to your Alibaba Cloud account are queried.
+        # Separate multiple domain names with commas (,). If you do not specify a value for this parameter, data for all accelerated domain names is queried.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
-        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
         # Specify whether to implement padding with zeros. Valid values:
         # 
-        # *   **true**: Yes
-        # *   **false**: No
+        # *   **true**\
+        # *   **false**\
         self.fix_time_gap = fix_time_gap  # type: str
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
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP) for Dynamic Route for CDN (DCDN).
+        # The name of the Internet service provider (ISP).
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~207199~~) operation to query the most recent ISP list. If you do not specify an ISP, all ISPs are queried.
+        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en  # type: str
         # The name of the region.
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~207199~~) operation to query the most recent region list. If you do not specify a region, all regions are queried.
+        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query.
         # 
-        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
-        # Specify whether to automatically calculate the value of the **Interval** parameter. If you set the **TimeMerge** parameter to **1**, the value of the **Interval** parameter is automatically assigned based on the **StartTime** and **EndTime** parameters. You can set this parameter or the **Interval** parameter.
+        # Specifies whether to automatically calculate the value of the **interval**. If the **timeMerge** parameter is set to **1**, the value of **inteval** is calculated based on **StartTime** and **EndTime**. You can set either this parameter or the **interval** parameter.
         self.time_merge = time_merge  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainIpaTrafficDataRequest, self).to_map()
@@ -8230,15 +9229,15 @@
         return self
 
 
 class DescribeDcdnDomainIpaTrafficDataResponseBodyTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(self, ipa_traffic=None, time_stamp=None):
         # The total amount of network traffic.
         self.ipa_traffic = ipa_traffic  # type: float
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainIpaTrafficDataResponseBodyTrafficDataPerIntervalDataModule, self).to_map()
@@ -8296,21 +9295,21 @@
 class DescribeDcdnDomainIpaTrafficDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  traffic_data_per_interval=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
-        # The monitoring data of network traffic that was collected at each interval.
+        # The network traffic that was collected at each interval.
         self.traffic_data_per_interval = traffic_data_per_interval  # type: DescribeDcdnDomainIpaTrafficDataResponseBodyTrafficDataPerInterval
 
     def validate(self):
         if self.traffic_data_per_interval:
             self.traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -8388,23 +9387,19 @@
             temp_model = DescribeDcdnDomainIpaTrafficDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainIspDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The accelerated domain name. You can specify only one domain name in each request.
-        # 
-        # If you do not specify an accelerated domain name, the data of all accelerated domain names that belong to your account is queried.
+        # The beginning of the time range during which data was queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # The accelerated domain name.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainIspDataRequest, self).to_map()
@@ -8430,35 +9425,43 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainIspDataResponseBodyValueIspProportionData(TeaModel):
     def __init__(self, avg_object_size=None, avg_response_rate=None, avg_response_time=None, bps=None,
                  bytes_proportion=None, isp=None, isp_ename=None, proportion=None, qps=None, total_bytes=None, total_query=None):
-        # The average response size. Unit: bytes.
+        # The proportion of network traffic. For example, a value of 90 indicates that 90% of network traffic was coming from the specified ISP.
         self.avg_object_size = avg_object_size  # type: str
-        # The average response speed. Unit: byte/ms.
+        # The name of the ISP.
         self.avg_response_rate = avg_response_rate  # type: str
-        # The average response time. Unit: milliseconds.
-        self.avg_response_time = avg_response_time  # type: str
         # The bandwidth.
+        self.avg_response_time = avg_response_time  # type: str
+        # The information about the ISP.
         self.bps = bps  # type: str
-        # The proportion of network traffic. For example, a value of 90 indicates that 90% of network traffic was coming from the specified ISP.
+        # The total amount of network traffic.
         self.bytes_proportion = bytes_proportion  # type: str
-        # The information about the ISP.
-        self.isp = isp  # type: str
         # The name of the ISP.
+        self.isp = isp  # type: str
+        # > 
+        # *   You can call this operation up to 100 times per second.
+        # *   If **StartTime** is set but **EndTime** is not set, the data within the hour that starts from **StartTime** is queried.
+        # *   If **EndTime** is set but **StartTime** is not set, the data within the last hour that precedes **EndTime** is queried.
+        # *   You can query data of a domain name or all domain names that belong to your account.
+        # *   You can view data that is collected over the last seven days. The interval at which data is queried is based on the time range specified by **StartTime** and **EndTime**.
+        #     *   **If the time range is shorter than or equal to one hour**, data is queried every minute.
+        #     *   **If the time range is longer than 1 hour but shorter than or equal to three days**, data is queried every five minutes.
+        #     *   **If the time range is longer than three days but shorter than or equal to seven days**, data is queried every hour.
         self.isp_ename = isp_ename  # type: str
-        # The proportion of requests.
+        # The information about the ISP.
         self.proportion = proportion  # type: str
-        # The number of queries per second.
+        # The average response time. Unit: milliseconds.
         self.qps = qps  # type: str
-        # The total amount of network traffic.
+        # The average response size. Unit: bytes.
         self.total_bytes = total_bytes  # type: str
-        # The total number of requests.
+        # The proportion of requests.
         self.total_query = total_query  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainIspDataResponseBodyValueIspProportionData, self).to_map()
@@ -8548,25 +9551,25 @@
                 self.isp_proportion_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainIspDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  value=None):
-        # The time interval between the data entries returned. Unit: seconds.
+        # The total amount of network traffic.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
+        # The total number of requests.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
+        # The time interval between the data entries returned. Unit: seconds.
         self.end_time = end_time  # type: str
-        # The ID of the request.
+        # The number of queries per second.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which data was queried.
-        self.start_time = start_time  # type: str
         # The access statistics by ISP.
+        self.start_time = start_time  # type: str
+        # The average response speed. Unit: byte/ms.
         self.value = value  # type: DescribeDcdnDomainIspDataResponseBodyValue
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -8644,33 +9647,27 @@
             temp_model = DescribeDcdnDomainIspDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainLogRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, page_number=None, page_size=None, start_time=None):
-        # The accelerated domain name that you want to query. You can specify only one domain name in each call.
-        self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # >  The end time must be later than the start time.
+        self.domain_name = domain_name  # type: str
+        # The total number of entries returned on the current page.
         self.end_time = end_time  # type: str
-        # The number of the page to return. Pages start from page **1**.
-        # 
-        # Default value: **1**.
+        # The ID of the request.
         self.page_number = page_number  # type: long
-        # The number of entries to return on each page.
-        # 
-        # Valid values: **1** to **1000**. Default value: **300**. Maximum value: **1000**.
+        # The domain name.
         self.page_size = page_size  # type: long
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The log information. The log information is indicated by the DomainLogDetail parameter.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainLogRequest, self).to_map()
@@ -8703,25 +9700,25 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailLogInfosLogInfoDetail(TeaModel):
     def __init__(self, end_time=None, log_name=None, log_path=None, log_size=None, start_time=None):
-        # The end of the time range during which data was queried.
-        self.end_time = end_time  # type: str
-        # The name of the log file.
-        self.log_name = log_name  # type: str
         # The path of the log file.
         # 
         # Take note of the Expires field (expiration timestamp) in the response parameter LogPath. If the log download URL expires, you must obtain it again. For more information, see [LogPath field](~~31952~~).
+        self.end_time = end_time  # type: str
+        # The number of entries returned per page.
+        self.log_name = log_name  # type: str
+        # The total number of entries returned.
         self.log_path = log_path  # type: str
-        # The size of the log file. Unit: bytes.
+        # The page information. The page information is indicated by the PageInfoDetail parameter.
         self.log_size = log_size  # type: long
-        # The beginning of the time range during which data was queried.
+        # The page number of the returned page.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailLogInfosLogInfoDetail, self).to_map()
@@ -8786,19 +9783,21 @@
                 temp_model = DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailLogInfosLogInfoDetail()
                 self.log_info_detail.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailPageInfos(TeaModel):
     def __init__(self, page_index=None, page_size=None, total=None):
-        # The page number of the returned page.
+        # The end of the time range during which data was queried.
         self.page_index = page_index  # type: long
-        # The number of entries returned per page.
+        # The number of entries to return on each page.
+        # 
+        # Valid values: **1** to **1000**. Default value: **300**. Maximum value: **1000**.
         self.page_size = page_size  # type: long
-        # The total number of entries returned.
+        # The total number of entries returned on the current page.
         self.total = total  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailPageInfos, self).to_map()
@@ -8823,19 +9822,21 @@
         if m.get('Total') is not None:
             self.total = m.get('Total')
         return self
 
 
 class DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetail(TeaModel):
     def __init__(self, log_count=None, log_infos=None, page_infos=None):
-        # The total number of entries returned on the current page.
+        # The beginning of the time range during which data was queried.
         self.log_count = log_count  # type: long
-        # The log information. The log information is indicated by the LogInfoDetail parameter.
+        # The name of the log file.
         self.log_infos = log_infos  # type: DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailLogInfos
-        # The page information. The page information is indicated by the PageInfoDetail parameter.
+        # > 
+        # *   If you specify neither the **StartTime** parameter nor the **EndTime** parameter, the data in the last 24 hours is returned. If you specify the **StartTime** and **EndTime** parameters, the data within the specified time range is returned.
+        # *   You can call this operation up to 100 times per second per account.
         self.page_infos = page_infos  # type: DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetailPageInfos
 
     def validate(self):
         if self.log_infos:
             self.log_infos.validate()
         if self.page_infos:
             self.page_infos.validate()
@@ -8897,19 +9898,19 @@
                 temp_model = DescribeDcdnDomainLogResponseBodyDomainLogDetailsDomainLogDetail()
                 self.domain_log_detail.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainLogResponseBody(TeaModel):
     def __init__(self, domain_log_details=None, domain_name=None, request_id=None):
-        # The log information. The log information is indicated by the DomainLogDetail parameter.
+        # The size of the log file. Unit: bytes.
         self.domain_log_details = domain_log_details  # type: DescribeDcdnDomainLogResponseBodyDomainLogDetails
-        # The domain name.
+        # The log information. The log information is indicated by the LogInfoDetail parameter.
         self.domain_name = domain_name  # type: str
-        # The ID of the request.
+        # The end of the time range during which data was queried.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domain_log_details:
             self.domain_log_details.validate()
 
     def to_map(self):
@@ -8981,24 +9982,24 @@
     def __init__(self, domain_name=None, end_time=None, start_time=None):
         # If this parameter is not set, data of all your accelerated domain names is queried.
         # 
         # You can specify one or more accelerated domain names. Separate domain names with commas (,).
         self.domain_name = domain_name  # type: str
         # The end time must be later than the start time.
         # 
-        # *   Specify the time in the ISO 8601 standard
-        # *   in the YYYY-MM-DDThh:mm:ssZ format. The time is displayed in UTC.
+        # *   Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format.
+        # *   The time must be in UTC.
         # *   You must set both the start time and the end time.
         self.end_time = end_time  # type: str
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
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -9024,19 +10025,19 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainMultiUsageDataResponseBodyRequestPerIntervalRequestDataModule(TeaModel):
     def __init__(self, domain=None, request=None, time_stamp=None, type=None):
-        # The accelerated domain name.
+        # The domain name.
         self.domain = domain  # type: str
         # The number of requests.
         self.request = request  # type: long
-        # The timestamp of the data entry.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
         # The type of the requests. Valid values: StaticHttps, DynamicHttps, DynamicHttp, StaticQuic, and DynamicQuic.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
@@ -9099,21 +10100,21 @@
                 temp_model = DescribeDcdnDomainMultiUsageDataResponseBodyRequestPerIntervalRequestDataModule()
                 self.request_data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainMultiUsageDataResponseBodyTrafficPerIntervalTrafficDataModule(TeaModel):
     def __init__(self, area=None, bps=None, domain=None, time_stamp=None, type=None):
-        # The name of the district.
+        # The name of the region.
         self.area = area  # type: str
         # The number of bits per second.
         self.bps = bps  # type: float
-        # The accelerated domain name.
+        # The domain name.
         self.domain = domain  # type: str
-        # The timestamp of the data entry.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
         # The type of the network traffic. Valid values: Simple, IPA, and WebSocket.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
@@ -9181,21 +10182,21 @@
                 self.traffic_data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainMultiUsageDataResponseBody(TeaModel):
     def __init__(self, end_time=None, request_id=None, request_per_interval=None, start_time=None,
                  traffic_per_interval=None):
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The information about requests collected every 5 minutes.
         self.request_per_interval = request_per_interval  # type: DescribeDcdnDomainMultiUsageDataResponseBodyRequestPerInterval
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The statistics of network traffic collected every 5 minutes.
         self.traffic_per_interval = traffic_per_interval  # type: DescribeDcdnDomainMultiUsageDataResponseBodyTrafficPerInterval
 
     def validate(self):
         if self.request_per_interval:
             self.request_per_interval.validate()
@@ -9738,15 +10739,15 @@
             temp_model = DescribeDcdnDomainOriginTrafficDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainPropertyRequest(TeaModel):
     def __init__(self, domain_name=None):
-        # The accelerated domain name that you want to query. You can specify only one domain name in each call.
+        # The ID of the request.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainPropertyRequest, self).to_map()
@@ -9763,22 +10764,22 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class DescribeDcdnDomainPropertyResponseBody(TeaModel):
     def __init__(self, domain_name=None, protocol=None, request_id=None):
-        # The accelerated domain name that is queried.
-        self.domain_name = domain_name  # type: str
         # The name of the protocol. Valid values:
         # 
         # *   **udp**: User Datagram Protocol (UDP)
         # *   **tcp**: Transmission Control Protocol (TCP)
+        self.domain_name = domain_name  # type: str
+        # >  The maximum number of times that users can call this operation per second is 10.
         self.protocol = protocol  # type: str
-        # The ID of the request.
+        # The accelerated domain name that is queried.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainPropertyResponseBody, self).to_map()
@@ -9842,15 +10843,15 @@
             temp_model = DescribeDcdnDomainPropertyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainPvDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The name of the accelerated domain. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
@@ -9881,15 +10882,15 @@
         return self
 
 
 class DescribeDcdnDomainPvDataResponseBodyPvDataIntervalUsageData(TeaModel):
     def __init__(self, time_stamp=None, value=None):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The consumed network traffic.
+        # The number of PVs.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainPvDataResponseBodyPvDataIntervalUsageData, self).to_map()
@@ -9943,25 +10944,25 @@
                 self.usage_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainPvDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, pv_data_interval=None, request_id=None,
                  start_time=None):
-        # The data collection interval. Unit: second.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The name of the accelerated domain for which the data was returned.
+        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which the data was collected.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The number of PVs at each interval.
         self.pv_data_interval = pv_data_interval  # type: DescribeDcdnDomainPvDataResponseBodyPvDataInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which the data was collected.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.pv_data_interval:
             self.pv_data_interval.validate()
 
     def to_map(self):
@@ -10326,39 +11327,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainQpsDataByLayerRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, layer=None,
                  location_name_en=None, start_time=None):
-        # The accelerated domain name. You can specify multiple domain names and separate them with commas (,). You can specify up to 500 domain names in each request. The query results of multiple domain names are aggregated.
-        # 
-        # If you do not specify a domain name, data of all domain names is queried.
+        # The QPS returned at each time interval.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # The number of queries per second outside the Chinese mainland.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries to return. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
+        # The layer at which the data was collected.
         self.interval = interval  # type: str
-        # The name of the ISP. You can call the DescribeDcdnRegionAndIsp operation to query the ISP name. If you do not specify a value for this parameter, all ISPs are queried.
-        self.isp_name_en = isp_name_en  # type: str
-        # The layers at which you want to query the QPS. The network layer supports IPv4 and IPv6. The application layer supports http, https, and quic. You can also set the value to all.
-        # 
-        # Default value: all.
-        self.layer = layer  # type: str
-        # The name of the region. You can call the DescribeDcdnRegionAndIsp operation to query the region name. If you do not specify a value for this parameter, all regions are queried.
-        self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The minimum data granularity is 5 minutes.
         # 
         # If you do not set this parameter, data in the last 24 hours is queried.
+        self.isp_name_en = isp_name_en  # type: str
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  The end time must be later than the start time.
+        self.layer = layer  # type: str
+        # The accelerated domain name.
+        self.location_name_en = location_name_en  # type: str
+        # The number of requests in the Chinese mainland.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainQpsDataByLayerRequest, self).to_map()
@@ -10400,27 +11395,31 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainQpsDataByLayerResponseBodyQpsDataIntervalDataModule(TeaModel):
     def __init__(self, acc_domestic_value=None, acc_overseas_value=None, acc_value=None, domestic_value=None,
                  overseas_value=None, time_stamp=None, value=None):
-        # The number of requests in the Chinese mainland.
-        self.acc_domestic_value = acc_domestic_value  # type: str
         # The number of requests outside the Chinese mainland.
+        self.acc_domestic_value = acc_domestic_value  # type: str
+        # The beginning of the time range during which data was queried.
         self.acc_overseas_value = acc_overseas_value  # type: str
-        # The total number of requests.
-        self.acc_value = acc_value  # type: str
         # The number of queries per second in the Chinese mainland.
+        self.acc_value = acc_value  # type: str
+        # The time interval between the data entries returned. Unit: seconds.
         self.domestic_value = domestic_value  # type: str
-        # The number of queries per second outside the Chinese mainland.
+        # The total number of queries per second.
         self.overseas_value = overseas_value  # type: str
-        # The timestamp of the data returned.
+        # The time interval between the data entries to return. Unit: seconds.
+        # 
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
         self.time_stamp = time_stamp  # type: str
-        # The total number of queries per second.
+        # The accelerated domain name. You can specify multiple domain names and separate them with commas (,). You can specify up to 500 domain names in each request. The query results of multiple domain names are aggregated.
+        # 
+        # If you do not specify a domain name, data of all domain names is queried.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainQpsDataByLayerResponseBodyQpsDataIntervalDataModule, self).to_map()
@@ -10494,27 +11493,29 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainQpsDataByLayerResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, layer=None, qps_data_interval=None,
                  request_id=None, start_time=None):
-        # The time interval between the data entries returned. Unit: seconds.
+        # The end of the time range during which data was queried.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
+        # The name of the ISP. You can call the DescribeDcdnRegionAndIsp operation to query the ISP name. If you do not specify a value for this parameter, all ISPs are queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
+        # The layers at which you want to query the QPS. The network layer supports IPv4 and IPv6. The application layer supports http, https, and quic. You can also set the value to all.
+        # 
+        # Default value: all.
         self.end_time = end_time  # type: str
-        # The layer at which the data was collected.
+        # The operation that you want to perform. Set the value to **DescribeDcdnDomainQpsDataByLayer**.
         self.layer = layer  # type: str
-        # The QPS returned at each time interval.
+        # The name of the region. You can call the DescribeDcdnRegionAndIsp operation to query the region name. If you do not specify a value for this parameter, all regions are queried.
         self.qps_data_interval = qps_data_interval  # type: DescribeDcdnDomainQpsDataByLayerResponseBodyQpsDataInterval
-        # The ID of the request.
+        # The timestamp of the data returned.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which data was queried.
+        # The total number of requests.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.qps_data_interval:
             self.qps_data_interval.validate()
 
     def to_map(self):
@@ -10955,47 +11956,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainRealTimeDetailDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, field=None, isp_name_en=None, location_name_en=None,
                  merge=None, merge_loc_isp=None, start_time=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
+        # Specifies whether to return a summary value of **LocationNameEn** and **IspNameEn**. Valid values:
+        # 
+        # *   **true**: yes
+        # *   **false**: no
+        # 
+        # The default value is **false**.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # > The end time must be later than the start time, and the maximum time range to query is 10 minutes.
         self.end_time = end_time  # type: str
-        # The type of the information that you want to query. Separate multiple types with commas (,). Valid values:
-        # 
-        # *   **qps**: queries per second
-        # *   **bps**: bandwidth
-        # *   **http_code**: HTTP status code
-        self.field = field  # type: str
-        # The name of the ISP. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the ISP name.
-        # 
-        # If you do not specify a value for this parameter, all ISPs are queried.
-        self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the region name.
-        # 
-        # If you do not specify a value for this parameter, all regions are queried.
-        self.location_name_en = location_name_en  # type: str
         # Specifies whether to return a summary value. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
         # 
         # The default value is **false**.
-        self.merge = merge  # type: str
-        # Specifies whether to return a summary value of **LocationNameEn** and **IspNameEn**. Valid values:
+        self.field = field  # type: str
+        # The information returned.
+        self.isp_name_en = isp_name_en  # type: str
+        # The type of the information that you want to query. Separate multiple types with commas (,). Valid values:
         # 
-        # *   **true**: yes
-        # *   **false**: no
+        # *   **qps**: queries per second
+        # *   **bps**: bandwidth
+        # *   **http_code**: HTTP status code
+        self.location_name_en = location_name_en  # type: str
+        # The ID of the request.
+        self.merge = merge  # type: str
+        # The name of the region. You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query the region name.
         # 
-        # The default value is **false**.
+        # If you do not specify a value for this parameter, all regions are queried.
         self.merge_loc_isp = merge_loc_isp  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -11042,17 +12041,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainRealTimeDetailDataResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The information returned.
+        # DescribeDcdnDomainRealTimeDetailData
         self.data = data  # type: str
-        # The ID of the request.
+        # Queries traffic data and the number of visits of each ISP in each region. Data is collected every minute. The maximum time range to query for this operation is 10 minutes.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainRealTimeDetailDataResponseBody, self).to_map()
@@ -11605,15 +12604,15 @@
 
 class DescribeDcdnDomainRealTimeReqHitRateDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
         # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The end time must be later than the start time.
+        # The end time needs to be later than the start time.
         self.end_time = end_time  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -11642,15 +12641,15 @@
         return self
 
 
 class DescribeDcdnDomainRealTimeReqHitRateDataResponseBodyDataReqHitRateDataModel(TeaModel):
     def __init__(self, req_hit_rate=None, time_stamp=None):
         # The request hit ratio.
         self.req_hit_rate = req_hit_rate  # type: float
-        # The timestamp of the data returned. The time follows the ISO 8601 standard. The time is displayed in UTC.
+        # The timestamp of the data returned. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainRealTimeReqHitRateDataResponseBodyDataReqHitRateDataModel, self).to_map()
@@ -11703,15 +12702,15 @@
                 temp_model = DescribeDcdnDomainRealTimeReqHitRateDataResponseBodyDataReqHitRateDataModel()
                 self.req_hit_rate_data_model.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainRealTimeReqHitRateDataResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The list of request hit ratios.
+        # The list of byte hit ratios.
         self.data = data  # type: DescribeDcdnDomainRealTimeReqHitRateDataResponseBodyData
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -12269,21 +13268,16 @@
             temp_model = DescribeDcdnDomainRealTimeSrcHttpCodeDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainRealTimeSrcTrafficDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainRealTimeSrcTrafficDataRequest, self).to_map()
@@ -12308,17 +13302,15 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The traffic value at each time interval.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerIntervalDataModule, self).to_map()
@@ -12372,27 +13364,19 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainRealTimeSrcTrafficDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None,
                  real_time_src_traffic_data_per_interval=None, request_id=None, start_time=None):
-        # The time interval between the data entries returned. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The amount of origin traffic returned at each time interval. Unit: bytes.
         self.real_time_src_traffic_data_per_interval = real_time_src_traffic_data_per_interval  # type: DescribeDcdnDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerInterval
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_src_traffic_data_per_interval:
             self.real_time_src_traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -12474,19 +13458,19 @@
 
 class DescribeDcdnDomainRealTimeTrafficDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
         # The accelerated domain name. You can specify one or more domain names and separate them with commas (,).
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. The end time must be later than the start time.
         # 
-        # >  If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
+        # > If you do not specify StartTime or EndTime, data within the last hour is queried. If you specify both StartTime and EndTime, data within the specified time range is queried.
         self.end_time = end_time  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
+        # > If you do not specify StartTime or EndTime, data within the last hour is queried. If you specify both StartTime and EndTime, data within the specified time range is queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainRealTimeTrafficDataRequest, self).to_map()
@@ -12513,17 +13497,17 @@
         return self
 
 
 class DescribeDcdnDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, value=None):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The amount of back-to-origin network traffic.
+        # The traffic value at each time interval.
         # 
-        # >  The network traffic is measured in bytes.
+        # > The network traffic is measured in bytes.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerIntervalDataModule, self).to_map()
@@ -12577,23 +13561,23 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainRealTimeTrafficDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None,
                  real_time_traffic_data_per_interval=None, request_id=None, start_time=None):
-        # The time interval between the data entries returned. Unit: seconds.
+        # The time interval between the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600 (1 hour). For more information, see **Description**.
+        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The amount of back-to-origin network traffic returned at each interval.
+        # The amount of back-to-origin traffic returned at each interval.
         self.real_time_traffic_data_per_interval = real_time_traffic_data_per_interval  # type: DescribeDcdnDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The beginning of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
@@ -13120,26 +14104,26 @@
         return self
 
 
 class DescribeDcdnDomainTopReferVisitRequest(TeaModel):
     def __init__(self, domain_name=None, sort_by=None, start_time=None):
         # The accelerated domain name. You can specify only one domain name.
         self.domain_name = domain_name  # type: str
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
         self.sort_by = sort_by  # type: str
         # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # To query the data on a specified day, use the yyyy-MM-ddT16:00:00Z format.
         # 
-        # If you do not specify this parameter, data collected within the last 24 hours is queried by default.
+        # If you leave this parameter empty, data collected in the last 24 hours is queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTopReferVisitRequest, self).to_map()
@@ -13164,23 +14148,23 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainTopReferVisitResponseBodyTopReferListReferList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, refer_detail=None, visit_data=None, visit_proportion=None):
-        # The network traffic. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of the network traffic.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
         # The complete referenced URL.
         self.refer_detail = refer_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of the visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTopReferVisitResponseBodyTopReferListReferList, self).to_map()
@@ -13249,15 +14233,15 @@
 
 class DescribeDcdnDomainTopReferVisitResponseBody(TeaModel):
     def __init__(self, domain_name=None, request_id=None, start_time=None, top_refer_list=None):
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which the data is collected.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The list of frequently referenced URLs returned.
         self.top_refer_list = top_refer_list  # type: DescribeDcdnDomainTopReferVisitResponseBodyTopReferList
 
     def validate(self):
         if self.top_refer_list:
             self.top_refer_list.validate()
@@ -13329,30 +14313,30 @@
             temp_model = DescribeDcdnDomainTopReferVisitResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainTopUrlVisitRequest(TeaModel):
     def __init__(self, domain_name=None, sort_by=None, start_time=None):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
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
         self.sort_by = sort_by  # type: str
         # The start of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the YYYY-MM-DDThh:mm:ssZ format. The time must be in UTC.
         # 
         # To query the data on a specified day, use the format: yyyy-MM-ddT16:00:00Z.
         # 
-        # >  If you do not set this parameter, the data within the last 24 hours is queried.
+        # > If you do not specify this parameter, the data in the last 24 hours is queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTopUrlVisitRequest, self).to_map()
@@ -13377,23 +14361,23 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainTopUrlVisitResponseBodyAllUrlListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTopUrlVisitResponseBodyAllUrlListUrlList, self).to_map()
@@ -13458,19 +14442,19 @@
                 temp_model = DescribeDcdnDomainTopUrlVisitResponseBodyAllUrlListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainTopUrlVisitResponseBodyUrl200ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
         # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
@@ -13539,23 +14523,23 @@
                 temp_model = DescribeDcdnDomainTopUrlVisitResponseBodyUrl200ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainTopUrlVisitResponseBodyUrl300ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTopUrlVisitResponseBodyUrl300ListUrlList, self).to_map()
@@ -13620,23 +14604,23 @@
                 temp_model = DescribeDcdnDomainTopUrlVisitResponseBodyUrl300ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainTopUrlVisitResponseBodyUrl400ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTopUrlVisitResponseBodyUrl400ListUrlList, self).to_map()
@@ -13701,23 +14685,23 @@
                 temp_model = DescribeDcdnDomainTopUrlVisitResponseBodyUrl400ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainTopUrlVisitResponseBodyUrl500ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The network traffic that was consumed by visits to the URLs. Unit: bytes.
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete string of the URL that was queried.
+        # The complete URL.
         self.url_detail = url_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTopUrlVisitResponseBodyUrl500ListUrlList, self).to_map()
@@ -13785,19 +14769,19 @@
 
 
 class DescribeDcdnDomainTopUrlVisitResponseBody(TeaModel):
     def __init__(self, all_url_list=None, domain_name=None, request_id=None, start_time=None, url_200list=None,
                  url_300list=None, url_400list=None, url_500list=None):
         # A list of frequently requested URLs.
         self.all_url_list = all_url_list  # type: DescribeDcdnDomainTopUrlVisitResponseBodyAllUrlList
-        # The accelerated domain name for which the data was returned.
+        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which the data was collected.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # A list of URLs for which 2xx status codes were returned.
         self.url_200list = url_200list  # type: DescribeDcdnDomainTopUrlVisitResponseBodyUrl200List
         # A list of URLs for which 3xx status codes were returned.
         self.url_300list = url_300list  # type: DescribeDcdnDomainTopUrlVisitResponseBodyUrl300List
         # A list of URLs for which 4xx status codes were returned.
         self.url_400list = url_400list  # type: DescribeDcdnDomainTopUrlVisitResponseBodyUrl400List
@@ -13904,39 +14888,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainTrafficDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, location_name_en=None,
                  start_time=None):
-        # The accelerated domain name.
-        # 
-        # Separate multiple domain names with commas (,). If you do not specify a value for this parameter, all accelerated domain names are queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time granularity for a query. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP).
-        # 
-        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region.
-        # 
-        # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTrafficDataRequest, self).to_map()
@@ -13974,25 +14938,19 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainTrafficDataResponseBodyTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(self, dynamic_http_traffic=None, dynamic_https_traffic=None, static_http_traffic=None,
                  static_https_traffic=None, time_stamp=None, traffic=None):
-        # The network traffic that was consumed to deliver dynamic content over HTTP.
         self.dynamic_http_traffic = dynamic_http_traffic  # type: float
-        # The network traffic that was consumed to deliver dynamic content over HTTPS.
         self.dynamic_https_traffic = dynamic_https_traffic  # type: float
-        # The network traffic that was consumed to deliver static content over HTTP.
         self.static_http_traffic = static_http_traffic  # type: float
-        # The network traffic that was consumed to deliver static content over HTTPS.
         self.static_https_traffic = static_https_traffic  # type: float
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The total amount of network traffic.
         self.traffic = traffic  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainTrafficDataResponseBodyTrafficDataPerIntervalDataModule, self).to_map()
@@ -14062,25 +15020,19 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainTrafficDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  traffic_data_per_interval=None):
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which data was queried.
         self.start_time = start_time  # type: str
-        # The network traffic returned at each time interval. Unit: bytes.
         self.traffic_data_per_interval = traffic_data_per_interval  # type: DescribeDcdnDomainTrafficDataResponseBodyTrafficDataPerInterval
 
     def validate(self):
         if self.traffic_data_per_interval:
             self.traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -14443,17 +15395,17 @@
             temp_model = DescribeDcdnDomainUsageDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainUvDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The name of the accelerated domain. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         # 
-        # By default, all the accelerated domains are queried.
+        # If you do not specify a domain name, this operation queries UV data of all accelerated domain names in your account.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The end time must be later than the start time.
         self.end_time = end_time  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
@@ -14548,23 +15500,23 @@
                 self.usage_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainUvDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  uv_data_interval=None):
-        # The data collection interval. Unit: second.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The name of the accelerated domain for which the data was returned.
+        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which the data was collected.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which the data was collected.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The number of UVs at each interval.
         self.uv_data_interval = uv_data_interval  # type: DescribeDcdnDomainUvDataResponseBodyUvDataInterval
 
     def validate(self):
         if self.uv_data_interval:
             self.uv_data_interval.validate()
@@ -14875,37 +15827,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainWebsocketHttpCodeDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, location_name_en=None,
                  start_time=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
+        # The accelerated domain name. You can specify multiple accelerated domain names and separate them with commas (,).
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries to return. Unit: seconds.
+        # The time granularity for a query. Unit: seconds.
         # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
         # The name of the Internet service provider (ISP).
         # 
         # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query ISPs.
         self.isp_name_en = isp_name_en  # type: str
         # The name of the region.
         # 
         # You can call the [DescribeDcdnRegionAndIsp](~~207199~~) operation to query regions.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainWebsocketHttpCodeDataRequest, self).to_map()
@@ -14942,17 +15894,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnDomainWebsocketHttpCodeDataResponseBodyHttpCodeDataPerIntervalDataModuleWebsocketHttpCodeHttpCodeDataModule(TeaModel):
     def __init__(self, code=None, count=None, proportion=None):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code  # type: int
-        # The total number of times that the HTTP status code was returned.
+        # The total number of entries returned.
         self.count = count  # type: float
         # The proportion of the HTTP status code.
         self.proportion = proportion  # type: float
 
     def validate(self):
         pass
 
@@ -15011,17 +15963,17 @@
                 temp_model = DescribeDcdnDomainWebsocketHttpCodeDataResponseBodyHttpCodeDataPerIntervalDataModuleWebsocketHttpCodeHttpCodeDataModule()
                 self.http_code_data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnDomainWebsocketHttpCodeDataResponseBodyHttpCodeDataPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, websocket_http_code=None):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The information about the HTTP status codes.
+        # The proportions of the HTTP status codes.
         self.websocket_http_code = websocket_http_code  # type: DescribeDcdnDomainWebsocketHttpCodeDataResponseBodyHttpCodeDataPerIntervalDataModuleWebsocketHttpCode
 
     def validate(self):
         if self.websocket_http_code:
             self.websocket_http_code.validate()
 
     def to_map(self):
@@ -15083,19 +16035,19 @@
                  request_id=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The HTTP status codes.
+        # The HTTP status code.
         self.http_code_data_per_interval = http_code_data_per_interval  # type: DescribeDcdnDomainWebsocketHttpCodeDataResponseBodyHttpCodeDataPerInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which data was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.http_code_data_per_interval:
             self.http_code_data_per_interval.validate()
 
     def to_map(self):
@@ -15405,27 +16357,27 @@
         return self
 
 
 class DescribeDcdnErUsageDataRequest(TeaModel):
     def __init__(self, end_time=None, routine_id=None, spec=None, split_by=None, start_time=None):
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The ID of the ER.
+        # The ID of the routine.
         self.routine_id = routine_id  # type: str
-        # The specification of the ER. Valid values:
+        # The specification of the routine. Valid values:
         # 
         # *   5ms
         # *   50ms
         # *   100ms
         self.spec = spec  # type: str
-        # Specifies how the results are grouped. If you set this parameter to routine, the returned results are grouped based on the ER ID. If you set this parameter to spec, the returned results are grouped based on the ER specification.
+        # Specifies how the results are grouped. If you set this parameter to routine, the returned results are grouped based on the routine ID. If you set this parameter to spec, the returned results are grouped based on the routine specification.
         # 
-        # >  If you leave this parameter empty, the returned results are not grouped.
+        # > If you leave this parameter empty, the returned results are not grouped.
         self.split_by = split_by  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -15460,19 +16412,19 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnErUsageDataResponseBodyErAccDataErAccItem(TeaModel):
     def __init__(self, er_acc=None, routine=None, spec=None, time_stamp=None):
-        # The number of ER requests.
+        # The number of requests.
         self.er_acc = er_acc  # type: long
-        # The ID of the ER. This parameter is returned only when SplitBy is set to routine.
+        # The ID of the routine. This parameter is returned only when SplitBy is set to routine.
         self.routine = routine  # type: str
-        # The specification of the ER. This parameter is returned only when SplitBy is set to spec.
+        # The specification of the routine. This parameter is returned only when SplitBy is set to spec.
         self.spec = spec  # type: str
         # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
@@ -15537,19 +16489,19 @@
         return self
 
 
 class DescribeDcdnErUsageDataResponseBody(TeaModel):
     def __init__(self, end_time=None, er_acc_data=None, request_id=None, start_time=None):
         # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The list of the returned data.
+        # The list of the data returned.
         self.er_acc_data = er_acc_data  # type: DescribeDcdnErUsageDataResponseBodyErAccData
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which data was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.er_acc_data:
             self.er_acc_data.validate()
 
     def to_map(self):
@@ -15870,19 +16822,28 @@
             temp_model = DescribeDcdnFullDomainsBlockIPHistoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnHttpsDomainListRequest(TeaModel):
     def __init__(self, keyword=None, page_number=None, page_size=None):
-        # The keyword used for search.
+        # The status of the certificate. Valid values:
+        # 
+        # *   **ok**: The certificate is working as expected.
+        # *   **mismatch**: The certificate does not match the specified domain name.
+        # *   **expired**: The certificate has expired.
+        # *   **expire_soon**: The certificate is about to expire.
         self.keyword = keyword  # type: str
-        # The number of pages to return. Valid values: **1 to 100000**.
+        # The total number of entries returned.
         self.page_number = page_number  # type: int
-        # The number of entries to return on each page. Valid values: **1 to 500**. Default value: **20**.
+        # The type of the certificate. Valid values:
+        # 
+        # *   **free**: A free certificate.
+        # *   **cas**: A certificate that is purchased through Alibaba Cloud SSL Certificates Service.
+        # *   **upload**: A user-uploaded certificate.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnHttpsDomainListRequest, self).to_map()
@@ -15908,38 +16869,29 @@
             self.page_size = m.get('PageSize')
         return self
 
 
 class DescribeDcdnHttpsDomainListResponseBodyCertInfosCertInfo(TeaModel):
     def __init__(self, cert_common_name=None, cert_expire_time=None, cert_name=None, cert_start_time=None,
                  cert_status=None, cert_type=None, cert_update_time=None, domain_name=None):
-        # The returned primary domain name of the certificate.
+        # The certificate information about the domain name.
         self.cert_common_name = cert_common_name  # type: str
-        # The time when the certificate expires.
-        self.cert_expire_time = cert_expire_time  # type: str
         # The name of the certificate.
+        self.cert_expire_time = cert_expire_time  # type: str
+        # The accelerated domain name for which the certificate information was queried.
         self.cert_name = cert_name  # type: str
-        # The time when the certificate became effective.
+        # The time when the certificate expires.
         self.cert_start_time = cert_start_time  # type: str
-        # The status of the certificate. Valid values:
-        # 
-        # *   **ok**: The certificate is working as expected.
-        # *   **mismatch**: The certificate does not match the specified domain name.
-        # *   **expired**: The certificate has expired.
-        # *   **expire_soon**: The certificate is about to expire.
+        # The number of pages to return. Valid values: **1 to 100000**.
         self.cert_status = cert_status  # type: str
-        # The type of the certificate. Valid values:
-        # 
-        # *   **free**: A free certificate.
-        # *   **cas**: A certificate that is purchased through Alibaba Cloud SSL Certificates Service.
-        # *   **upload**: A user-uploaded certificate.
+        # The operation that you want to perform. Set the value to **DescribeDcdnHttpsDomainList**.
         self.cert_type = cert_type  # type: str
-        # The time when the certificate was updated.
+        # The keyword used for search.
         self.cert_update_time = cert_update_time  # type: str
-        # The accelerated domain name for which the certificate information was queried.
+        # The time when the certificate was updated.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnHttpsDomainListResponseBodyCertInfosCertInfo, self).to_map()
@@ -16016,19 +16968,19 @@
                 temp_model = DescribeDcdnHttpsDomainListResponseBodyCertInfosCertInfo()
                 self.cert_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnHttpsDomainListResponseBody(TeaModel):
     def __init__(self, cert_infos=None, request_id=None, total_count=None):
-        # The certificate information about the domain name.
+        # The time when the certificate became effective.
         self.cert_infos = cert_infos  # type: DescribeDcdnHttpsDomainListResponseBodyCertInfos
-        # The ID of the request.
+        # The returned primary domain name of the certificate.
         self.request_id = request_id  # type: str
-        # The total number of entries returned.
+        # The number of entries to return on each page. Valid values: **1 to 500**. Default value: **20**.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
 
     def to_map(self):
@@ -16119,26 +17071,26 @@
         if m.get('IP') is not None:
             self.ip = m.get('IP')
         return self
 
 
 class DescribeDcdnIpInfoResponseBody(TeaModel):
     def __init__(self, dcdn_ip=None, isp=None, isp_ename=None, region=None, region_ename=None, request_id=None):
-        # Indicates whether the specified IP address is assigned to an Alibaba Cloud DCDN node.
+        # Indicates whether the specified IP address is assigned to an Alibaba Cloud DCDN POP.
         # 
-        # *   True: The specified IP address is assigned to an Alibaba Cloud DCDN node.
-        # *   False: The specified IP address is not assigned to an Alibaba Cloud DCDN node.
+        # *   True
+        # *   False
         self.dcdn_ip = dcdn_ip  # type: str
-        # The Internet service provider (ISP) to which the specified IP address belongs.
+        # The ISP to which the specified IP address belongs.
         self.isp = isp  # type: str
-        # The name of the ISP.
+        # The name of the Internet service provider (ISP).
         self.isp_ename = isp_ename  # type: str
-        # The region to which the specified IP address belongs.
+        # The Chinese name of the region.
         self.region = region  # type: str
-        # The name of the region.
+        # The English name of the region.
         self.region_ename = region_ename  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -16216,17 +17168,17 @@
             temp_model = DescribeDcdnIpInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnIpaDomainConfigsRequest(TeaModel):
     def __init__(self, domain_name=None, function_names=None, owner_id=None, security_token=None):
-        # The accelerated domain names. Separate multiple domain names with commas (,).
+        # The accelerated domain name. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The name of the feature. Only the protogw value is supported, which indicates IP Application Accelerator (IPA).
+        # The name of the feature. Set the value to protogw, which indicates IP Application Accelerator (IPA).
         self.function_names = function_names  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -16810,15 +17762,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeDcdnIpaServiceResponseBodyOperationLocksLockReason(TeaModel):
     def __init__(self, lock_reason=None):
-        # The reason why the IPA service was locked. A value of **financial** indicates that your account has an overdue payment.
+        # The reason why the instance is locked. For example, a value of **financial** indicates that an overdue payment exists.
         self.lock_reason = lock_reason  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnIpaServiceResponseBodyOperationLocksLockReason, self).to_map()
@@ -16872,37 +17824,37 @@
 class DescribeDcdnIpaServiceResponseBody(TeaModel):
     def __init__(self, changing_affect_time=None, changing_charge_type=None, instance_id=None,
                  internet_charge_type=None, opening_time=None, operation_locks=None, request_id=None):
         # The time when the change of the billing method starts to take effect. The time is in GMT. This time appears on the frontend only when it is later than the current time.
         self.changing_affect_time = changing_affect_time  # type: str
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
         self.changing_charge_type = changing_charge_type  # type: str
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
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
         self.internet_charge_type = internet_charge_type  # type: str
-        # The time when the IPA service was activated. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mmZ format.
+        # The time when the DCDN service was activated. The time follows the ISO 8601 standard.
         self.opening_time = opening_time  # type: str
-        # The lock status of the IPA service.
+        # The lock status of secure DCDN.
         self.operation_locks = operation_locks  # type: DescribeDcdnIpaServiceResponseBodyOperationLocks
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.operation_locks:
             self.operation_locks.validate()
@@ -16986,17 +17938,17 @@
             temp_model = DescribeDcdnIpaServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnIpaUserDomainsRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
-        # The tag key. Valid values of N: 1 to 20. You can call the TagDcdnResources operation to set a tag for a domain name.
+        # The array that consists of multiple PageData parameters. The details about each accelerated domain name are included in a separate PageData parameter.
         self.key = key  # type: str
-        # The tag value. Valid values of N: 1 to 20.
+        # The time when the accelerated domain name was added to Alibaba Cloud Dynamic Route for CDN (DCDN).
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnIpaUserDomainsRequestTag, self).to_map()
@@ -17019,55 +17971,45 @@
         return self
 
 
 class DescribeDcdnIpaUserDomainsRequest(TeaModel):
     def __init__(self, check_domain_show=None, domain_name=None, domain_search_type=None, domain_status=None,
                  func_filter=None, func_id=None, owner_id=None, page_number=None, page_size=None, resource_group_id=None,
                  tag=None):
-        # Specifies whether to display domain names that are under review, failed the review, or failed to be configured. Valid values:
-        # 
-        # *   **true**\
-        # *   **false**\
+        # The tag key. Valid values of N: 1 to 20. You can call the TagDcdnResources operation to set a tag for a domain name.
         self.check_domain_show = check_domain_show  # type: bool
-        # The domain name that is used as a keyword to filter domain names. Fuzzy match is supported.
+        # The ID of the resource group.
         self.domain_name = domain_name  # type: str
-        # The search method. Default value: full_match. Valid values:
-        # 
-        # *   **fuzzy_match**: fuzzy match
-        # *   **pre_match**: prefix match
-        # *   **suf_match**: suffix match
-        # *   **full_match**: exact match
-        self.domain_search_type = domain_search_type  # type: str
-        # The status of the domain name. Valid values:
-        # 
-        # *   **online**: enabled
-        # *   **offline**: disabled
-        # *   **configuring**: configuring
-        # *   **configure_failed**: configuration failed
-        # *   **checking**: reviewing
-        # *   **check_failed**: review failed
-        self.domain_status = domain_status  # type: str
         # The status of the feature.
         # 
         # *   config: The feature is enabled.
         # *   unconfig: The feature is not enabled.
-        self.func_filter = func_filter  # type: str
+        self.domain_search_type = domain_search_type  # type: str
         # The ID of the feature. For example, a value of 7 specifies the feature of configuring an expiration rule for a specific directory. For more information about feature IDs, see [Parameters for configuring features for domain names](~~410622~~).
+        self.domain_status = domain_status  # type: str
+        # The number of the returned page.
+        self.func_filter = func_filter  # type: str
+        # The ID of the request.
         self.func_id = func_id  # type: str
         self.owner_id = owner_id  # type: long
-        # The number of the page to return. Valid values: **1** to **100000**.
+        # Specifies whether to display domain names that are under review, failed the review, or failed to be configured. Valid values:
         # 
-        # Default value: **1**.
+        # *   **true**\
+        # *   **false**\
         self.page_number = page_number  # type: int
-        # The number of domain names to return on each page. Default value: **20**. Maximum value: **500**.
+        # The search method. Default value: full_match. Valid values:
         # 
-        # Valid values: an integer from **1** to **500**.
+        # *   **fuzzy_match**: fuzzy match
+        # *   **pre_match**: prefix match
+        # *   **suf_match**: suffix match
+        # *   **full_match**: exact match
         self.page_size = page_size  # type: int
-        # The ID of the resource group.
+        # The tag value. Valid values of N: 1 to 20.
         self.resource_group_id = resource_group_id  # type: str
+        # The number of domain names returned per page.
         self.tag = tag  # type: list[DescribeDcdnIpaUserDomainsRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -17132,23 +18074,20 @@
                 temp_model = DescribeDcdnIpaUserDomainsRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnIpaUserDomainsResponseBodyDomainsPageDataSourcesSource(TeaModel):
     def __init__(self, content=None, port=None, priority=None, type=None, weight=None):
-        # The address of the origin server.
         self.content = content  # type: str
-        # The port of the origin server.
         self.port = port  # type: int
-        # The priority of the origin server.
         self.priority = priority  # type: str
-        # The type of the origin server.
+        # Queries information about all domain names that are accelerated by IPA in your account.
+        #                   Fuzzy search and filtering by domain name status are supported.
         self.type = type  # type: str
-        # The weight of the origin server if multiple origin servers have been specified.
         self.weight = weight  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnIpaUserDomainsResponseBodyDomainsPageDataSourcesSource, self).to_map()
@@ -17214,43 +18153,33 @@
                 self.source.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnIpaUserDomainsResponseBodyDomainsPageData(TeaModel):
     def __init__(self, cname=None, description=None, domain_name=None, domain_status=None, gmt_created=None,
                  gmt_modified=None, resource_group_id=None, sslprotocol=None, sandbox=None, sources=None):
-        # The CNAME assigned to the accelerated domain name.
+        # The priority of the origin server.
         self.cname = cname  # type: str
-        # The reason why the accelerated domain name failed the review.
+        # The time when the accelerated domain name was modified.
         self.description = description  # type: str
-        # The accelerated domain name.
+        # The address of the origin server.
         self.domain_name = domain_name  # type: str
-        # The status of the accelerated domain name. Valid values:
-        # 
-        # *   **online**: enabled
-        # *   **offline**: disabled
-        # *   **configuring**: configuring
-        # *   **configure_failed**: configuration failed
-        # *   **checking**: reviewing
-        # *   **check_failed**: review failed
+        # The weight of the origin server if multiple origin servers have been specified.
         self.domain_status = domain_status  # type: str
-        # The time when the accelerated domain name was added to Alibaba Cloud Dynamic Route for CDN (DCDN).
+        # The CNAME assigned to the accelerated domain name.
         self.gmt_created = gmt_created  # type: str
-        # The time when the accelerated domain name was modified.
+        # The port of the origin server.
         self.gmt_modified = gmt_modified  # type: str
-        # The ID of the resource group.
+        # The information about the origin server.
         self.resource_group_id = resource_group_id  # type: str
-        # The status of HTTPS.
-        # 
-        # *   **on**\
-        # *   **off**\
+        # The accelerated domain name.
         self.sslprotocol = sslprotocol  # type: str
-        # Indicates whether the accelerated domain name was in a sandbox.
+        # The type of the origin server.
         self.sandbox = sandbox  # type: str
-        # The information about the origin server.
+        # >  You can call this operation up to 30 times per second per account.
         self.sources = sources  # type: DescribeDcdnIpaUserDomainsResponseBodyDomainsPageDataSources
 
     def validate(self):
         if self.sources:
             self.sources.validate()
 
     def to_map(self):
@@ -17337,23 +18266,33 @@
                 temp_model = DescribeDcdnIpaUserDomainsResponseBodyDomainsPageData()
                 self.page_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnIpaUserDomainsResponseBody(TeaModel):
     def __init__(self, domains=None, page_number=None, page_size=None, request_id=None, total_count=None):
-        # The array that consists of multiple PageData parameters. The details about each accelerated domain name are included in a separate PageData parameter.
+        # The status of the accelerated domain name. Valid values:
+        # 
+        # *   **online**: enabled
+        # *   **offline**: disabled
+        # *   **configuring**: configuring
+        # *   **configure_failed**: configuration failed
+        # *   **checking**: reviewing
+        # *   **check_failed**: review failed
         self.domains = domains  # type: DescribeDcdnIpaUserDomainsResponseBodyDomains
-        # The number of the returned page.
+        # The status of HTTPS.
+        # 
+        # *   **on**\
+        # *   **off**\
         self.page_number = page_number  # type: long
-        # The number of domain names returned per page.
+        # The ID of the resource group.
         self.page_size = page_size  # type: long
-        # The ID of the request.
+        # The reason why the accelerated domain name failed the review.
         self.request_id = request_id  # type: str
-        # The total number of domain names returned.
+        # Indicates whether the accelerated domain name was in a sandbox.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.domains:
             self.domains.validate()
 
     def to_map(self):
@@ -17723,37 +18662,39 @@
         return self
 
 
 class DescribeDcdnRefreshQuotaResponseBody(TeaModel):
     def __init__(self, block_quota=None, block_remain=None, dir_quota=None, dir_remain=None,
                  ignore_params_quota=None, ignore_params_remain=None, preload_quota=None, preload_remain=None, regex_quota=None,
                  regex_remain=None, request_id=None, url_quota=None, url_remain=None):
-        # The maximum number of URLs that can be blocked.
+        # The ID of the request.
         self.block_quota = block_quota  # type: str
-        # The remaining number of URLs that can be blocked each day.
+        # The remaining number of URLs that can be refreshed each day.
         self.block_remain = block_remain  # type: str
-        # The maximum number of directories that can be refreshed each day.
+        # > 
+        # *   You can call the **RefreshDcdnObjectCaches** operation to refresh content and call the **PreloadDcdnObjectCaches** operation to prefetch content.
+        # *   You can call this operation up to 20 times per second.
         self.dir_quota = dir_quota  # type: str
-        # The remaining number of directories that can be refreshed each day.
+        # The maximum number of URLs that can be prefetched each day.
         self.dir_remain = dir_remain  # type: str
         self.ignore_params_quota = ignore_params_quota  # type: str
         self.ignore_params_remain = ignore_params_remain  # type: str
-        # The maximum number of URLs that can be prefetched each day.
+        # The maximum number of URLs that can be blocked.
         self.preload_quota = preload_quota  # type: str
-        # The remaining number of URLs that can be prefetched each day.
+        # The maximum number of directories that can be refreshed each day.
         self.preload_remain = preload_remain  # type: str
-        # The maximum number of URLs or directories that can be refreshed by using regular expressions each day.
+        # The maximum number of URLs that can be refreshed each day.
         self.regex_quota = regex_quota  # type: str
-        # The remaining number of URLs or directories that can be refreshed by using regular expressions each day.
+        # The remaining number of directories that can be refreshed each day.
         self.regex_remain = regex_remain  # type: str
-        # The ID of the request.
-        self.request_id = request_id  # type: str
         # The maximum number of URLs that can be refreshed each day.
+        self.request_id = request_id  # type: str
+        # The remaining number of URLs that can be blocked each day.
         self.url_quota = url_quota  # type: str
-        # The remaining number of URLs that can be refreshed each day.
+        # The maximum number of URLs or directories that can be refreshed by using regular expressions each day.
         self.url_remain = url_remain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnRefreshQuotaResponseBody, self).to_map()
@@ -17857,20 +18798,20 @@
             temp_model = DescribeDcdnRefreshQuotaResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnRefreshTaskByIdRequest(TeaModel):
     def __init__(self, task_id=None):
-        # The ID of the task that you want to query. You can query task IDs by performing the following operations:
+        # The ID of the task that you want to query. The following signature algorithms require different message digest algorithms:
         # 
         # *   Perform the [RefreshDcdnObjectCaches](~~130620~~) operation to query refresh task IDs.
         # *   Perform the [PreloadDcdnObjectCaches](~~130636~~) operation to query prefetch task IDs.
         # 
-        # >  You can specify at most 10 task IDs in each call. Separate IDs with commas (,).
+        # > You can specify at most 10 task IDs in each call. Separate IDs with commas (,).
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnRefreshTaskByIdRequest, self).to_map()
@@ -17888,38 +18829,38 @@
             self.task_id = m.get('TaskId')
         return self
 
 
 class DescribeDcdnRefreshTaskByIdResponseBodyTasks(TeaModel):
     def __init__(self, creation_time=None, description=None, object_path=None, object_type=None, process=None,
                  status=None, task_id=None):
-        # The time when the task was created. The time follows the ISO 8601 standard in the YYYY-MM-DDThh:mm:ssZ format. The time is displayed in UTC.
+        # The time when the task was created. The time follows the ISO8601 standard in the YYYY-MM-DDThh:mmZ format. The time is displayed in UTC.
         self.creation_time = creation_time  # type: str
         # The error returned when the refresh or prefetch task failed. Valid values:
         # 
         # *   **Internal Error**: An internal error occurred.
         # *   **Origin Timeout**: The response from the origin server timed out.
-        # *   **Origin Return StatusCode 5XX**: The origin server returned an HTTP 5xx status code.
+        # *   **Origin Return StatusCode 5XX**: The origin server returned a 5XX error.
         self.description = description  # type: str
         # The path of the refresh or prefetch object.
         self.object_path = object_path  # type: str
         # The type of the refresh or prefetch task. Valid values:
         # 
         # *   **file**: refreshes an individual file.
-        # *   **directory**: refreshes files under a specified directory.
+        # *   **directory**: refreshes files under the specified directory.
         # *   **preload**: prefetches an individual file.
         self.object_type = object_type  # type: str
         # The progress of the task, in percentage.
         self.process = process  # type: str
         # The status of the task. Valid values:
         # 
-        # *   **Complete**: The task has completed.
+        # *   **Complete**: The task is complete.
         # *   **Pending**: The task is pending.
-        # *   **Refreshing**: The task is in progress.
-        # *   **Failed**: The task has failed.
+        # *   **Refreshing**: The task is running.
+        # *   **Failed**: The task failed.
         self.status = status  # type: str
         # The ID of the task.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
@@ -18047,45 +18988,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnRefreshTasksRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, object_path=None, object_type=None, owner_id=None,
                  page_number=None, page_size=None, security_token=None, start_time=None, status=None, task_id=None):
-        # The accelerated domain name. You can specify only one domain name in each request.
-        self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # > The end time must be later than the start time.
+        # >  The end time must be later than the start time.
+        self.domain_name = domain_name  # type: str
+        # The number of tasks.
         self.end_time = end_time  # type: str
-        # The path of the object. The path is used as a condition for exact matching.
-        self.object_path = object_path  # type: str
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
+        self.object_path = object_path  # type: str
+        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.object_type = object_type  # type: str
         self.owner_id = owner_id  # type: long
-        # The number of the page to return. Valid values: **1** to **100000**.
-        self.page_number = page_number  # type: int
         # The number of entries to return on each page. Default value: **20**. Maximum value: **50**. Valid values: **1** to **50**.
+        self.page_number = page_number  # type: int
+        # The page number of the returned page.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The number of entries returned per page.
         self.start_time = start_time  # type: str
-        # The status of the task.
-        # 
-        # *   **Complete**: The task is complete.
-        # *   **Refreshing**: The task is in progress.
-        # *   **Failed**: The task failed.
+        # The ID of the request.
         self.status = status  # type: str
-        # The ID of the task. A task ID is assigned when you create a refresh or prefetch task.
+        # The accelerated domain name. You can specify only one domain name in each call.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnRefreshTasksRequest, self).to_map()
@@ -18143,39 +19078,43 @@
             self.task_id = m.get('TaskId')
         return self
 
 
 class DescribeDcdnRefreshTasksResponseBodyTasksTask(TeaModel):
     def __init__(self, creation_time=None, description=None, object_path=None, object_type=None, process=None,
                  status=None, task_id=None):
-        # The time when the task was created. The time is displayed in UTC.
+        # The URL of the object to be refreshed.
         self.creation_time = creation_time  # type: str
-        # The type of error returned when the refresh or prefetch task has failed.
-        # 
-        # *   **InternalError**: An internal error occurred.
-        # *   **OriginTimeout**: The response from the origin server timed out.
-        # *   **OriginReturn StatusCode 5XX**: The origin server returned a 5XX error.
-        self.description = description  # type: str
-        # The URL of the object refreshed.
-        self.object_path = object_path  # type: str
         # The type of the task.
         # 
         # *   **file**: URL-based refresh
         # *   **path**: directory-based refresh
         # *   **preload**: URL-based prefetch
-        self.object_type = object_type  # type: str
-        # The progress of the task in percentage.
-        self.process = process  # type: str
+        self.description = description  # type: str
         # The status of the task.
         # 
-        # *   **Complete**: The task is complete.
+        # *   **Complete**: The task has completed.
         # *   **Refreshing**: The task is in progress.
         # *   **Failed**: The task failed.
-        self.status = status  # type: str
+        self.object_path = object_path  # type: str
         # The ID of the task.
+        self.object_type = object_type  # type: str
+        # > 
+        # *   You can query the status information by task ID or URL.
+        # *   You can set both the **TaskId** parameter and the **ObjectPath** parameter to query. If you set neither the **TaskId** parameter nor the **ObjectPath** parameter, the data in the last 3 days on the first page is returned. By default, a maximum of 20 entries can be displayed on each page.
+        # *   If you specify the **DomainName** or **Status** parameter, you must also specify the **ObjectType** parameter.
+        # *   You can call this operation up to 10 times per second per account.
+        self.process = process  # type: str
+        # The type of error returned when the refresh or prefetch task has failed.
+        # 
+        # *   **InternalError**: An internal error occurred.
+        # *   **OriginTimeout**: The response from the origin server timed out.
+        # *   **OriginReturn StatusCode 5XX**: The origin server returned a 5XX error.
+        self.status = status  # type: str
+        # The URL of the object to be refreshed.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnRefreshTasksResponseBodyTasksTask, self).to_map()
@@ -18248,23 +19187,31 @@
                 temp_model = DescribeDcdnRefreshTasksResponseBodyTasksTask()
                 self.task.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnRefreshTasksResponseBody(TeaModel):
     def __init__(self, page_number=None, page_size=None, request_id=None, tasks=None, total_count=None):
-        # The page number of the returned page.
+        # The status of the task.
+        # 
+        # *   **Complete**: The task has completed.
+        # *   **Refreshing**: The task is in progress.
+        # *   **Failed**: The task failed.
         self.page_number = page_number  # type: long
-        # The number of entries returned per page.
+        # The time when the task was created. The time is displayed in UTC.
         self.page_size = page_size  # type: long
-        # The ID of the request.
-        self.request_id = request_id  # type: str
         # Details about tasks.
+        self.request_id = request_id  # type: str
+        # The progress of the task, in percentage.
         self.tasks = tasks  # type: DescribeDcdnRefreshTasksResponseBodyTasks
-        # The number of tasks.
+        # The type of the task.
+        # 
+        # *   **file**: URL-based refresh
+        # *   **path**: directory-based refresh
+        # *   **preload**: URL-based prefetch
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.tasks:
             self.tasks.validate()
 
     def to_map(self):
@@ -18367,17 +19314,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeDcdnRegionAndIspResponseBodyIspsIsp(TeaModel):
     def __init__(self, name_en=None, name_zh=None):
-        # The English name of the ISP.
         self.name_en = name_en  # type: str
-        # The Chinese name of the ISP.
         self.name_zh = name_zh  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnRegionAndIspResponseBodyIspsIsp, self).to_map()
@@ -18430,17 +19375,15 @@
                 temp_model = DescribeDcdnRegionAndIspResponseBodyIspsIsp()
                 self.isp.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnRegionAndIspResponseBodyRegionsRegion(TeaModel):
     def __init__(self, name_en=None, name_zh=None):
-        # The English name of the region.
         self.name_en = name_en  # type: str
-        # The Chinese name of the region.
         self.name_zh = name_zh  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnRegionAndIspResponseBodyRegionsRegion, self).to_map()
@@ -18493,19 +19436,16 @@
                 temp_model = DescribeDcdnRegionAndIspResponseBodyRegionsRegion()
                 self.region.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnRegionAndIspResponseBody(TeaModel):
     def __init__(self, isps=None, regions=None, request_id=None):
-        # The list of ISPs.
         self.isps = isps  # type: DescribeDcdnRegionAndIspResponseBodyIsps
-        # The list of regions.
         self.regions = regions  # type: DescribeDcdnRegionAndIspResponseBodyRegions
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.isps:
             self.isps.validate()
         if self.regions:
             self.regions.validate()
@@ -18839,38 +19779,38 @@
 
 
 class DescribeDcdnSLSRealtimeLogDeliveryResponseBodyContent(TeaModel):
     def __init__(self, business_type=None, data_center=None, domain_name=None, field_name=None, project_name=None,
                  slslog_store=None, slsproject=None, slsregion=None, sampling_rate=None, status=None, type=None):
         # The type of the collected logs. Default value: cdn_log_access_l1. Valid values:
         # 
-        # *   **cdn_log_access_l1**: access logs of Dynamic Route for CDN (DCDN) points of presence (POPs)
+        # *   **cdn_log_access_l1**: access logs of Dynamic Content Delivery Network (DCDN) points of presence (POPs)
         # *   **cdn_log_origin**: back-to-origin logs
         # *   **cdn_log_er**: EdgeRoutine logs
         self.business_type = business_type  # type: str
         # The region from which logs were collected.
         self.data_center = data_center  # type: str
         # The domain names from which logs were collected. You can specify one or more domain names. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
         # The name of the field. For more information about fields in real-time log entries, see [Fields in a real-time log](~~324199~~).
         self.field_name = field_name  # type: str
-        # The name of the Log Service project
+        # The name of the project.
         self.project_name = project_name  # type: str
         # The name of the Logstore.
         self.slslog_store = slslog_store  # type: str
-        # The name of the Log Service project.
+        # The name of the log file.
         self.slsproject = slsproject  # type: str
         # The region to which logs were delivered.
         self.slsregion = slsregion  # type: str
         # The sampling rate.
         self.sampling_rate = sampling_rate  # type: str
         # The status of real-time logs.
         # 
-        # *   **success**: The transcoded stream is uploaded.
-        # *   **fail**: The transcoded stream fails to be uploaded.
+        # *   **success**\
+        # *   **fail**\
         self.status = status  # type: str
         # The type of log delivery. Only **SLS_POST** is supported.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
@@ -19399,15 +20339,15 @@
         self.content = content  # type: list[DescribeDcdnSecFuncInfoResponseBodyContent]
         # The description of HTTP responses.
         self.description = description  # type: str
         # The HTTP status code.
         self.http_status = http_status  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The return value for HTTP requests.
+        # The return value for HTTP requests. Valid values:
         # 
         # *   0: OK.
         # *   Values other than 0: an error.
         self.ret_code = ret_code  # type: str
 
     def validate(self):
         if self.content:
@@ -19679,15 +20619,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeDcdnServiceResponseBodyOperationLocksLockReason(TeaModel):
     def __init__(self, lock_reason=None):
-        # The reason why the service was locked. For example, a value of financial indicates that an overdue payment exists.
+        # The reason why the instance is locked. For example, a value of financial indicates that an overdue payment exists.
         self.lock_reason = lock_reason  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnServiceResponseBodyOperationLocksLockReason, self).to_map()
@@ -19738,41 +20678,41 @@
         return self
 
 
 class DescribeDcdnServiceResponseBody(TeaModel):
     def __init__(self, changing_affect_time=None, changing_charge_type=None, instance_id=None,
                  internet_charge_type=None, opening_time=None, operation_locks=None, request_id=None, websocket_changing_time=None,
                  websocket_changing_type=None, websocket_type=None):
-        # The start time when the next billing method takes effect. The time is displayed in UTC.
+        # The time when the renewed secure DCDN takes effect. The time is displayed in UTC.
         self.changing_affect_time = changing_affect_time  # type: str
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
         self.changing_charge_type = changing_charge_type  # type: str
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
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
         self.internet_charge_type = internet_charge_type  # type: str
         # The time when the DCDN service was activated. The time follows the ISO 8601 standard.
         self.opening_time = opening_time  # type: str
-        # The lock status of the DCDN service.
+        # The lock status of secure DCDN.
         self.operation_locks = operation_locks  # type: DescribeDcdnServiceResponseBodyOperationLocks
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The time when the changes of the WebSocket configuration take effect. The value is the same as that of the ChangingAffectTime parameter. This parameter can be displayed in the console only if the specified time is later than the current time.
         self.websocket_changing_time = websocket_changing_time  # type: str
         # The next effective billing method of WebSocket. Valid values: **websockettraffic** and **websocketbps**. A value of websockettraffic indicates that you are billed based on the traffic volume. A value of websocketbps indicates that you are billed based on the bandwidth.
         self.websocket_changing_type = websocket_changing_type  # type: str
@@ -20299,27 +21239,27 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnTopDomainsByFlowResponseBodyTopDomainsTopDomain(TeaModel):
     def __init__(self, domain_name=None, max_bps=None, max_bps_time=None, rank=None, total_access=None,
                  total_traffic=None, traffic_percent=None):
-        # The name of the accelerated domain.
+        # The domain name.
         self.domain_name = domain_name  # type: str
-        # The peak bandwidth.
+        # The peak bandwidth value.
         self.max_bps = max_bps  # type: long
         # The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         self.max_bps_time = max_bps_time  # type: str
-        # The ranking of the domains.
+        # The ranking of the accelerated domain name.
         self.rank = rank  # type: long
-        # The number of visits to the URL that was queried.
+        # The number of visits to the URL.
         self.total_access = total_access  # type: long
-        # The total amount of network traffic.
+        # The total volume of traffic.
         self.total_traffic = total_traffic  # type: str
-        # The proportion of the network traffic that was consumed for accessing the URL.
+        # The proportion of network traffic consumed to access the URL.
         self.traffic_percent = traffic_percent  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnTopDomainsByFlowResponseBodyTopDomainsTopDomain, self).to_map()
@@ -20397,19 +21337,19 @@
 class DescribeDcdnTopDomainsByFlowResponseBody(TeaModel):
     def __init__(self, domain_count=None, domain_online_count=None, end_time=None, request_id=None, start_time=None,
                  top_domains=None):
         # The total number of accelerated domains under your account.
         self.domain_count = domain_count  # type: long
         # The total number of accelerated domains that are in the **Enabled** state under your account.
         self.domain_online_count = domain_online_count  # type: long
-        # The end of the time range during which the data was collected.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which the data was collected.
+        # The beginning of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The top N domain names ranked by network traffic.
         self.top_domains = top_domains  # type: DescribeDcdnTopDomainsByFlowResponseBodyTopDomains
 
     def validate(self):
         if self.top_domains:
             self.top_domains.validate()
@@ -20756,23 +21696,19 @@
         return self
 
 
 class DescribeDcdnUserBillTypeRequest(TeaModel):
     def __init__(self, end_time=None, start_time=None):
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard
-        # 
-        # in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end time must be later than the start time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time  # type: str
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard
-        # 
-        # in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnUserBillTypeRequest, self).to_map()
@@ -20796,34 +21732,34 @@
 
 
 class DescribeDcdnUserBillTypeResponseBodyBillTypeDataBillTypeDataItem(TeaModel):
     def __init__(self, bill_type=None, billing_cycle=None, dimension=None, end_time=None, product=None,
                  start_time=None):
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
         self.bill_type = bill_type  # type: str
         # The billing cycle.
         self.billing_cycle = billing_cycle  # type: str
         # The dimension. Valid values:
         # 
         # *   **flow**: network traffic and bandwidth
         # *   **vas**: value-added services (HTTPS and requests for dynamic content)
         # *   **websocket**: WebSocket
-        # *   **quic**: the number of QUIC requests
+        # *   **quic**: QUIC requests
         # *   **rtlog2sls**: log entries delivered to Log Service in real time
         self.dimension = dimension  # type: str
         # The time when the metering method ends.
         self.end_time = end_time  # type: str
         # The name of the service.
         self.product = product  # type: str
         # The time when the metering method takes effect.
@@ -21669,15 +22605,15 @@
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # Specifies whether the feature that is specified by the FuncId parameter is enabled. Valid values:
         # 
         # *   **config**: enabled
         # *   **unconfig**: not enabled
         self.func_filter = func_filter  # type: str
-        # The ID of the feature. For more information about how to query feature IDs, see [Feature settings for a domain name](~~410622~~). For example, the ID of the origin host feature (set_req_host_header) is 18.
+        # The ID of the feature. For more information about how to query feature IDs, see [Parameters for configuring features for domain names](~~410622~~). For example, the ID of the origin host feature (set_req_host_header) is 18.
         self.func_id = func_id  # type: int
         # The number of the page to return. Default value: **1**. Valid values: **1 to 100000**.
         self.page_number = page_number  # type: int
         # The number of entries to return on each page. Default value: **20**. Valid values: **1 to 500**.
         self.page_size = page_size  # type: int
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
@@ -21810,22 +22746,22 @@
         self.cname = cname  # type: str
         # The reason why the accelerated domain name failed the review.
         self.description = description  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
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
         self.domain_status = domain_status  # type: str
-        # The time when the accelerated domain name was added.
+        # The time when the accelerated domain name was added to Dynamic Content Delivery Network (DCDN).
         self.gmt_created = gmt_created  # type: str
         # The time when the accelerated domain name was modified.
         self.gmt_modified = gmt_modified  # type: str
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         # Indicates whether the accelerated domain name was in a sandbox.
         self.sandbox = sandbox  # type: str
@@ -21925,21 +22861,21 @@
                 temp_model = DescribeDcdnUserDomainsByFuncResponseBodyDomainsPageData()
                 self.page_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnUserDomainsByFuncResponseBody(TeaModel):
     def __init__(self, domains=None, page_number=None, page_size=None, request_id=None, total_count=None):
-        # The detailed information about each accelerated domain name. The returned information is displayed in the format that is specified by the PageData parameter.
+        # The array that consists of multiple PageData parameters. The details about each accelerated domain name are included in a separate PageData parameter.
         self.domains = domains  # type: DescribeDcdnUserDomainsByFuncResponseBodyDomains
-        # The page number of the returned page.
+        # The number of the returned page.
         self.page_number = page_number  # type: long
         # The number of entries returned per page.
         self.page_size = page_size  # type: long
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
         # The total number of domain names returned.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.domains:
             self.domains.validate()
@@ -22341,16 +23277,16 @@
 
 class DescribeDcdnUserResourcePackageRequest(TeaModel):
     def __init__(self, owner_id=None, security_token=None, status=None):
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
         # The status of the resource plan. Valid values:
         # 
-        # *   **valid**: The resource plan is valid.
-        # *   **closed**: The resource plan is expired.
+        # *   **valid**: valid
+        # *   **closed**: expired
         # *   If you leave this parameter empty, all resource plans are queried.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -22386,29 +23322,29 @@
         # The remaining quota of the resource plan.
         # 
         # *   The unit for traffic: bytes.
         # *   The unit for requests: count.
         self.curr_capacity = curr_capacity  # type: str
         # The name of the resource plan.
         self.display_name = display_name  # type: str
-        # The time when the resource plan expires. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The expiration time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time  # type: str
         # The total quota of the resource plan.
         # 
         # *   The unit for traffic: bytes.
         # *   The unit for requests: count.
         self.init_capacity = init_capacity  # type: str
         # The ID of the resource plan.
         self.instance_id = instance_id  # type: str
-        # The time when the resource plan takes effect. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The validation time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
         # The status of the resource plan. Valid values:
         # 
-        # *   **valid**: The resource plan is valid.
-        # *   **closed**: The resource package is expired.
+        # *   **valid**: valid
+        # *   **closed**: expired
         self.status = status  # type: str
         # The name of the template.
         self.template_name = template_name  # type: str
 
     def validate(self):
         pass
 
@@ -22697,33 +23633,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnUserSecDropByMinuteRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, lang=None, object=None, page_number=None, page_size=None,
                  rule_name=None, sec_func=None, start_time=None):
-        # The domain name.
+        # The number of the page to return. Pages start from page 1.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0. Example: 2006-01-02T15:05:04Z.
-        # 
-        # >  The end time must be later than the start time.
+        # The ID of the request.
         self.end_time = end_time  # type: str
-        # The language. Valid values: en and zh. Default value: en
+        # The number of the returned page.
         self.lang = lang  # type: str
-        # The object that triggered the rule.
+        # The number of entries to return on each page. Maximum value: 100.
         self.object = object  # type: str
-        # The number of the page to return. Pages start from page 1.
+        # The total number of entries returned.
         self.page_number = page_number  # type: long
-        # The number of entries to return on each page. Maximum value: 100.
+        # The description of HTTP responses.
         self.page_size = page_size  # type: long
-        # The rule that was triggered.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0. Example: 2006-01-02T15:05:04Z.
+        # 
+        # >  The end time must be later than the start time.
         self.rule_name = rule_name  # type: str
-        # The name of the security feature.
-        self.sec_func = sec_func  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0. Example: 2006-01-02T15:04:04Z.
+        self.sec_func = sec_func  # type: str
+        # The language. Valid values: en and zh. Default value: en
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnUserSecDropByMinuteRequest, self).to_map()
@@ -22772,25 +23708,25 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDcdnUserSecDropByMinuteResponseBodyRows(TeaModel):
     def __init__(self, domain=None, drops=None, object=None, rule_name=None, sec_func=None, tm_str=None):
-        # The domain name.
+        # The security feature that blocked the packets.
         self.domain = domain  # type: str
-        # The number of packets blocked within 5 minutes.
+        # >  The maximum number of times that users can call this operation per second is 50.
         self.drops = drops  # type: int
-        # The object that triggered the rule.
+        # The total number of entries returned.
         self.object = object  # type: str
-        # The rule that is triggered.
+        # The total number of entries returned.
         self.rule_name = rule_name  # type: str
-        # The security feature that blocked the packets.
+        # The array returned.
         self.sec_func = sec_func  # type: str
-        # The beginning of the time range that was queried. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is in UTC+0.
+        # The rule that is triggered.
         self.tm_str = tm_str  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnUserSecDropByMinuteResponseBodyRows, self).to_map()
@@ -22828,27 +23764,27 @@
             self.tm_str = m.get('TmStr')
         return self
 
 
 class DescribeDcdnUserSecDropByMinuteResponseBody(TeaModel):
     def __init__(self, description=None, len=None, page_number=None, page_size=None, request_id=None, rows=None,
                  total_count=None):
-        # The description of HTTP responses.
-        self.description = description  # type: str
         # The total number of entries returned.
+        self.description = description  # type: str
+        # The array returned.
         self.len = len  # type: int
-        # The number of the returned page.
+        # The domain name.
         self.page_number = page_number  # type: int
-        # The number of entries returned on each page.
+        # The beginning of the time range that was queried. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is in UTC+0.
         self.page_size = page_size  # type: int
-        # The ID of the request.
+        # The number of entries returned on each page.
         self.request_id = request_id  # type: str
-        # The array returned.
+        # The object that triggered the rule.
         self.rows = rows  # type: list[DescribeDcdnUserSecDropByMinuteResponseBodyRows]
-        # The total number of entries returned.
+        # The number of packets blocked within 5 minutes.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.rows:
             for k in self.rows:
                 if k:
                     k.validate()
@@ -22936,17 +23872,16 @@
             temp_model = DescribeDcdnUserSecDropByMinuteResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnUserTagsResponseBodyTags(TeaModel):
     def __init__(self, key=None, value=None):
-        # The key of the returned tag.
-        self.key = key  # type: str
         # The value of the returned tag.
+        self.key = key  # type: str
         self.value = value  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnUserTagsResponseBodyTags, self).to_map()
@@ -22967,17 +23902,17 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class DescribeDcdnUserTagsResponseBody(TeaModel):
     def __init__(self, request_id=None, tags=None):
-        # The ID of the request.
-        self.request_id = request_id  # type: str
         # The tags.
+        self.request_id = request_id  # type: str
+        # The key of the returned tag.
         self.tags = tags  # type: list[DescribeDcdnUserTagsResponseBodyTags]
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -23323,15 +24258,15 @@
             temp_model = DescribeDcdnWafDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnWafDomainDetailRequest(TeaModel):
     def __init__(self, domain_name=None):
-        # The accelerated domain name. You can specify only one domain name in each request. Exact match is supported.
+        # The types of the protection policies.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnWafDomainDetailRequest, self).to_map()
@@ -23348,23 +24283,16 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class DescribeDcdnWafDomainDetailResponseBodyDomainDefenseScenes(TeaModel):
     def __init__(self, defense_scene=None, policy_id=None, policy_ids=None):
-        # The type of the protection policy. Valid values:
-        # 
-        # *   waf_group: basic web protection
-        # *   custom_acl: custom protection
-        # *   whitelist: IP address whitelist
         self.defense_scene = defense_scene  # type: str
-        # The ID of the protection policy. If multiple IDs exist, only one ID is returned.
         self.policy_id = policy_id  # type: long
-        # The IDs of the protection policies. Multiple IDs are separated by commas (,).
         self.policy_ids = policy_ids  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnWafDomainDetailResponseBodyDomainDefenseScenes, self).to_map()
@@ -23389,17 +24317,15 @@
         if m.get('PolicyIds') is not None:
             self.policy_ids = m.get('PolicyIds')
         return self
 
 
 class DescribeDcdnWafDomainDetailResponseBodyDomain(TeaModel):
     def __init__(self, defense_scenes=None, domain_name=None):
-        # The types of the protection policies.
         self.defense_scenes = defense_scenes  # type: list[DescribeDcdnWafDomainDetailResponseBodyDomainDefenseScenes]
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         if self.defense_scenes:
             for k in self.defense_scenes:
                 if k:
                     k.validate()
@@ -23428,17 +24354,21 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class DescribeDcdnWafDomainDetailResponseBody(TeaModel):
     def __init__(self, domain=None, request_id=None):
-        # The information about the accelerated domain name.
+        # The IDs of the protection policies. Multiple IDs are separated by commas (,).
         self.domain = domain  # type: DescribeDcdnWafDomainDetailResponseBodyDomain
-        # The ID of the request.
+        # The type of the protection policy. Valid values:
+        # 
+        # *   waf_group: basic web protection
+        # *   custom_acl: custom protection
+        # *   whitelist: IP address whitelist
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domain:
             self.domain.validate()
 
     def to_map(self):
@@ -24190,25 +25120,25 @@
             temp_model = DescribeDcdnWafGeoInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnWafLogsRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, page_number=None, page_size=None, start_time=None):
-        # The accelerated domain name. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query the logs.
+        # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time  # type: str
-        # The number of the page to return. Valid values: positive integers.
+        # The number of the page to return. Valid values: an integer greater than 0.
         self.page_number = page_number  # type: long
         # The number of entries to return on each page. Default value: **300**. Valid values: **1 to 1000**.
         self.page_size = page_size  # type: long
-        # The beginning of the time range to query the logs.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -24335,15 +25265,15 @@
     def __init__(self, domain_name=None, log_count=None, log_infos=None, page_infos=None):
         # The WAF domain name.
         self.domain_name = domain_name  # type: str
         # The total number of entries returned on the current page.
         self.log_count = log_count  # type: long
         # The log information.
         self.log_infos = log_infos  # type: list[DescribeDcdnWafLogsResponseBodyDomainLogDetailsLogInfos]
-        # The page information. The page information is indicated by the PageInfoDetail parameter.
+        # The page information.
         self.page_infos = page_infos  # type: DescribeDcdnWafLogsResponseBodyDomainLogDetailsPageInfos
 
     def validate(self):
         if self.log_infos:
             for k in self.log_infos:
                 if k:
                     k.validate()
@@ -24383,15 +25313,15 @@
             temp_model = DescribeDcdnWafLogsResponseBodyDomainLogDetailsPageInfos()
             self.page_infos = temp_model.from_map(m['PageInfos'])
         return self
 
 
 class DescribeDcdnWafLogsResponseBody(TeaModel):
     def __init__(self, domain_log_details=None, request_id=None):
-        # Details about domain logs.
+        # Details about logs returned.
         self.domain_log_details = domain_log_details  # type: list[DescribeDcdnWafLogsResponseBodyDomainLogDetails]
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domain_log_details:
             for k in self.domain_log_details:
@@ -24693,15 +25623,15 @@
 
 class DescribeDcdnWafPolicyResponseBodyPolicy(TeaModel):
     def __init__(self, defense_scene=None, domain_count=None, gmt_modified=None, policy_id=None, policy_name=None,
                  policy_status=None, policy_type=None, rule_configs=None, rule_count=None):
         # The type of the protection policy. Valid values:
         # 
         # *   waf_group: basic web protection
-        # *   custom_acl: custom
+        # *   custom_acl: custom protection
         # *   whitelist: whitelist
         self.defense_scene = defense_scene  # type: str
         # The number of domain names that use the protection policy.
         self.domain_count = domain_count  # type: int
         # The time when the protection policy was modified. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.gmt_modified = gmt_modified  # type: str
         # The ID of the protection policy.
@@ -24711,18 +25641,18 @@
         # The status of the protection policy. Valid values:
         # 
         # *   on
         # *   off
         self.policy_status = policy_status  # type: str
         # Indicates whether the current policy is the default policy. Valid values:
         # 
-        # *   default: The current policy is the default policy.
-        # *   custom: The current policy is not the default policy.
+        # *   default
+        # *   custom
         self.policy_type = policy_type  # type: str
-        # The protection rule configurations corresponding to the protection policy. The configurations only support Bot management. For more information, see [Configure protection rules](~~423350~~).
+        # The protection rule configurations that are defined in the protection policy. The configurations only support bot management. For more information, see [Configure protection rules](~~423350~~).
         self.rule_configs = rule_configs  # type: str
         # The number of protection rules in the protection policy.
         self.rule_count = rule_count  # type: long
 
     def validate(self):
         pass
 
@@ -24845,19 +25775,19 @@
             temp_model = DescribeDcdnWafPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnWafPolicyDomainsRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, policy_id=None):
-        # The number of the page to return. Valid values: **1** to **100000**. Default value: **1**.
+        # The page number of the returned page, which is the same as the PageNumber parameter in request parameters.
         self.page_number = page_number  # type: int
-        # The number of domain names to return per page. Valid values: an integer from **1** to **500**. Default value: **20**.
+        # The total number of domain names returned.
         self.page_size = page_size  # type: int
-        # The ID of the protection policy. You can specify only one ID in each request.
+        # The ID of the request.
         self.policy_id = policy_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnWafPolicyDomainsRequest, self).to_map()
@@ -24907,21 +25837,21 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class DescribeDcdnWafPolicyDomainsResponseBody(TeaModel):
     def __init__(self, domains=None, page_number=None, page_size=None, request_id=None, total_count=None):
-        # The accelerated domain names.
+        # The ID of the protection policy. You can specify only one ID in each request.
         self.domains = domains  # type: list[DescribeDcdnWafPolicyDomainsResponseBodyDomains]
-        # The page number of the returned page, which is the same as the PageNumber parameter in request parameters.
+        # >You can call this operation up to 20 times per second per account.
         self.page_number = page_number  # type: int
-        # The number of domain names returned per page, which is the same as the PageSize parameter in request parameters.
+        # The accelerated domain names.
         self.page_size = page_size  # type: int
-        # The ID of the request.
+        # The accelerated domain name that was protected by the specified protection policy.
         self.request_id = request_id  # type: str
         # The total number of domain names returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.domains:
             for k in self.domains:
@@ -25414,19 +26344,19 @@
         return self
 
 
 class DescribeDcdnWafRulesRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, query_args=None):
         # The number of the page to return. Valid values: **1** to **100000**. Default value: **1**.
         self.page_number = page_number  # type: int
-        # The number of protection rules to return per page. Valid values: an integer from **1** to **500**. Default value: **20**.
+        # The number of protection rules to return per page. Valid values: integers from **1** to **500**. Default value: **20**.
         self.page_size = page_size  # type: int
-        # The query conditions. The value is a string in the JSON format: `QueryArgs={"PolicyIds":"The range of protection policy IDs","RuleIds":"The range of protection rule IDs","RuleNameLike":"The name of the protection rule","DomainNames":"The protected domain names","DefenseScenes":"waf_group","RuleStatus":"on","OrderBy":"GmtModified","Desc":"false"}`
+        # The query conditions. The value needs to be a JSON string in the following format: `QueryArgs={"PolicyIds":"The range of protection policy IDs","RuleIds":"The range of protection rule IDs","RuleNameLike":"The name of the protection rule","DomainNames":"The protected domain names","DefenseScenes":"waf_group","RuleStatus":"on","OrderBy":"GmtModified","Desc":"false"}`.
         # 
-        # >  If you do not specify this parameter, all protection rules are queried.
+        # > If you do not specify this parameter, all protection rules are queried.
         self.query_args = query_args  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnWafRulesRequest, self).to_map()
@@ -25452,27 +26382,27 @@
             self.query_args = m.get('QueryArgs')
         return self
 
 
 class DescribeDcdnWafRulesResponseBodyRules(TeaModel):
     def __init__(self, defense_scene=None, gmt_modified=None, policy_id=None, rule_config=None, rule_id=None,
                  rule_name=None, rule_status=None):
-        # The type of the protection policy, which is the same as the DefenseScenes field in the QueryArgs parameter.
+        # The type of the protection policy. The value of this parameter is the same as that of the DefenseScene field in QueryArgst.
         self.defense_scene = defense_scene  # type: str
-        # The modification time. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The time when the protection policy was last modified. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.gmt_modified = gmt_modified  # type: str
         # The ID of the protection policy.
         self.policy_id = policy_id  # type: long
         # The configuration information about the protection rule.
         self.rule_config = rule_config  # type: str
         # The ID of the protection rule.
         self.rule_id = rule_id  # type: long
         # The name of the protection rule.
         self.rule_name = rule_name  # type: str
-        # The status of the protection rule, which is the same as the RuleStatus field in the QueryArgs parameter.
+        # The status of the protection rule. The value of this parameter is the same as that of the RuleStatus field in QueryArgst.
         self.rule_status = rule_status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnWafRulesResponseBodyRules, self).to_map()
@@ -25513,17 +26443,17 @@
         if m.get('RuleStatus') is not None:
             self.rule_status = m.get('RuleStatus')
         return self
 
 
 class DescribeDcdnWafRulesResponseBody(TeaModel):
     def __init__(self, page_number=None, page_size=None, request_id=None, rules=None, total_count=None):
-        # The page number of the returned page, which is the same as the PageNumber parameter in request parameters.
+        # The page number of the returned page. The value of this parameter is the same as that of the PageNumber parameter in the request.
         self.page_number = page_number  # type: int
-        # The number of protection rules returned per page, which is the same as the PageSize parameter in request parameters.
+        # The number of protection rules returned per page. The value of this parameter is the same as that of the PageSize parameter in the request.
         self.page_size = page_size  # type: int
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The information about the protection rule.
         self.rules = rules  # type: list[DescribeDcdnWafRulesResponseBodyRules]
         # The total number of protection rules.
         self.total_count = total_count  # type: int
@@ -27017,15 +27947,15 @@
             temp_model = DescribeRDDomainsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRoutineRequest(TeaModel):
     def __init__(self, name=None):
-        # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
+        # The metadata of the routine. The next table describes the fields.
         self.name = name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRoutineRequest, self).to_map()
@@ -27042,17 +27972,17 @@
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
 class DescribeRoutineResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The metadata of the routine. The next table describes the fields.
-        self.content = content  # type: dict[str, any]
         # The ID of the request.
+        self.content = content  # type: dict[str, any]
+        # The operation that you want to perform. Set the value to **DescribeRoutine**.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRoutineResponseBody, self).to_map()
@@ -27112,17 +28042,17 @@
             temp_model = DescribeRoutineResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRoutineCanaryEnvsResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The canary release environments that are supported by the edge routine.
-        self.content = content  # type: dict[str, any]
         # The ID of the region.
+        self.content = content  # type: dict[str, any]
+        # The operation that you want to perform. Set the value to **DescribeRoutineCanaryEnvs**.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRoutineCanaryEnvsResponseBody, self).to_map()
@@ -27213,15 +28143,15 @@
         if m.get('SelectCodeRevision') is not None:
             self.select_code_revision = m.get('SelectCodeRevision')
         return self
 
 
 class DescribeRoutineCodeRevisionResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The JavaScript code returned.
+        # The information about the JavaScript code version.
         self.content = content  # type: dict[str, any]
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -27454,17 +28384,17 @@
         return self
 
 
 class DescribeUserDcdnIpaStatusResponseBody(TeaModel):
     def __init__(self, enabled=None, in_debt=None, in_debt_overdue=None, on_service=None, request_id=None):
         # Indicates whether the IPA service is activated.
         self.enabled = enabled  # type: bool
-        # Indicates whether your IPA service has overdue payments.
+        # Indicates whether you have overdue payments.
         self.in_debt = in_debt  # type: bool
-        # Indicates whether an overdue bill has been paid within a specified period.
+        # Indicates whether the grace period for your overdue payments expired.
         self.in_debt_overdue = in_debt_overdue  # type: bool
         # Indicates whether the IPA service is available. The IPA service is available when no payment is overdue.
         self.on_service = on_service  # type: bool
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
@@ -27566,17 +28496,17 @@
         return self
 
 
 class DescribeUserDcdnStatusResponseBody(TeaModel):
     def __init__(self, enabled=None, in_debt=None, in_debt_overdue=None, on_service=None, request_id=None):
         # Indicates whether the DCDN service is activated.
         self.enabled = enabled  # type: bool
-        # Indicates whether the DCDN service has overdue payments.
+        # Indicates whether your account has overdue payments.
         self.in_debt = in_debt  # type: bool
-        # Indicates whether an overdue bill has been paid within the specified period.
+        # Indicates whether the grace period for your overdue payments expired.
         self.in_debt_overdue = in_debt_overdue  # type: bool
         # Indicates whether the service is available.
         self.on_service = on_service  # type: bool
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
@@ -27678,31 +28608,31 @@
         return self
 
 
 class DescribeUserErStatusResponseBody(TeaModel):
     def __init__(self, enabled=None, in_debt=None, in_debt_overdue=None, on_service=None, request_id=None):
         # Indicates whether ER is activated.
         # 
-        # *   true: activated
-        # *   false: not activated
+        # *   true
+        # *   false
         self.enabled = enabled  # type: bool
         # Indicates whether ER has an overdue payment.
         # 
-        # *   true: has an overdue payment
-        # *   false: does not have an overdue payment
+        # *   true
+        # *   false
         self.in_debt = in_debt  # type: bool
         # Indicates whether an overdue payment of ER has passed the grace period.
         # 
-        # *   true: has passed the grace period
-        # *   false: has not passed the grace period
+        # *   true
+        # *   false
         self.in_debt_overdue = in_debt_overdue  # type: bool
         # Indicates whether ER is available.
         # 
-        # *   true: available
-        # *   false: unavailable
+        # *   true
+        # *   false
         self.on_service = on_service  # type: bool
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -27807,31 +28737,31 @@
         return self
 
 
 class DescribeUserLogserviceStatusResponseBody(TeaModel):
     def __init__(self, enabled=None, in_debt=None, in_debt_overdue=None, on_service=None, request_id=None):
         # Indicates whether Log Service is activated.
         # 
-        # *   true: activated
-        # *   false: not activated
+        # *   true
+        # *   false
         self.enabled = enabled  # type: bool
         # Indicates whether your Log Service has overdue payments.
         # 
-        # *   true: Your Log Service has overdue payments.
-        # *   false: Your Log Service does not have overdue payments.
+        # *   true
+        # *   false
         self.in_debt = in_debt  # type: bool
-        # Indicates whether the overdue payments of Log Service have passed the grace period.
+        # Indicates whether an overdue payment of your Log Service has passed the grace period.
         # 
-        # *   true: The overdue payments of Log Service have passed the grace period.
-        # *   false: The overdue payments of Log Service have not passed the grace period.
+        # *   true
+        # *   false
         self.in_debt_overdue = in_debt_overdue  # type: bool
         # Indicates whether Log Service is available.
         # 
-        # *   true: available
-        # *   false: unavailable
+        # *   true
+        # *   false
         self.on_service = on_service  # type: bool
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -28063,17 +28993,17 @@
             temp_model = EditRoutineConfResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetDcdnKvRequest(TeaModel):
     def __init__(self, key=None, namespace=None):
-        # The name of the key that you want to query.
-        self.key = key  # type: str
         # The name of the namespace.
+        self.key = key  # type: str
+        # Queries the value of the key in a key-value pair.
         self.namespace = namespace  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetDcdnKvRequest, self).to_map()
@@ -28094,17 +29024,17 @@
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
         return self
 
 
 class GetDcdnKvResponseBody(TeaModel):
     def __init__(self, request_id=None, value=None):
-        # The ID of the request.
-        self.request_id = request_id  # type: str
         # The value of the key.
+        self.request_id = request_id  # type: str
+        # The name of the key that you want to query.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetDcdnKvResponseBody, self).to_map()
@@ -28509,22 +29439,22 @@
 
 class ModifyDcdnWafPolicyRequest(TeaModel):
     def __init__(self, policy_id=None, policy_name=None, policy_status=None):
         # The ID of the protection policy that you want to modify. You can specify only one ID in each request.
         self.policy_id = policy_id  # type: long
         # The new name of the protection policy.
         # 
-        # >  You must specify PolicyName or PolicyStatus.
+        # > You must specify PolicyName or PolicyStatus.
         self.policy_name = policy_name  # type: str
         # The new status of the protection policy. Valid values:
         # 
         # *   **on**\
         # *   **off**\
         # 
-        # >  You must specify PolicyName or PolicyStatus.
+        # > You must specify PolicyName or PolicyStatus.
         self.policy_status = policy_status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDcdnWafPolicyRequest, self).to_map()
@@ -28613,24 +29543,17 @@
             temp_model = ModifyDcdnWafPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyDcdnWafPolicyDomainsRequest(TeaModel):
     def __init__(self, bind_domains=None, method=None, policy_id=None, unbind_domains=None):
-        # The domain names that you want to bind to the protection policy. You can specify up to 50 domain names. Separate multiple domain names with commas (,).
-        # 
-        # > You can configure only one of the **BindDomains** and **UnbindDomains** parameters.
         self.bind_domains = bind_domains  # type: str
         self.method = method  # type: int
-        # The ID of the protection policy. You can specify only one ID in each request.
         self.policy_id = policy_id  # type: long
-        # The domain names that you want to unbind from the protection policy. You can specify up to 50 domain names. Separate multiple domain names with commas (,).
-        # 
-        # > You can configure only one of the **BindDomains** and **UnbindDomains** parameters.
         self.unbind_domains = unbind_domains  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDcdnWafPolicyDomainsRequest, self).to_map()
@@ -28659,15 +29582,14 @@
         if m.get('UnbindDomains') is not None:
             self.unbind_domains = m.get('UnbindDomains')
         return self
 
 
 class ModifyDcdnWafPolicyDomainsResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDcdnWafPolicyDomainsResponseBody, self).to_map()
@@ -28725,15 +29647,15 @@
         return self
 
 
 class ModifyDcdnWafRuleRequest(TeaModel):
     def __init__(self, rule_config=None, rule_id=None, rule_name=None, rule_status=None):
         # The new configurations of the protection rule.
         # 
-        # >  After you modify the configurations of the protection rule, the previous configurations are overwritten.
+        # > After you modify the configurations of the protection rule, the previous configurations are overwritten.
         self.rule_config = rule_config  # type: str
         # The ID of the protection rule. You can specify only one ID in each request.
         self.rule_id = rule_id  # type: long
         # The new name of the protection rule.
         self.rule_name = rule_name  # type: str
         # The new status of the protection rule. Valid values:
         # 
@@ -28948,26 +29870,26 @@
 
 class PreloadDcdnObjectCachesRequest(TeaModel):
     def __init__(self, area=None, l_2preload=None, object_path=None, owner_id=None, security_token=None,
                  with_header=None):
         # The acceleration region in which you want to prefetch content. If you do not specify a region, the value overseas is used.
         # 
         # *   **domestic**: Chinese mainland
-        # *   **overseas**: global (excluding the Chinese mainland)
+        # *   **overseas**: outside the Chinese mainland
         self.area = area  # type: str
-        # Specifies whether to prefetch content to POPs. Default value: false. Valid values:
+        # Specifies whether to prefetch content to POPs. Valid values:
         # 
-        # *   **true**: prefetches content to POPs that include L2 POPs.
+        # *   **true**: prefetches content to nodes that include L2 DCDN nodes.
         # *   **false**: prefetches content to L2 POPs or L3 POPs.
         self.l_2preload = l_2preload  # type: bool
         # The path of the content that you want to prefetch. Separate multiple URLs with line feed characters (\n) or a pair of carriage return and line feed characters (\r\n).
         self.object_path = object_path  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
-        # The custom header for prefetch in JSON format.
+        # The custom header for prefetch in the JSON format.
         self.with_header = with_header  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PreloadDcdnObjectCachesRequest, self).to_map()
@@ -29074,15 +29996,15 @@
             temp_model = PreloadDcdnObjectCachesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PublishDcdnStagingConfigToProductionRequest(TeaModel):
     def __init__(self, domain_name=None, function_name=None):
-        # The name of the accelerated domain. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
         # The name of the feature.
         self.function_name = function_name  # type: str
 
     def validate(self):
         pass
 
@@ -29172,16 +30094,18 @@
 
 
 class PublishRoutineCodeRevisionRequest(TeaModel):
     def __init__(self, envs=None, name=None, select_code_revision=None):
         # The environment to which you want to publish the code.
         # 
         # > 
+        # 
         # *   production: the name of the environment, including the environment name (SpecName) and the domain name whitelist (AllowedHosts).
-        # *   presetCanary: **You can add canary release environments based on your business requirements. This parameter is optional.
+        # 
+        # *   Preset_Canary_xx: You can add canary release environments based on your business requirements. This parameter is optional.
         self.envs = envs  # type: dict[str, any]
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
         self.name = name  # type: str
         # The version of the routine code that you want to publish.
         self.select_code_revision = select_code_revision  # type: str
 
     def validate(self):
@@ -29213,16 +30137,18 @@
 
 
 class PublishRoutineCodeRevisionShrinkRequest(TeaModel):
     def __init__(self, envs_shrink=None, name=None, select_code_revision=None):
         # The environment to which you want to publish the code.
         # 
         # > 
+        # 
         # *   production: the name of the environment, including the environment name (SpecName) and the domain name whitelist (AllowedHosts).
-        # *   presetCanary: **You can add canary release environments based on your business requirements. This parameter is optional.
+        # 
+        # *   Preset_Canary_xx: You can add canary release environments based on your business requirements. This parameter is optional.
         self.envs_shrink = envs_shrink  # type: str
         # The name of the routine. The name must be unique among the routines that belong to the same Alibaba Cloud account.
         self.name = name  # type: str
         # The version of the routine code that you want to publish.
         self.select_code_revision = select_code_revision  # type: str
 
     def validate(self):
@@ -29253,15 +30179,15 @@
         return self
 
 
 class PublishRoutineCodeRevisionResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
         # The version of the routine code that is published to the specified environment.
         self.content = content  # type: dict[str, any]
-        # The ID of the region.
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PublishRoutineCodeRevisionResponseBody, self).to_map()
@@ -29321,19 +30247,19 @@
             temp_model = PublishRoutineCodeRevisionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutDcdnKvRequest(TeaModel):
     def __init__(self, key=None, namespace=None, value=None):
-        # The name of the key. The name can be up to 512 characters in length, and cannot contain spaces.
+        # The length of the key.
         self.key = key  # type: str
-        # The name of the namespace.
-        self.namespace = namespace  # type: str
         # The content of the key. The maximum size is 2 MB (2 x 1000 x 1000 bytes).
+        self.namespace = namespace  # type: str
+        # The content of the key. If the value exceeds 256 characters in length, the first 100 characters and the last 100 characters are retained and other characters are discarded.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PutDcdnKvRequest, self).to_map()
@@ -29358,19 +30284,17 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class PutDcdnKvResponseBody(TeaModel):
     def __init__(self, length=None, request_id=None, value=None):
-        # The length of the key.
-        self.length = length  # type: int
         # The ID of the request.
+        self.length = length  # type: int
         self.request_id = request_id  # type: str
-        # The content of the key. If the value exceeds 256 characters in length, the first 100 characters and the last 100 characters are retained and other characters are discarded.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PutDcdnKvResponseBody, self).to_map()
@@ -29436,15 +30360,15 @@
         return self
 
 
 class RefreshDcdnObjectCachesRequest(TeaModel):
     def __init__(self, object_path=None, object_type=None, owner_id=None, security_token=None):
         # The path of the objects that you want to refresh. Separate multiple URLs with line feed characters (\n) or a pair of carriage return and line feed characters (\r\n).
         self.object_path = object_path  # type: str
-        # The refresh type. Default value: File. Valid values:
+        # The refresh type. Valid values:
         # 
         # *   **File**: URL
         # *   **Directory**: directory
         self.object_type = object_type  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
@@ -29548,15 +30472,15 @@
             temp_model = RefreshDcdnObjectCachesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RollbackDcdnStagingConfigRequest(TeaModel):
     def __init__(self, domain_name=None):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # >  You can call this operation up to 30 times per second per account.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RollbackDcdnStagingConfigRequest, self).to_map()
@@ -29573,15 +30497,15 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class RollbackDcdnStagingConfigResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The accelerated domain name. You can specify only one domain name in each call.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RollbackDcdnStagingConfigResponseBody, self).to_map()
@@ -29638,43 +30562,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetDcdnDomainCertificateRequest(TeaModel):
     def __init__(self, cert_name=None, cert_type=None, domain_name=None, force_set=None, owner_id=None, region=None,
                  sslpri=None, sslprotocol=None, sslpub=None, security_token=None):
-        # The name of the certificate.
+        # Specifies whether to enable the SSL certificate. Default value: off. Valid values:
+        # 
+        # *   **on**: enables the SSL certificate.
+        # *   **off**: disables the SSL certificate.
         self.cert_name = cert_name  # type: str
+        # The content of the certificate. This parameter is required only if you enable the SSL certificate.
+        self.cert_type = cert_type  # type: str
         # The type of the certificate.
         # 
         # *   **upload**: a user-uploaded SSL certificate.
         # *   **cas**: a certificate that is acquired through SSL Certificates Service.
         # *   **free**: a free certificate.
         # 
         # > 
         # *   If the value of the CertType parameter is **cas**, the **SSLPri** parameter is not required.
         # *   If the value of the CertType parameter is **free**, the **SSLPri** and **SSLPub** parameters are not required.
-        self.cert_type = cert_type  # type: str
-        # The accelerated domain name. You can specify only one domain name.
-        # 
-        # HTTPS acceleration must be enabled for the accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information about the existing certificate that uses the same name.
+        # >  You can call this operation up to 30 times per second per account.
         self.force_set = force_set  # type: str
         self.owner_id = owner_id  # type: long
-        # The region. Default value: ch-hangzhou.
+        # The ID of the request.
         self.region = region  # type: str
-        # The private key. This parameter is required only if you enable the SSL certificate.
+        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information about the existing certificate that uses the same name.
         self.sslpri = sslpri  # type: str
-        # Specifies whether to enable the SSL certificate. Default value: off. Valid values:
-        # 
-        # *   **on**: enables the SSL certificate.
-        # *   **off**: disables the SSL certificate.
+        # The private key. This parameter is required only if you enable the SSL certificate.
         self.sslprotocol = sslprotocol  # type: str
-        # The content of the certificate. This parameter is required only if you enable the SSL certificate.
+        # The region. Default value: ch-hangzhou.
         self.sslpub = sslpub  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -29728,15 +30650,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class SetDcdnDomainCertificateResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The private key. This parameter is required only if you enable the SSL certificate.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetDcdnDomainCertificateResponseBody, self).to_map()
@@ -30032,15 +30954,15 @@
             temp_model = SetDcdnDomainStagingConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetDcdnUserConfigRequest(TeaModel):
     def __init__(self, configs=None, function_id=None, owner_account=None, owner_id=None, security_token=None):
-        # The configuration parameters of the features.
+        # The configuration parameters of the feature.
         self.configs = configs  # type: str
         # The ID of the feature.
         self.function_id = function_id  # type: int
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
@@ -30146,20 +31068,17 @@
 
 class SetRoutineSubdomainRequest(TeaModel):
     def __init__(self, subdomains=None):
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
         self.subdomains = subdomains  # type: dict[str, any]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetRoutineSubdomainRequest, self).to_map()
@@ -30180,20 +31099,17 @@
 
 class SetRoutineSubdomainShrinkRequest(TeaModel):
     def __init__(self, subdomains_shrink=None):
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
         self.subdomains_shrink = subdomains_shrink  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetRoutineSubdomainShrinkRequest, self).to_map()
@@ -30280,15 +31196,14 @@
             temp_model = SetRoutineSubdomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StartDcdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, security_token=None):
-        # The name of the accelerated domain to be enabled. You can specify only one domain name.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -30315,15 +31230,14 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class StartDcdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StartDcdnDomainResponseBody, self).to_map()
@@ -30379,15 +31293,14 @@
             temp_model = StartDcdnDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StartDcdnIpaDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, security_token=None):
-        # The name of the accelerated domain to be enabled. You can specify only one accelerated domain name at a time.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -30414,15 +31327,14 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class StartDcdnIpaDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StartDcdnIpaDomainResponseBody, self).to_map()
@@ -31036,23 +31948,23 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateDcdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, resource_group_id=None, security_token=None, sources=None,
                  top_level_domain=None):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The top-level domain name.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
-        # The ID of the resource group.
+        # The ID of the request.
         self.resource_group_id = resource_group_id  # type: str
         self.security_token = security_token  # type: str
-        # The information about the addresses of origin servers.
+        # The accelerated domain name. You can specify only one domain name in each call.
         self.sources = sources  # type: str
-        # The top-level domain name.
+        # The operation that you want to perform. Set the value to **UpdateDcdnDomain**.
         self.top_level_domain = top_level_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateDcdnDomainRequest, self).to_map()
@@ -31089,15 +32001,15 @@
         if m.get('TopLevelDomain') is not None:
             self.top_level_domain = m.get('TopLevelDomain')
         return self
 
 
 class UpdateDcdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The information about the addresses of origin servers.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateDcdnDomainResponseBody, self).to_map()
@@ -31275,23 +32187,23 @@
         # 
         # *   **cn**: Chinese mainland
         # *   **sg**: Singapore
         # *   **in**: India
         # *   **eu**: Europe
         # *   **us**: United States
         self.data_center = data_center  # type: str
-        # The domain names. You can specify one or more domain names. Separate multiple domain names with commas (,).
+        # The domain names from which logs were collected. You can specify one or more domain names. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The name of the real-time log delivery project.
+        # The name of the project.
         self.project_name = project_name  # type: str
         # The name of the Logstore.
         self.slslog_store = slslog_store  # type: str
-        # The name of the Log Service project.
+        # The name of the log file.
         self.slsproject = slsproject  # type: str
-        # The region to which logs are delivered.
+        # The region to which logs were delivered.
         self.slsregion = slsregion  # type: str
         # The sampling rate.
         self.sampling_rate = sampling_rate  # type: str
 
     def validate(self):
         pass
 
@@ -31336,17 +32248,17 @@
         return self
 
 
 class UpdateDcdnSLSRealtimeLogDeliveryResponseBodyContentDomains(TeaModel):
     def __init__(self, desc=None, domain_name=None, region=None, status=None):
         # The description of the returned result.
         self.desc = desc  # type: str
-        # The domain name for which the real-time log delivery project was updated.
+        # The domain name.
         self.domain_name = domain_name  # type: str
-        # The region from which logs were collected.
+        # The name of the region.
         self.region = region  # type: str
         # Indicates whether the real-time log delivery project was successfully updated. Valid values:
         # 
         # *   **success**\
         # *   **fail**\
         self.status = status  # type: str
 
@@ -31486,19 +32398,17 @@
         return self
 
 
 class UpdateDcdnSubTaskRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, report_ids=None, start_time=None):
         # The domain names that you want to include in the operations report. If you do not specify a domain name, all domain names that belong to your Alibaba Cloud account are included.
         self.domain_name = domain_name  # type: str
-        # The end time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time  # type: str
-        # The IDs of operations reports that you want to update. Separate IDs with commas (,). You can call the [DescribeDcdnSubList](~~270075~~) operation to query report IDs.
+        # The operation that you want to perform. Set the value to **UpdateDcdnSubTask**.
         self.report_ids = report_ids  # type: str
-        # The start time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateDcdnSubTaskRequest, self).to_map()
@@ -31527,15 +32437,14 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class UpdateDcdnSubTaskResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateDcdnSubTaskResponseBody, self).to_map()
@@ -31721,15 +32630,15 @@
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
 class UploadRoutineCodeResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The content returned that includes the code version number and information about code upload.
+        # The content returned, such as the code version number and information about the code upload.
         self.content = content  # type: dict[str, any]
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO` & `alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dcdn20180115-py2
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.7/setup.py` & `alibabacloud_dcdn20180115_py2-1.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dcdn20180115_py2.
 
-Created on 19/05/2023
+Created on 22/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dcdn20180115"
 NAME = "alibabacloud_dcdn20180115_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dcdn (20180115) SDK Library for Python2"
```

