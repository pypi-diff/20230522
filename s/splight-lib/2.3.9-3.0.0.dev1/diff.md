# Comparing `tmp/splight-lib-2.3.9.tar.gz` & `tmp/splight-lib-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-2.3.9.tar", last modified: Mon May  8 14:01:19 2023, max compression
+gzip compressed data, was "splight-lib-3.0.0.dev1.tar", last modified: Mon May 22 13:43:36 2023, max compression
```

## Comparing `splight-lib-2.3.9.tar` & `splight-lib-3.0.0.dev1.tar`

### file list

```diff
@@ -1,143 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.338043 splight-lib-2.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:18.000000 splight-lib-2.3.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-08 14:01:19.338043 splight-lib-2.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 14:01:18.000000 splight-lib-2.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.322043 splight-lib-2.3.9/remote_splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.322043 splight-lib-2.3.9/remote_splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.322043 splight-lib-2.3.9/remote_splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/communication/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.322043 splight-lib-2.3.9/remote_splight_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/database/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.322043 splight-lib-2.3.9/remote_splight_lib/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/datalake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.322043 splight-lib-2.3.9/remote_splight_lib/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-08 14:01:18.000000 splight-lib-2.3.9/remote_splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:01:19.338043 splight-lib-2.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-08 14:01:18.000000 splight-lib-2.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.322043 splight-lib-2.3.9/splight_abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/auth/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/cache/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/client/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/client/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/communication/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/database/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/database/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/datalake/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/deployment/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/hub/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/notification/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.326043 splight-lib-2.3.9/splight_abstract/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/remote/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.330043 splight-lib-2.3.9/splight_abstract/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_abstract/storage/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.330043 splight-lib-2.3.9/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.330043 splight-lib-2.3.9/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.330043 splight-lib-2.3.9/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.334043 splight-lib-2.3.9/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.334043 splight-lib-2.3.9/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.334043 splight-lib-2.3.9/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27544 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.334043 splight-lib-2.3.9/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.334043 splight-lib-2.3.9/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.330043 splight-lib-2.3.9/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-08 14:01:19.000000 splight-lib-2.3.9/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-08 14:01:19.000000 splight-lib-2.3.9/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:01:19.000000 splight-lib-2.3.9/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:01:19.000000 splight-lib-2.3.9/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-08 14:01:19.000000 splight-lib-2.3.9/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 14:01:19.000000 splight-lib-2.3.9/splight_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.338043 splight-lib-2.3.9/splight_models/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:01:19.338043 splight-lib-2.3.9/splight_models/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/communication/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/communication/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/datalake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 14:01:18.000000 splight-lib-2.3.9/splight_models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.636748 splight-lib-3.0.0.dev1/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.636748 splight-lib-3.0.0.dev1/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.636748 splight-lib-3.0.0.dev1/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.636748 splight-lib-3.0.0.dev1/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.636748 splight-lib-3.0.0.dev1/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.640748 splight-lib-3.0.0.dev1/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:43:36.636748 splight-lib-3.0.0.dev1/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 13:43:36.000000 splight-lib-3.0.0.dev1/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-2.3.9/PKG-INFO` & `splight-lib-3.0.0.dev1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.3.9
+Version: 3.0.0.dev1
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-2.3.9/remote_splight_lib/communication/client.py` & `splight-lib-3.0.0.dev1/splight_lib/client/communication/remote_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import logging
 from typing import Callable, Dict
 
 import pysher
 import requests
 from furl import furl
-from remote_splight_lib.auth.auth import SplightAuthToken
-from remote_splight_lib.communication.classmap import CLASSMAP
-from remote_splight_lib.settings import settings
 from retry import retry
