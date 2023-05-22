# Comparing `tmp/energinet-ml-sdk-1.0.0.dev24.tar.gz` & `tmp/energinet-ml-sdk-1.0.0.dev25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energinet-ml-sdk-1.0.0.dev24.tar", last modified: Wed May 17 14:36:16 2023, max compression
+gzip compressed data, was "energinet-ml-sdk-1.0.0.dev25.tar", last modified: Mon May 22 07:50:30 2023, max compression
```

## Comparing `energinet-ml-sdk-1.0.0.dev24.tar` & `energinet-ml-sdk-1.0.0.dev25.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/
--rw-r--r--   0 vsts      (1001) docker     (123)      592 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1733 2023-05-17 14:36:05.147612 energinet-ml-sdk-1.0.0.dev24/README
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/
--rw-r--r--   0 vsts      (1001) docker     (123)      210 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13179 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/backend.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8140 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/datasets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4352 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/interactive.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2130 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/submitting.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6853 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/training.py
--rw-r--r--   0 vsts      (1001) docker     (123)      190 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/backend.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)      833 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      581 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/files.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3886 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/init.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3133 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/release.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5525 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/submit.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5250 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/train.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/project/
--rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/project/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/project/init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7294 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11202 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/projects.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2062 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/verify.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/core/
--rw-r--r--   0 vsts      (1001) docker     (123)       33 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4552 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/backend.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4381 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/configurable.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3006 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/files.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3760 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27424 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2555 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1871 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/requirements.py
--rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/submitting.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9048 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/templates.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3293 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/training.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/
--rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/COMMAND_NAME
--rw-r--r--   0 vsts      (1001) docker     (123)       17 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/PACKAGE_NAME
--rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-05-17 14:36:16.179858 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/PACKAGE_VERSION
--rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/PYTHON_VERSION
--rw-r--r--   0 vsts      (1001) docker     (123)     2793 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/settings.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/static/
--rw-r--r--   0 vsts      (1001) docker     (123)      492 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/static/Dockerfile
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      147 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1728 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4490 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (123)      715 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/constants.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/ml_deployment/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/ml_deployment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/ml_deployment/deployment_smoke_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/webapp_deployment/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/webapp_deployment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      515 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/webapp_deployment/deployment_smoke_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8099 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/backend_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4350 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/datasets_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)      675 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/training_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      899 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/files_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3739 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/init_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/release_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9074 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/submit_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3566 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/train_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/project/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/project/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2310 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/project/init_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4922 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/decorators_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7759 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/projects_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2197 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/backend_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1126 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/configurable_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/files_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/logger_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14679 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/model_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2874 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/project_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2378 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/requirements_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/submitting_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/
+-rw-r--r--   0 vsts      (1001) docker     (123)      592 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1733 2023-05-22 07:50:15.862798 energinet-ml-sdk-1.0.0.dev25/README
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/
+-rw-r--r--   0 vsts      (1001) docker     (123)      210 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13179 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8140 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/datasets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4352 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2130 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/submitting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6853 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/training.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      190 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/backend.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      581 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/files.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2965 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/init.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3133 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/release.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5525 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/submit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5250 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/train.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/project/init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7294 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11202 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/projects.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2062 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/verify.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/core/
+-rw-r--r--   0 vsts      (1001) docker     (123)       33 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4552 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4381 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/configurable.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3006 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/files.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3760 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27442 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2555 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1871 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/requirements.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/submitting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9048 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/templates.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3293 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/training.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/
+-rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/COMMAND_NAME
+-rw-r--r--   0 vsts      (1001) docker     (123)       17 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/PACKAGE_NAME
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-05-22 07:50:30.098775 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/PACKAGE_VERSION
+-rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/PYTHON_VERSION
+-rw-r--r--   0 vsts      (1001) docker     (123)     2793 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/settings.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/static/
+-rw-r--r--   0 vsts      (1001) docker     (123)      492 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/static/Dockerfile
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      147 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1728 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4481 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      715 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/constants.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/ml_deployment/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/ml_deployment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/ml_deployment/deployment_smoke_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/webapp_deployment/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/webapp_deployment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      515 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/webapp_deployment/deployment_smoke_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8099 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/backend_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4350 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/datasets_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      675 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/training_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      899 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/files_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3739 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/init_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/release_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9074 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/submit_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3566 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/train_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2310 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/project/init_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4922 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/decorators_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7759 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/projects_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2197 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/backend_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1126 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/configurable_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/files_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/logger_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14679 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/model_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2874 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/project_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2378 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/requirements_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/submitting_test.py
```

### Comparing `energinet-ml-sdk-1.0.0.dev24/PKG-INFO` & `energinet-ml-sdk-1.0.0.dev25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energinet-ml-sdk
-Version: 1.0.0.dev24
+Version: 1.0.0.dev25
 Summary: Energinet Machine Learning
 Home-page: UNKNOWN
 Author: Koncern Digitalisering Advanced Analytics Team
 Author-email: mny@energinet.dk, xjakk@energinet.dk
 License: Apache Software License 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `energinet-ml-sdk-1.0.0.dev24/README` & `energinet-ml-sdk-1.0.0.dev25/README`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/backend.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/backend.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/datasets.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/datasets.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/interactive.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/interactive.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/logger.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/logger.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/submitting.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/submitting.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/training.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/training.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/__init__.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Hack OS version to avoid licencing problems in azureml
 # TODO How else to get azureml Datasets working?
 # TODO Move to somewhere else?
 runtime.version = ("18", "10", "0")
 
 from energinetml.settings import PACKAGE_VERSION  # noqa: E402
 
