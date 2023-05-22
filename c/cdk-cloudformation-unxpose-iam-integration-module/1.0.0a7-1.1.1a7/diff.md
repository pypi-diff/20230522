# Comparing `tmp/cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7.tar.gz` & `tmp/cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/unxpose-iam-integration-module/dist/python/cdk-cloudfor", last modified: Mon Apr 24 06:13:19 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/unxpose-iam-integration-module/dist/python/cdk-cloudfor", last modified: Mon May 22 06:14:22 2023, max compression
```

## Comparing `cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7.tar` & `cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2850 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1901 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1960 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    20463 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      476 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    19584 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/unxpose-iam-integration-module@1.0.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-24 06:13:13.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2850 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      752 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       50 2023-04-24 06:13:19.000000 cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2850 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1901 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1959 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    20704 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      476 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    19636 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/unxpose-iam-integration-module@1.1.1-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-22 06:14:16.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2850 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      752 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       50 2023-05-22 06:14:22.000000 cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/LICENSE` & `cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/PKG-INFO` & `cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-unxpose-iam-integration-module
-Version: 1.0.0a7
+Version: 1.1.1a7
 Summary: Schema for Module Fragment of type Unxpose::IAM::Integration::MODULE
 Home-page: https://github.com/cdklabs/cdk-cloudformation.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # unxpose-iam-integration-module
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Unxpose::IAM::Integration::MODULE` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Unxpose::IAM::Integration::MODULE` v1.1.1.
 
 ## Description
 
 Schema for Module Fragment of type Unxpose::IAM::Integration::MODULE
 
 ## Usage
 
@@ -51,13 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Unxpose::IAM::Integration::MODULE`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Funxpose-iam-integration-module+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Funxpose-iam-integration-module+v1.1.1).
 * Issues related to `Unxpose::IAM::Integration::MODULE` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/README.md` & `cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # unxpose-iam-integration-module
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Unxpose::IAM::Integration::MODULE` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Unxpose::IAM::Integration::MODULE` v1.1.1.
 
 ## Description
 
 Schema for Module Fragment of type Unxpose::IAM::Integration::MODULE
 
 ## Usage
 
@@ -28,13 +28,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Unxpose::IAM::Integration::MODULE`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Funxpose-iam-integration-module+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Funxpose-iam-integration-module+v1.1.1).
 * Issues related to `Unxpose::IAM::Integration::MODULE` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/setup.py` & `cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-unxpose-iam-integration-module",
