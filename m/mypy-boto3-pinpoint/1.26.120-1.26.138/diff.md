# Comparing `tmp/mypy-boto3-pinpoint-1.26.120.tar.gz` & `tmp/mypy-boto3-pinpoint-1.26.138.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-1.26.120.tar", last modified: Tue Apr 25 21:20:46 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.26.138.tar", last modified: Mon May 22 19:33:39 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-1.26.120.tar` & `mypy-boto3-pinpoint-1.26.138.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-04-25 21:20:32.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-25 21:20:32.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-04-25 21:20:32.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   159068 2023-04-25 21:20:36.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   158851 2023-04-25 21:20:34.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   158826 2023-05-22 19:31:54.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158609 2023-05-22 19:31:52.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/setup.py
```

### Comparing `mypy-boto3-pinpoint-1.26.120/LICENSE` & `mypy-boto3-pinpoint-1.26.138/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.120/PKG-INFO` & `mypy-boto3-pinpoint-1.26.138/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.26.120
-Summary: Type annotations for boto3.Pinpoint 1.26.120 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.138
+Summary: Type annotations for boto3.Pinpoint 1.26.138 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.120](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.138](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -358,14 +358,15 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
+    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -408,15 +409,14 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -502,15 +502,14 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -520,49 +519,50 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    GetAdmChannelResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
-    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdmChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    GetAppResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    RemoveAttributesResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.26.120/README.md` & `mypy-boto3-pinpoint-1.26.138/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.120](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.138](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -326,14 +326,15 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
+    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -376,15 +377,14 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -470,15 +470,14 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -488,49 +487,50 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    GetAdmChannelResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
-    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdmChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    GetAppResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    RemoveAttributesResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/__main__.py` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pinpoint 1.26.120\nVersion:         1.26.120\nBuilder version:"
+        "Type annotations for boto3.Pinpoint 1.26.138\nVersion:         1.26.138\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.120")
+    print("1.26.138")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,14 +343,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -369,14 +370,15 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
```

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -341,14 +341,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -367,14 +368,15 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
```

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
@@ -86,14 +85,15 @@
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
@@ -136,15 +136,14 @@
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
@@ -230,15 +229,14 @@
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
     "RandomSplitEntryTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
@@ -248,49 +246,50 @@
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
     "VerifyOTPMessageRequestParametersTypeDef",
     "UpdateAdmChannelRequestRequestTypeDef",
-    "DeleteAdmChannelResponseTypeDef",
-    "GetAdmChannelResponseTypeDef",
-    "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
-    "DeleteApnsChannelResponseTypeDef",
-    "GetApnsChannelResponseTypeDef",
-    "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
-    "DeleteApnsSandboxChannelResponseTypeDef",
-    "GetApnsSandboxChannelResponseTypeDef",
-    "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
-    "DeleteApnsVoipChannelResponseTypeDef",
-    "GetApnsVoipChannelResponseTypeDef",
-    "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
-    "GetApnsVoipSandboxChannelResponseTypeDef",
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "GetAppResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
     "WriteApplicationSettingsRequestTypeDef",
-    "RemoveAttributesResponseTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
-    "DeleteBaiduChannelResponseTypeDef",
-    "GetBaiduChannelResponseTypeDef",
-    "UpdateBaiduChannelResponseTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
+    "CreateAppResponseTypeDef",
+    "DeleteAdmChannelResponseTypeDef",
+    "DeleteApnsChannelResponseTypeDef",
+    "DeleteApnsSandboxChannelResponseTypeDef",
+    "DeleteApnsVoipChannelResponseTypeDef",
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "DeleteBaiduChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAdmChannelResponseTypeDef",
+    "GetApnsChannelResponseTypeDef",
+    "GetApnsSandboxChannelResponseTypeDef",
+    "GetApnsVoipChannelResponseTypeDef",
+    "GetApnsVoipSandboxChannelResponseTypeDef",
+    "GetAppResponseTypeDef",
+    "GetBaiduChannelResponseTypeDef",
+    "RemoveAttributesResponseTypeDef",
+    "UpdateAdmChannelResponseTypeDef",
+    "UpdateApnsChannelResponseTypeDef",
+    "UpdateApnsSandboxChannelResponseTypeDef",
+    "UpdateApnsVoipChannelResponseTypeDef",
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+    "UpdateBaiduChannelResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
@@ -517,21 +516,19 @@
     "_OptionalADMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class ADMChannelRequestTypeDef(
     _RequiredADMChannelRequestTypeDef, _OptionalADMChannelRequestTypeDef
 ):
     pass
 
-
 _RequiredADMChannelResponseTypeDef = TypedDict(
     "_RequiredADMChannelResponseTypeDef",
     {
         "Platform": str,
     },
 )
 _OptionalADMChannelResponseTypeDef = TypedDict(
@@ -546,21 +543,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class ADMChannelResponseTypeDef(
     _RequiredADMChannelResponseTypeDef, _OptionalADMChannelResponseTypeDef
 ):
     pass
 
-
 ADMMessageTypeDef = TypedDict(
     "ADMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ConsolidationKey": str,
         "Data": Mapping[str, str],
@@ -615,21 +610,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSChannelResponseTypeDef(
     _RequiredAPNSChannelResponseTypeDef, _OptionalAPNSChannelResponseTypeDef
 ):
     pass
 
-
 APNSMessageTypeDef = TypedDict(
     "APNSMessageTypeDef",
     {
         "APNSPushType": str,
         "Action": ActionType,
         "Badge": int,
         "Body": str,
@@ -700,21 +693,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSSandboxChannelResponseTypeDef(
     _RequiredAPNSSandboxChannelResponseTypeDef, _OptionalAPNSSandboxChannelResponseTypeDef
 ):
     pass
 
-
 APNSVoipChannelRequestTypeDef = TypedDict(
     "APNSVoipChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -746,21 +737,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSVoipChannelResponseTypeDef(
     _RequiredAPNSVoipChannelResponseTypeDef, _OptionalAPNSVoipChannelResponseTypeDef
 ):
     pass
 
-
 APNSVoipSandboxChannelRequestTypeDef = TypedDict(
     "APNSVoipSandboxChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -792,21 +781,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSVoipSandboxChannelResponseTypeDef(
     _RequiredAPNSVoipSandboxChannelResponseTypeDef, _OptionalAPNSVoipSandboxChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredActivityResponseTypeDef = TypedDict(
     "_RequiredActivityResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "Id": str,
     },
@@ -825,19 +812,17 @@
         "TotalEndpointCount": int,
         "TreatmentId": str,
         "ExecutionMetrics": Dict[str, str],
     },
     total=False,
 )
 
-
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
-
 ContactCenterActivityTypeDef = TypedDict(
     "ContactCenterActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
@@ -852,19 +837,17 @@
     "_OptionalHoldoutActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
 
-
 class HoldoutActivityTypeDef(_RequiredHoldoutActivityTypeDef, _OptionalHoldoutActivityTypeDef):
     pass
 
-
 AddressConfigurationTypeDef = TypedDict(
     "AddressConfigurationTypeDef",
     {
         "BodyOverride": str,
         "ChannelType": ChannelTypeType,
         "Context": Mapping[str, str],
         "RawContent": str,
@@ -903,21 +886,19 @@
     {
         "tags": Dict[str, str],
         "CreationDate": str,
     },
     total=False,
 )
 
-
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
-
 CampaignHookTypeDef = TypedDict(
     "CampaignHookTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
@@ -955,21 +936,19 @@
     "_OptionalAttributeDimensionTypeDef",
     {
         "AttributeType": AttributeTypeType,
     },
     total=False,
 )
 
-
 class AttributeDimensionTypeDef(
     _RequiredAttributeDimensionTypeDef, _OptionalAttributeDimensionTypeDef
 ):
     pass
 
-
 _RequiredAttributesResourceTypeDef = TypedDict(
     "_RequiredAttributesResourceTypeDef",
     {
         "ApplicationId": str,
         "AttributeType": str,
     },
 )
@@ -977,21 +956,19 @@
     "_OptionalAttributesResourceTypeDef",
     {
         "Attributes": List[str],
     },
     total=False,
 )
 
-
 class AttributesResourceTypeDef(
     _RequiredAttributesResourceTypeDef, _OptionalAttributesResourceTypeDef
 ):
     pass
 
-
 _RequiredBaiduChannelRequestTypeDef = TypedDict(
     "_RequiredBaiduChannelRequestTypeDef",
     {
         "ApiKey": str,
         "SecretKey": str,
     },
 )
@@ -999,21 +976,19 @@
     "_OptionalBaiduChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class BaiduChannelRequestTypeDef(
     _RequiredBaiduChannelRequestTypeDef, _OptionalBaiduChannelRequestTypeDef
 ):
     pass
 
-
 _RequiredBaiduChannelResponseTypeDef = TypedDict(
     "_RequiredBaiduChannelResponseTypeDef",
     {
         "Credential": str,
         "Platform": str,
     },
 )
@@ -1029,21 +1004,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class BaiduChannelResponseTypeDef(
     _RequiredBaiduChannelResponseTypeDef, _OptionalBaiduChannelResponseTypeDef
 ):
     pass
 
-
 BaiduMessageTypeDef = TypedDict(
     "BaiduMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Data": Mapping[str, str],
         "IconReference": str,
@@ -1098,21 +1071,19 @@
     "_OptionalCustomDeliveryConfigurationTypeDef",
     {
         "EndpointTypes": Sequence[EndpointTypesElementType],
     },
     total=False,
 )
 
-
 class CustomDeliveryConfigurationTypeDef(
     _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
 ):
     pass
 
-
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
@@ -1167,20 +1138,29 @@
     "_OptionalCreateApplicationRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestTypeDef(
     _RequiredCreateApplicationRequestTypeDef, _OptionalCreateApplicationRequestTypeDef
 ):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
 
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": str,
         "HtmlPart": str,
         "RecommenderId": str,
@@ -1214,19 +1194,17 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
-
 class ExportJobRequestTypeDef(_RequiredExportJobRequestTypeDef, _OptionalExportJobRequestTypeDef):
     pass
 
-
 _RequiredImportJobRequestTypeDef = TypedDict(
     "_RequiredImportJobRequestTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -1239,19 +1217,17 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
-
 class ImportJobRequestTypeDef(_RequiredImportJobRequestTypeDef, _OptionalImportJobRequestTypeDef):
     pass
 
-
 TemplateCreateMessageBodyTypeDef = TypedDict(
     "TemplateCreateMessageBodyTypeDef",
     {
         "Arn": str,
         "Message": str,
         "RequestID": str,
     },
@@ -1275,21 +1251,19 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class CreateRecommenderConfigurationTypeDef(
     _RequiredCreateRecommenderConfigurationTypeDef, _OptionalCreateRecommenderConfigurationTypeDef
 ):
     pass
 
-
 _RequiredRecommenderConfigurationResponseTypeDef = TypedDict(
     "_RequiredRecommenderConfigurationResponseTypeDef",
     {
         "CreationDate": str,
         "Id": str,
         "LastModifiedDate": str,
         "RecommendationProviderRoleArn": str,
@@ -1306,22 +1280,20 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class RecommenderConfigurationResponseTypeDef(
     _RequiredRecommenderConfigurationResponseTypeDef,
     _OptionalRecommenderConfigurationResponseTypeDef,
 ):
     pass
 
-
 SMSTemplateRequestTypeDef = TypedDict(
     "SMSTemplateRequestTypeDef",
     {
         "Body": str,
         "DefaultSubstitutions": str,
         "RecommenderId": str,
         "tags": Mapping[str, str],
@@ -1365,21 +1337,19 @@
         "BorderRadius": int,
         "Link": str,
         "TextColor": str,
     },
     total=False,
 )
 
-
 class DefaultButtonConfigurationTypeDef(
     _RequiredDefaultButtonConfigurationTypeDef, _OptionalDefaultButtonConfigurationTypeDef
 ):
     pass
 
-
 DefaultMessageTypeDef = TypedDict(
     "DefaultMessageTypeDef",
     {
         "Body": str,
         "Substitutions": Mapping[str, Sequence[str]],
     },
     total=False,
@@ -1498,43 +1468,39 @@
         "MessagesPerSecond": int,
         "RoleArn": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class EmailChannelResponseTypeDef(
     _RequiredEmailChannelResponseTypeDef, _OptionalEmailChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteEmailTemplateRequestRequestTypeDef(
     _RequiredDeleteEmailTemplateRequestRequestTypeDef,
     _OptionalDeleteEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 MessageBodyTypeDef = TypedDict(
     "MessageBodyTypeDef",
     {
         "Message": str,
         "RequestID": str,
     },
     total=False,
@@ -1569,19 +1535,17 @@
         "ExternalId": str,
         "LastModifiedDate": str,
         "LastUpdatedBy": str,
     },
     total=False,
 )
 
-
 class EventStreamTypeDef(_RequiredEventStreamTypeDef, _OptionalEventStreamTypeDef):
     pass
 
-
 DeleteGcmChannelRequestRequestTypeDef = TypedDict(
     "DeleteGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -1604,43 +1568,39 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class GCMChannelResponseTypeDef(
     _RequiredGCMChannelResponseTypeDef, _OptionalGCMChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInAppTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteInAppTemplateRequestRequestTypeDef(
     _RequiredDeleteInAppTemplateRequestRequestTypeDef,
     _OptionalDeleteInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteJourneyRequestRequestTypeDef = TypedDict(
     "DeleteJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
     },
 )
@@ -1655,22 +1615,20 @@
     "_OptionalDeletePushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeletePushTemplateRequestRequestTypeDef(
     _RequiredDeletePushTemplateRequestRequestTypeDef,
     _OptionalDeletePushTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -1711,42 +1669,38 @@
         "ShortCode": str,
         "TransactionalMessagesPerSecond": int,
         "Version": int,
     },
     total=False,
 )
 
-
 class SMSChannelResponseTypeDef(
     _RequiredSMSChannelResponseTypeDef, _OptionalSMSChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSmsTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteSmsTemplateRequestRequestTypeDef(
     _RequiredDeleteSmsTemplateRequestRequestTypeDef, _OptionalDeleteSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 DeleteUserEndpointsRequestRequestTypeDef = TypedDict(
     "DeleteUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -1776,43 +1730,39 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class VoiceChannelResponseTypeDef(
     _RequiredVoiceChannelResponseTypeDef, _OptionalVoiceChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteVoiceTemplateRequestRequestTypeDef(
     _RequiredDeleteVoiceTemplateRequestRequestTypeDef,
     _OptionalDeleteVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 GCMMessageTypeDef = TypedDict(
     "GCMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
@@ -1874,21 +1824,19 @@
         "ConfigurationSet": str,
         "Enabled": bool,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class EmailChannelRequestTypeDef(
     _RequiredEmailChannelRequestTypeDef, _OptionalEmailChannelRequestTypeDef
 ):
     pass
 
-
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
@@ -1922,28 +1870,19 @@
         "TemplateDescription": str,
         "TextPart": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class EmailTemplateResponseTypeDef(
     _RequiredEmailTemplateResponseTypeDef, _OptionalEmailTemplateResponseTypeDef
 ):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": str,
         "Locale": str,
         "Make": str,
         "Model": str,
@@ -2000,21 +1939,19 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
-
 class EndpointMessageResultTypeDef(
     _RequiredEndpointMessageResultTypeDef, _OptionalEndpointMessageResultTypeDef
 ):
     pass
 
-
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": str,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -2041,19 +1978,17 @@
     "_OptionalSetDimensionTypeDef",
     {
         "DimensionType": DimensionTypeType,
     },
     total=False,
 )
 
-
 class SetDimensionTypeDef(_RequiredSetDimensionTypeDef, _OptionalSetDimensionTypeDef):
     pass
 
-
 EventItemResponseTypeDef = TypedDict(
     "EventItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
@@ -2071,19 +2006,17 @@
     {
         "Duration": int,
         "StopTimestamp": str,
     },
     total=False,
 )
 
-
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
-
 _RequiredExportJobResourceTypeDef = TypedDict(
     "_RequiredExportJobResourceTypeDef",
     {
         "RoleArn": str,
         "S3UrlPrefix": str,
     },
 )
@@ -2092,42 +2025,38 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
-
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
-
 _RequiredGCMChannelRequestTypeDef = TypedDict(
     "_RequiredGCMChannelRequestTypeDef",
     {
         "ApiKey": str,
     },
 )
 _OptionalGCMChannelRequestTypeDef = TypedDict(
     "_OptionalGCMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class GCMChannelRequestTypeDef(
     _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
 ):
     pass
 
-
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -2188,22 +2117,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetApplicationDateRangeKpiRequestRequestTypeDef(
     _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
     _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 GetApplicationSettingsRequestRequestTypeDef = TypedDict(
     "GetApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2235,22 +2162,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignActivitiesRequestRequestTypeDef(
     _RequiredGetCampaignActivitiesRequestRequestTypeDef,
     _OptionalGetCampaignActivitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "KpiName": str,
     },
@@ -2262,22 +2187,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetCampaignDateRangeKpiRequestRequestTypeDef(
     _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
     _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
     },
 )
@@ -2303,22 +2226,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignVersionsRequestRequestTypeDef(
     _RequiredGetCampaignVersionsRequestRequestTypeDef,
     _OptionalGetCampaignVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCampaignsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetCampaignsRequestRequestTypeDef = TypedDict(
@@ -2326,21 +2247,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignsRequestRequestTypeDef(
     _RequiredGetCampaignsRequestRequestTypeDef, _OptionalGetCampaignsRequestRequestTypeDef
 ):
     pass
 
-
 GetChannelsRequestRequestTypeDef = TypedDict(
     "GetChannelsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2361,21 +2280,19 @@
     "_OptionalGetEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetEmailTemplateRequestRequestTypeDef(
     _RequiredGetEmailTemplateRequestRequestTypeDef, _OptionalGetEmailTemplateRequestRequestTypeDef
 ):
     pass
 
-
 GetEndpointRequestRequestTypeDef = TypedDict(
     "GetEndpointRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2406,21 +2323,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetExportJobsRequestRequestTypeDef(
     _RequiredGetExportJobsRequestRequestTypeDef, _OptionalGetExportJobsRequestRequestTypeDef
 ):
     pass
 
-
 GetGcmChannelRequestRequestTypeDef = TypedDict(
     "GetGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2443,21 +2358,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetImportJobsRequestRequestTypeDef(
     _RequiredGetImportJobsRequestRequestTypeDef, _OptionalGetImportJobsRequestRequestTypeDef
 ):
     pass
 
-
 GetInAppMessagesRequestRequestTypeDef = TypedDict(
     "GetInAppMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2472,21 +2385,19 @@
     "_OptionalGetInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetInAppTemplateRequestRequestTypeDef(
     _RequiredGetInAppTemplateRequestRequestTypeDef, _OptionalGetInAppTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "KpiName": str,
     },
@@ -2498,22 +2409,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetJourneyDateRangeKpiRequestRequestTypeDef(
     _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
     _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
     },
@@ -2523,22 +2432,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2559,22 +2466,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2603,22 +2508,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2641,22 +2544,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2676,42 +2577,38 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunsRequestRequestTypeDef(
     _RequiredGetJourneyRunsRequestRequestTypeDef, _OptionalGetJourneyRunsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetPushTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetPushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetPushTemplateRequestRequestTypeDef(
     _RequiredGetPushTemplateRequestRequestTypeDef, _OptionalGetPushTemplateRequestRequestTypeDef
 ):
     pass
 
-
 GetRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -2736,22 +2633,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentExportJobsRequestRequestTypeDef(
     _RequiredGetSegmentExportJobsRequestRequestTypeDef,
     _OptionalGetSegmentExportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSegmentImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentImportJobsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2760,22 +2655,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentImportJobsRequestRequestTypeDef(
     _RequiredGetSegmentImportJobsRequestRequestTypeDef,
     _OptionalGetSegmentImportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 GetSegmentRequestRequestTypeDef = TypedDict(
     "GetSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2801,22 +2694,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentVersionsRequestRequestTypeDef(
     _RequiredGetSegmentVersionsRequestRequestTypeDef,
     _OptionalGetSegmentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSegmentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetSegmentsRequestRequestTypeDef = TypedDict(
@@ -2824,21 +2715,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentsRequestRequestTypeDef(
     _RequiredGetSegmentsRequestRequestTypeDef, _OptionalGetSegmentsRequestRequestTypeDef
 ):
     pass
 
-
 GetSmsChannelRequestRequestTypeDef = TypedDict(
     "GetSmsChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2852,21 +2741,19 @@
     "_OptionalGetSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetSmsTemplateRequestRequestTypeDef(
     _RequiredGetSmsTemplateRequestRequestTypeDef, _OptionalGetSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSMSTemplateResponseTypeDef = TypedDict(
     "_RequiredSMSTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2882,21 +2769,19 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class SMSTemplateResponseTypeDef(
     _RequiredSMSTemplateResponseTypeDef, _OptionalSMSTemplateResponseTypeDef
 ):
     pass
 
-
 GetUserEndpointsRequestRequestTypeDef = TypedDict(
     "GetUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -2918,21 +2803,19 @@
     "_OptionalGetVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetVoiceTemplateRequestRequestTypeDef(
     _RequiredGetVoiceTemplateRequestRequestTypeDef, _OptionalGetVoiceTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredVoiceTemplateResponseTypeDef = TypedDict(
     "_RequiredVoiceTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2949,21 +2832,19 @@
         "TemplateDescription": str,
         "Version": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-
 class VoiceTemplateResponseTypeDef(
     _RequiredVoiceTemplateResponseTypeDef, _OptionalVoiceTemplateResponseTypeDef
 ):
     pass
 
-
 _RequiredImportJobResourceTypeDef = TypedDict(
     "_RequiredImportJobResourceTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -2976,21 +2857,19 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
-
 class ImportJobResourceTypeDef(
     _RequiredImportJobResourceTypeDef, _OptionalImportJobResourceTypeDef
 ):
     pass
 
-
 InAppMessageBodyConfigTypeDef = TypedDict(
     "InAppMessageBodyConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Body": str,
         "TextColor": str,
     },
@@ -3006,21 +2885,19 @@
     "_OptionalOverrideButtonConfigurationTypeDef",
     {
         "Link": str,
     },
     total=False,
 )
 
-
 class OverrideButtonConfigurationTypeDef(
     _RequiredOverrideButtonConfigurationTypeDef, _OptionalOverrideButtonConfigurationTypeDef
 ):
     pass
 
-
 InAppMessageHeaderConfigTypeDef = TypedDict(
     "InAppMessageHeaderConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Header": str,
         "TextColor": str,
     },
@@ -3105,21 +2982,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class ListJourneysRequestRequestTypeDef(
     _RequiredListJourneysRequestRequestTypeDef, _OptionalListJourneysRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3142,22 +3017,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class ListTemplateVersionsRequestRequestTypeDef(
     _RequiredListTemplateVersionsRequestRequestTypeDef,
     _OptionalListTemplateVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": str,
         "Prefix": str,
         "TemplateType": str,
@@ -3197,19 +3070,17 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
-
 class MessageResultTypeDef(_RequiredMessageResultTypeDef, _OptionalMessageResultTypeDef):
     pass
 
-
 NumberValidateRequestTypeDef = TypedDict(
     "NumberValidateRequestTypeDef",
     {
         "IsoCountryCode": str,
         "PhoneNumber": str,
     },
     total=False,
@@ -3274,25 +3145,14 @@
     "UpdateAttributesRequestTypeDef",
     {
         "Blacklist": Sequence[str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ResultRowValueTypeDef = TypedDict(
     "ResultRowValueTypeDef",
     {
         "Key": str,
         "Type": str,
         "Value": str,
     },
@@ -3325,19 +3185,17 @@
     "_OptionalSegmentReferenceTypeDef",
     {
         "Version": int,
     },
     total=False,
 )
 
-
 class SegmentReferenceTypeDef(_RequiredSegmentReferenceTypeDef, _OptionalSegmentReferenceTypeDef):
     pass
 
-
 _RequiredSegmentImportResourceTypeDef = TypedDict(
     "_RequiredSegmentImportResourceTypeDef",
     {
         "ExternalId": str,
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
@@ -3348,21 +3206,19 @@
     "_OptionalSegmentImportResourceTypeDef",
     {
         "ChannelCounts": Dict[str, int],
     },
     total=False,
 )
 
-
 class SegmentImportResourceTypeDef(
     _RequiredSegmentImportResourceTypeDef, _OptionalSegmentImportResourceTypeDef
 ):
     pass
 
-
 _RequiredSendOTPMessageRequestParametersTypeDef = TypedDict(
     "_RequiredSendOTPMessageRequestParametersTypeDef",
     {
         "BrandName": str,
         "Channel": str,
         "DestinationIdentity": str,
         "OriginationIdentity": str,
@@ -3378,21 +3234,19 @@
         "Language": str,
         "TemplateId": str,
         "ValidityPeriod": int,
     },
     total=False,
 )
 
-
 class SendOTPMessageRequestParametersTypeDef(
     _RequiredSendOTPMessageRequestParametersTypeDef, _OptionalSendOTPMessageRequestParametersTypeDef
 ):
     pass
 
-
 SimpleEmailPartTypeDef = TypedDict(
     "SimpleEmailPartTypeDef",
     {
         "Charset": str,
         "Data": str,
     },
     total=False,
@@ -3432,19 +3286,17 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class TemplateResponseTypeDef(_RequiredTemplateResponseTypeDef, _OptionalTemplateResponseTypeDef):
     pass
 
-
 _RequiredTemplateVersionResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": str,
@@ -3456,21 +3308,19 @@
         "DefaultSubstitutions": str,
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class TemplateVersionResponseTypeDef(
     _RequiredTemplateVersionResponseTypeDef, _OptionalTemplateVersionResponseTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -3492,21 +3342,19 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class UpdateRecommenderConfigurationTypeDef(
     _RequiredUpdateRecommenderConfigurationTypeDef, _OptionalUpdateRecommenderConfigurationTypeDef
 ):
     pass
 
-
 VoiceChannelRequestTypeDef = TypedDict(
     "VoiceChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -3532,328 +3380,331 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     {
         "ADMChannelRequest": ADMChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-DeleteAdmChannelResponseTypeDef = TypedDict(
-    "DeleteAdmChannelResponseTypeDef",
+UpdateApnsChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSChannelRequest": APNSChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-GetAdmChannelResponseTypeDef = TypedDict(
-    "GetAdmChannelResponseTypeDef",
+UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-UpdateAdmChannelResponseTypeDef = TypedDict(
-    "UpdateAdmChannelResponseTypeDef",
+UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-UpdateApnsChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsChannelRequestRequestTypeDef",
+UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     {
-        "APNSChannelRequest": APNSChannelRequestTypeDef,
+        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-DeleteApnsChannelResponseTypeDef = TypedDict(
-    "DeleteApnsChannelResponseTypeDef",
+_RequiredActivitiesResponseTypeDef = TypedDict(
+    "_RequiredActivitiesResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Item": List[ActivityResponseTypeDef],
     },
 )
-
-GetApnsChannelResponseTypeDef = TypedDict(
-    "GetApnsChannelResponseTypeDef",
+_OptionalActivitiesResponseTypeDef = TypedDict(
+    "_OptionalActivitiesResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextToken": str,
     },
+    total=False,
 )
 
-UpdateApnsChannelResponseTypeDef = TypedDict(
-    "UpdateApnsChannelResponseTypeDef",
+class ActivitiesResponseTypeDef(
+    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
+):
+    pass
+
+ApplicationsResponseTypeDef = TypedDict(
+    "ApplicationsResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Item": List[ApplicationResponseTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelRequestRequestTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
-
-DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsSandboxChannelResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsSandboxChannelResponseTypeDef",
-    {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
 
-UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelResponseTypeDef",
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipChannelRequestRequestTypeDef",
+UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
+    "UpdateBaiduChannelRequestRequestTypeDef",
     {
-        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
         "ApplicationId": str,
+        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-DeleteApnsVoipChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipChannelResponseTypeDef",
+ChannelsResponseTypeDef = TypedDict(
+    "ChannelsResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-GetApnsVoipChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipChannelResponseTypeDef",
+ClosedDaysTypeDef = TypedDict(
+    "ClosedDaysTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
+        "SMS": Sequence[ClosedDaysRuleTypeDef],
+        "PUSH": Sequence[ClosedDaysRuleTypeDef],
+        "VOICE": Sequence[ClosedDaysRuleTypeDef],
+        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateApnsVoipChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipChannelResponseTypeDef",
+WaitActivityTypeDef = TypedDict(
+    "WaitActivityTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextActivity": str,
+        "WaitTime": WaitTimeTypeDef,
     },
+    total=False,
 )
 
-UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
-        "ApplicationId": str,
+        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
     },
 )
 
-DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipSandboxChannelResponseTypeDef",
+DeleteAdmChannelResponseTypeDef = TypedDict(
+    "DeleteAdmChannelResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+DeleteApnsChannelResponseTypeDef = TypedDict(
+    "DeleteApnsChannelResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActivitiesResponseTypeDef = TypedDict(
-    "_RequiredActivitiesResponseTypeDef",
-    {
-        "Item": List[ActivityResponseTypeDef],
-    },
-)
-_OptionalActivitiesResponseTypeDef = TypedDict(
-    "_OptionalActivitiesResponseTypeDef",
+DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsSandboxChannelResponseTypeDef",
     {
-        "NextToken": str,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ActivitiesResponseTypeDef(
-    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
-):
-    pass
-
-
-ApplicationsResponseTypeDef = TypedDict(
-    "ApplicationsResponseTypeDef",
+DeleteApnsVoipChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipChannelResponseTypeDef",
     {
-        "Item": List[ApplicationResponseTypeDef],
-        "NextToken": str,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppResponseTypeDef = TypedDict(
     "DeleteAppResponseTypeDef",
     {
         "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+DeleteBaiduChannelResponseTypeDef = TypedDict(
+    "DeleteBaiduChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "ApplicationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+GetAdmChannelResponseTypeDef = TypedDict(
+    "GetAdmChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetApnsChannelResponseTypeDef = TypedDict(
+    "GetApnsChannelResponseTypeDef",
+    {
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
-
-
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+GetApnsSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-RemoveAttributesResponseTypeDef = TypedDict(
-    "RemoveAttributesResponseTypeDef",
+GetApnsVoipChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipChannelResponseTypeDef",
     {
-        "AttributesResource": AttributesResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
-    "UpdateBaiduChannelRequestRequestTypeDef",
+GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationId": str,
-        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteBaiduChannelResponseTypeDef = TypedDict(
-    "DeleteBaiduChannelResponseTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBaiduChannelResponseTypeDef = TypedDict(
     "GetBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBaiduChannelResponseTypeDef = TypedDict(
-    "UpdateBaiduChannelResponseTypeDef",
+RemoveAttributesResponseTypeDef = TypedDict(
+    "RemoveAttributesResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttributesResource": AttributesResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChannelsResponseTypeDef = TypedDict(
-    "ChannelsResponseTypeDef",
+UpdateAdmChannelResponseTypeDef = TypedDict(
+    "UpdateAdmChannelResponseTypeDef",
     {
-        "Channels": Dict[str, ChannelResponseTypeDef],
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ClosedDaysTypeDef = TypedDict(
-    "ClosedDaysTypeDef",
+UpdateApnsChannelResponseTypeDef = TypedDict(
+    "UpdateApnsChannelResponseTypeDef",
     {
-        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
-        "SMS": Sequence[ClosedDaysRuleTypeDef],
-        "PUSH": Sequence[ClosedDaysRuleTypeDef],
-        "VOICE": Sequence[ClosedDaysRuleTypeDef],
-        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-WaitActivityTypeDef = TypedDict(
-    "WaitActivityTypeDef",
+UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelResponseTypeDef",
     {
-        "NextActivity": str,
-        "WaitTime": WaitTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+UpdateApnsVoipChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipChannelResponseTypeDef",
     {
-        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+    {
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBaiduChannelResponseTypeDef = TypedDict(
+    "UpdateBaiduChannelResponseTypeDef",
+    {
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "EmailTemplateRequest": EmailTemplateRequestTypeDef,
@@ -3873,51 +3724,49 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePushTemplateResponseTypeDef = TypedDict(
     "CreatePushTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSmsTemplateResponseTypeDef = TypedDict(
     "CreateSmsTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVoiceTemplateResponseTypeDef = TypedDict(
     "CreateVoiceTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExportJobRequestRequestTypeDef = TypedDict(
     "CreateExportJobRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -3933,46 +3782,46 @@
     },
 )
 
 CreateInAppTemplateResponseTypeDef = TypedDict(
     "CreateInAppTemplateResponseTypeDef",
     {
         "TemplateCreateMessageBody": TemplateCreateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecommenderConfigurationRequestRequestTypeDef",
     {
         "CreateRecommenderConfiguration": CreateRecommenderConfigurationTypeDef,
     },
 )
 
 CreateRecommenderConfigurationResponseTypeDef = TypedDict(
     "CreateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRecommenderConfigurationResponseTypeDef = TypedDict(
     "DeleteRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommenderConfigurationResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListRecommenderConfigurationsResponseTypeDef = TypedDict(
     "_RequiredListRecommenderConfigurationsResponseTypeDef",
     {
         "Item": List[RecommenderConfigurationResponseTypeDef],
@@ -3982,27 +3831,25 @@
     "_OptionalListRecommenderConfigurationsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRecommenderConfigurationsResponseTypeDef(
     _RequiredListRecommenderConfigurationsResponseTypeDef,
     _OptionalListRecommenderConfigurationsResponseTypeDef,
 ):
     pass
 
-
 UpdateRecommenderConfigurationResponseTypeDef = TypedDict(
     "UpdateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSmsTemplateRequestRequestTypeDef = TypedDict(
     "CreateSmsTemplateRequestRequestTypeDef",
     {
         "SMSTemplateRequest": SMSTemplateRequestTypeDef,
@@ -4022,21 +3869,19 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateSmsTemplateRequestRequestTypeDef(
     _RequiredUpdateSmsTemplateRequestRequestTypeDef, _OptionalUpdateSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 CreateVoiceTemplateRequestRequestTypeDef = TypedDict(
     "CreateVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "VoiceTemplateRequest": VoiceTemplateRequestTypeDef,
     },
 )
@@ -4053,22 +3898,20 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateVoiceTemplateRequestRequestTypeDef(
     _RequiredUpdateVoiceTemplateRequestRequestTypeDef,
     _OptionalUpdateVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 CustomMessageActivityTypeDef = TypedDict(
     "CustomMessageActivityTypeDef",
     {
         "DeliveryUri": str,
         "EndpointTypes": Sequence[EndpointTypesElementType],
         "MessageConfig": JourneyCustomMessageTypeDef,
         "NextActivity": str,
@@ -4117,243 +3960,241 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class PushNotificationTemplateResponseTypeDef(
     _RequiredPushNotificationTemplateResponseTypeDef,
     _OptionalPushNotificationTemplateResponseTypeDef,
 ):
     pass
 
-
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEmailChannelResponseTypeDef = TypedDict(
     "GetEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailChannelResponseTypeDef = TypedDict(
     "UpdateEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEmailTemplateResponseTypeDef = TypedDict(
     "DeleteEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInAppTemplateResponseTypeDef = TypedDict(
     "DeleteInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePushTemplateResponseTypeDef = TypedDict(
     "DeletePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSmsTemplateResponseTypeDef = TypedDict(
     "DeleteSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVoiceTemplateResponseTypeDef = TypedDict(
     "DeleteVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailTemplateResponseTypeDef = TypedDict(
     "UpdateEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointsBatchResponseTypeDef = TypedDict(
     "UpdateEndpointsBatchResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInAppTemplateResponseTypeDef = TypedDict(
     "UpdateInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePushTemplateResponseTypeDef = TypedDict(
     "UpdatePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSmsTemplateResponseTypeDef = TypedDict(
     "UpdateSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTemplateActiveVersionResponseTypeDef = TypedDict(
     "UpdateTemplateActiveVersionResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceTemplateResponseTypeDef = TypedDict(
     "UpdateVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventStreamResponseTypeDef = TypedDict(
     "DeleteEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventStreamResponseTypeDef = TypedDict(
     "PutEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGcmChannelResponseTypeDef = TypedDict(
     "DeleteGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGcmChannelResponseTypeDef = TypedDict(
     "GetGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGcmChannelResponseTypeDef = TypedDict(
     "UpdateGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSmsChannelResponseTypeDef = TypedDict(
     "DeleteSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSmsChannelResponseTypeDef = TypedDict(
     "GetSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSmsChannelResponseTypeDef = TypedDict(
     "UpdateSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVoiceChannelResponseTypeDef = TypedDict(
     "DeleteVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceChannelResponseTypeDef = TypedDict(
     "GetVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceChannelResponseTypeDef = TypedDict(
     "UpdateVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailChannelRequestRequestTypeDef = TypedDict(
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4372,15 +4213,15 @@
     total=False,
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": str,
@@ -4468,21 +4309,19 @@
     {
         "RequestId": str,
         "Result": Dict[str, Dict[str, EndpointMessageResultTypeDef]],
     },
     total=False,
 )
 
-
 class SendUsersMessageResponseTypeDef(
     _RequiredSendUsersMessageResponseTypeDef, _OptionalSendUsersMessageResponseTypeDef
 ):
     pass
 
-
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "EventType": SetDimensionTypeDef,
         "Metrics": Mapping[str, MetricDimensionTypeDef],
     },
@@ -4529,19 +4368,17 @@
         "Metrics": Mapping[str, float],
         "SdkName": str,
         "Session": SessionTypeDef,
     },
     total=False,
 )
 
-
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
-
 _RequiredExportJobResponseTypeDef = TypedDict(
     "_RequiredExportJobResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
         "Definition": ExportJobResourceTypeDef,
         "Id": str,
@@ -4559,21 +4396,19 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
-
 class ExportJobResponseTypeDef(
     _RequiredExportJobResponseTypeDef, _OptionalExportJobResponseTypeDef
 ):
     pass
 
-
 UpdateGcmChannelRequestRequestTypeDef = TypedDict(
     "UpdateGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "GCMChannelRequest": GCMChannelRequestTypeDef,
     },
 )
@@ -4588,68 +4423,66 @@
     "_OptionalGPSPointDimensionTypeDef",
     {
         "RangeInKilometers": float,
     },
     total=False,
 )
 
-
 class GPSPointDimensionTypeDef(
     _RequiredGPSPointDimensionTypeDef, _OptionalGPSPointDimensionTypeDef
 ):
     pass
 
-
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionMetricsResponseTypeDef",
     {
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyRunExecutionActivityMetricsResponse": (
             JourneyRunExecutionActivityMetricsResponseTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     {
         "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSmsTemplateResponseTypeDef = TypedDict(
     "GetSmsTemplateResponseTypeDef",
     {
         "SMSTemplateResponse": SMSTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceTemplateResponseTypeDef = TypedDict(
     "GetVoiceTemplateResponseTypeDef",
     {
         "VoiceTemplateResponse": VoiceTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportJobResponseTypeDef = TypedDict(
     "_RequiredImportJobResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4670,21 +4503,19 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
-
 class ImportJobResponseTypeDef(
     _RequiredImportJobResponseTypeDef, _OptionalImportJobResponseTypeDef
 ):
     pass
 
-
 InAppMessageButtonTypeDef = TypedDict(
     "InAppMessageButtonTypeDef",
     {
         "Android": OverrideButtonConfigurationTypeDef,
         "DefaultConfig": DefaultButtonConfigurationTypeDef,
         "IOS": OverrideButtonConfigurationTypeDef,
         "Web": OverrideButtonConfigurationTypeDef,
@@ -4713,21 +4544,19 @@
     "_OptionalJourneyRunsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneyRunsResponseTypeDef(
     _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
 ):
     pass
 
-
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4744,15 +4573,15 @@
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagsModel": TagsModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -4772,31 +4601,29 @@
         "EndpointResult": Dict[str, EndpointMessageResultTypeDef],
         "RequestId": str,
         "Result": Dict[str, MessageResultTypeDef],
     },
     total=False,
 )
 
-
 class MessageResponseTypeDef(_RequiredMessageResponseTypeDef, _OptionalMessageResponseTypeDef):
     pass
 
-
 PhoneNumberValidateRequestRequestTypeDef = TypedDict(
     "PhoneNumberValidateRequestRequestTypeDef",
     {
         "NumberValidateRequest": NumberValidateRequestTypeDef,
     },
 )
 
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4905,21 +4732,19 @@
     "_OptionalTemplatesResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class TemplatesResponseTypeDef(
     _RequiredTemplatesResponseTypeDef, _OptionalTemplatesResponseTypeDef
 ):
     pass
 
-
 _RequiredTemplateVersionsResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionsResponseTypeDef",
     {
         "Item": List[TemplateVersionResponseTypeDef],
     },
 )
 _OptionalTemplateVersionsResponseTypeDef = TypedDict(
@@ -4928,21 +4753,19 @@
         "Message": str,
         "NextToken": str,
         "RequestID": str,
     },
     total=False,
 )
 
-
 class TemplateVersionsResponseTypeDef(
     _RequiredTemplateVersionsResponseTypeDef, _OptionalTemplateVersionsResponseTypeDef
 ):
     pass
 
-
 UpdateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
         "UpdateRecommenderConfiguration": UpdateRecommenderConfigurationTypeDef,
     },
 )
@@ -4955,15 +4778,15 @@
     },
 )
 
 VerifyOTPMessageResponseTypeDef = TypedDict(
     "VerifyOTPMessageResponseTypeDef",
     {
         "VerificationResponse": VerificationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifyOTPMessageRequestRequestTypeDef = TypedDict(
     "VerifyOTPMessageRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4971,39 +4794,39 @@
     },
 )
 
 GetCampaignActivitiesResponseTypeDef = TypedDict(
     "GetCampaignActivitiesResponseTypeDef",
     {
         "ActivitiesResponse": ActivitiesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppsResponseTypeDef = TypedDict(
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationSettingsResponseTypeDef = TypedDict(
     "GetApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationSettingsResponseTypeDef = TypedDict(
     "UpdateApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
     "UpdateApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5011,23 +4834,23 @@
     },
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommenderConfigurationsResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
@@ -5047,27 +4870,25 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdatePushTemplateRequestRequestTypeDef(
     _RequiredUpdatePushTemplateRequestRequestTypeDef,
     _OptionalUpdatePushTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 GetPushTemplateResponseTypeDef = TypedDict(
     "GetPushTemplateResponseTypeDef",
     {
         "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
@@ -5083,38 +4904,38 @@
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointsResponseTypeDef = TypedDict(
     "EndpointsResponseTypeDef",
     {
         "Item": List[EndpointResponseTypeDef],
     },
 )
 
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendUsersMessagesResponseTypeDef = TypedDict(
     "SendUsersMessagesResponseTypeDef",
     {
         "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -5155,15 +4976,15 @@
     },
 )
 
 CreateExportJobResponseTypeDef = TypedDict(
     "CreateExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportJobsResponseTypeDef = TypedDict(
     "_RequiredExportJobsResponseTypeDef",
     {
         "Item": List[ExportJobResponseTypeDef],
@@ -5173,26 +4994,24 @@
     "_OptionalExportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ExportJobsResponseTypeDef(
     _RequiredExportJobsResponseTypeDef, _OptionalExportJobsResponseTypeDef
 ):
     pass
 
-
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
@@ -5201,23 +5020,23 @@
     total=False,
 )
 
 CreateImportJobResponseTypeDef = TypedDict(
     "CreateImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportJobsResponseTypeDef = TypedDict(
     "_RequiredImportJobsResponseTypeDef",
     {
         "Item": List[ImportJobResponseTypeDef],
@@ -5227,21 +5046,19 @@
     "_OptionalImportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ImportJobsResponseTypeDef(
     _RequiredImportJobsResponseTypeDef, _OptionalImportJobsResponseTypeDef
 ):
     pass
 
-
 InAppMessageContentTypeDef = TypedDict(
     "InAppMessageContentTypeDef",
     {
         "BackgroundColor": str,
         "BodyConfig": InAppMessageBodyConfigTypeDef,
         "HeaderConfig": InAppMessageHeaderConfigTypeDef,
         "ImageUrl": str,
@@ -5251,31 +5068,31 @@
     total=False,
 )
 
 GetJourneyRunsResponseTypeDef = TypedDict(
     "GetJourneyRunsResponseTypeDef",
     {
         "JourneyRunsResponse": JourneyRunsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendMessagesResponseTypeDef = TypedDict(
     "SendMessagesResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendOTPMessageResponseTypeDef = TypedDict(
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
@@ -5296,23 +5113,23 @@
     total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesResponse": TemplatesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5320,23 +5137,23 @@
     },
 )
 
 DeleteUserEndpointsResponseTypeDef = TypedDict(
     "DeleteUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserEndpointsResponseTypeDef = TypedDict(
     "GetUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
@@ -5361,56 +5178,54 @@
         "IsLocalTime": bool,
         "QuietTime": QuietTimeTypeDef,
         "Timezone": str,
     },
     total=False,
 )
 
-
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
-
 EventStartConditionTypeDef = TypedDict(
     "EventStartConditionTypeDef",
     {
         "EventFilter": EventFilterTypeDef,
         "SegmentId": str,
     },
     total=False,
 )
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "EventsResponse": EventsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventsRequestTypeDef = TypedDict(
     "EventsRequestTypeDef",
     {
         "BatchItem": Mapping[str, EventsBatchTypeDef],
     },
 )
 
 GetExportJobsResponseTypeDef = TypedDict(
     "GetExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
@@ -5423,23 +5238,23 @@
     total=False,
 )
 
 GetImportJobsResponseTypeDef = TypedDict(
     "GetImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": str,
@@ -5491,21 +5306,19 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class InAppTemplateResponseTypeDef(
     _RequiredInAppTemplateResponseTypeDef, _OptionalInAppTemplateResponseTypeDef
 ):
     pass
 
-
 _RequiredApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "KpiName": str,
         "KpiResult": BaseKpiResultTypeDef,
@@ -5516,21 +5329,19 @@
     "_OptionalApplicationDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ApplicationDateRangeKpiResponseTypeDef(
     _RequiredApplicationDateRangeKpiResponseTypeDef, _OptionalApplicationDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 _RequiredCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredCampaignDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "EndTime": datetime,
         "KpiName": str,
@@ -5542,21 +5353,19 @@
     "_OptionalCampaignDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class CampaignDateRangeKpiResponseTypeDef(
     _RequiredCampaignDateRangeKpiResponseTypeDef, _OptionalCampaignDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 _RequiredJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredJourneyDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "JourneyId": str,
         "KpiName": str,
@@ -5568,21 +5377,19 @@
     "_OptionalJourneyDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneyDateRangeKpiResponseTypeDef(
     _RequiredJourneyDateRangeKpiResponseTypeDef, _OptionalJourneyDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 DirectMessageConfigurationTypeDef = TypedDict(
     "DirectMessageConfigurationTypeDef",
     {
         "ADMMessage": ADMMessageTypeDef,
         "APNSMessage": APNSMessageTypeDef,
         "BaiduMessage": BaiduMessageTypeDef,
         "DefaultMessage": DefaultMessageTypeDef,
@@ -5685,51 +5492,49 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateInAppTemplateRequestRequestTypeDef(
     _RequiredUpdateInAppTemplateRequestRequestTypeDef,
     _OptionalUpdateInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 GetInAppTemplateResponseTypeDef = TypedDict(
     "GetInAppTemplateResponseTypeDef",
     {
         "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "GetCampaignDateRangeKpiResponseTypeDef",
     {
         "CampaignDateRangeKpiResponse": CampaignDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "GetJourneyDateRangeKpiResponseTypeDef",
     {
         "JourneyDateRangeKpiResponse": JourneyDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMessageRequestTypeDef = TypedDict(
     "_RequiredMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
@@ -5743,19 +5548,17 @@
         "Endpoints": Mapping[str, EndpointSendConfigurationTypeDef],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
-
 class MessageRequestTypeDef(_RequiredMessageRequestTypeDef, _OptionalMessageRequestTypeDef):
     pass
 
-
 _RequiredSendUsersMessageRequestTypeDef = TypedDict(
     "_RequiredSendUsersMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
         "Users": Mapping[str, EndpointSendConfigurationTypeDef],
     },
 )
@@ -5765,21 +5568,19 @@
         "Context": Mapping[str, str],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
-
 class SendUsersMessageRequestTypeDef(
     _RequiredSendUsersMessageRequestTypeDef, _OptionalSendUsersMessageRequestTypeDef
 ):
     pass
 
-
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": Sequence[SegmentGroupTypeDef],
         "Include": IncludeType,
     },
     total=False,
@@ -5820,21 +5621,19 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
-
 class TreatmentResourceTypeDef(
     _RequiredTreatmentResourceTypeDef, _OptionalTreatmentResourceTypeDef
 ):
     pass
 
-
 _RequiredWriteTreatmentResourceTypeDef = TypedDict(
     "_RequiredWriteTreatmentResourceTypeDef",
     {
         "SizePercent": int,
     },
 )
 _OptionalWriteTreatmentResourceTypeDef = TypedDict(
@@ -5846,21 +5645,19 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
-
 class WriteTreatmentResourceTypeDef(
     _RequiredWriteTreatmentResourceTypeDef, _OptionalWriteTreatmentResourceTypeDef
 ):
     pass
 
-
 InAppMessagesResponseTypeDef = TypedDict(
     "InAppMessagesResponseTypeDef",
     {
         "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
     },
     total=False,
 )
@@ -5901,19 +5698,17 @@
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Dict[str, str],
         "Version": int,
     },
     total=False,
 )
 
-
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
-
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": SegmentDimensionsTypeDef,
         "Name": str,
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Mapping[str, str],
@@ -5975,19 +5770,17 @@
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
     },
     total=False,
 )
 
-
 class CampaignResponseTypeDef(_RequiredCampaignResponseTypeDef, _OptionalCampaignResponseTypeDef):
     pass
 
-
 WriteCampaignRequestTypeDef = TypedDict(
     "WriteCampaignRequestTypeDef",
     {
         "AdditionalTreatments": Sequence[WriteTreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "Description": str,
         "HoldoutPercent": int,
@@ -6008,47 +5801,47 @@
     total=False,
 )
 
 GetInAppMessagesResponseTypeDef = TypedDict(
     "GetInAppMessagesResponseTypeDef",
     {
         "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSegmentResponseTypeDef = TypedDict(
     "DeleteSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentVersionResponseTypeDef = TypedDict(
     "GetSegmentVersionResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSegmentsResponseTypeDef = TypedDict(
     "_RequiredSegmentsResponseTypeDef",
     {
         "Item": List[SegmentResponseTypeDef],
@@ -6058,24 +5851,22 @@
     "_OptionalSegmentsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SegmentsResponseTypeDef(_RequiredSegmentsResponseTypeDef, _OptionalSegmentsResponseTypeDef):
     pass
 
-
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6120,58 +5911,56 @@
     "_OptionalCampaignsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class CampaignsResponseTypeDef(
     _RequiredCampaignsResponseTypeDef, _OptionalCampaignsResponseTypeDef
 ):
     pass
 
-
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCampaignResponseTypeDef = TypedDict(
     "DeleteCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignResponseTypeDef = TypedDict(
     "GetCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignVersionResponseTypeDef = TypedDict(
     "GetCampaignVersionResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCampaignResponseTypeDef = TypedDict(
     "UpdateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCampaignRequestRequestTypeDef = TypedDict(
     "CreateCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6188,23 +5977,23 @@
     },
 )
 
 GetSegmentVersionsResponseTypeDef = TypedDict(
     "GetSegmentVersionsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentsResponseTypeDef = TypedDict(
     "GetSegmentsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJourneyResponseTypeDef = TypedDict(
     "_RequiredJourneyResponseTypeDef",
     {
         "ApplicationId": str,
@@ -6233,19 +6022,17 @@
         "SendingSchedule": bool,
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
     },
     total=False,
 )
 
-
 class JourneyResponseTypeDef(_RequiredJourneyResponseTypeDef, _OptionalJourneyResponseTypeDef):
     pass
 
-
 _RequiredWriteJourneyRequestTypeDef = TypedDict(
     "_RequiredWriteJourneyRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalWriteJourneyRequestTypeDef = TypedDict(
@@ -6268,58 +6055,56 @@
         "SendingSchedule": bool,
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
     },
     total=False,
 )
 
-
 class WriteJourneyRequestTypeDef(
     _RequiredWriteJourneyRequestTypeDef, _OptionalWriteJourneyRequestTypeDef
 ):
     pass
 
-
 GetCampaignVersionsResponseTypeDef = TypedDict(
     "GetCampaignVersionsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignsResponseTypeDef = TypedDict(
     "GetCampaignsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJourneyResponseTypeDef = TypedDict(
     "CreateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteJourneyResponseTypeDef = TypedDict(
     "DeleteJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyResponseTypeDef = TypedDict(
     "GetJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJourneysResponseTypeDef = TypedDict(
     "_RequiredJourneysResponseTypeDef",
     {
         "Item": List[JourneyResponseTypeDef],
@@ -6329,32 +6114,30 @@
     "_OptionalJourneysResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneysResponseTypeDef(_RequiredJourneysResponseTypeDef, _OptionalJourneysResponseTypeDef):
     pass
 
-
 UpdateJourneyResponseTypeDef = TypedDict(
     "UpdateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJourneyStateResponseTypeDef = TypedDict(
     "UpdateJourneyStateResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJourneyRequestRequestTypeDef = TypedDict(
     "CreateJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6371,10 +6154,10 @@
     },
 )
 
 ListJourneysResponseTypeDef = TypedDict(
     "ListJourneysResponseTypeDef",
     {
         "JourneysResponse": JourneysResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
@@ -85,14 +86,15 @@
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
@@ -135,15 +137,14 @@
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
@@ -229,15 +230,14 @@
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
     "RandomSplitEntryTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
@@ -247,49 +247,50 @@
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
     "VerifyOTPMessageRequestParametersTypeDef",
     "UpdateAdmChannelRequestRequestTypeDef",
-    "DeleteAdmChannelResponseTypeDef",
-    "GetAdmChannelResponseTypeDef",
-    "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
-    "DeleteApnsChannelResponseTypeDef",
-    "GetApnsChannelResponseTypeDef",
-    "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
-    "DeleteApnsSandboxChannelResponseTypeDef",
-    "GetApnsSandboxChannelResponseTypeDef",
-    "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
-    "DeleteApnsVoipChannelResponseTypeDef",
-    "GetApnsVoipChannelResponseTypeDef",
-    "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
-    "GetApnsVoipSandboxChannelResponseTypeDef",
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "GetAppResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
     "WriteApplicationSettingsRequestTypeDef",
-    "RemoveAttributesResponseTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
-    "DeleteBaiduChannelResponseTypeDef",
-    "GetBaiduChannelResponseTypeDef",
-    "UpdateBaiduChannelResponseTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
+    "CreateAppResponseTypeDef",
+    "DeleteAdmChannelResponseTypeDef",
+    "DeleteApnsChannelResponseTypeDef",
+    "DeleteApnsSandboxChannelResponseTypeDef",
+    "DeleteApnsVoipChannelResponseTypeDef",
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "DeleteBaiduChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAdmChannelResponseTypeDef",
+    "GetApnsChannelResponseTypeDef",
+    "GetApnsSandboxChannelResponseTypeDef",
+    "GetApnsVoipChannelResponseTypeDef",
+    "GetApnsVoipSandboxChannelResponseTypeDef",
+    "GetAppResponseTypeDef",
+    "GetBaiduChannelResponseTypeDef",
+    "RemoveAttributesResponseTypeDef",
+    "UpdateAdmChannelResponseTypeDef",
+    "UpdateApnsChannelResponseTypeDef",
+    "UpdateApnsSandboxChannelResponseTypeDef",
+    "UpdateApnsVoipChannelResponseTypeDef",
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+    "UpdateBaiduChannelResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
@@ -516,19 +517,21 @@
     "_OptionalADMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class ADMChannelRequestTypeDef(
     _RequiredADMChannelRequestTypeDef, _OptionalADMChannelRequestTypeDef
 ):
     pass
 
+
 _RequiredADMChannelResponseTypeDef = TypedDict(
     "_RequiredADMChannelResponseTypeDef",
     {
         "Platform": str,
     },
 )
 _OptionalADMChannelResponseTypeDef = TypedDict(
@@ -543,19 +546,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class ADMChannelResponseTypeDef(
     _RequiredADMChannelResponseTypeDef, _OptionalADMChannelResponseTypeDef
 ):
     pass
 
+
 ADMMessageTypeDef = TypedDict(
     "ADMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ConsolidationKey": str,
         "Data": Mapping[str, str],
@@ -610,19 +615,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSChannelResponseTypeDef(
     _RequiredAPNSChannelResponseTypeDef, _OptionalAPNSChannelResponseTypeDef
 ):
     pass
 
+
 APNSMessageTypeDef = TypedDict(
     "APNSMessageTypeDef",
     {
         "APNSPushType": str,
         "Action": ActionType,
         "Badge": int,
         "Body": str,
@@ -693,19 +700,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSSandboxChannelResponseTypeDef(
     _RequiredAPNSSandboxChannelResponseTypeDef, _OptionalAPNSSandboxChannelResponseTypeDef
 ):
     pass
 
+
 APNSVoipChannelRequestTypeDef = TypedDict(
     "APNSVoipChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -737,19 +746,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSVoipChannelResponseTypeDef(
     _RequiredAPNSVoipChannelResponseTypeDef, _OptionalAPNSVoipChannelResponseTypeDef
 ):
     pass
 
+
 APNSVoipSandboxChannelRequestTypeDef = TypedDict(
     "APNSVoipSandboxChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -781,19 +792,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSVoipSandboxChannelResponseTypeDef(
     _RequiredAPNSVoipSandboxChannelResponseTypeDef, _OptionalAPNSVoipSandboxChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredActivityResponseTypeDef = TypedDict(
     "_RequiredActivityResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "Id": str,
     },
@@ -812,17 +825,19 @@
         "TotalEndpointCount": int,
         "TreatmentId": str,
         "ExecutionMetrics": Dict[str, str],
     },
     total=False,
 )
 
+
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
+
 ContactCenterActivityTypeDef = TypedDict(
     "ContactCenterActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
@@ -837,17 +852,19 @@
     "_OptionalHoldoutActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
 
+
 class HoldoutActivityTypeDef(_RequiredHoldoutActivityTypeDef, _OptionalHoldoutActivityTypeDef):
     pass
 
+
 AddressConfigurationTypeDef = TypedDict(
     "AddressConfigurationTypeDef",
     {
         "BodyOverride": str,
         "ChannelType": ChannelTypeType,
         "Context": Mapping[str, str],
         "RawContent": str,
@@ -886,19 +903,21 @@
     {
         "tags": Dict[str, str],
         "CreationDate": str,
     },
     total=False,
 )
 
+
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
+
 CampaignHookTypeDef = TypedDict(
     "CampaignHookTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
@@ -936,19 +955,21 @@
     "_OptionalAttributeDimensionTypeDef",
     {
         "AttributeType": AttributeTypeType,
     },
     total=False,
 )
 
+
 class AttributeDimensionTypeDef(
     _RequiredAttributeDimensionTypeDef, _OptionalAttributeDimensionTypeDef
 ):
     pass
 
+
 _RequiredAttributesResourceTypeDef = TypedDict(
     "_RequiredAttributesResourceTypeDef",
     {
         "ApplicationId": str,
         "AttributeType": str,
     },
 )
@@ -956,19 +977,21 @@
     "_OptionalAttributesResourceTypeDef",
     {
         "Attributes": List[str],
     },
     total=False,
 )
 
+
 class AttributesResourceTypeDef(
     _RequiredAttributesResourceTypeDef, _OptionalAttributesResourceTypeDef
 ):
     pass
 
+
 _RequiredBaiduChannelRequestTypeDef = TypedDict(
     "_RequiredBaiduChannelRequestTypeDef",
     {
         "ApiKey": str,
         "SecretKey": str,
     },
 )
@@ -976,19 +999,21 @@
     "_OptionalBaiduChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class BaiduChannelRequestTypeDef(
     _RequiredBaiduChannelRequestTypeDef, _OptionalBaiduChannelRequestTypeDef
 ):
     pass
 
+
 _RequiredBaiduChannelResponseTypeDef = TypedDict(
     "_RequiredBaiduChannelResponseTypeDef",
     {
         "Credential": str,
         "Platform": str,
     },
 )
@@ -1004,19 +1029,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class BaiduChannelResponseTypeDef(
     _RequiredBaiduChannelResponseTypeDef, _OptionalBaiduChannelResponseTypeDef
 ):
     pass
 
+
 BaiduMessageTypeDef = TypedDict(
     "BaiduMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Data": Mapping[str, str],
         "IconReference": str,
@@ -1071,19 +1098,21 @@
     "_OptionalCustomDeliveryConfigurationTypeDef",
     {
         "EndpointTypes": Sequence[EndpointTypesElementType],
     },
     total=False,
 )
 
+
 class CustomDeliveryConfigurationTypeDef(
     _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
 ):
     pass
 
+
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
@@ -1138,19 +1167,32 @@
     "_OptionalCreateApplicationRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestTypeDef(
     _RequiredCreateApplicationRequestTypeDef, _OptionalCreateApplicationRequestTypeDef
 ):
     pass
 
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": str,
         "HtmlPart": str,
         "RecommenderId": str,
         "Subject": str,
@@ -1183,17 +1225,19 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
+
 class ExportJobRequestTypeDef(_RequiredExportJobRequestTypeDef, _OptionalExportJobRequestTypeDef):
     pass
 
+
 _RequiredImportJobRequestTypeDef = TypedDict(
     "_RequiredImportJobRequestTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -1206,17 +1250,19 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
+
 class ImportJobRequestTypeDef(_RequiredImportJobRequestTypeDef, _OptionalImportJobRequestTypeDef):
     pass
 
+
 TemplateCreateMessageBodyTypeDef = TypedDict(
     "TemplateCreateMessageBodyTypeDef",
     {
         "Arn": str,
         "Message": str,
         "RequestID": str,
     },
@@ -1240,19 +1286,21 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class CreateRecommenderConfigurationTypeDef(
     _RequiredCreateRecommenderConfigurationTypeDef, _OptionalCreateRecommenderConfigurationTypeDef
 ):
     pass
 
+
 _RequiredRecommenderConfigurationResponseTypeDef = TypedDict(
     "_RequiredRecommenderConfigurationResponseTypeDef",
     {
         "CreationDate": str,
         "Id": str,
         "LastModifiedDate": str,
         "RecommendationProviderRoleArn": str,
@@ -1269,20 +1317,22 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class RecommenderConfigurationResponseTypeDef(
     _RequiredRecommenderConfigurationResponseTypeDef,
     _OptionalRecommenderConfigurationResponseTypeDef,
 ):
     pass
 
+
 SMSTemplateRequestTypeDef = TypedDict(
     "SMSTemplateRequestTypeDef",
     {
         "Body": str,
         "DefaultSubstitutions": str,
         "RecommenderId": str,
         "tags": Mapping[str, str],
@@ -1326,19 +1376,21 @@
         "BorderRadius": int,
         "Link": str,
         "TextColor": str,
     },
     total=False,
 )
 
+
 class DefaultButtonConfigurationTypeDef(
     _RequiredDefaultButtonConfigurationTypeDef, _OptionalDefaultButtonConfigurationTypeDef
 ):
     pass
 
+
 DefaultMessageTypeDef = TypedDict(
     "DefaultMessageTypeDef",
     {
         "Body": str,
         "Substitutions": Mapping[str, Sequence[str]],
     },
     total=False,
@@ -1457,39 +1509,43 @@
         "MessagesPerSecond": int,
         "RoleArn": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class EmailChannelResponseTypeDef(
     _RequiredEmailChannelResponseTypeDef, _OptionalEmailChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteEmailTemplateRequestRequestTypeDef(
     _RequiredDeleteEmailTemplateRequestRequestTypeDef,
     _OptionalDeleteEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 MessageBodyTypeDef = TypedDict(
     "MessageBodyTypeDef",
     {
         "Message": str,
         "RequestID": str,
     },
     total=False,
@@ -1524,17 +1580,19 @@
         "ExternalId": str,
         "LastModifiedDate": str,
         "LastUpdatedBy": str,
     },
     total=False,
 )
 
+
 class EventStreamTypeDef(_RequiredEventStreamTypeDef, _OptionalEventStreamTypeDef):
     pass
 
+
 DeleteGcmChannelRequestRequestTypeDef = TypedDict(
     "DeleteGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -1557,39 +1615,43 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class GCMChannelResponseTypeDef(
     _RequiredGCMChannelResponseTypeDef, _OptionalGCMChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInAppTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteInAppTemplateRequestRequestTypeDef(
     _RequiredDeleteInAppTemplateRequestRequestTypeDef,
     _OptionalDeleteInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteJourneyRequestRequestTypeDef = TypedDict(
     "DeleteJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
     },
 )
@@ -1604,20 +1666,22 @@
     "_OptionalDeletePushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeletePushTemplateRequestRequestTypeDef(
     _RequiredDeletePushTemplateRequestRequestTypeDef,
     _OptionalDeletePushTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -1658,38 +1722,42 @@
         "ShortCode": str,
         "TransactionalMessagesPerSecond": int,
         "Version": int,
     },
     total=False,
 )
 
+
 class SMSChannelResponseTypeDef(
     _RequiredSMSChannelResponseTypeDef, _OptionalSMSChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSmsTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteSmsTemplateRequestRequestTypeDef(
     _RequiredDeleteSmsTemplateRequestRequestTypeDef, _OptionalDeleteSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 DeleteUserEndpointsRequestRequestTypeDef = TypedDict(
     "DeleteUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -1719,39 +1787,43 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class VoiceChannelResponseTypeDef(
     _RequiredVoiceChannelResponseTypeDef, _OptionalVoiceChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteVoiceTemplateRequestRequestTypeDef(
     _RequiredDeleteVoiceTemplateRequestRequestTypeDef,
     _OptionalDeleteVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 GCMMessageTypeDef = TypedDict(
     "GCMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
@@ -1813,19 +1885,21 @@
         "ConfigurationSet": str,
         "Enabled": bool,
         "RoleArn": str,
     },
     total=False,
 )
 
+
 class EmailChannelRequestTypeDef(
     _RequiredEmailChannelRequestTypeDef, _OptionalEmailChannelRequestTypeDef
 ):
     pass
 
+
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
@@ -1859,25 +1933,20 @@
         "TemplateDescription": str,
         "TextPart": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class EmailTemplateResponseTypeDef(
     _RequiredEmailTemplateResponseTypeDef, _OptionalEmailTemplateResponseTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": str,
         "Locale": str,
         "Make": str,
@@ -1935,19 +2004,21 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
+
 class EndpointMessageResultTypeDef(
     _RequiredEndpointMessageResultTypeDef, _OptionalEndpointMessageResultTypeDef
 ):
     pass
 
+
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": str,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -1974,17 +2045,19 @@
     "_OptionalSetDimensionTypeDef",
     {
         "DimensionType": DimensionTypeType,
     },
     total=False,
 )
 
+
 class SetDimensionTypeDef(_RequiredSetDimensionTypeDef, _OptionalSetDimensionTypeDef):
     pass
 
+
 EventItemResponseTypeDef = TypedDict(
     "EventItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
@@ -2002,17 +2075,19 @@
     {
         "Duration": int,
         "StopTimestamp": str,
     },
     total=False,
 )
 
+
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
+
 _RequiredExportJobResourceTypeDef = TypedDict(
     "_RequiredExportJobResourceTypeDef",
     {
         "RoleArn": str,
         "S3UrlPrefix": str,
     },
 )
@@ -2021,38 +2096,42 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
+
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
+
 _RequiredGCMChannelRequestTypeDef = TypedDict(
     "_RequiredGCMChannelRequestTypeDef",
     {
         "ApiKey": str,
     },
 )
 _OptionalGCMChannelRequestTypeDef = TypedDict(
     "_OptionalGCMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class GCMChannelRequestTypeDef(
     _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
 ):
     pass
 
+
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -2113,20 +2192,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetApplicationDateRangeKpiRequestRequestTypeDef(
     _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
     _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 GetApplicationSettingsRequestRequestTypeDef = TypedDict(
     "GetApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2158,20 +2239,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignActivitiesRequestRequestTypeDef(
     _RequiredGetCampaignActivitiesRequestRequestTypeDef,
     _OptionalGetCampaignActivitiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "KpiName": str,
     },
@@ -2183,20 +2266,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetCampaignDateRangeKpiRequestRequestTypeDef(
     _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
     _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
     },
 )
@@ -2222,20 +2307,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignVersionsRequestRequestTypeDef(
     _RequiredGetCampaignVersionsRequestRequestTypeDef,
     _OptionalGetCampaignVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCampaignsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetCampaignsRequestRequestTypeDef = TypedDict(
@@ -2243,19 +2330,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignsRequestRequestTypeDef(
     _RequiredGetCampaignsRequestRequestTypeDef, _OptionalGetCampaignsRequestRequestTypeDef
 ):
     pass
 
+
 GetChannelsRequestRequestTypeDef = TypedDict(
     "GetChannelsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2276,19 +2365,21 @@
     "_OptionalGetEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetEmailTemplateRequestRequestTypeDef(
     _RequiredGetEmailTemplateRequestRequestTypeDef, _OptionalGetEmailTemplateRequestRequestTypeDef
 ):
     pass
 
+
 GetEndpointRequestRequestTypeDef = TypedDict(
     "GetEndpointRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2319,19 +2410,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetExportJobsRequestRequestTypeDef(
     _RequiredGetExportJobsRequestRequestTypeDef, _OptionalGetExportJobsRequestRequestTypeDef
 ):
     pass
 
+
 GetGcmChannelRequestRequestTypeDef = TypedDict(
     "GetGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2354,19 +2447,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetImportJobsRequestRequestTypeDef(
     _RequiredGetImportJobsRequestRequestTypeDef, _OptionalGetImportJobsRequestRequestTypeDef
 ):
     pass
 
+
 GetInAppMessagesRequestRequestTypeDef = TypedDict(
     "GetInAppMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2381,19 +2476,21 @@
     "_OptionalGetInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetInAppTemplateRequestRequestTypeDef(
     _RequiredGetInAppTemplateRequestRequestTypeDef, _OptionalGetInAppTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "KpiName": str,
     },
@@ -2405,20 +2502,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetJourneyDateRangeKpiRequestRequestTypeDef(
     _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
     _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
     },
@@ -2428,20 +2527,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2462,20 +2563,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2504,20 +2607,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2540,20 +2645,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2573,38 +2680,42 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunsRequestRequestTypeDef(
     _RequiredGetJourneyRunsRequestRequestTypeDef, _OptionalGetJourneyRunsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetPushTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetPushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetPushTemplateRequestRequestTypeDef(
     _RequiredGetPushTemplateRequestRequestTypeDef, _OptionalGetPushTemplateRequestRequestTypeDef
 ):
     pass
 
+
 GetRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -2629,20 +2740,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentExportJobsRequestRequestTypeDef(
     _RequiredGetSegmentExportJobsRequestRequestTypeDef,
     _OptionalGetSegmentExportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSegmentImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentImportJobsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2651,20 +2764,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentImportJobsRequestRequestTypeDef(
     _RequiredGetSegmentImportJobsRequestRequestTypeDef,
     _OptionalGetSegmentImportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 GetSegmentRequestRequestTypeDef = TypedDict(
     "GetSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2690,20 +2805,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentVersionsRequestRequestTypeDef(
     _RequiredGetSegmentVersionsRequestRequestTypeDef,
     _OptionalGetSegmentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSegmentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetSegmentsRequestRequestTypeDef = TypedDict(
@@ -2711,19 +2828,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentsRequestRequestTypeDef(
     _RequiredGetSegmentsRequestRequestTypeDef, _OptionalGetSegmentsRequestRequestTypeDef
 ):
     pass
 
+
 GetSmsChannelRequestRequestTypeDef = TypedDict(
     "GetSmsChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2737,19 +2856,21 @@
     "_OptionalGetSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetSmsTemplateRequestRequestTypeDef(
     _RequiredGetSmsTemplateRequestRequestTypeDef, _OptionalGetSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSMSTemplateResponseTypeDef = TypedDict(
     "_RequiredSMSTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2765,19 +2886,21 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class SMSTemplateResponseTypeDef(
     _RequiredSMSTemplateResponseTypeDef, _OptionalSMSTemplateResponseTypeDef
 ):
     pass
 
+
 GetUserEndpointsRequestRequestTypeDef = TypedDict(
     "GetUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -2799,19 +2922,21 @@
     "_OptionalGetVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetVoiceTemplateRequestRequestTypeDef(
     _RequiredGetVoiceTemplateRequestRequestTypeDef, _OptionalGetVoiceTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredVoiceTemplateResponseTypeDef = TypedDict(
     "_RequiredVoiceTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2828,19 +2953,21 @@
         "TemplateDescription": str,
         "Version": str,
         "VoiceId": str,
     },
     total=False,
 )
 
+
 class VoiceTemplateResponseTypeDef(
     _RequiredVoiceTemplateResponseTypeDef, _OptionalVoiceTemplateResponseTypeDef
 ):
     pass
 
+
 _RequiredImportJobResourceTypeDef = TypedDict(
     "_RequiredImportJobResourceTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -2853,19 +2980,21 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
+
 class ImportJobResourceTypeDef(
     _RequiredImportJobResourceTypeDef, _OptionalImportJobResourceTypeDef
 ):
     pass
 
+
 InAppMessageBodyConfigTypeDef = TypedDict(
     "InAppMessageBodyConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Body": str,
         "TextColor": str,
     },
@@ -2881,19 +3010,21 @@
     "_OptionalOverrideButtonConfigurationTypeDef",
     {
         "Link": str,
     },
     total=False,
 )
 
+
 class OverrideButtonConfigurationTypeDef(
     _RequiredOverrideButtonConfigurationTypeDef, _OptionalOverrideButtonConfigurationTypeDef
 ):
     pass
 
+
 InAppMessageHeaderConfigTypeDef = TypedDict(
     "InAppMessageHeaderConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Header": str,
         "TextColor": str,
     },
@@ -2978,19 +3109,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class ListJourneysRequestRequestTypeDef(
     _RequiredListJourneysRequestRequestTypeDef, _OptionalListJourneysRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3013,20 +3146,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class ListTemplateVersionsRequestRequestTypeDef(
     _RequiredListTemplateVersionsRequestRequestTypeDef,
     _OptionalListTemplateVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": str,
         "Prefix": str,
         "TemplateType": str,
@@ -3066,17 +3201,19 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
+
 class MessageResultTypeDef(_RequiredMessageResultTypeDef, _OptionalMessageResultTypeDef):
     pass
 
+
 NumberValidateRequestTypeDef = TypedDict(
     "NumberValidateRequestTypeDef",
     {
         "IsoCountryCode": str,
         "PhoneNumber": str,
     },
     total=False,
@@ -3141,25 +3278,14 @@
     "UpdateAttributesRequestTypeDef",
     {
         "Blacklist": Sequence[str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ResultRowValueTypeDef = TypedDict(
     "ResultRowValueTypeDef",
     {
         "Key": str,
         "Type": str,
         "Value": str,
     },
@@ -3192,17 +3318,19 @@
     "_OptionalSegmentReferenceTypeDef",
     {
         "Version": int,
     },
     total=False,
 )
 
+
 class SegmentReferenceTypeDef(_RequiredSegmentReferenceTypeDef, _OptionalSegmentReferenceTypeDef):
     pass
 
+
 _RequiredSegmentImportResourceTypeDef = TypedDict(
     "_RequiredSegmentImportResourceTypeDef",
     {
         "ExternalId": str,
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
@@ -3213,19 +3341,21 @@
     "_OptionalSegmentImportResourceTypeDef",
     {
         "ChannelCounts": Dict[str, int],
     },
     total=False,
 )
 
+
 class SegmentImportResourceTypeDef(
     _RequiredSegmentImportResourceTypeDef, _OptionalSegmentImportResourceTypeDef
 ):
     pass
 
+
 _RequiredSendOTPMessageRequestParametersTypeDef = TypedDict(
     "_RequiredSendOTPMessageRequestParametersTypeDef",
     {
         "BrandName": str,
         "Channel": str,
         "DestinationIdentity": str,
         "OriginationIdentity": str,
@@ -3241,19 +3371,21 @@
         "Language": str,
         "TemplateId": str,
         "ValidityPeriod": int,
     },
     total=False,
 )
 
+
 class SendOTPMessageRequestParametersTypeDef(
     _RequiredSendOTPMessageRequestParametersTypeDef, _OptionalSendOTPMessageRequestParametersTypeDef
 ):
     pass
 
+
 SimpleEmailPartTypeDef = TypedDict(
     "SimpleEmailPartTypeDef",
     {
         "Charset": str,
         "Data": str,
     },
     total=False,
@@ -3293,17 +3425,19 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class TemplateResponseTypeDef(_RequiredTemplateResponseTypeDef, _OptionalTemplateResponseTypeDef):
     pass
 
+
 _RequiredTemplateVersionResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": str,
@@ -3315,19 +3449,21 @@
         "DefaultSubstitutions": str,
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class TemplateVersionResponseTypeDef(
     _RequiredTemplateVersionResponseTypeDef, _OptionalTemplateVersionResponseTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -3349,19 +3485,21 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class UpdateRecommenderConfigurationTypeDef(
     _RequiredUpdateRecommenderConfigurationTypeDef, _OptionalUpdateRecommenderConfigurationTypeDef
 ):
     pass
 
+
 VoiceChannelRequestTypeDef = TypedDict(
     "VoiceChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -3387,324 +3525,335 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     {
         "ADMChannelRequest": ADMChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-DeleteAdmChannelResponseTypeDef = TypedDict(
-    "DeleteAdmChannelResponseTypeDef",
+UpdateApnsChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSChannelRequest": APNSChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-GetAdmChannelResponseTypeDef = TypedDict(
-    "GetAdmChannelResponseTypeDef",
+UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-UpdateAdmChannelResponseTypeDef = TypedDict(
-    "UpdateAdmChannelResponseTypeDef",
+UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-UpdateApnsChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsChannelRequestRequestTypeDef",
+UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     {
-        "APNSChannelRequest": APNSChannelRequestTypeDef,
+        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-DeleteApnsChannelResponseTypeDef = TypedDict(
-    "DeleteApnsChannelResponseTypeDef",
+_RequiredActivitiesResponseTypeDef = TypedDict(
+    "_RequiredActivitiesResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Item": List[ActivityResponseTypeDef],
     },
 )
-
-GetApnsChannelResponseTypeDef = TypedDict(
-    "GetApnsChannelResponseTypeDef",
+_OptionalActivitiesResponseTypeDef = TypedDict(
+    "_OptionalActivitiesResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextToken": str,
     },
+    total=False,
 )
 
-UpdateApnsChannelResponseTypeDef = TypedDict(
-    "UpdateApnsChannelResponseTypeDef",
+
+class ActivitiesResponseTypeDef(
+    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
+):
+    pass
+
+
+ApplicationsResponseTypeDef = TypedDict(
+    "ApplicationsResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Item": List[ApplicationResponseTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelRequestRequestTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
-
-DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsSandboxChannelResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsSandboxChannelResponseTypeDef",
-    {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelResponseTypeDef",
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipChannelRequestRequestTypeDef",
+UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
+    "UpdateBaiduChannelRequestRequestTypeDef",
     {
-        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
         "ApplicationId": str,
+        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-DeleteApnsVoipChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipChannelResponseTypeDef",
+ChannelsResponseTypeDef = TypedDict(
+    "ChannelsResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-GetApnsVoipChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipChannelResponseTypeDef",
+ClosedDaysTypeDef = TypedDict(
+    "ClosedDaysTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
+        "SMS": Sequence[ClosedDaysRuleTypeDef],
+        "PUSH": Sequence[ClosedDaysRuleTypeDef],
+        "VOICE": Sequence[ClosedDaysRuleTypeDef],
+        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateApnsVoipChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipChannelResponseTypeDef",
+WaitActivityTypeDef = TypedDict(
+    "WaitActivityTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextActivity": str,
+        "WaitTime": WaitTimeTypeDef,
     },
+    total=False,
 )
 
-UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
-        "ApplicationId": str,
+        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
     },
 )
 
-DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipSandboxChannelResponseTypeDef",
+DeleteAdmChannelResponseTypeDef = TypedDict(
+    "DeleteAdmChannelResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+DeleteApnsChannelResponseTypeDef = TypedDict(
+    "DeleteApnsChannelResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActivitiesResponseTypeDef = TypedDict(
-    "_RequiredActivitiesResponseTypeDef",
-    {
-        "Item": List[ActivityResponseTypeDef],
-    },
-)
-_OptionalActivitiesResponseTypeDef = TypedDict(
-    "_OptionalActivitiesResponseTypeDef",
+DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsSandboxChannelResponseTypeDef",
     {
-        "NextToken": str,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ActivitiesResponseTypeDef(
-    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
-):
-    pass
-
-ApplicationsResponseTypeDef = TypedDict(
-    "ApplicationsResponseTypeDef",
+DeleteApnsVoipChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipChannelResponseTypeDef",
     {
-        "Item": List[ApplicationResponseTypeDef],
-        "NextToken": str,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppResponseTypeDef = TypedDict(
     "DeleteAppResponseTypeDef",
     {
         "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+DeleteBaiduChannelResponseTypeDef = TypedDict(
+    "DeleteBaiduChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "ApplicationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+GetAdmChannelResponseTypeDef = TypedDict(
+    "GetAdmChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
+GetApnsChannelResponseTypeDef = TypedDict(
+    "GetApnsChannelResponseTypeDef",
+    {
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+GetApnsSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-RemoveAttributesResponseTypeDef = TypedDict(
-    "RemoveAttributesResponseTypeDef",
+GetApnsVoipChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipChannelResponseTypeDef",
     {
-        "AttributesResource": AttributesResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
-    "UpdateBaiduChannelRequestRequestTypeDef",
+GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationId": str,
-        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteBaiduChannelResponseTypeDef = TypedDict(
-    "DeleteBaiduChannelResponseTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBaiduChannelResponseTypeDef = TypedDict(
     "GetBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBaiduChannelResponseTypeDef = TypedDict(
-    "UpdateBaiduChannelResponseTypeDef",
+RemoveAttributesResponseTypeDef = TypedDict(
+    "RemoveAttributesResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttributesResource": AttributesResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChannelsResponseTypeDef = TypedDict(
-    "ChannelsResponseTypeDef",
+UpdateAdmChannelResponseTypeDef = TypedDict(
+    "UpdateAdmChannelResponseTypeDef",
     {
-        "Channels": Dict[str, ChannelResponseTypeDef],
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ClosedDaysTypeDef = TypedDict(
-    "ClosedDaysTypeDef",
+UpdateApnsChannelResponseTypeDef = TypedDict(
+    "UpdateApnsChannelResponseTypeDef",
     {
-        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
-        "SMS": Sequence[ClosedDaysRuleTypeDef],
-        "PUSH": Sequence[ClosedDaysRuleTypeDef],
-        "VOICE": Sequence[ClosedDaysRuleTypeDef],
-        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-WaitActivityTypeDef = TypedDict(
-    "WaitActivityTypeDef",
+UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelResponseTypeDef",
     {
-        "NextActivity": str,
-        "WaitTime": WaitTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+UpdateApnsVoipChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipChannelResponseTypeDef",
     {
-        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+    {
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBaiduChannelResponseTypeDef = TypedDict(
+    "UpdateBaiduChannelResponseTypeDef",
+    {
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "EmailTemplateRequest": EmailTemplateRequestTypeDef,
@@ -3724,49 +3873,51 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePushTemplateResponseTypeDef = TypedDict(
     "CreatePushTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSmsTemplateResponseTypeDef = TypedDict(
     "CreateSmsTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVoiceTemplateResponseTypeDef = TypedDict(
     "CreateVoiceTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExportJobRequestRequestTypeDef = TypedDict(
     "CreateExportJobRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -3782,46 +3933,46 @@
     },
 )
 
 CreateInAppTemplateResponseTypeDef = TypedDict(
     "CreateInAppTemplateResponseTypeDef",
     {
         "TemplateCreateMessageBody": TemplateCreateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecommenderConfigurationRequestRequestTypeDef",
     {
         "CreateRecommenderConfiguration": CreateRecommenderConfigurationTypeDef,
     },
 )
 
 CreateRecommenderConfigurationResponseTypeDef = TypedDict(
     "CreateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRecommenderConfigurationResponseTypeDef = TypedDict(
     "DeleteRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommenderConfigurationResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListRecommenderConfigurationsResponseTypeDef = TypedDict(
     "_RequiredListRecommenderConfigurationsResponseTypeDef",
     {
         "Item": List[RecommenderConfigurationResponseTypeDef],
@@ -3831,25 +3982,27 @@
     "_OptionalListRecommenderConfigurationsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRecommenderConfigurationsResponseTypeDef(
     _RequiredListRecommenderConfigurationsResponseTypeDef,
     _OptionalListRecommenderConfigurationsResponseTypeDef,
 ):
     pass
 
+
 UpdateRecommenderConfigurationResponseTypeDef = TypedDict(
     "UpdateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSmsTemplateRequestRequestTypeDef = TypedDict(
     "CreateSmsTemplateRequestRequestTypeDef",
     {
         "SMSTemplateRequest": SMSTemplateRequestTypeDef,
@@ -3869,19 +4022,21 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateSmsTemplateRequestRequestTypeDef(
     _RequiredUpdateSmsTemplateRequestRequestTypeDef, _OptionalUpdateSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 CreateVoiceTemplateRequestRequestTypeDef = TypedDict(
     "CreateVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "VoiceTemplateRequest": VoiceTemplateRequestTypeDef,
     },
 )
@@ -3898,20 +4053,22 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateVoiceTemplateRequestRequestTypeDef(
     _RequiredUpdateVoiceTemplateRequestRequestTypeDef,
     _OptionalUpdateVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 CustomMessageActivityTypeDef = TypedDict(
     "CustomMessageActivityTypeDef",
     {
         "DeliveryUri": str,
         "EndpointTypes": Sequence[EndpointTypesElementType],
         "MessageConfig": JourneyCustomMessageTypeDef,
         "NextActivity": str,
@@ -3960,241 +4117,243 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class PushNotificationTemplateResponseTypeDef(
     _RequiredPushNotificationTemplateResponseTypeDef,
     _OptionalPushNotificationTemplateResponseTypeDef,
 ):
     pass
 
+
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEmailChannelResponseTypeDef = TypedDict(
     "GetEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailChannelResponseTypeDef = TypedDict(
     "UpdateEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEmailTemplateResponseTypeDef = TypedDict(
     "DeleteEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInAppTemplateResponseTypeDef = TypedDict(
     "DeleteInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePushTemplateResponseTypeDef = TypedDict(
     "DeletePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSmsTemplateResponseTypeDef = TypedDict(
     "DeleteSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVoiceTemplateResponseTypeDef = TypedDict(
     "DeleteVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailTemplateResponseTypeDef = TypedDict(
     "UpdateEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointsBatchResponseTypeDef = TypedDict(
     "UpdateEndpointsBatchResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInAppTemplateResponseTypeDef = TypedDict(
     "UpdateInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePushTemplateResponseTypeDef = TypedDict(
     "UpdatePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSmsTemplateResponseTypeDef = TypedDict(
     "UpdateSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTemplateActiveVersionResponseTypeDef = TypedDict(
     "UpdateTemplateActiveVersionResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceTemplateResponseTypeDef = TypedDict(
     "UpdateVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventStreamResponseTypeDef = TypedDict(
     "DeleteEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventStreamResponseTypeDef = TypedDict(
     "PutEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGcmChannelResponseTypeDef = TypedDict(
     "DeleteGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGcmChannelResponseTypeDef = TypedDict(
     "GetGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGcmChannelResponseTypeDef = TypedDict(
     "UpdateGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSmsChannelResponseTypeDef = TypedDict(
     "DeleteSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSmsChannelResponseTypeDef = TypedDict(
     "GetSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSmsChannelResponseTypeDef = TypedDict(
     "UpdateSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVoiceChannelResponseTypeDef = TypedDict(
     "DeleteVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceChannelResponseTypeDef = TypedDict(
     "GetVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceChannelResponseTypeDef = TypedDict(
     "UpdateVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailChannelRequestRequestTypeDef = TypedDict(
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4213,15 +4372,15 @@
     total=False,
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": str,
@@ -4309,19 +4468,21 @@
     {
         "RequestId": str,
         "Result": Dict[str, Dict[str, EndpointMessageResultTypeDef]],
     },
     total=False,
 )
 
+
 class SendUsersMessageResponseTypeDef(
     _RequiredSendUsersMessageResponseTypeDef, _OptionalSendUsersMessageResponseTypeDef
 ):
     pass
 
+
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "EventType": SetDimensionTypeDef,
         "Metrics": Mapping[str, MetricDimensionTypeDef],
     },
@@ -4368,17 +4529,19 @@
         "Metrics": Mapping[str, float],
         "SdkName": str,
         "Session": SessionTypeDef,
     },
     total=False,
 )
 
+
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
+
 _RequiredExportJobResponseTypeDef = TypedDict(
     "_RequiredExportJobResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
         "Definition": ExportJobResourceTypeDef,
         "Id": str,
@@ -4396,19 +4559,21 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
+
 class ExportJobResponseTypeDef(
     _RequiredExportJobResponseTypeDef, _OptionalExportJobResponseTypeDef
 ):
     pass
 
+
 UpdateGcmChannelRequestRequestTypeDef = TypedDict(
     "UpdateGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "GCMChannelRequest": GCMChannelRequestTypeDef,
     },
 )
@@ -4423,66 +4588,68 @@
     "_OptionalGPSPointDimensionTypeDef",
     {
         "RangeInKilometers": float,
     },
     total=False,
 )
 
+
 class GPSPointDimensionTypeDef(
     _RequiredGPSPointDimensionTypeDef, _OptionalGPSPointDimensionTypeDef
 ):
     pass
 
+
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionMetricsResponseTypeDef",
     {
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyRunExecutionActivityMetricsResponse": (
             JourneyRunExecutionActivityMetricsResponseTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     {
         "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSmsTemplateResponseTypeDef = TypedDict(
     "GetSmsTemplateResponseTypeDef",
     {
         "SMSTemplateResponse": SMSTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceTemplateResponseTypeDef = TypedDict(
     "GetVoiceTemplateResponseTypeDef",
     {
         "VoiceTemplateResponse": VoiceTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportJobResponseTypeDef = TypedDict(
     "_RequiredImportJobResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4503,19 +4670,21 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
+
 class ImportJobResponseTypeDef(
     _RequiredImportJobResponseTypeDef, _OptionalImportJobResponseTypeDef
 ):
     pass
 
+
 InAppMessageButtonTypeDef = TypedDict(
     "InAppMessageButtonTypeDef",
     {
         "Android": OverrideButtonConfigurationTypeDef,
         "DefaultConfig": DefaultButtonConfigurationTypeDef,
         "IOS": OverrideButtonConfigurationTypeDef,
         "Web": OverrideButtonConfigurationTypeDef,
@@ -4544,19 +4713,21 @@
     "_OptionalJourneyRunsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneyRunsResponseTypeDef(
     _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
 ):
     pass
 
+
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4573,15 +4744,15 @@
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagsModel": TagsModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -4601,29 +4772,31 @@
         "EndpointResult": Dict[str, EndpointMessageResultTypeDef],
         "RequestId": str,
         "Result": Dict[str, MessageResultTypeDef],
     },
     total=False,
 )
 
+
 class MessageResponseTypeDef(_RequiredMessageResponseTypeDef, _OptionalMessageResponseTypeDef):
     pass
 
+
 PhoneNumberValidateRequestRequestTypeDef = TypedDict(
     "PhoneNumberValidateRequestRequestTypeDef",
     {
         "NumberValidateRequest": NumberValidateRequestTypeDef,
     },
 )
 
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4732,19 +4905,21 @@
     "_OptionalTemplatesResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class TemplatesResponseTypeDef(
     _RequiredTemplatesResponseTypeDef, _OptionalTemplatesResponseTypeDef
 ):
     pass
 
+
 _RequiredTemplateVersionsResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionsResponseTypeDef",
     {
         "Item": List[TemplateVersionResponseTypeDef],
     },
 )
 _OptionalTemplateVersionsResponseTypeDef = TypedDict(
@@ -4753,19 +4928,21 @@
         "Message": str,
         "NextToken": str,
         "RequestID": str,
     },
     total=False,
 )
 
+
 class TemplateVersionsResponseTypeDef(
     _RequiredTemplateVersionsResponseTypeDef, _OptionalTemplateVersionsResponseTypeDef
 ):
     pass
 
+
 UpdateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
         "UpdateRecommenderConfiguration": UpdateRecommenderConfigurationTypeDef,
     },
 )
@@ -4778,15 +4955,15 @@
     },
 )
 
 VerifyOTPMessageResponseTypeDef = TypedDict(
     "VerifyOTPMessageResponseTypeDef",
     {
         "VerificationResponse": VerificationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifyOTPMessageRequestRequestTypeDef = TypedDict(
     "VerifyOTPMessageRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4794,39 +4971,39 @@
     },
 )
 
 GetCampaignActivitiesResponseTypeDef = TypedDict(
     "GetCampaignActivitiesResponseTypeDef",
     {
         "ActivitiesResponse": ActivitiesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppsResponseTypeDef = TypedDict(
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationSettingsResponseTypeDef = TypedDict(
     "GetApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationSettingsResponseTypeDef = TypedDict(
     "UpdateApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
     "UpdateApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4834,23 +5011,23 @@
     },
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommenderConfigurationsResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
@@ -4870,25 +5047,27 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdatePushTemplateRequestRequestTypeDef(
     _RequiredUpdatePushTemplateRequestRequestTypeDef,
     _OptionalUpdatePushTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 GetPushTemplateResponseTypeDef = TypedDict(
     "GetPushTemplateResponseTypeDef",
     {
         "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
@@ -4904,38 +5083,38 @@
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointsResponseTypeDef = TypedDict(
     "EndpointsResponseTypeDef",
     {
         "Item": List[EndpointResponseTypeDef],
     },
 )
 
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendUsersMessagesResponseTypeDef = TypedDict(
     "SendUsersMessagesResponseTypeDef",
     {
         "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -4976,15 +5155,15 @@
     },
 )
 
 CreateExportJobResponseTypeDef = TypedDict(
     "CreateExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportJobsResponseTypeDef = TypedDict(
     "_RequiredExportJobsResponseTypeDef",
     {
         "Item": List[ExportJobResponseTypeDef],
@@ -4994,24 +5173,26 @@
     "_OptionalExportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ExportJobsResponseTypeDef(
     _RequiredExportJobsResponseTypeDef, _OptionalExportJobsResponseTypeDef
 ):
     pass
 
+
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
@@ -5020,23 +5201,23 @@
     total=False,
 )
 
 CreateImportJobResponseTypeDef = TypedDict(
     "CreateImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportJobsResponseTypeDef = TypedDict(
     "_RequiredImportJobsResponseTypeDef",
     {
         "Item": List[ImportJobResponseTypeDef],
@@ -5046,19 +5227,21 @@
     "_OptionalImportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ImportJobsResponseTypeDef(
     _RequiredImportJobsResponseTypeDef, _OptionalImportJobsResponseTypeDef
 ):
     pass
 
+
 InAppMessageContentTypeDef = TypedDict(
     "InAppMessageContentTypeDef",
     {
         "BackgroundColor": str,
         "BodyConfig": InAppMessageBodyConfigTypeDef,
         "HeaderConfig": InAppMessageHeaderConfigTypeDef,
         "ImageUrl": str,
@@ -5068,31 +5251,31 @@
     total=False,
 )
 
 GetJourneyRunsResponseTypeDef = TypedDict(
     "GetJourneyRunsResponseTypeDef",
     {
         "JourneyRunsResponse": JourneyRunsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendMessagesResponseTypeDef = TypedDict(
     "SendMessagesResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendOTPMessageResponseTypeDef = TypedDict(
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
@@ -5113,23 +5296,23 @@
     total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesResponse": TemplatesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5137,23 +5320,23 @@
     },
 )
 
 DeleteUserEndpointsResponseTypeDef = TypedDict(
     "DeleteUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserEndpointsResponseTypeDef = TypedDict(
     "GetUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
@@ -5178,54 +5361,56 @@
         "IsLocalTime": bool,
         "QuietTime": QuietTimeTypeDef,
         "Timezone": str,
     },
     total=False,
 )
 
+
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
+
 EventStartConditionTypeDef = TypedDict(
     "EventStartConditionTypeDef",
     {
         "EventFilter": EventFilterTypeDef,
         "SegmentId": str,
     },
     total=False,
 )
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "EventsResponse": EventsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventsRequestTypeDef = TypedDict(
     "EventsRequestTypeDef",
     {
         "BatchItem": Mapping[str, EventsBatchTypeDef],
     },
 )
 
 GetExportJobsResponseTypeDef = TypedDict(
     "GetExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
@@ -5238,23 +5423,23 @@
     total=False,
 )
 
 GetImportJobsResponseTypeDef = TypedDict(
     "GetImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": str,
@@ -5306,19 +5491,21 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class InAppTemplateResponseTypeDef(
     _RequiredInAppTemplateResponseTypeDef, _OptionalInAppTemplateResponseTypeDef
 ):
     pass
 
+
 _RequiredApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "KpiName": str,
         "KpiResult": BaseKpiResultTypeDef,
@@ -5329,19 +5516,21 @@
     "_OptionalApplicationDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ApplicationDateRangeKpiResponseTypeDef(
     _RequiredApplicationDateRangeKpiResponseTypeDef, _OptionalApplicationDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 _RequiredCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredCampaignDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "EndTime": datetime,
         "KpiName": str,
@@ -5353,19 +5542,21 @@
     "_OptionalCampaignDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class CampaignDateRangeKpiResponseTypeDef(
     _RequiredCampaignDateRangeKpiResponseTypeDef, _OptionalCampaignDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 _RequiredJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredJourneyDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "JourneyId": str,
         "KpiName": str,
@@ -5377,19 +5568,21 @@
     "_OptionalJourneyDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneyDateRangeKpiResponseTypeDef(
     _RequiredJourneyDateRangeKpiResponseTypeDef, _OptionalJourneyDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 DirectMessageConfigurationTypeDef = TypedDict(
     "DirectMessageConfigurationTypeDef",
     {
         "ADMMessage": ADMMessageTypeDef,
         "APNSMessage": APNSMessageTypeDef,
         "BaiduMessage": BaiduMessageTypeDef,
         "DefaultMessage": DefaultMessageTypeDef,
@@ -5492,49 +5685,51 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateInAppTemplateRequestRequestTypeDef(
     _RequiredUpdateInAppTemplateRequestRequestTypeDef,
     _OptionalUpdateInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 GetInAppTemplateResponseTypeDef = TypedDict(
     "GetInAppTemplateResponseTypeDef",
     {
         "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "GetCampaignDateRangeKpiResponseTypeDef",
     {
         "CampaignDateRangeKpiResponse": CampaignDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "GetJourneyDateRangeKpiResponseTypeDef",
     {
         "JourneyDateRangeKpiResponse": JourneyDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMessageRequestTypeDef = TypedDict(
     "_RequiredMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
@@ -5548,17 +5743,19 @@
         "Endpoints": Mapping[str, EndpointSendConfigurationTypeDef],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
+
 class MessageRequestTypeDef(_RequiredMessageRequestTypeDef, _OptionalMessageRequestTypeDef):
     pass
 
+
 _RequiredSendUsersMessageRequestTypeDef = TypedDict(
     "_RequiredSendUsersMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
         "Users": Mapping[str, EndpointSendConfigurationTypeDef],
     },
 )
@@ -5568,19 +5765,21 @@
         "Context": Mapping[str, str],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
+
 class SendUsersMessageRequestTypeDef(
     _RequiredSendUsersMessageRequestTypeDef, _OptionalSendUsersMessageRequestTypeDef
 ):
     pass
 
+
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": Sequence[SegmentGroupTypeDef],
         "Include": IncludeType,
     },
     total=False,
@@ -5621,19 +5820,21 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
+
 class TreatmentResourceTypeDef(
     _RequiredTreatmentResourceTypeDef, _OptionalTreatmentResourceTypeDef
 ):
     pass
 
+
 _RequiredWriteTreatmentResourceTypeDef = TypedDict(
     "_RequiredWriteTreatmentResourceTypeDef",
     {
         "SizePercent": int,
     },
 )
 _OptionalWriteTreatmentResourceTypeDef = TypedDict(
@@ -5645,19 +5846,21 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
+
 class WriteTreatmentResourceTypeDef(
     _RequiredWriteTreatmentResourceTypeDef, _OptionalWriteTreatmentResourceTypeDef
 ):
     pass
 
+
 InAppMessagesResponseTypeDef = TypedDict(
     "InAppMessagesResponseTypeDef",
     {
         "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
     },
     total=False,
 )
@@ -5698,17 +5901,19 @@
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Dict[str, str],
         "Version": int,
     },
     total=False,
 )
 
+
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
+
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": SegmentDimensionsTypeDef,
         "Name": str,
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Mapping[str, str],
@@ -5770,17 +5975,19 @@
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
     },
     total=False,
 )
 
+
 class CampaignResponseTypeDef(_RequiredCampaignResponseTypeDef, _OptionalCampaignResponseTypeDef):
     pass
 
+
 WriteCampaignRequestTypeDef = TypedDict(
     "WriteCampaignRequestTypeDef",
     {
         "AdditionalTreatments": Sequence[WriteTreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "Description": str,
         "HoldoutPercent": int,
@@ -5801,47 +6008,47 @@
     total=False,
 )
 
 GetInAppMessagesResponseTypeDef = TypedDict(
     "GetInAppMessagesResponseTypeDef",
     {
         "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSegmentResponseTypeDef = TypedDict(
     "DeleteSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentVersionResponseTypeDef = TypedDict(
     "GetSegmentVersionResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSegmentsResponseTypeDef = TypedDict(
     "_RequiredSegmentsResponseTypeDef",
     {
         "Item": List[SegmentResponseTypeDef],
@@ -5851,22 +6058,24 @@
     "_OptionalSegmentsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SegmentsResponseTypeDef(_RequiredSegmentsResponseTypeDef, _OptionalSegmentsResponseTypeDef):
     pass
 
+
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5911,56 +6120,58 @@
     "_OptionalCampaignsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class CampaignsResponseTypeDef(
     _RequiredCampaignsResponseTypeDef, _OptionalCampaignsResponseTypeDef
 ):
     pass
 
+
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCampaignResponseTypeDef = TypedDict(
     "DeleteCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignResponseTypeDef = TypedDict(
     "GetCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignVersionResponseTypeDef = TypedDict(
     "GetCampaignVersionResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCampaignResponseTypeDef = TypedDict(
     "UpdateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCampaignRequestRequestTypeDef = TypedDict(
     "CreateCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5977,23 +6188,23 @@
     },
 )
 
 GetSegmentVersionsResponseTypeDef = TypedDict(
     "GetSegmentVersionsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentsResponseTypeDef = TypedDict(
     "GetSegmentsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJourneyResponseTypeDef = TypedDict(
     "_RequiredJourneyResponseTypeDef",
     {
         "ApplicationId": str,
@@ -6022,17 +6233,19 @@
         "SendingSchedule": bool,
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
     },
     total=False,
 )
 
+
 class JourneyResponseTypeDef(_RequiredJourneyResponseTypeDef, _OptionalJourneyResponseTypeDef):
     pass
 
+
 _RequiredWriteJourneyRequestTypeDef = TypedDict(
     "_RequiredWriteJourneyRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalWriteJourneyRequestTypeDef = TypedDict(
@@ -6055,56 +6268,58 @@
         "SendingSchedule": bool,
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
     },
     total=False,
 )
 
+
 class WriteJourneyRequestTypeDef(
     _RequiredWriteJourneyRequestTypeDef, _OptionalWriteJourneyRequestTypeDef
 ):
     pass
 
+
 GetCampaignVersionsResponseTypeDef = TypedDict(
     "GetCampaignVersionsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignsResponseTypeDef = TypedDict(
     "GetCampaignsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJourneyResponseTypeDef = TypedDict(
     "CreateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteJourneyResponseTypeDef = TypedDict(
     "DeleteJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyResponseTypeDef = TypedDict(
     "GetJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJourneysResponseTypeDef = TypedDict(
     "_RequiredJourneysResponseTypeDef",
     {
         "Item": List[JourneyResponseTypeDef],
@@ -6114,30 +6329,32 @@
     "_OptionalJourneysResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneysResponseTypeDef(_RequiredJourneysResponseTypeDef, _OptionalJourneysResponseTypeDef):
     pass
 
+
 UpdateJourneyResponseTypeDef = TypedDict(
     "UpdateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJourneyStateResponseTypeDef = TypedDict(
     "UpdateJourneyStateResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJourneyRequestRequestTypeDef = TypedDict(
     "CreateJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6154,10 +6371,10 @@
     },
 )
 
 ListJourneysResponseTypeDef = TypedDict(
     "ListJourneysResponseTypeDef",
     {
         "JourneysResponse": JourneysResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.26.120
-Summary: Type annotations for boto3.Pinpoint 1.26.120 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.138
+Summary: Type annotations for boto3.Pinpoint 1.26.138 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.120](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.138](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -358,14 +358,15 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
+    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -408,15 +409,14 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -502,15 +502,14 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -520,49 +519,50 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    GetAdmChannelResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
-    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdmChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    GetAppResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    RemoveAttributesResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.120/setup.py` & `mypy-boto3-pinpoint-1.26.138/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.26.120",
+    version="1.26.138",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pinpoint 1.26.120 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Pinpoint 1.26.138 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

