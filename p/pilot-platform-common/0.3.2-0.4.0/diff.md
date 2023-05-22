# Comparing `tmp/pilot-platform-common-0.3.2.tar.gz` & `tmp/pilot-platform-common-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-platform-common-0.3.2.tar", last modified: Fri May  5 18:50:55 2023, max compression
+gzip compressed data, was "pilot-platform-common-0.4.0.tar", last modified: Mon May 22 14:33:27 2023, max compression
```

## Comparing `pilot-platform-common-0.3.2.tar` & `pilot-platform-common-0.4.0.tar`

### file list

```diff
@@ -1,69 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/geid/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/geid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/geid/geid_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/jwt_handler/
--rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/jwt_handler/JWTHandler.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/jwt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/jwt_handler/jwt_handler_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/lineage/entity_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     8976 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/lineage/lineage_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/lineage/lineage_object.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/logger/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logger/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logger/logger_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/models/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/models/config_center_policy.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/models/service_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/common/object_storage_adaptor/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/base_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/boto3_admin_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    16665 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/minio_policy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/common/permissions/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/permissions/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/common/project/
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8203 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/project/project_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/project/project_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/common/vault/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/vault/vault_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/vault/vault_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8104 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/fixtures/fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_geid_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4019 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_lineage_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_logger_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_project_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_vault_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.788512 pilot-platform-common-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-22 14:33:27.788512 pilot-platform-common-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     1265 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/geid/
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/geid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/geid/geid_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/jwt_handler/
+-rw-r--r--   0 runner    (1001) docker     (122)     4295 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/jwt_handler/JWTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/jwt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/jwt_handler/jwt_handler_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/jwt_handler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/lineage/entity_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8968 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/lineage/lineage_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/lineage/lineage_object.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/models/config_center_policy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/models/service_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/object_storage_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/boto3_admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16665 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/minio_policy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/permissions/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3234 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/permissions/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/project/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8179 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/project/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/project/project_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/vault/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/vault/vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/vault/vault_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 14:33:27.788512 pilot-platform-common-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8103 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.788512 pilot-platform-common-0.4.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/fixtures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_geid_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7063 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_lineage_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_project_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_vault_client.py
```

### Comparing `pilot-platform-common-0.3.2/PKG-INFO` & `pilot-platform-common-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.3.2
+Version: 0.4.0
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Research
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # common
 
 [![Run Tests](https://github.com/PilotDataPlatform/common/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/common/actions/workflows/run-tests.yml)
 [![Python](https://img.shields.io/badge/python-3.8-brightgreen.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/pilot-platform-common.svg)](https://pypi.org/project/pilot-platform-common/)
```

### Comparing `pilot-platform-common-0.3.2/README.md` & `pilot-platform-common-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/__init__.py` & `pilot-platform-common-0.4.0/common/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (C) 2022-2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 from .geid import GEIDClient
 from .jwt_handler import JWTHandler
 from .lineage import LineageClient
-from .logger import LoggerFactory
 from .logging import configure_logging
 from .object_storage_adaptor import NotFoundError
 from .object_storage_adaptor import TokenError
 from .object_storage_adaptor import get_boto3_admin_client
 from .object_storage_adaptor import get_boto3_client
 from .object_storage_adaptor import get_minio_policy_client
 from .permissions import get_project_role
@@ -21,15 +20,14 @@
 from .project import ProjectNotFoundException
 from .vault import VaultClient
 
 __all__ = [
     'GEIDClient',
     'JWTHandler',
     'LineageClient',
-    'LoggerFactory',
     'configure_logging',
     'get_boto3_admin_client',
     'get_boto3_client',
     'get_minio_policy_client',
     'TokenError',
     'NotFoundError',
     'get_project_role',
```

### Comparing `pilot-platform-common-0.3.2/common/geid/geid_client.py` & `pilot-platform-common-0.4.0/common/geid/geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/lineage/entity_object.py` & `pilot-platform-common-0.4.0/common/lineage/entity_object.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/lineage/lineage_client.py` & `pilot-platform-common-0.4.0/common/lineage/lineage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # Copyright (C) 2022-2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
-import logging
 import time
 from logging import DEBUG
 from logging import ERROR
 
 import httpx
 
 from common.lineage.entity_object import Entity
 from common.lineage.entity_object import FileDataAttribute
 from common.lineage.lineage_object import Lineage
 from common.lineage.lineage_object import LineageAttirbute
+from common.logging import logger
 
 
 class LineageClient:
     def __init__(self, atlas_endpoint: str, username: str, password: str) -> None:
         self.atlas_endpoint = atlas_endpoint
         self.username = username
         self.password = password
 
         self.headers = {'content-type': 'application/json'}
 
-        self.logger = logging.getLogger('pilot.common')
+        self.logger = logger
         self.logger.setLevel(ERROR)
 
     async def debug_on(self):
         """
         Summary:
             The funtion will switch the log level to DEBUG
         """
```

### Comparing `pilot-platform-common-0.3.2/common/lineage/lineage_object.py` & `pilot-platform-common-0.4.0/common/lineage/lineage_object.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/logger/formatter.py` & `pilot-platform-common-0.4.0/common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/logging/logging.py` & `pilot-platform-common-0.4.0/common/logging/logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/models/config_center_policy.py` & `pilot-platform-common-0.4.0/common/models/config_center_policy.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/object_storage_adaptor/base_client.py` & `pilot-platform-common-0.4.0/common/object_storage_adaptor/base_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # Copyright (C) 2022-2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
-import logging
 from logging import DEBUG
 from logging import ERROR
 
+from common.logging import logger
+
 
 class BaseClient:
     """
     Summary:
         The base client for all object storage class that will
         include some basic functions:
             - set logger level to DEBUG
             - set logger level to ERROR
     """
 
     def __init__(self, client_name: str) -> None:
         self.client_name = client_name
 
         # the flag to turn on class-wide logs
-        self.logger = logging.getLogger('pilot.common')
+        self.logger = logger
         # initially only print out error info
         self.logger.setLevel(ERROR)
 
     async def debug_on(self):
         """
         Summary:
             The funtion will switch the log level to DEBUG
```

### Comparing `pilot-platform-common-0.3.2/common/object_storage_adaptor/boto3_admin_client.py` & `pilot-platform-common-0.4.0/common/object_storage_adaptor/boto3_admin_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/object_storage_adaptor/boto3_client.py` & `pilot-platform-common-0.4.0/common/object_storage_adaptor/boto3_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/object_storage_adaptor/minio_policy_client.py` & `pilot-platform-common-0.4.0/common/object_storage_adaptor/minio_policy_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/permissions/permissions.py` & `pilot-platform-common-0.4.0/common/permissions/permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # Copyright (C) 2022-2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
-import logging
+from typing import Any
+from typing import Optional
 
 from httpx import AsyncClient
 
-logger = logging.getLogger('pilot.common')
+from common.logging import logger
 
 
 async def has_permission(
-    auth_url: str, project_code: str, resource: str, zone: str, operation: str, current_identity: str
-):
-    if current_identity['role'] == 'admin':
-        role = 'platform_admin'
-    else:
-        if not project_code:
-            logger.info('No project code and not a platform admin, permission denied')
-            return False
-        role = await get_project_role(project_code, current_identity)
-        if not role:
-            logger.info('Unable to get project role in permissions check, user might not belong to project')
-            return False
+    auth_url: str, project_code: str, resource: str, zone: str, operation: str, current_identity: dict[str, Any]
+) -> bool:
+    if not project_code:
+        logger.info('No project code and not a platform admin, permission denied')
+        return False
+    role = await get_project_role(project_code, current_identity)
+    if not role:
+        logger.info('Unable to get project role in permissions check, user might not belong to project')
+        return False
 
     try:
         payload = {
             'role': role,
             'resource': resource,
             'zone': zone,
             'operation': operation,
@@ -42,15 +40,15 @@
         return False
     except Exception as e:
         error_msg = str(e)
         logger.info(f'Exception on authorize call: {error_msg}')
         raise Exception(f'Error calling authorize API - {error_msg}')
 
 
-async def get_project_role(project_code, current_identity):
+async def get_project_role(project_code: str, current_identity: dict[str, Any]) -> Optional[str]:
     role = None
     if current_identity['role'] == 'admin':
         role = 'platform_admin'
     else:
         for realm_role in current_identity['realm_roles']:
             # if this is a role for the correct project
             if realm_role.startswith(project_code + '-'):
```

### Comparing `pilot-platform-common-0.3.2/common/project/project_client.py` & `pilot-platform-common-0.4.0/common/project/project_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Copyright (C) 2022-2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 import asyncio
 import json
-import logging
 
 import httpx
 from redis.asyncio.utils import from_url
 from redis.exceptions import ConnectionError
 
+from common.logging import logger
+
 from .project_exceptions import ProjectException
 from .project_exceptions import ProjectNotFoundException
 
 CACHE_PREFIX = 'project_client-'
 CACHE_EXPIRY = 300
 
-logger = logging.getLogger('pilot.common')
-
 
 class ProjectObject(object):
     attributes = [
         'id',
         'code',
         'name',
         'description',
```

### Comparing `pilot-platform-common-0.3.2/common/project/project_exceptions.py` & `pilot-platform-common-0.4.0/common/project/project_exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/common/vault/vault_client.py` & `pilot-platform-common-0.4.0/common/vault/vault_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/pilot_platform_common.egg-info/PKG-INFO` & `pilot-platform-common-0.4.0/pilot_platform_common.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.3.2
+Version: 0.4.0
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Research
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # common
 
 [![Run Tests](https://github.com/PilotDataPlatform/common/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/common/actions/workflows/run-tests.yml)
 [![Python](https://img.shields.io/badge/python-3.8-brightgreen.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/pilot-platform-common.svg)](https://pypi.org/project/pilot-platform-common/)
```

### Comparing `pilot-platform-common-0.3.2/pilot_platform_common.egg-info/SOURCES.txt` & `pilot-platform-common-0.4.0/pilot_platform_common.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 setup.py
 common/__init__.py
 common/geid/__init__.py
 common/geid/geid_client.py
 common/jwt_handler/JWTHandler.py
 common/jwt_handler/__init__.py
 common/jwt_handler/jwt_handler_exception.py
+common/jwt_handler/models.py
 common/lineage/__init__.py
 common/lineage/entity_object.py
 common/lineage/lineage_client.py
 common/lineage/lineage_object.py
-common/logger/__init__.py
-common/logger/formatter.py
-common/logger/logger_factory.py
 common/logging/__init__.py
+common/logging/formatter.py
+common/logging/logger.py
 common/logging/logging.py
 common/models/__init__.py
 common/models/config_center_policy.py
 common/models/service_id_generator.py
 common/object_storage_adaptor/__init__.py
 common/object_storage_adaptor/base_client.py
 common/object_storage_adaptor/boto3_admin_client.py
@@ -39,14 +39,13 @@
 pilot_platform_common.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_formatter.py
 tests/test_geid_client.py
 tests/test_jwt_handler.py
 tests/test_lineage_client.py
-tests/test_logger_factory.py
 tests/test_logging.py
 tests/test_permissions.py
 tests/test_project_client.py
 tests/test_vault_client.py
 tests/fixtures/__init__.py
 tests/fixtures/fake.py
```

### Comparing `pilot-platform-common-0.3.2/pyproject.toml` & `pilot-platform-common-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "common"
-version = "0.3.2"
+version = "0.4.0"
 description = ""
 authors = ["Indoc Research"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 python-dotenv = ">=0.19.1"
 python-json-logger = ">= 0.1.11, <= 2.02"
 aioboto3 = "^9.6.0"
 xmltodict = "^0.13.0"
 minio = "^7.1.8"
 httpx = "^0.23.0"
 pyjwt = "2.6.0"
```

### Comparing `pilot-platform-common-0.3.2/setup.py` & `pilot-platform-common-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pilot-platform-common',
-    version='0.3.2',
+    version='0.4.0',
     author='Indoc Research',
     author_email='etaylor@indocresearch.org',
     description='Generates entity ID and connects with Vault (secret engine) to retrieve credentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.9',
     install_requires=[
         'python-dotenv==0.19.1',
         'httpx==0.23.0',
         'redis>=4.5.0,<5.0.0',
         'aioboto3==9.6.0',
         'xmltodict==0.13.0',
         'minio==7.1.8',
```

### Comparing `pilot-platform-common-0.3.2/tests/conftest.py` & `pilot-platform-common-0.4.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     else:
         roles = [f'{project_code}-{project_role}']
     current_time = time.time() - 240 if expired else time.time()
     return {
         'exp': current_time + 240,
         'iat': current_time - 60,
         'aud': 'account',
-        'sub': platform_role,
+        'sub': str(uuid4()),
         'typ': 'Bearer',
         'acr': '1',
         'realm_access': {'roles': roles},
         'resource_access': {'account': {'roles': roles}},
         'email_verified': True,
         'name': 'test test',
         'preferred_username': 'test',
```

### Comparing `pilot-platform-common-0.3.2/tests/test_formatter.py` & `pilot-platform-common-0.4.0/tests/test_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 import logging
 from logging import LogRecord
 
 import pytest
 
-from common.logger.formatter import CustomJsonFormatter
-from common.logger.formatter import get_formatter
+from common.logging.formatter import CustomJsonFormatter
+from common.logging.formatter import get_formatter
 
 
 @pytest.fixture
 def custom_json_formatter():
     yield CustomJsonFormatter()
```

### Comparing `pilot-platform-common-0.3.2/tests/test_lineage_client.py` & `pilot-platform-common-0.4.0/tests/test_lineage_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/tests/test_logging.py` & `pilot-platform-common-0.4.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/tests/test_permissions.py` & `pilot-platform-common-0.4.0/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/tests/test_project_client.py` & `pilot-platform-common-0.4.0/tests/test_project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.2/tests/test_vault_client.py` & `pilot-platform-common-0.4.0/tests/test_vault_client.py`

 * *Files identical despite different names*