-    "version": "1.0.0.a7",
+    "version": "1.1.1.a7",
     "description": "Schema for Module Fragment of type Unxpose::IAM::Integration::MODULE",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-cloudformation.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_cloudformation_unxpose_iam_integration_module",
         "cdk_cloudformation_unxpose_iam_integration_module._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_unxpose_iam_integration_module._jsii": [
-            "unxpose-iam-integration-module@1.0.0-alpha.7.jsii.tgz"
+            "unxpose-iam-integration-module@1.1.1-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_unxpose_iam_integration_module": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.72.1, <3.0.0",
-        "constructs>=10.1.302, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "aws-cdk-lib>=2.80.0, <3.0.0",
+        "constructs>=10.2.31, <11.0.0",
+        "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module/__init__.py` & `cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # unxpose-iam-integration-module
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Unxpose::IAM::Integration::MODULE` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Unxpose::IAM::Integration::MODULE` v1.1.1.
 
 ## Description
 
 Schema for Module Fragment of type Unxpose::IAM::Integration::MODULE
 
 ## Usage
 
@@ -29,15 +29,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Unxpose::IAM::Integration::MODULE`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Funxpose-iam-integration-module+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Funxpose-iam-integration-module+v1.1.1).
 * Issues related to `Unxpose::IAM::Integration::MODULE` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
@@ -266,52 +266,55 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="@cdk-cloudformation/unxpose-iam-integration-module.CfnIntegrationModulePropsResources",
     jsii_struct_bases=[],
-    name_mapping={"unxpose_policy": "unxposePolicy", "unxpose_role": "unxposeRole"},
+    name_mapping={
+        "unxpose_managed_policy": "unxposeManagedPolicy",
+        "unxpose_role": "unxposeRole",
+    },
 )
 class CfnIntegrationModulePropsResources:
     def __init__(
         self,
         *,
-        unxpose_policy: typing.Optional[typing.Union["CfnIntegrationModulePropsResourcesUnxposePolicy", typing.Dict[builtins.str, typing.Any]]] = None,
+        unxpose_managed_policy: typing.Optional[typing.Union["CfnIntegrationModulePropsResourcesUnxposeManagedPolicy", typing.Dict[builtins.str, typing.Any]]] = None,
         unxpose_role: typing.Optional[typing.Union["CfnIntegrationModulePropsResourcesUnxposeRole", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
-        :param unxpose_policy: 
+        :param unxpose_managed_policy: 
         :param unxpose_role: 
 
         :schema: CfnIntegrationModulePropsResources
         '''
-        if isinstance(unxpose_policy, dict):
-            unxpose_policy = CfnIntegrationModulePropsResourcesUnxposePolicy(**unxpose_policy)
+        if isinstance(unxpose_managed_policy, dict):
+            unxpose_managed_policy = CfnIntegrationModulePropsResourcesUnxposeManagedPolicy(**unxpose_managed_policy)
         if isinstance(unxpose_role, dict):
             unxpose_role = CfnIntegrationModulePropsResourcesUnxposeRole(**unxpose_role)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__45ca08dc9374092b77f3e2462f88d86c15ec638f3ca898f12587f76db702ab52)
-            check_type(argname="argument unxpose_policy", value=unxpose_policy, expected_type=type_hints["unxpose_policy"])
+            check_type(argname="argument unxpose_managed_policy", value=unxpose_managed_policy, expected_type=type_hints["unxpose_managed_policy"])
             check_type(argname="argument unxpose_role", value=unxpose_role, expected_type=type_hints["unxpose_role"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if unxpose_policy is not None:
-            self._values["unxpose_policy"] = unxpose_policy
+        if unxpose_managed_policy is not None:
+            self._values["unxpose_managed_policy"] = unxpose_managed_policy
         if unxpose_role is not None:
             self._values["unxpose_role"] = unxpose_role
 
     @builtins.property
-    def unxpose_policy(
+    def unxpose_managed_policy(
         self,
-    ) -> typing.Optional["CfnIntegrationModulePropsResourcesUnxposePolicy"]:
+    ) -> typing.Optional["CfnIntegrationModulePropsResourcesUnxposeManagedPolicy"]:
         '''
-        :schema: CfnIntegrationModulePropsResources#UnxposePolicy
+        :schema: CfnIntegrationModulePropsResources#UnxposeManagedPolicy
         '''
-        result = self._values.get("unxpose_policy")
-        return typing.cast(typing.Optional["CfnIntegrationModulePropsResourcesUnxposePolicy"], result)
+        result = self._values.get("unxpose_managed_policy")
+        return typing.cast(typing.Optional["CfnIntegrationModulePropsResourcesUnxposeManagedPolicy"], result)
 
     @builtins.property
     def unxpose_role(
         self,
     ) -> typing.Optional["CfnIntegrationModulePropsResourcesUnxposeRole"]:
         '''
         :schema: CfnIntegrationModulePropsResources#UnxposeRole
@@ -328,65 +331,65 @@
     def __repr__(self) -> str:
         return "CfnIntegrationModulePropsResources(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdk-cloudformation/unxpose-iam-integration-module.CfnIntegrationModulePropsResourcesUnxposePolicy",
+    jsii_type="@cdk-cloudformation/unxpose-iam-integration-module.CfnIntegrationModulePropsResourcesUnxposeManagedPolicy",
     jsii_struct_bases=[],
     name_mapping={"properties": "properties", "type": "type"},
 )
-class CfnIntegrationModulePropsResourcesUnxposePolicy:
+class CfnIntegrationModulePropsResourcesUnxposeManagedPolicy:
     def __init__(
         self,
         *,
         properties: typing.Any = None,
         type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param properties: 
         :param type: 
 
-        :schema: CfnIntegrationModulePropsResourcesUnxposePolicy
+        :schema: CfnIntegrationModulePropsResourcesUnxposeManagedPolicy
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__54b5edd81ee288f35fa2ebe96875365b97e71d951ea5ed5f3543b533dfbf855c)
+            type_hints = typing.get_type_hints(_typecheckingstub__ca77cfd3036d34cb2ab929edf9216ee7a861ebc86d607e619022bf8255dc8a67)
             check_type(argname="argument properties", value=properties, expected_type=type_hints["properties"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if properties is not None:
             self._values["properties"] = properties
         if type is not None:
             self._values["type"] = type
 
     @builtins.property
     def properties(self) -> typing.Any:
         '''
-        :schema: CfnIntegrationModulePropsResourcesUnxposePolicy#Properties
+        :schema: CfnIntegrationModulePropsResourcesUnxposeManagedPolicy#Properties
         '''
         result = self._values.get("properties")
         return typing.cast(typing.Any, result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''
-        :schema: CfnIntegrationModulePropsResourcesUnxposePolicy#Type
+        :schema: CfnIntegrationModulePropsResourcesUnxposeManagedPolicy#Type
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "CfnIntegrationModulePropsResourcesUnxposePolicy(%s)" % ", ".join(
+        return "CfnIntegrationModulePropsResourcesUnxposeManagedPolicy(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="@cdk-cloudformation/unxpose-iam-integration-module.CfnIntegrationModulePropsResourcesUnxposeRole",
     jsii_struct_bases=[],
@@ -445,15 +448,15 @@
 
 __all__ = [
     "CfnIntegrationModule",
     "CfnIntegrationModuleProps",
     "CfnIntegrationModulePropsParameters",
     "CfnIntegrationModulePropsParametersExternalId",
     "CfnIntegrationModulePropsResources",
-    "CfnIntegrationModulePropsResourcesUnxposePolicy",
+    "CfnIntegrationModulePropsResourcesUnxposeManagedPolicy",
     "CfnIntegrationModulePropsResourcesUnxposeRole",
 ]
 
 publication.publish()
 
 def _typecheckingstub__e007634bd28c31434790d2267792872f19c4eb0a079e63e0ff87fe468940bd5f(
     scope: _constructs_77d1e7e8.Construct,
@@ -486,21 +489,21 @@
     type: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__45ca08dc9374092b77f3e2462f88d86c15ec638f3ca898f12587f76db702ab52(
     *,
-    unxpose_policy: typing.Optional[typing.Union[CfnIntegrationModulePropsResourcesUnxposePolicy, typing.Dict[builtins.str, typing.Any]]] = None,
+    unxpose_managed_policy: typing.Optional[typing.Union[CfnIntegrationModulePropsResourcesUnxposeManagedPolicy, typing.Dict[builtins.str, typing.Any]]] = None,
     unxpose_role: typing.Optional[typing.Union[CfnIntegrationModulePropsResourcesUnxposeRole, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__54b5edd81ee288f35fa2ebe96875365b97e71d951ea5ed5f3543b533dfbf855c(
+def _typecheckingstub__ca77cfd3036d34cb2ab929edf9216ee7a861ebc86d607e619022bf8255dc8a67(
     *,
     properties: typing.Any = None,
     type: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/PKG-INFO` & `cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-unxpose-iam-integration-module
-Version: 1.0.0a7
+Version: 1.1.1a7
 Summary: Schema for Module Fragment of type Unxpose::IAM::Integration::MODULE
 Home-page: https://github.com/cdklabs/cdk-cloudformation.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # unxpose-iam-integration-module
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Unxpose::IAM::Integration::MODULE` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Unxpose::IAM::Integration::MODULE` v1.1.1.
 
 ## Description
 
 Schema for Module Fragment of type Unxpose::IAM::Integration::MODULE
 
 ## Usage
 
@@ -51,13 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Unxpose::IAM::Integration::MODULE`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Funxpose-iam-integration-module+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Funxpose-iam-integration-module+v1.1.1).
 * Issues related to `Unxpose::IAM::Integration::MODULE` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-unxpose-iam-integration-module-1.0.0a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/SOURCES.txt` & `cdk-cloudformation-unxpose-iam-integration-module-1.1.1a7/src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_unxpose_iam_integration_module/py.typed
 src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/PKG-INFO
 src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/SOURCES.txt
 src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/dependency_links.txt
 src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/requires.txt
 src/cdk_cloudformation_unxpose_iam_integration_module.egg-info/top_level.txt
 src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/__init__.py
-src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/unxpose-iam-integration-module@1.0.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_unxpose_iam_integration_module/_jsii/unxpose-iam-integration-module@1.1.1-alpha.7.jsii.tgz
```

