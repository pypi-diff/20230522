# Comparing `tmp/openapi_pydantic-0.2.1.tar.gz` & `tmp/openapi_pydantic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_pydantic-0.2.1.tar", max compression
+gzip compressed data, was "openapi_pydantic-0.2.2.tar", max compression
```

## Comparing `openapi_pydantic-0.2.1.tar` & `openapi_pydantic-0.2.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1896 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/LICENSE
--rw-r--r--   0        0        0     8376 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/README.md
--rw-r--r--   0        0        0     1329 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/__init__.py
--rw-r--r--   0        0        0       26 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/py.typed
--rw-r--r--   0        0        0     5464 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/util.py
--rw-r--r--   0        0        0     1419 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/__init__.py
--rw-r--r--   0        0        0      447 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/parser.py
--rw-r--r--   0        0        0     1603 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/README.md
--rw-r--r--   0        0        0     1941 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/__init__.py
--rw-r--r--   0        0        0      747 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/callback.py
--rw-r--r--   0        0        0     5491 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/components.py
--rw-r--r--   0        0        0      865 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/contact.py
--rw-r--r--   0        0        0      215 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/datatype.py
--rw-r--r--   0        0        0     1282 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/discriminator.py
--rw-r--r--   0        0        0     3141 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/encoding.py
--rw-r--r--   0        0        0     1554 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/example.py
--rw-r--r--   0        0        0      731 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/external_documentation.py
--rw-r--r--   0        0        0     1073 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/header.py
--rw-r--r--   0        0        0     1982 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/info.py
--rw-r--r--   0        0        0      645 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/license.py
--rw-r--r--   0        0        0     2958 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/link.py
--rw-r--r--   0        0        0     2980 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/media_type.py
--rw-r--r--   0        0        0     2125 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/oauth_flow.py
--rw-r--r--   0        0        0      835 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/oauth_flows.py
--rw-r--r--   0        0        0     2684 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/open_api.py
--rw-r--r--   0        0        0     6422 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/operation.py
--rw-r--r--   0        0        0     8047 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/parameter.py
--rw-r--r--   0        0        0     4930 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/path_item.py
--rw-r--r--   0        0        0     1017 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/paths.py
--rw-r--r--   0        0        0      894 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/reference.py
--rw-r--r--   0        0        0     3209 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/request_body.py
--rw-r--r--   0        0        0     3719 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/response.py
--rw-r--r--   0        0        0     2050 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/responses.py
--rw-r--r--   0        0        0    22285 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/schema.py
--rw-r--r--   0        0        0     1325 2023-05-21 20:07:00.743044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/security_requirement.py
--rw-r--r--   0        0        0     3545 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/security_scheme.py
--rw-r--r--   0        0        0     1889 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/server.py
--rw-r--r--   0        0        0     1071 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/server_variable.py
--rw-r--r--   0        0        0      887 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/tag.py
--rw-r--r--   0        0        0     5464 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/util.py
--rw-r--r--   0        0        0     1850 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/xml.py
--rw-r--r--   0        0        0     1663 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/README.md
--rw-r--r--   0        0        0     1941 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/__init__.py
--rw-r--r--   0        0        0      806 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/callback.py
--rw-r--r--   0        0        0     5650 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/components.py
--rw-r--r--   0        0        0      861 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/contact.py
--rw-r--r--   0        0        0      238 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/datatype.py
--rw-r--r--   0        0        0     1282 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/discriminator.py
--rw-r--r--   0        0        0     3573 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/encoding.py
--rw-r--r--   0        0        0     1633 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/example.py
--rw-r--r--   0        0        0      729 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/external_documentation.py
--rw-r--r--   0        0        0     1076 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/header.py
--rw-r--r--   0        0        0     2112 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/info.py
--rw-r--r--   0        0        0     1028 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/license.py
--rw-r--r--   0        0        0     3038 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/link.py
--rw-r--r--   0        0        0     3060 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/media_type.py
--rw-r--r--   0        0        0     2306 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/oauth_flow.py
--rw-r--r--   0        0        0      835 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/oauth_flows.py
--rw-r--r--   0        0        0     3522 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/open_api.py
--rw-r--r--   0        0        0     6704 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/operation.py
--rw-r--r--   0        0        0     8049 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/parameter.py
--rw-r--r--   0        0        0     5010 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/path_item.py
--rw-r--r--   0        0        0     1040 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/paths.py
--rw-r--r--   0        0        0     1463 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/reference.py
--rw-r--r--   0        0        0     3209 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/request_body.py
--rw-r--r--   0        0        0     3545 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/response.py
--rw-r--r--   0        0        0     2048 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/responses.py
--rw-r--r--   0        0        0    38873 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/schema.py
--rw-r--r--   0        0        0     1434 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/security_requirement.py
--rw-r--r--   0        0        0     3932 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/security_scheme.py
--rw-r--r--   0        0        0     1890 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/server.py
--rw-r--r--   0        0        0     1069 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/server_variable.py
--rw-r--r--   0        0        0      887 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/tag.py
--rw-r--r--   0        0        0     1962 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/xml.py
--rw-r--r--   0        0        0     1222 2023-05-21 20:07:00.747044 openapi_pydantic-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9245 1970-01-01 00:00:00.000000 openapi_pydantic-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1896 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/LICENSE
+-rw-r--r--   0        0        0     8376 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/README.md
+-rw-r--r--   0        0        0     1366 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/py.typed
+-rw-r--r--   0        0        0     5464 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/util.py
+-rw-r--r--   0        0        0     1419 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/__init__.py
+-rw-r--r--   0        0        0      447 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/parser.py
+-rw-r--r--   0        0        0     1603 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/README.md
+-rw-r--r--   0        0        0     1941 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/__init__.py
+-rw-r--r--   0        0        0      747 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/callback.py
+-rw-r--r--   0        0        0     5491 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/components.py
+-rw-r--r--   0        0        0      865 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/contact.py
+-rw-r--r--   0        0        0      215 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/datatype.py
+-rw-r--r--   0        0        0     1282 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/discriminator.py
+-rw-r--r--   0        0        0     3141 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/encoding.py
+-rw-r--r--   0        0        0     1554 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/example.py
+-rw-r--r--   0        0        0      731 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/external_documentation.py
+-rw-r--r--   0        0        0     1073 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/header.py
+-rw-r--r--   0        0        0     1982 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/info.py
+-rw-r--r--   0        0        0      645 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/license.py
+-rw-r--r--   0        0        0     2958 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/link.py
+-rw-r--r--   0        0        0     2980 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/media_type.py
+-rw-r--r--   0        0        0     2125 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/oauth_flow.py
+-rw-r--r--   0        0        0      835 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/oauth_flows.py
+-rw-r--r--   0        0        0     2684 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/open_api.py
+-rw-r--r--   0        0        0     6422 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/operation.py
+-rw-r--r--   0        0        0     8047 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/parameter.py
+-rw-r--r--   0        0        0     4930 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/path_item.py
+-rw-r--r--   0        0        0     1017 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/paths.py
+-rw-r--r--   0        0        0      894 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/reference.py
+-rw-r--r--   0        0        0     3209 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/request_body.py
+-rw-r--r--   0        0        0     3719 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/response.py
+-rw-r--r--   0        0        0     2050 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/responses.py
+-rw-r--r--   0        0        0    22285 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/schema.py
+-rw-r--r--   0        0        0     1325 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/security_requirement.py
+-rw-r--r--   0        0        0     3545 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/security_scheme.py
+-rw-r--r--   0        0        0     1889 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/server.py
+-rw-r--r--   0        0        0     1071 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/server_variable.py
+-rw-r--r--   0        0        0      887 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/tag.py
+-rw-r--r--   0        0        0     5464 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/util.py
+-rw-r--r--   0        0        0     1850 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/xml.py
+-rw-r--r--   0        0        0     1663 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/README.md
+-rw-r--r--   0        0        0     1941 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/__init__.py
+-rw-r--r--   0        0        0      806 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/callback.py
+-rw-r--r--   0        0        0     5650 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/components.py
+-rw-r--r--   0        0        0      861 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/contact.py
+-rw-r--r--   0        0        0      238 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/datatype.py
+-rw-r--r--   0        0        0     1282 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/discriminator.py
+-rw-r--r--   0        0        0     3573 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/encoding.py
+-rw-r--r--   0        0        0     1633 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/example.py
+-rw-r--r--   0        0        0      729 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/external_documentation.py
+-rw-r--r--   0        0        0     1076 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/header.py
+-rw-r--r--   0        0        0     2112 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/info.py
+-rw-r--r--   0        0        0     1028 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/license.py
+-rw-r--r--   0        0        0     3038 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/link.py
+-rw-r--r--   0        0        0     3060 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/media_type.py
+-rw-r--r--   0        0        0     2306 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/oauth_flow.py
+-rw-r--r--   0        0        0      835 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/oauth_flows.py
+-rw-r--r--   0        0        0     3522 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/open_api.py
+-rw-r--r--   0        0        0     6704 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/operation.py
+-rw-r--r--   0        0        0     8049 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/parameter.py
+-rw-r--r--   0        0        0     5010 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/path_item.py
+-rw-r--r--   0        0        0     1040 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/paths.py
+-rw-r--r--   0        0        0     1463 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/reference.py
+-rw-r--r--   0        0        0     3209 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/request_body.py
+-rw-r--r--   0        0        0     3545 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/response.py
+-rw-r--r--   0        0        0     2048 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/responses.py
+-rw-r--r--   0        0        0    38873 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/schema.py
+-rw-r--r--   0        0        0     1434 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/security_requirement.py
+-rw-r--r--   0        0        0     3932 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/security_scheme.py
+-rw-r--r--   0        0        0     1890 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/server.py
+-rw-r--r--   0        0        0     1069 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/server_variable.py
+-rw-r--r--   0        0        0      887 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/tag.py
+-rw-r--r--   0        0        0     1962 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/xml.py
+-rw-r--r--   0        0        0     1222 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9245 1970-01-01 00:00:00.000000 openapi_pydantic-0.2.2/PKG-INFO
```

### Comparing `openapi_pydantic-0.2.1/LICENSE` & `openapi_pydantic-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/README.md` & `openapi_pydantic-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/__init__.py` & `openapi_pydantic-0.2.2/openapi_pydantic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 from .v3 import XML as XML
 from .v3 import Callback as Callback
 from .v3 import Components as Components
 from .v3 import Contact as Contact