-from .cluster import cluster_group  # noqa: E402
 from .model import model_group  # noqa: E402
 from .project import project_group  # noqa: E402
 
 
 @click.command()
 def version():
     """
@@ -32,9 +31,8 @@
     Click main entrypoint.
     """
     pass
 
 
 main.add_command(project_group, "project")
 main.add_command(model_group, "model")
-main.add_command(cluster_group, "cluster")
 main.add_command(version)
```

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/__init__.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/__init__.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/release.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/release.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/submit.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/submit.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/train.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/train.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/project/init.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/project/init.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/decorators.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/projects.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/projects.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/verify.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/verify.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/backend.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/backend.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/configurable.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/configurable.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/files.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/files.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/logger.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/logger.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/model.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,24 +565,24 @@
 
     path: str
     run_id: str
     experiment_name: str
     project_meta: Dict[str, str]
     _tempdir: tempfile.TemporaryDirectory = None
 
-    @property
-    def portal_url(self) -> str:
-        """The URL to a training run.
+    # @property
+    # def portal_url(self) -> str:
+    #     """The URL to a training run.
 
-        Returns:
-            str: The URL of the training run
-        """
-        return backend.get_portal_url(
-            self.project_meta, self.experiment_name, self.run_id
-        )
+    #     Returns:
+    #         str: The URL of the training run
+    #     """
+    #     return backend.get_portal_url(
+    #         self.project_meta, self.experiment_name, self.run_id
+    #     )
 
     @classmethod
     def from_cloud(
         cls, experiment_name: str, run_id: str, path=None, project_meta=None
     ) -> "ModelArtifact":
         """Download model and trained_model files from cloud environment
         to a (temporary) folder.
```

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/project.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/project.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/requirements.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/requirements.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/submitting.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/submitting.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/templates.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/templates.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/core/training.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/core/training.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/settings.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/settings.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/model.py` & `energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/model.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/setup.py` & `energinet-ml-sdk-1.0.0.dev25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,18 +102,19 @@
     install_requires=[
         "requests",
         "pandas>=1.2.0",
         "packaging==20.9",
         "click==8.0.3",
         "click-spinner==0.1.10",
         "requirements-parser==0.2.0",
-        "azure-cli-core~=2.34.1",
-        "azure-identity~=1.7.0",
-        "azureml-core~=1.39.0",
-        "azureml-dataset-runtime~=1.39.0",
+        "azure-core",
+        "azure-cli-core",
+        "azure-identity",
+        "azureml-core",
+        "azureml-dataset-runtime",
     ],
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={"dev": [], "build": [], "test": []},
     cmdclass={"sdist": sdist_hg},
```

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/conftest.py` & `energinet-ml-sdk-1.0.0.dev25/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/constants.py` & `energinet-ml-sdk-1.0.0.dev25/tests/constants.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/smoketest/ml_deployment/deployment_smoke_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/smoketest/ml_deployment/deployment_smoke_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/smoketest/webapp_deployment/deployment_smoke_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/smoketest/webapp_deployment/deployment_smoke_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/backend_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/backend_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/datasets_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/datasets_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/training_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/training_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/files_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/files_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/init_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/init_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/submit_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/submit_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/train_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/train_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/project/init_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/project/init_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/decorators_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/decorators_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/projects_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/projects_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/backend_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/backend_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/configurable_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/configurable_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/files_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/files_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/logger_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/logger_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/model_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/model_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/project_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/project_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/requirements_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/requirements_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/submitting_test.py` & `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/submitting_test.py`

 * *Files identical despite different names*