-from splight_abstract.communication import (
+from splight_lib.auth import SplightAuthToken
+from splight_lib.client.communication.abstract import (
     AbstractCommunicationClient,
-    ClientNotReady,
 )
+from splight_lib.client.communication.classmap import CLASSMAP
+from splight_lib.client.communication.exceptions import ClientNotReady
 from splight_lib.logging._internal import LogTags, get_splight_logger
-from splight_models.communication import (
+from splight_lib.models.communication import (
     CommunicationClientStatus,
     CommunicationContext,
-    CommunicationEvent,
 )
+from splight_lib.models.event import CommunicationEvent
 
 logger = get_splight_logger()
 
 
 class CommunicationFactory:
-    def __init__(self, model):
+    def __init__(self, model, base_url, access_id: str, secret_key: str):
         self._model = model
+        self._base_url = furl(base_url)
+        self._access_id = access_id
+        self._secret_key = secret_key
 
     def get_url(self):
-        base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
-        return base_url / CLASSMAP.get(self._model)
+        return self._base_url / CLASSMAP.get(self._model)
 
     def get_headers(self):
         auth_token = SplightAuthToken(
-            access_key=settings.SPLIGHT_ACCESS_ID,
-            secret_key=settings.SPLIGHT_SECRET_KEY,
+            access_key=self._access_id,
+            secret_key=self._secret_key,
         )
         return auth_token.header
 
     def create(self, data: Dict):
         response = requests.post(
             self.get_url(), json=data, headers=self.get_headers()
         )
@@ -53,17 +54,28 @@
         assert (
             response.status_code == 200
         ), f"Cant fetch communication {self._model}."
         data = response.json()
         return self._model.parse_obj(data)
 
 
-class CommunicationClient(AbstractCommunicationClient):
-    def __init__(self, daemon: bool = True, *args, **kwargs):
+class RemoteCommunicationClient(AbstractCommunicationClient):
+    def __init__(
+        self,
+        url: str,
+        access_id: str,
+        secret_key: str,
+        daemon: bool = True,
+        *args,
+        **kwargs,
+    ):
         super().__init__(*args, **kwargs)
+        self._base_url = url
+        self._access_id = access_id
+        self._secret_key = secret_key
         self._status = CommunicationClientStatus.STOPPED
         self._channel_bindings = []
         self._client, self._context = None, None
         self._system_bindings = [
             (
                 "pusher:connection_established",
                 self.__on_connection_established,
@@ -77,15 +89,16 @@
             self.__load_client()
             self.__check_readiness()
             logger.info(
                 "Communication client started.", tags=LogTags.COMMUNICATION
             )
         except Exception as e:
             logger.warning(
-                "Failed to start communication client due to exception %s. Moving forward without remote commands.",
+                "Failed to start communication client due to exception %s. "
+                "Moving forward without remote commands.",
                 e,
                 exc_info=True,
                 tags=LogTags.COMMUNICATION,
             )
             self._status = CommunicationClientStatus.ERROR
 
     @property
@@ -100,15 +113,20 @@
     def __check_readiness(self):
         if self.status != CommunicationClientStatus.READY:
             raise ClientNotReady
 
     @retry(Exception, tries=3, delay=2, jitter=1)
     def __load_context(self):
         params = {"instance_id": self.instance_id}
-        self._context = CommunicationFactory(CommunicationContext).get(params)
+        self._context = CommunicationFactory(
+            CommunicationContext,
+            base_url=self._base_url,
+            access_id=self._access_id,
+            secret_key=self._secret_key,
+        ).get(params)
 
     @retry(Exception, tries=3, delay=2, jitter=1)
     def __load_client(self):
         if not self._context:
             raise NotImplementedError
         self._client = pysher.Pusher(
             key=self._context.key,
@@ -157,15 +175,18 @@
         self._private_room_channel.bind(event_name, event_handler)
 
     def unbind(self, event_name: str, event_handler: Callable) -> None:
         # TODO implement this
         raise NotImplementedError
 
     def trigger(self, event: CommunicationEvent):
-        return CommunicationFactory(CommunicationEvent).create(
-            data=event.dict()
-        )
+        return CommunicationFactory(
+            CommunicationEvent,
+            base_url=self._base_url,
+            access_id=self._access_id,
+            secret_key=self._secret_key,
+        ).create(data=event.dict())
 
     def authenticate(
         self, channel_name: str, socket_id: str, custom_data: Dict = None
     ) -> Dict:
         raise NotImplementedError
```

### Comparing `splight-lib-2.3.9/remote_splight_lib/database/client.py` & `splight-lib-3.0.0.dev1/splight_lib/client/database/remote_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,164 +1,185 @@
-import json
 from tempfile import NamedTemporaryFile
-from typing import Dict, List, Type
+from typing import Any, Dict, Generator, List, Optional, Union
 
 from furl import furl
-from pydantic import BaseModel
-from remote_splight_lib.auth import SplightAuthToken
-from remote_splight_lib.exceptions import InvalidModel
-from remote_splight_lib.settings import settings
-from requests import Session
-from requests.exceptions import ConnectionError, Timeout
+from httpx._status_codes import codes
 from retry import retry
-from splight_abstract.database import AbstractDatabaseClient
-from splight_abstract.remote import AbstractRemoteClient
+from splight_lib.abstract.client import AbstractRemoteClient
+from splight_lib.auth import SplightAuthToken
+from splight_lib.client.database.abstract import AbstractDatabaseClient
+from splight_lib.client.database.classmap import (
+    CUSTOM_PATHS_MAP,
+    MODEL_NAME_MAP,
+)
+from splight_lib.client.exceptions import (
+    SPLIGHT_REQUEST_EXCEPTIONS,
+    InstanceNotFound,
+    InvalidModelName,
+)
+from splight_lib.constants import ENGINE_PREFIX
 from splight_lib.encryption import EncryptionClient
 from splight_lib.logging._internal import LogTags, get_splight_logger
-from splight_models import File
-
-from .classmap import CLASSMAP
+from splight_lib.restclient import SplightRestClient
+from typing_extensions import TypedDict
 
 logger = get_splight_logger()
 
-REQUEST_EXCEPTIONS = (ConnectionError, Timeout)
+
+class PaginatedResponse(TypedDict):
+    count: int
+    next: Optional[str]
+    previous: Optional[str]
+    results: List[Any]
 
 
-class DatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
+class RemoteDatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
     """Splight API Database Client.
     Responsible for interacting with database resources using HTTP requests
     to the Splight API.
     """
 
-    def __init__(self, namespace: str = "default"):
-        super(DatabaseClient, self).__init__(namespace=namespace)
-        self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
+    def __init__(
+        self,
+        base_url: str,
+        access_id: str,
+        secret_key: str,
+        *args,
+        **kwargs,
+    ):
+        super().__init__()
+        self._base_url = furl(base_url)
         token = SplightAuthToken(
-            access_key=settings.SPLIGHT_ACCESS_ID,
-            secret_key=settings.SPLIGHT_SECRET_KEY,
+            access_key=access_id,
+            secret_key=secret_key,
+        )
+        self._restclient = SplightRestClient()
+        self._restclient.update_headers(token.header)
+        logger.debug(
+            "Remote database client initialized.", tags=LogTags.DATABASE
         )
-        self._session = Session()
-        self._session.headers.update(token.header)
-        logger.info("Database client initialized.", tags=LogTags.DATABASE)
-
-    @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
-    def save(self, instance: BaseModel) -> BaseModel:
-        """Creates or updates a new resource depending on the model if
+
+    @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
+    def save(self, resource_name: str, instance: Dict) -> Dict:
+        """Creates or updates a resource depending on the name if
         it contains the id or not.
 
         Parameters
         ----------
-        instance : BaseModel
-            The instance of the model to be created or updated
+        resource_name: str
+            The name of the resource to be created or updated.
+        instance : Dict
+            A dictionary with resource to be created or updated
 
         Returns
         -------
-        BaseModel with the created or updated resource.
+        Dict with the created or updated resource.
 
         Raises
         ------
-        InvalidModel thrown when the model name is not correct.
+        InvalidModelName thrown when the model name is not correct.
         """
-        logger.debug("Saving instance %s.", instance.id, tags=LogTags.DATABASE)
-
-        constructor = type(instance)
-        model_data = self._get_model_data(constructor)
-
-        path = model_data["path"]
-        if instance.id:
-            output = self._update(path, instance.id, instance)
+        if instance.get("id"):
+            output = self._update(resource_name, instance["id"], instance)
         else:
-            output = self._create(path, instance)
-            instance.id = output["id"]
-        return constructor.parse_obj(output)
+            output = self._create(resource_name, instance)
+        return output
 
-    @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
-    def delete(self, resource_type: Type, id: str):
+    @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
+    def delete(self, resource_name: str, id: str):
         """Deletes a resource from the database
 
         Parameters
         ----------
-        resource_type : Type
-            The resource type to be deleted
+        resource_name : str
+            The resource name
         id : str
             The resource's id.
 
         Raises
         ------
-        InvalidModel thrown when the model name is not correct.
+        InvalidModelName thrown when the model name is not correct.
         """
         logger.debug("Deleting instance %s.", id, tags=LogTags.DATABASE)
-        model_data = self._get_model_data(resource_type)
-        path = model_data["path"]
-        url = self._base_url / f"{path}/{id}/"
-        response = self._session.delete(url)
+        api_path = self._get_api_path(resource_name)
+        url = self._base_url / api_path / f"{id}/"
+        response = self._restclient.delete(url)
         response.raise_for_status()
 
-    @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
+    @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
     def _get(
         self,
-        resource_type: Type,
+        resource_name: str,
         first: bool = False,
-        limit_: int = -1,
-        skip_: int = 0,
-        page_size: int = -1,
-        deleted: bool = False,
         **kwargs,
-    ) -> List[BaseModel]:
-        model_data = self._get_model_data(resource_type)
-        path = model_data["path"]
-        response = self._list(
-            path,
-            limit_=limit_,
-            skip_=skip_,
-            deleted=deleted,
-            page_size=page_size,
-            **kwargs,
-        )
-        parsed = [
-            resource_type.parse_obj(resource)
-            for resource in response["results"]
-        ]
-        if first:
-            return parsed[0] if parsed else None
-        return parsed
-
-    @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
-    def count(self, resource_type: Type, **kwargs) -> int:
-        """Returns the number of resources in the database for a given model
+    ) -> Union[Dict, List[Dict]]:
+        """Retrieves one or multiple resources. If the parameter id is passed
+        as a kwarg, the instance with that id will be retrieved.
 
         Parameters
         ----------
-        resource_type : str
-            The model name
+        resource_name : str
+            The name of the resource.
+        first: bool
+            Whether to retrieve first element or not.
 
         Returns
         -------
-        int
-
-        Raises
-        ------
-        InvalidModel thrown when the model name is not correct.
+        Union[Dict, List[Dict]] list of resource or single resource.
         """
+        if kwargs.get("id"):
+            instances = self._retrieve_single(resource_name, id=kwargs["id"])
+        else:
+            instances = self._retrieve_multiple(
+                resource_name, first=first, **kwargs
+            )
+        return instances
 
-        model_data = self._get_model_data(resource_type)
-        path = model_data["path"]
-        kwargs["page"] = 1  # Always start from the first page
-        response = self._list(path, **kwargs)
-        logger.debug(
-            "Counted %s objects of type: %s.",
-            response["count"],
-            resource_type,
-            tags=LogTags.DATABASE,
-        )
-        return response["count"]
+    def operate(self, resource_name: str, instance: Dict) -> Dict:
+        model_name = resource_name.lower()
+        api_path = CUSTOM_PATHS_MAP.get(model_name)
+        if not api_path:
+            raise InvalidModelName(model_name)
+        api_path = api_path.format_map({"prefix": ENGINE_PREFIX, **instance})
+        url = self._base_url / api_path
+        response = self._restclient.post(url, json=instance)
+        response.raise_for_status()
+        return response.json()
+
+    def _retrieve_multiple(
+        self, resource_name: str, first: bool = False, **kwargs
+    ) -> List[Dict]:
+        api_path = self._get_api_path(resource_name)
+        url = self._base_url / api_path
+        instances = []
+        for page in self._pages(url, page=1, **kwargs):
+            instances.extend(page["results"])
+
+        if first:
+            return [instances[0]] if instances else []
+        return instances
+
+    @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
+    def _retrieve_single(self, resource_name: str, id: str) -> Dict:
+        api_path = self._get_api_path(resource_name)
+        url = self._base_url / api_path / f"{id}/"
+        response = self._restclient.get(url)
+        if response.status_code == codes.NOT_FOUND:
+            raise InstanceNotFound(resource_name, id)
+        else:
+            response.raise_for_status()
+        return response.json()
 
-    @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
+    @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
     def download(
-        self, instance: BaseModel, decrypt: bool = True, **kwargs
+        self,
+        resource_name: str,
+        instance: Dict,
+        decrypt: bool = True,
+        **kwargs,
     ) -> NamedTemporaryFile:
         """Returns the number of resources in the database for a given model
 
         Parameters
         ----------
         instance : BaseModel
             The instance of the model to be downloaded
@@ -166,70 +187,81 @@
         Returns
         -------
         TemporaryFile
             the file object
 
         Raises
         ------
-        InvalidModel thrown when the model name is not correct.
+        InvalidModelName thrown when the model name is not correct.
         """
-        constructor = type(instance)
-        model_data = self._get_model_data(constructor)
-        path = model_data["path"]
-        url = self._base_url / f"{path}/{instance.id}/download"
-        response = self._session.get(url)
+        api_path = self._get_api_path(resource_name)
+        resource_id = instance.get("id")
+        url = self._base_url / api_path / f"{resource_id}/download/"
+        response = self._restclient.get(url)
         response.raise_for_status()
         f = NamedTemporaryFile("wb+")
         f.write(response.content)
         f.seek(0)
         if decrypt and instance.encrypted:
             encryption_manager = EncryptionClient()
             encryption_manager.decrypt_file(path=f.name)
         logger.debug("Downloaded instance %s.", id, tags=LogTags.DATABASE)
         return f
 
-    def _pages(self, path: str, **kwargs):
+    def _pages(
+        self, url: furl, **kwargs
+    ) -> Generator[PaginatedResponse, None, None]:
         next_page = kwargs["page"]
         while next_page:
-            response = self._list(path, **kwargs)
+            response = self._list(url, **kwargs)
             yield response
             next_page = (
                 response["next"].split("page=")[1]
                 if response["next"]
                 else None
             )
             kwargs["page"] = next_page
 
-    def _list(self, path: str, **kwargs):
-        url = self._base_url / f"{path}/"
+    def _list(self, url: furl, **kwargs) -> PaginatedResponse:
         params = self._parse_params(**kwargs)
-        response = self._session.get(url, params=params)
+        response = self._restclient.get(url, params=params)
         response.raise_for_status()
         return response.json()
 
-    @staticmethod
-    def _get_model_data(constructor: Type):
-        model_data = CLASSMAP.get(constructor)
-        if not model_data:
-            raise InvalidModel(constructor.schema()["title"])
-        return model_data
-
-    def _create(self, path: str, instance: BaseModel) -> Dict:
-        url = self._base_url / f"{path}/"
-        data = json.loads(instance.json(exclude_none=True))
-        if isinstance(instance, File):
-            with open(instance.file, "rb") as f:
+    def _create(self, resource_name: str, instance: Dict) -> Dict:
+        logger.debug("Saving new instance", tags=LogTags.DATABASE)
+        model_name = resource_name.lower()
+        api_path = self._get_api_path(resource_name)
+        url = self._base_url / api_path
+        if model_name == "file":
+            with open(instance["file"], "rb") as f:
                 file = {"file": f}
-                response = self._session.post(url, data=data, files=file)
+                response = self._restclient.post(
+                    url, data=instance, files=file
+                )
         else:
-            response = self._session.post(url, json=data)
+            response = self._restclient.post(url, json=instance)
 
         response.raise_for_status()
-        return response.json()
-
-    def _update(self, path: str, resource_id: str, data: BaseModel) -> Dict:
-        url = self._base_url / f"{path}/{resource_id}/"
-        response = self._session.put(
-            url, json=json.loads(data.json(exclude_none=True))
+        instance = response.json()
+        logger.debug(
+            "Instance %s created", instance["id"], tags=LogTags.DATABASE
         )
+        return instance
+
+    def _update(
+        self, resource_name: str, resource_id: str, instance: Dict
+    ) -> Dict:
+        logger.debug("Saving instance %s", resource_id, tags=LogTags.DATABASE)
+        api_path = self._get_api_path(resource_name)
+        url = self._base_url / api_path / f"{resource_id}/"
+        response = self._restclient.put(url, json=instance)
         response.raise_for_status()
         return response.json()
+
+    @staticmethod
+    def _get_api_path(resource_name: str) -> str:
+        model_name = resource_name.lower()
+        api_path = MODEL_NAME_MAP.get(model_name)
+        if not api_path:
+            raise InvalidModelName(model_name)
+        return api_path
```

### Comparing `splight-lib-2.3.9/remote_splight_lib/hub/client.py` & `splight-lib-3.0.0.dev1/splight_lib/client/hub/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Dict, List, Optional, Tuple, Type
 
 import requests
 from furl import furl
 from pydantic import BaseModel
-from remote_splight_lib.auth import SplightAuthToken
-from remote_splight_lib.settings import settings
-from splight_abstract import (
+from splight_lib.auth import SplightAuthToken
+from splight_lib.client.hub.abstract import (
     AbstractHubClient,
     AbstractHubSubClient,
     validate_client_resource_type,
 )
-from splight_models import HubComponent, HubComponentVersion
+from splight_lib.models.hub import HubComponent, HubComponentVersion
+from splight_lib.settings import settings
 
 
 class _SplightHubGenericClient(AbstractHubSubClient):
     _PREFIX: str = "v2/hub"
     valid_classes = [
         HubComponent,
         HubComponentVersion,
@@ -126,23 +126,23 @@
         response = self._session.post(url, headers=self.headers)
         assert (
             response.status_code == 204
         ), f"Failed to rebuild component. {response.content}"
 
 
 class SplightHubClient(AbstractHubClient):
-    def __init__(
-        self, headers: Optional[Dict[str, str]] = {}, *args, **kwargs
-    ) -> None:
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__()
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
-        self._all = _SplightHubGenericClient(base_path="all", headers=headers)
+        self._all = _SplightHubGenericClient(
+            base_path="all", headers=token.header
+        )
         self._mine = _SplightHubGenericClient(
             base_path="mine", headers=token.header
         )
         self._public = _SplightHubGenericClient(
             base_path="public", headers=token.header
         )
         self._private = _SplightHubGenericClient(
@@ -166,21 +166,14 @@
     def download(self, data: Dict) -> Tuple:
         url = self._host / "v2/hub/download/"
         response = requests.post(url, data=data, headers=self._headers)
         status_code = response.status_code
         assert status_code == 200, "Unable to download component"
         return response.content, status_code
 
-    def random_picture(self) -> Tuple:
-        url = self._host / "hub/random_picture/"
-        response = requests.get(url, headers=self._headers)
-        status_code = response.status_code
-        assert status_code == 200, "Unable to retrieve random picture"
-        return response.content, status_code
-
     @property
     def all(self) -> AbstractHubSubClient:
         return self._all
 
     @property
     def mine(self) -> AbstractHubSubClient:
         return self._mine
```

### Comparing `splight-lib-2.3.9/setup.py` & `splight-lib-3.0.0.dev1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="2.3.9",
+    version="3.0.0.dev1",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-2.3.9/splight_abstract/database/abstract.py` & `splight-lib-3.0.0.dev1/splight_lib/client/database/abstract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,28 @@
 from abc import abstractmethod
 from tempfile import NamedTemporaryFile
-from typing import List, Type
+from typing import Dict, List, Union
 
-from pydantic import BaseModel
-from splight_abstract.client import AbstractClient, QuerySet
+from splight_lib.abstract.client import AbstractClient, QuerySet
 
 
 class AbstractDatabaseClient(AbstractClient):
     @abstractmethod
-    def save(self, instance: BaseModel) -> BaseModel:
+    def save(self, resource_name: str, instance: Dict) -> Dict:
         pass
 
     @abstractmethod
     def _get(
-        self,
-        resource_type: Type,
-        first: bool = False,
-        limit_: int = -1,
-        skip_: int = 0,
-        deleted: bool = False,
-        **kwargs
-    ) -> List[BaseModel]:
+        self, resource_name: str, first: bool = False, **kwargs
+    ) -> Union[Dict, List[Dict]]:
         pass
 
-    def get(self, resource_type: Type, *args, **kwargs) -> QuerySet:
-        return QuerySet(self, resource_type, *args, **kwargs)
+    def get(self, resource_name: str, *args, **kwargs) -> QuerySet:
+        return QuerySet(self, resource_name, *args, **kwargs)
 
     @abstractmethod
-    def delete(self, resource_type: Type, id: str) -> None:
+    def delete(self, resource_name: str, id: str) -> None:
         pass
 
     @abstractmethod
-    def count(self, resource_type: Type, **kwargs) -> int:
-        pass
-
-    @abstractmethod
-    def download(self, instance: BaseModel) -> NamedTemporaryFile:
+    def download(self, instance: Dict) -> NamedTemporaryFile:
         pass
```

### Comparing `splight-lib-2.3.9/splight_abstract/storage/abstract.py` & `splight-lib-3.0.0.dev1/splight_lib/client/communication/abstract.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-from abc import abstractmethod
-from typing import List, Optional, Type
+from abc import abstractmethod, abstractproperty
+from typing import Callable, Dict
 
-from pydantic import BaseModel
-from splight_abstract.client import AbstractClient, QuerySet
+from splight_lib.abstract.client import AbstractClient
+from splight_lib.models.communication import CommunicationContext
+from splight_lib.models.event import CommunicationEvent
 
 
-class AbstractStorageClient(AbstractClient):
-    @abstractmethod
-    def save(self, instance: BaseModel) -> BaseModel:
-        pass
+class AbstractCommunicationClient(AbstractClient):
+    def __init__(self, instance_id: str = None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.instance_id = instance_id
 
-    def get(self, *args, **kwargs) -> QuerySet:
-        kwargs["get_func"] = "_get"
-        kwargs["count_func"] = "None"
-        return QuerySet(self, *args, **kwargs)
+    @abstractproperty
+    def context(self) -> CommunicationContext:
+        pass
 
-    @abstractmethod
-    def _get(
-        self,
-        resource_type: Type,
-        first=False,
-        prefix: Optional[str] = None,
-        limit_: int = -1,
-        skip_: int = 0,
-        **kwargs
-    ) -> List[BaseModel]:
+    @abstractproperty
+    def status(self):
         pass
 
     @abstractmethod
-    def copy(self, old_name: str, new_name: str):
+    def bind(self, event_name: str, event_handler: Callable) -> None:
         pass
 
     @abstractmethod
-    def delete(self, resource_type: Type, id: str) -> None:
+    def unbind(self, event_name: str, event_handler: Callable) -> None:
         pass
 
     @abstractmethod
-    def download(self, resource_type: Type, id: str, target: str) -> str:
+    def trigger(self, event: CommunicationEvent):
         pass
 
     @abstractmethod
-    def get_temporary_link(self, filename: str, target: str) -> str:
+    def authenticate(
+        self, channel_name: str, socket_id: str, custom_data: Dict = None
+    ) -> dict:
         pass
```

### Comparing `splight-lib-2.3.9/splight_lib/auth/mac_auth.py` & `splight-lib-3.0.0.dev1/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/client/datalake/local_client.py` & `splight-lib-3.0.0.dev1/splight_lib/client/datalake/local_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,194 +1,162 @@
 import json
 import os
 from datetime import timedelta, timezone
 from functools import partial
-from typing import Dict, List, Type, Union
+from typing import Dict, List, Optional, Union
 
 import pandas as pd
-from splight_abstract.client import QuerySet
-from splight_abstract.datalake import AbstractDatalakeClient
+from splight_lib.client.datalake.abstract import AbstractDatalakeClient
 from splight_lib.client.file_handler import FixedLineNumberFileHandler
 from splight_lib.client.filter import value_filter
 from splight_lib.logging._internal import LogTags, get_splight_logger
-from splight_models import DatalakeModel, Query
-
-DLResource = Type[DatalakeModel]
 
 logger = get_splight_logger()
 
 
 class LocalDatalakeClient(AbstractDatalakeClient):
     """Datalake client implementation for a storing locally documents
     in different files.
     """
 
     _DEFAULT = "default"
-    _PREFIX = "dl_"
+    _PREFIX = "splight-dl_"
     _TOTAL_DOCS = 10000
 
-    def __init__(self, namespace: str, path: str):
-        super().__init__(namespace=namespace)
+    def __init__(self, path: str, *args, **kwargs):
+        super().__init__()
         self._base_path = path
         logger.info(
             "Local datalake client initialized.", tags=LogTags.DATALAKE
         )
 
+    def save(
+        self,
+        collection: str,
+        instances: Union[List[Dict], Dict],
+    ) -> List[Dict]:
+        instances = instances if isinstance(instances, list) else [instances]
+
+        logger.debug("Saving instances %s.", instances, tags=LogTags.DATALAKE)
+        instances = [json.dumps(instance) for instance in instances]
+
+        file_path = os.path.join(
+            self._base_path, self._get_file_name(collection)
+        )
+        handler = FixedLineNumberFileHandler(
+            file_path=file_path, total_lines=self._TOTAL_DOCS
+        )
+        handler.write(instances)
+        return instances
+
     def _raw_get(
         self,
-        resource_type: DLResource,
+        resource_name: str,
+        collection: str,
         limit_: int = 1000,
         skip_: int = 0,
         sort: Union[List, str] = ["timestamp__desc"],
-        group_id: Union[List, str] = [],
-        group_fields: Union[List, str] = [],
+        group_id: Optional[Union[List, str]] = None,
+        group_fields: Optional[Union[List, str]] = None,
         tzinfo: timezone = timezone(timedelta()),
-        **kwargs,
-    ) -> List[DLResource]:
-        collection = resource_type.Meta.collection_name
+        **filters,
+    ) -> List[Dict]:
+        filters.update(
+            {
+                "output_format": resource_name,
+            }
+        )
+        filters = self._parse_filters(filters)
+
         file_path = os.path.join(
             self._base_path, self._get_file_name(collection)
         )
         handler = FixedLineNumberFileHandler(
             file_path=file_path, total_lines=self._TOTAL_DOCS
         )
-        documents = [json.loads(doc) for doc in handler.read()]
-
-        filters = kwargs
-        filters.update({"output_format": resource_type.__name__})
+        documents = [
+            json.loads(doc) for doc in handler.read()[skip_ : skip_ + limit_]
+        ]
         documents = self._filter(documents, filters=filters)
 
         reverse = False
         if "__desc" not in sort:
             reverse = True
         documents.sort(key=lambda x: x["timestamp"], reverse=reverse)
 
-        # TODO: review how to apply grouping
-        return [
-            resource_type.parse_obj(doc)
-            for doc in documents[skip_ : limit_ + 1]
-        ]
+        return documents
 
-    def get(
+    def get_dataframe(
         self,
-        resource_type: Type,
-        limit_: int = 50,
-        skip_: int = 0,
+        resource_name: str,
+        collection: str,
         sort: Union[List, str] = ["timestamp__desc"],
-        group_id: Union[List, str] = [],
-        group_fields: Union[List, str] = [],
+        group_id: Optional[Union[List, str]] = None,
+        group_fields: Optional[Union[List, str]] = None,
         tzinfo: timezone = timezone(timedelta()),
-        **kwargs,
-    ) -> QuerySet:
-        logger.debug(
-            "Retrieving object of type %s from datalake.",
-            resource_type,
-            tags=LogTags.DATALAKE,
-        )
-
-        kwargs["get_func"] = "_raw_get"
-        kwargs["count_func"] = "None"
-        kwargs["collection"] = resource_type.Meta.collection_name
-        kwargs["resource_type"] = resource_type
-        return QuerySet(
-            self,
-            limit_,
-            skip_,
-            sort,
-            group_id,
-            group_fields,
-            tzinfo,
-            **kwargs,
-        )
-
-    def get_output(self, query: Query) -> List[Dict]:
-        raise NotImplementedError()
-
-    def get_dataframe(
-        self, resource_type: Type, freq: str = "H", **kwargs
+        **filters,
     ) -> pd.DataFrame:
-        """Reads documents and returns a dataframe"""
         logger.debug(
             "Retrieving dataframe from datalake.", tags=LogTags.DATALAKE
         )
-        documents = self._raw_get(resource_type, **kwargs)
-        df = pd.DataFrame([x.dict() for x in documents])
-        if not df.empty:
-            df.set_index("timestamp", inplace=True, verify_integrity=False)
-        return df
 
-    def get_dataset(self, queries: List[Query]) -> pd.DataFrame:
-        raise NotImplementedError()
-
-    def save(self, instances: List[DatalakeModel]) -> List[DatalakeModel]:
-        documents = [instance.json() for instance in instances]
-        if not instances:
-            return instances
+        filters.update(
+            {
+                "resource_name": resource_name,
+                "collection": collection,
+                "sort": sort,
+                "group_id": group_id,
+                "group_fields": group_fields,
+                "tzinfo": tzinfo,
+            }
+        )
 
-        logger.debug("Saving instances %s.", instances, tags=LogTags.DATALAKE)
+        documents = self._raw_get(**filters)
+        df = pd.DataFrarame([x.dict() for x in documents])
 
-        collection = instances[0].Meta.collection_name
+        if not df.empty:
+            df["timestamp"] = pd.to_datetime(df["timestamp"])
+            df.set_index("timestamp", inplace=True, verify_integrity=False)
 
-        file_path = os.path.join(
-            self._base_path, self._get_file_name(collection)
-        )
-        handler = FixedLineNumberFileHandler(
-            file_path=file_path, total_lines=self._TOTAL_DOCS
-        )
-        handler.write(documents)
-        return instances
+        return df
 
-    def save_dataframe(
-        self, resource_type: DLResource, dataframe: pd.DataFrame
-    ) -> None:
+    def save_dataframe(self, collection: str, dataframe: pd.DataFrame) -> None:
         logger.debug("Saving dataframe.", tags=LogTags.DATALAKE)
 
-        instances = dataframe.apply(
-            lambda x: resource_type.parse_obj(x.to_dict()), axis=1
-        )
-        instances = instances.to_list()
-        _ = self.save(instances)
+        dataframe["timestamp"] = dataframe["timestamp"].astype(str)
+        instances = list(dataframe.to_dict("index").values())
+        _ = self.save(collection, instances)
 
-    def delete(self, resource_type: DLResource, **kwargs) -> None:
+    def delete(self, collection: str, **kwargs) -> None:
         logger.debug(
-            "Deleting resources of type %s from datalake.",
-            resource_type,
-            tags=LogTags.DATALAKE,
+            "Skipping deleting objects when using Local datalake client."
         )
-        collection = resource_type.Meta.collection_name
-        file_path = os.path.join(
-            self._base_path, self._get_file_name(collection)
-        )
-        handler = FixedLineNumberFileHandler(
-            file_path=file_path, total_lines=self._TOTAL_DOCS
-        )
-        documents = [json.loads(doc) for doc in handler.read()]
-        id = kwargs.get("instance_id")
-        if id:
-            documents = [d for d in documents if d["instance_id"] != id]
-        # jsonify python dicts
-        documents = [json.loads(json.dumps(d)) for d in documents]
-        handler.write(documents, override=True)
 
     def create_index(self, collection: str, index: list) -> None:
         logger.debug(
             "Skipping index creation when using Local datalake client."
         )
 
     def raw_aggregate(
         self, collection: str, pipeline: List[Dict]
     ) -> List[Dict]:
         logger.debug(
             "Skipping raw aggregation when using Local datalake client."
         )
 
-    def _filter(
-        self, instances: List[DLResource], filters: Dict
-    ) -> List[DLResource]:
+    def _filter(self, instances: List[dict], filters: Dict) -> List[dict]:
         filtered = instances
         for key, value in filters.items():
             filtered = filter(partial(value_filter, key, value), filtered)
             filtered = list(filtered)
         return filtered
 
+    def _parse_filters(self, filters: List[dict]):
+        new_filters = {}
+        for key, value in filters.items():
+            if value is None:
+                continue
+            new_filters[key] = value
+        return new_filters
+
     def _get_file_name(self, collection: str) -> str:
         return f"{self._PREFIX}{collection}"
```

### Comparing `splight-lib-2.3.9/splight_lib/client/exceptions.py` & `splight-lib-3.0.0.dev1/splight_lib/client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from splight_lib.restclient import ConnectError, HTTPError
 from splight_lib.restclient import Timeout as TimeoutError
 
 REQUEST_EXCEPTIONS = (ConnectionError, Timeout)
 SPLIGHT_REQUEST_EXCEPTIONS = (HTTPError, TimeoutError, ConnectError)
 
 
-class InvalidModel(Exception):
+class InvalidModelName(Exception):
     def __init__(self, model_name: str):
         self._msg = f"Model {model_name} is not a valid database model"
 
     def __str__(self) -> str:
         return self._msg
```

### Comparing `splight-lib-2.3.9/splight_lib/client/file_handler.py` & `splight-lib-3.0.0.dev1/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/client/filter.py` & `splight-lib-3.0.0.dev1/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/encryption.py` & `splight-lib-3.0.0.dev1/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/execution.py` & `splight-lib-3.0.0.dev1/splight_lib/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uuid
 from functools import wraps
 from subprocess import Popen as DefaultPopen
 from threading import Event, Lock
 from threading import Thread as DefaultThread
 from typing import Any, Callable, List, Tuple, Union
 
-from splight_abstract.client.abstract import AbstractClient
+from splight_lib.abstract.client import AbstractClient
 from splight_lib.logging._internal import LogTags, get_splight_logger
 
 logger = get_splight_logger()
 
 
 class Empty(object):
     pass
```

### Comparing `splight-lib-2.3.9/splight_lib/logging/_internal.py` & `splight-lib-3.0.0.dev1/splight_lib/logging/_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     SplightFormatter,
     SplightLogger,
     standard_output_handler,
 )
 from strenum import UppercaseStrEnum
 
 
-
 # TODO: add more tags
 class LogTags(UppercaseStrEnum):
     RUNTIME = auto()
     BINDING = auto()
     COMMUNICATION = auto()
     INDEX = auto()
     SECRET = auto()
```

### Comparing `splight-lib-2.3.9/splight_lib/logging/component.py` & `splight-lib-3.0.0.dev1/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/logging/logging.py` & `splight-lib-3.0.0.dev1/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/restclient/client.py` & `splight-lib-3.0.0.dev1/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/restclient/exceptions.py` & `splight-lib-3.0.0.dev1/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/restclient/types.py` & `splight-lib-3.0.0.dev1/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib/webhook.py` & `splight-lib-3.0.0.dev1/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.9/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.0.0.dev1/splight_lib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.3.9
+Version: 3.0.0.dev1
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-2.3.9/splight_models/communication/context.py` & `splight-lib-3.0.0.dev1/splight_lib/models/communication.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from enum import Enum
 from typing import Dict, Optional
 
-from splight_models import SplightBaseModel
-from splight_models.user import User
+from pydantic import BaseModel
 
 
-class CommunicationChannelData(SplightBaseModel):
+class CommunicationChannelData(BaseModel):
     user_id: str
     user_info: Dict
 
-    @classmethod
-    def parse_from_user(cls, user: User):
-        return cls.parse_obj(
-            {"user_id": user.user_id, "user_info": user.dict()}
-        )
+    # TODO: Review following method
+    # @classmethod
+    # def parse_from_user(cls, user: User):
+    #     return cls.parse_obj(
+    #         {"user_id": user.user_id, "user_info": user.dict()}
+    #     )
 
 
-class CommunicationContext(SplightBaseModel):
+class CommunicationContext(BaseModel):
     auth_headers: Optional[Dict] = None
     auth_endpoint: Optional[str] = None
     key: str
     channel: str
     private_room_channel: str
     presence_room_channel: str
     channel_data: Optional[CommunicationChannelData] = None
```

### Comparing `splight-lib-2.3.9/splight_models/datalake.py` & `splight-lib-3.0.0.dev1/splight_lib/models/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-from datetime import datetime, timezone
-from typing import Optional
-
-from pydantic import Field
-from splight_models.base import SplightBaseModel
-
-
-class DatalakeModel(SplightBaseModel):
-    timestamp: datetime = Field(
-        default_factory=lambda: datetime.now(timezone.utc)
-    )
-    instance_id: Optional[str] = None
-    instance_type: Optional[str] = None
-
-    class Config:
-        # pydantic
-        validate_assignment = True
-
-    class Meta:
-        collection_name = "DatalakeModel"
-
-    class SpecFields:
-        # Fields to reconstruct Spec .fields
-        pass
+import json
+import os
+from typing import Dict, Optional
+
+from pydantic import validator
+from splight_lib.models.base import SplightDatabaseBaseModel
+
+
+class File(SplightDatabaseBaseModel):
+    id: Optional[str] = None
+    file: str
+    description: Optional[str] = None
+    metadata: Dict = {}
+    content_type: Optional[str] = None
+    url: Optional[str] = None
+    encrypted: Optional[bool] = False
+
+    @validator("file", pre=True)
+    def validate_file(cls, v):
+        v = v.replace("/", os.sep)
+        v = v.replace("\\", os.sep)
+        return v
+
+    @property
+    def name(self):
+        return self.file.split(os.sep)[-1]
+
+    def download(self):
+        file = self._db_client.download(
+            resource_name=self.__class__.__name__,
+            instance=self.dict(),
+            decrypt=self.encrypted,
+        )
+        return file
 
     def dict(self, *args, **kwargs):
-        d = super().dict(*args, **kwargs)
-        return {
-            k: v["id"] if isinstance(v, dict) and "id" in v.keys() else v
-            for k, v in d.items()
-        }
+        res = super().dict(*args, **kwargs)
+        res["metadata"] = json.dumps(self.metadata)
+        return res
 
     def json(self, *args, **kwargs):
-        restore = {}
-
-        for k in self.__class__.__fields__.keys():
-            v = getattr(self, k)
-            if hasattr(v, "id"):
-                restore[k] = v.id
-                setattr(self, k, v.id)
-
+        prev_metadata = self.metadata
+        self.metadata = json.dumps(self.metadata)
         res = super().json(*args, **kwargs)
-
-        for k, v in restore.items():
-            setattr(self, k, v)
-
+        self.metadata = prev_metadata
         return res
```

### Comparing `splight-lib-2.3.9/splight_models/hub.py` & `splight-lib-3.0.0.dev1/splight_lib/models/hub.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import List, Optional
 
-from pydantic import validator
-from splight_models.component import BaseComponent
+from pydantic import BaseModel, validator
 
 VERIFICATION_CHOICES = ["verified", "unverified", "official"]
 
 
-class HubComponent(BaseComponent):
+class HubComponent(BaseModel):
     id: Optional[str]
     name: str
     splight_cli_version: str
     build_status: Optional[str]
     description: Optional[str]
     privacy_policy: Optional[str] = None
     component_type: Optional[str] = None
```

### Comparing `splight-lib-2.3.9/splight_models/query.py` & `splight-lib-3.0.0.dev1/splight_lib/models/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 from pydantic import validator
-from splight_models.base import SplightBaseModel
+from splight_lib.models.base import SplightDatabaseBaseModel
 
 
 class QuerySourceType(str, Enum):
     NATIVE = "Native"
     COMPONENT = "Component"
 
 
-class Query(SplightBaseModel):
+class Query(SplightDatabaseBaseModel):
     id: Optional[str]
     name: str
     description: Optional[str]
     source_type: QuerySourceType
     source_component_id: Optional[str] = None
     output_format: str
     target: str
@@ -76,13 +76,13 @@
             )
             query_params += f"&{joined_filters}"
         if self.output_format:
             query_params += f"&output_format={self.output_format}"
         query_params_fields = ["limit", "skip", "sort"]
         underscored_fields = ["limit", "skip"]
         for k in query_params_fields:
-            field = k if not k in underscored_fields else k + "_"
+            field = k if k not in underscored_fields else k + "_"
             if type(getattr(self, k)) == list:
                 query_params += f"&{field}={','.join(getattr(self, k))}"
             else:
                 query_params += f"&{field}={getattr(self, k)}"
         return query_params
```

### Comparing `splight-lib-2.3.9/splight_models/setpoint.py` & `splight-lib-3.0.0.dev1/splight_lib/models/setpoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime
 from enum import auto
 from typing import List, Optional, Union
 
-from pydantic import Field, ValidationError, validator
-from splight_models import CommunicationEvent, EventNames
+from pydantic import BaseModel, ValidationError, validator
+from splight_lib.models.asset import Asset
+from splight_lib.models.attribute import Attribute
+from splight_lib.models.base import SplightDatabaseBaseModel
 from strenum import LowercaseStrEnum, PascalCaseStrEnum
 
-from .base import SplightBaseModel
-
 
 class SetPointType(PascalCaseStrEnum):
     Number = auto()
     String = auto()
     Boolean = auto()
 
     def __str__(self):
@@ -23,51 +23,45 @@
     ERROR = auto()
     IGNORE = auto()
 
     def __str__(self):
         return self.value
 
 
-class SetPointResponse(SplightBaseModel):
+class SetPointResponse(BaseModel):
     id: Optional[str]
     component: str
     status: SetPointResponseStatus
     created_at: Optional[datetime] = None
 
 
-class SetPoint(SplightBaseModel):
+class SetPoint(SplightDatabaseBaseModel):
     id: Optional[str]
-    asset: str
-    attribute: str
+    asset: Asset
+    attribute: Attribute
     type: SetPointType
     value: Union[str, bool, float]
     responses: List[SetPointResponse] = []
 
     @validator("value")
     def cast_value(cls, v, values, **kwargs):
-        if not "type" in values:
+        if "type" not in values:
             raise ValueError("type is required")
 
-        if values["type"] == SetPointType.Number:
-            try:
-                return float(v)
-            except ValueError:
-                raise ValidationError("value must be a number")
-
-        if values["type"] == SetPointType.Boolean:
-            try:
-                return bool(v)
-            except ValueError:
-                raise ValidationError("value must be a boolean")
-
-        if values["type"] == SetPointType.String:
-            return str(v)
-
-
-class SetPointCreateEvent(CommunicationEvent):
-    event_name: str = Field(EventNames.SETPOINT_CREATE, const=True)
-    data: SetPoint
-
-
-class SetPointUpdateEvent(CommunicationEvent):
-    event_name: str = Field(EventNames.SETPOINT_UPDATE, const=True)
-    data: SetPoint
+        mapping_functions = {
+            SetPointType.Number: float,
+            SetPointType.Boolean: bool,
+            SetPointType.String: str,
+        }
+        parse_function = mapping_functions.get(values["type"])
+        try:
+            parsed_value = parse_function(v)
+        except ValueError as exc:
+            raise ValidationError(f"value must be a {str(type)}") from exc
+        return parsed_value
+
+    def save(self):
+        new_value = self.asset.set_attribute(
+            attribute=self.attribute, value=self.value, value_type=self.type
+        )
+        if not self.id:
+            self.id = new_value["id"]
```