+from .v3 import DataType as DataType
 from .v3 import Discriminator as Discriminator
 from .v3 import Encoding as Encoding
 from .v3 import Example as Example
 from .v3 import ExternalDocumentation as ExternalDocumentation
 from .v3 import Header as Header
 from .v3 import Info as Info
 from .v3 import License as License
```

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/util.py` & `openapi_pydantic-0.2.2/openapi_pydantic/util.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/__init__.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/README.md` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/__init__.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/callback.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/components.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/components.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/contact.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/contact.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/discriminator.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/encoding.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/example.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/example.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/external_documentation.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/external_documentation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/header.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/header.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/info.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/info.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/license.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/license.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/link.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/link.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/media_type.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/oauth_flow.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/oauth_flows.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/open_api.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/open_api.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/operation.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/parameter.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/path_item.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/paths.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/reference.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/reference.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/request_body.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/response.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/response.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/responses.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/schema.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/schema.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/security_requirement.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/security_scheme.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/security_scheme.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/server.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/server.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/server_variable.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/tag.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/tag.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/util.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/util.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_0_3/xml.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/xml.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/README.md` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/__init__.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/callback.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/components.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/components.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/contact.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/contact.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/discriminator.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/encoding.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/example.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/example.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/external_documentation.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/external_documentation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/header.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/header.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/info.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/info.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/license.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/license.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/link.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/link.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/media_type.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/oauth_flow.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/oauth_flows.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/open_api.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/open_api.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/operation.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/parameter.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/path_item.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/paths.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/reference.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/reference.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/request_body.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/response.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/response.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/responses.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/schema.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/schema.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/security_requirement.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/security_scheme.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/security_scheme.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/server.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/server.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/server_variable.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/tag.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/tag.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/openapi_pydantic/v3/v3_1_0/xml.py` & `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/xml.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.1/pyproject.toml` & `openapi_pydantic-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-pydantic"
-version = "0.2.1"
+version = "0.2.2"
 description = "Pydantic OpenAPI schema implementation"
 authors = ["Mike Oakley <mike-oakley@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/mike-oakley/openapi-pydantic"
 license = "MIT"
 keywords = [
   "openapi",
```

### Comparing `openapi_pydantic-0.2.1/PKG-INFO` & `openapi_pydantic-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pydantic OpenAPI schema implementation
 Home-page: https://github.com/mike-oakley/openapi-pydantic
 License: MIT
 Keywords: openapi,schema,parser,pydantic,validation
 Author: Mike Oakley
 Author-email: mike-oakley@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

