# Comparing `tmp/kynaylibs-1.7.2.tar.gz` & `tmp/kynaylibs-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-1.7.2.tar", last modified: Sun May 21 21:47:33 2023, max compression
+gzip compressed data, was "kynaylibs-1.7.3.tar", last modified: Sun May 21 22:07:59 2023, max compression
```

## Comparing `kynaylibs-1.7.2.tar` & `kynaylibs-1.7.3.tar`

### file list

```diff
@@ -1,511 +1,511 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.508961 kynaylibs-1.7.2/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      290 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2280 2023-05-21 21:47:33.508961 kynaylibs-1.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1175 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.464961 kynaylibs-1.7.2/compiler/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.464961 kynaylibs-1.7.2/compiler/api/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22917 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/api/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.464961 kynaylibs-1.7.2/compiler/api/source/
--rw-r--r--   0 root         (0) root         (0)     2233 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/api/source/auth_key.tl
--rw-r--r--   0 root         (0) root         (0)   157953 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/api/source/main_api.tl
--rw-r--r--   0 root         (0) root         (0)     3425 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.464961 kynaylibs-1.7.2/compiler/api/template/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/api/template/combinator.txt
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/api/template/type.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.464961 kynaylibs-1.7.2/compiler/errors/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/compiler.py
--rw-r--r--   0 root         (0) root         (0)     1263 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.464961 kynaylibs-1.7.2/compiler/errors/source/
--rw-r--r--   0 root         (0) root         (0)      470 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 root         (0) root         (0)    22290 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 root         (0) root         (0)     2000 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 root         (0) root         (0)     1177 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 root         (0) root         (0)      470 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 root         (0) root         (0)     4219 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.464961 kynaylibs-1.7.2/compiler/errors/template/
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/template/class.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.464961 kynaylibs-1.7.2/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2280 2023-05-21 21:47:33.000000 kynaylibs-1.7.2/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19580 2023-05-21 21:47:33.000000 kynaylibs-1.7.2/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 21:47:33.000000 kynaylibs-1.7.2/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 21:47:33.000000 kynaylibs-1.7.2/kynaylibs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-21 21:47:33.000000 kynaylibs-1.7.2/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-21 21:47:33.000000 kynaylibs-1.7.2/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 21:47:33.508961 kynaylibs-1.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2139 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.468961 kynaylibs-1.7.2/ubotlibs/
--rw-r--r--   0 root         (0) root         (0)     2893 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6633 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/assistant.py
--rw-r--r--   0 root         (0) root         (0)    43836 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.468961 kynaylibs-1.7.2/ubotlibs/connection/
--rw-r--r--   0 root         (0) root         (0)      854 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.468961 kynaylibs-1.7.2/ubotlibs/connection/transport/
--rw-r--r--   0 root         (0) root         (0)      838 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/transport/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.468961 kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/
--rw-r--r--   0 root         (0) root         (0)     1044 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4033 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.468961 kynaylibs-1.7.2/ubotlibs/crypto/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4059 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/crypto/aes.py
--rw-r--r--   0 root         (0) root         (0)     4865 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/crypto/mtproto.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/crypto/prime.py
--rw-r--r--   0 root         (0) root         (0)    10829 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/crypto/rsa.py
--rw-r--r--   0 root         (0) root         (0)    10865 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)   209155 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/emoji.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.468961 kynaylibs-1.7.2/ubotlibs/enums/
--rw-r--r--   0 root         (0) root         (0)     1749 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/auto_name.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4203 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/chat_event_action.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/chat_member_status.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/chat_members_filter.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/chat_type.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/message_entity_type.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/message_media_type.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/message_service_type.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/messages_filter.py
--rw-r--r--   0 root         (0) root         (0)     7764 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/msg_types.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/next_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/parse_mode.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/poll_type.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/sent_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1299 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/enums/user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.468961 kynaylibs-1.7.2/ubotlibs/errors/
--rw-r--r--   0 root         (0) root         (0)     2578 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/errors/rpc_error.py
--rw-r--r--   0 root         (0) root         (0)    15602 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/file_id.py
--rw-r--r--   0 root         (0) root         (0)    24704 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.472961 kynaylibs-1.7.2/ubotlibs/handlers/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/callback_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/chat_join_request_handler.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/chat_member_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)     2101 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 root         (0) root         (0)     2528 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/conversation_handler.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/deleted_messages_handler.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/disconnect_handler.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/edited_message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/handler.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/inline_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/poll_handler.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/raw_update_handler.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/handlers/user_status_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.472961 kynaylibs-1.7.2/ubotlibs/kynay/
--rw-r--r--   0 root         (0) root         (0)     1760 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.472961 kynaylibs-1.7.2/ubotlibs/kynay/nan/
--rw-r--r--   0 root         (0) root         (0)     1802 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.472961 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.472961 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)    13339 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/kynay/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.472961 kynaylibs-1.7.2/ubotlibs/methods/
--rw-r--r--   0 root         (0) root         (0)     1320 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.472961 kynaylibs-1.7.2/ubotlibs/methods/advanced/
--rw-r--r--   0 root         (0) root         (0)      974 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/advanced/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/advanced/invoke.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/advanced/resolve_peer.py
--rw-r--r--   0 root         (0) root         (0)     8320 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/advanced/save_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.476961 kynaylibs-1.7.2/ubotlibs/methods/auth/
--rw-r--r--   0 root         (0) root         (0)     1656 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 root         (0) root         (0)     1880 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/check_password.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/connect.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/disconnect.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/get_password_hint.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/log_out.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/recover_password.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/resend_code.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/send_code.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/send_recovery_code.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/sign_in.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/sign_in_bot.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/sign_up.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/auth/terminate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.476961 kynaylibs-1.7.2/ubotlibs/methods/bots/
--rw-r--r--   0 root         (0) root         (0)     2042 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/answer_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     4984 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/answer_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/answer_web_app_query.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/delete_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/get_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     2802 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/get_game_high_scores.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/request_callback_answer.py
--rw-r--r--   0 root         (0) root         (0)     3966 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/send_game.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 root         (0) root         (0)     2690 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/set_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     3264 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/bots/set_game_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.480961 kynaylibs-1.7.2/ubotlibs/methods/chats/
--rw-r--r--   0 root         (0) root         (0)     3440 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/add_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/archive_chats.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/ban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/create_channel.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/create_group.py
--rw-r--r--   0 root         (0) root         (0)     1887 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/create_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/delete_channel.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/delete_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/delete_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/delete_user_history.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat.py
--rw-r--r--   0 root         (0) root         (0)     4014 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_event_log.py
--rw-r--r--   0 root         (0) root         (0)     3206 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     5219 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_members_count.py
--rw-r--r--   0 root         (0) root         (0)     1715 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_online_count.py
--rw-r--r--   0 root         (0) root         (0)     3430 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_dialogs.py
--rw-r--r--   0 root         (0) root         (0)     2203 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_dialogs_count.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_nearby_chats.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/get_send_as_chats.py
--rw-r--r--   0 root         (0) root         (0)     2628 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/join_chat.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/leave_chat.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/mark_chat_unread.py
--rw-r--r--   0 root         (0) root         (0)     3158 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/pin_chat_message.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/promote_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/restrict_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_administrator_title.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_description.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     4523 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_title.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_username.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_send_as_chat.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/set_slow_mode.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/unarchive_chats.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/unban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.480961 kynaylibs-1.7.2/ubotlibs/methods/contacts/
--rw-r--r--   0 root         (0) root         (0)     1138 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/contacts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/contacts/add_contact.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/contacts/delete_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/contacts/get_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/contacts/get_contacts_count.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/contacts/import_contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.480961 kynaylibs-1.7.2/ubotlibs/methods/decorators/
--rw-r--r--   0 root         (0) root         (0)     1625 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2199 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_disconnect.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_edited_message.py
--rw-r--r--   0 root         (0) root         (0)     2176 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_message.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_poll.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_raw_update.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/decorators/on_user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.484961 kynaylibs-1.7.2/ubotlibs/methods/invite_links/
--rw-r--r--   0 root         (0) root         (0)     2436 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2031 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3515 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2546 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     2336 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.488961 kynaylibs-1.7.2/ubotlibs/methods/messages/
--rw-r--r--   0 root         (0) root         (0)     4071 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/copy_media_group.py
--rw-r--r--   0 root         (0) root         (0)     5182 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/copy_message.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/delete_messages.py
--rw-r--r--   0 root         (0) root         (0)     7751 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/download_media.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/edit_inline_caption.py
--rw-r--r--   0 root         (0) root         (0)    10100 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/edit_inline_media.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/edit_inline_text.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/edit_message_caption.py
--rw-r--r--   0 root         (0) root         (0)    12414 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/edit_message_media.py
--rw-r--r--   0 root         (0) root         (0)     3007 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3918 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     4542 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/forward_messages.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/get_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/get_chat_history_count.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/get_discussion_message.py
--rw-r--r--   0 root         (0) root         (0)     2809 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/get_discussion_replies.py
--rw-r--r--   0 root         (0) root         (0)     1951 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/get_media_group.py
--rw-r--r--   0 root         (0) root         (0)     4756 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/get_messages.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/inline_session.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/read_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/retract_vote.py
--rw-r--r--   0 root         (0) root         (0)     4111 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/search_global.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/search_global_count.py
--rw-r--r--   0 root         (0) root         (0)     5292 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/search_messages.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/search_messages_count.py
--rw-r--r--   0 root         (0) root         (0)    12756 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_animation.py
--rw-r--r--   0 root         (0) root         (0)    11465 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_audio.py
--rw-r--r--   0 root         (0) root         (0)     5554 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_cached_media.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_contact.py
--rw-r--r--   0 root         (0) root         (0)     4911 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_dice.py
--rw-r--r--   0 root         (0) root         (0)    10979 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_document.py
--rw-r--r--   0 root         (0) root         (0)     4576 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_location.py
--rw-r--r--   0 root         (0) root         (0)    20353 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_media_group.py
--rw-r--r--   0 root         (0) root         (0)     7292 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_message.py
--rw-r--r--   0 root         (0) root         (0)     9509 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_photo.py
--rw-r--r--   0 root         (0) root         (0)     8213 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_poll.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_reaction.py
--rw-r--r--   0 root         (0) root         (0)     8714 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_sticker.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_venue.py
--rw-r--r--   0 root         (0) root         (0)    12192 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_video.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_video_note.py
--rw-r--r--   0 root         (0) root         (0)     9643 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/send_voice.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/stop_poll.py
--rw-r--r--   0 root         (0) root         (0)     4068 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/stream_media.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/vote_poll.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/wait_for_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2659 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/messages/wait_for_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.488961 kynaylibs-1.7.2/ubotlibs/methods/password/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/password/change_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/password/enable_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.488961 kynaylibs-1.7.2/ubotlibs/methods/users/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/block_user.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/delete_profile_photos.py
--rw-r--r--   0 root         (0) root         (0)     4409 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/get_chat_photos.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/get_chat_photos_count.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/get_common_chats.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/get_me.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/get_users.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/set_emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     2698 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/set_profile_photo.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/set_username.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/unblock_user.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/users/update_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.488961 kynaylibs-1.7.2/ubotlibs/methods/utilities/
--rw-r--r--   0 root         (0) root         (0)     1254 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2316 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/add_handler.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/compose.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/export_session_string.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/idle.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/remove_handler.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/restart.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/run.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/start.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/stop.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/methods/utilities/stop_transmission.py
--rw-r--r--   0 root         (0) root         (0)    61915 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/mime_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.488961 kynaylibs-1.7.2/ubotlibs/parser/
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7567 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/parser/html.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/parser/markdown.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/parser/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.488961 kynaylibs-1.7.2/ubotlibs/raw/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.492961 kynaylibs-1.7.2/ubotlibs/raw/core/
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/future_salt.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/future_salts.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/gzip_packed.py
--rw-r--r--   0 root         (0) root         (0)     1090 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/list.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/message.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/msg_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.492961 kynaylibs-1.7.2/ubotlibs/raw/core/primitives/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/primitives/bool.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/primitives/bytes.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/primitives/double.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/primitives/int.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/primitives/string.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/primitives/vector.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/raw/core/tl_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.492961 kynaylibs-1.7.2/ubotlibs/session/
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/session/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10824 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/session/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.492961 kynaylibs-1.7.2/ubotlibs/session/internals/
--rw-r--r--   0 root         (0) root         (0)      917 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/session/internals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/session/internals/data_center.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/session/internals/msg_factory.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/session/internals/msg_id.py
--rw-r--r--   0 root         (0) root         (0)     1287 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/session/internals/seq_no.py
--rw-r--r--   0 root         (0) root         (0)    12971 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/session/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.492961 kynaylibs-1.7.2/ubotlibs/storage/
--rw-r--r--   0 root         (0) root         (0)      928 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/storage/file_storage.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/storage/memory_storage.py
--rw-r--r--   0 root         (0) root         (0)     6120 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/storage/storage.py
--rw-r--r--   0 root         (0) root         (0)     3982 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.492961 kynaylibs-1.7.2/ubotlibs/types/
--rw-r--r--   0 root         (0) root         (0)     1109 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.492961 kynaylibs-1.7.2/ubotlibs/types/authorization/
--rw-r--r--   0 root         (0) root         (0)      938 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/authorization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2322 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/authorization/sent_code.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/authorization/terms_of_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.496961 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/
--rw-r--r--   0 root         (0) root         (0)     2843 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 root         (0) root         (0)    12847 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 root         (0) root         (0)     2243 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 root         (0) root         (0)     7606 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     3370 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     3675 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 root         (0) root         (0)     1219 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 root         (0) root         (0)     4205 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 root         (0) root         (0)     1321 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.496961 kynaylibs-1.7.2/ubotlibs/types/inline_mode/
--rw-r--r--   0 root         (0) root         (0)     2824 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3783 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     7321 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2413 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result.py
--rw-r--r--   0 root         (0) root         (0)     5853 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 root         (0) root         (0)     3317 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 root         (0) root         (0)     4535 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 root         (0) root         (0)     4103 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 root         (0) root         (0)     4462 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 root         (0) root         (0)     4468 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 root         (0) root         (0)     4276 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 root         (0) root         (0)     5343 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 root         (0) root         (0)     5560 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 root         (0) root         (0)     4397 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.496961 kynaylibs-1.7.2/ubotlibs/types/input_media/
--rw-r--r--   0 root         (0) root         (0)     1335 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_media/input_media.py
--rw-r--r--   0 root         (0) root         (0)     3230 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_animation.py
--rw-r--r--   0 root         (0) root         (0)     3283 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_audio.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_document.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_photo.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_video.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.496961 kynaylibs-1.7.2/ubotlibs/types/input_message_content/
--rw-r--r--   0 root         (0) root         (0)     1000 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_message_content/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_message_content/input_message_content.py
--rw-r--r--   0 root         (0) root         (0)     2671 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.504961 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/
--rw-r--r--   0 root         (0) root         (0)     1917 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/animation.py
--rw-r--r--   0 root         (0) root         (0)     4037 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/audio.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/contact.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/dice.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/document.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/game.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/location.py
--rw-r--r--   0 root         (0) root         (0)   148353 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/message.py
--rw-r--r--   0 root         (0) root         (0)     4344 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/message_entity.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/message_reactions.py
--rw-r--r--   0 root         (0) root         (0)     4220 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/photo.py
--rw-r--r--   0 root         (0) root         (0)     7069 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/poll.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/poll_option.py
--rw-r--r--   0 root         (0) root         (0)     2496 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/reaction.py
--rw-r--r--   0 root         (0) root         (0)     7054 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/sticker.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/venue.py
--rw-r--r--   0 root         (0) root         (0)     4357 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/video.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/video_note.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/voice.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/web_app_data.py
--rw-r--r--   0 root         (0) root         (0)     6404 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/messages_and_media/web_page.py
--rw-r--r--   0 root         (0) root         (0)     3806 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/object.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:47:33.508961 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/
--rw-r--r--   0 root         (0) root         (0)     2298 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32847 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)    20448 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_event.py
--rw-r--r--   0 root         (0) root         (0)     5524 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 root         (0) root         (0)     4552 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     4100 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 root         (0) root         (0)     9490 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     4443 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     3993 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_preview.py
--rw-r--r--   0 root         (0) root         (0)     4953 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2404 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 root         (0) root         (0)     2664 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/dialog.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/restriction.py
--rw-r--r--   0 root         (0) root         (0)    13109 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/user.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 root         (0) root         (0)    10495 2023-05-21 21:47:06.000000 kynaylibs-1.7.2/ubotlibs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:59.002236 kynaylibs-1.7.3/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      290 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-05-21 22:07:59.002236 kynaylibs-1.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.942235 kynaylibs-1.7.3/compiler/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.942235 kynaylibs-1.7.3/compiler/api/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22917 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/api/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.942235 kynaylibs-1.7.3/compiler/api/source/
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/api/source/auth_key.tl
+-rw-r--r--   0 root         (0) root         (0)   157953 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/api/source/main_api.tl
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.942235 kynaylibs-1.7.3/compiler/api/template/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/api/template/combinator.txt
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/api/template/type.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.942235 kynaylibs-1.7.3/compiler/errors/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.946235 kynaylibs-1.7.3/compiler/errors/source/
+-rw-r--r--   0 root         (0) root         (0)      470 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 root         (0) root         (0)    22290 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 root         (0) root         (0)      470 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.946235 kynaylibs-1.7.3/compiler/errors/template/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/template/class.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.946235 kynaylibs-1.7.3/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-05-21 22:07:58.000000 kynaylibs-1.7.3/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19580 2023-05-21 22:07:58.000000 kynaylibs-1.7.3/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 22:07:58.000000 kynaylibs-1.7.3/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 22:07:58.000000 kynaylibs-1.7.3/kynaylibs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-21 22:07:58.000000 kynaylibs-1.7.3/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-21 22:07:58.000000 kynaylibs-1.7.3/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 22:07:59.002236 kynaylibs-1.7.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.946235 kynaylibs-1.7.3/ubotlibs/
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6633 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/assistant.py
+-rw-r--r--   0 root         (0) root         (0)    43836 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.950235 kynaylibs-1.7.3/ubotlibs/connection/
+-rw-r--r--   0 root         (0) root         (0)      854 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.950235 kynaylibs-1.7.3/ubotlibs/connection/transport/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/transport/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.950235 kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4033 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.950235 kynaylibs-1.7.3/ubotlibs/crypto/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/crypto/aes.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/crypto/mtproto.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/crypto/prime.py
+-rw-r--r--   0 root         (0) root         (0)    10829 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/crypto/rsa.py
+-rw-r--r--   0 root         (0) root         (0)    10865 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)   209155 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/emoji.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.950235 kynaylibs-1.7.3/ubotlibs/enums/
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/auto_name.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4203 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/chat_event_action.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/chat_member_status.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/chat_members_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/chat_type.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/message_entity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/message_media_type.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/message_service_type.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7764 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/msg_types.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/next_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/parse_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/poll_type.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/sent_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/enums/user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.950235 kynaylibs-1.7.3/ubotlibs/errors/
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/errors/rpc_error.py
+-rw-r--r--   0 root         (0) root         (0)    15602 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/file_id.py
+-rw-r--r--   0 root         (0) root         (0)    24704 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.954235 kynaylibs-1.7.3/ubotlibs/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/callback_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/chat_join_request_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/conversation_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/deleted_messages_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/disconnect_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/edited_message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/handler.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/inline_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/poll_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/raw_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/handlers/user_status_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.954235 kynaylibs-1.7.3/ubotlibs/kynay/
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.954235 kynaylibs-1.7.3/ubotlibs/kynay/nan/
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.958235 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.958235 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    13339 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/kynay/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.958235 kynaylibs-1.7.3/ubotlibs/methods/
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.958235 kynaylibs-1.7.3/ubotlibs/methods/advanced/
+-rw-r--r--   0 root         (0) root         (0)      974 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/advanced/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/advanced/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/advanced/resolve_peer.py
+-rw-r--r--   0 root         (0) root         (0)     8320 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/advanced/save_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.958235 kynaylibs-1.7.3/ubotlibs/methods/auth/
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/check_password.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/connect.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/get_password_hint.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/log_out.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/recover_password.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/resend_code.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/send_code.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/send_recovery_code.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/sign_in.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/sign_in_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/sign_up.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/auth/terminate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.962236 kynaylibs-1.7.3/ubotlibs/methods/bots/
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/answer_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/answer_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/get_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/request_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/send_game.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/set_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/bots/set_game_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.966235 kynaylibs-1.7.3/ubotlibs/methods/chats/
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/add_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/archive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/ban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/create_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/create_group.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/create_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/delete_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/delete_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/delete_user_history.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat.py
+-rw-r--r--   0 root         (0) root         (0)     4014 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     5219 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/join_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/leave_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/pin_chat_message.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/promote_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_administrator_title.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_description.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     4523 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_title.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_username.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/set_slow_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/unarchive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/unban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.966235 kynaylibs-1.7.3/ubotlibs/methods/contacts/
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/contacts/add_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/contacts/delete_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/contacts/get_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/contacts/import_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.966235 kynaylibs-1.7.3/ubotlibs/methods/decorators/
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_edited_message.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_message.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_poll.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_raw_update.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/decorators/on_user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.970235 kynaylibs-1.7.3/ubotlibs/methods/invite_links/
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     2336 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.982236 kynaylibs-1.7.3/ubotlibs/methods/messages/
+-rw-r--r--   0 root         (0) root         (0)     4071 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/copy_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     5182 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/copy_message.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     7751 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/download_media.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 root         (0) root         (0)    10100 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/edit_inline_media.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/edit_inline_text.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/edit_message_caption.py
+-rw-r--r--   0 root         (0) root         (0)    12414 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/edit_message_media.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     4542 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/forward_messages.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/get_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/get_discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/get_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     4756 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/get_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/inline_session.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/read_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/retract_vote.py
+-rw-r--r--   0 root         (0) root         (0)     4111 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/search_global.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/search_global_count.py
+-rw-r--r--   0 root         (0) root         (0)     5292 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/search_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/search_messages_count.py
+-rw-r--r--   0 root         (0) root         (0)    12756 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_animation.py
+-rw-r--r--   0 root         (0) root         (0)    11465 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_audio.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_cached_media.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_dice.py
+-rw-r--r--   0 root         (0) root         (0)    10979 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_document.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_location.py
+-rw-r--r--   0 root         (0) root         (0)    20353 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_message.py
+-rw-r--r--   0 root         (0) root         (0)     9509 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_photo.py
+-rw-r--r--   0 root         (0) root         (0)     8213 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     8714 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_venue.py
+-rw-r--r--   0 root         (0) root         (0)    12192 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_video.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_video_note.py
+-rw-r--r--   0 root         (0) root         (0)     9643 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/send_voice.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/stop_poll.py
+-rw-r--r--   0 root         (0) root         (0)     4068 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/stream_media.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/vote_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/wait_for_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/messages/wait_for_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.982236 kynaylibs-1.7.3/ubotlibs/methods/password/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/password/change_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/password/enable_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.982236 kynaylibs-1.7.3/ubotlibs/methods/users/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/block_user.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/delete_profile_photos.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/get_chat_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/get_common_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/get_me.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/get_users.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/set_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/set_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/set_username.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/unblock_user.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/users/update_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.986236 kynaylibs-1.7.3/ubotlibs/methods/utilities/
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/add_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/compose.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/export_session_string.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/idle.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/remove_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/restart.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/run.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/start.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/stop.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/methods/utilities/stop_transmission.py
+-rw-r--r--   0 root         (0) root         (0)    61915 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/mime_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.986236 kynaylibs-1.7.3/ubotlibs/parser/
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7567 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/parser/html.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/parser/markdown.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.986236 kynaylibs-1.7.3/ubotlibs/raw/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.986236 kynaylibs-1.7.3/ubotlibs/raw/core/
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/future_salt.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/future_salts.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/gzip_packed.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/list.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/msg_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.986236 kynaylibs-1.7.3/ubotlibs/raw/core/primitives/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/primitives/bool.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/primitives/bytes.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/primitives/double.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/primitives/int.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/primitives/string.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/primitives/vector.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/raw/core/tl_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.986236 kynaylibs-1.7.3/ubotlibs/session/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/session/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10824 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/session/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.986236 kynaylibs-1.7.3/ubotlibs/session/internals/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/session/internals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/session/internals/data_center.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/session/internals/msg_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/session/internals/msg_id.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/session/internals/seq_no.py
+-rw-r--r--   0 root         (0) root         (0)    12971 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/session/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.990236 kynaylibs-1.7.3/ubotlibs/storage/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/storage/file_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/storage/memory_storage.py
+-rw-r--r--   0 root         (0) root         (0)     6120 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/storage/storage.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.990236 kynaylibs-1.7.3/ubotlibs/types/
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.990236 kynaylibs-1.7.3/ubotlibs/types/authorization/
+-rw-r--r--   0 root         (0) root         (0)      938 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/authorization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/authorization/sent_code.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/authorization/terms_of_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.994236 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 root         (0) root         (0)    12847 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 root         (0) root         (0)     7606 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 root         (0) root         (0)     4205 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.998236 kynaylibs-1.7.3/ubotlibs/types/inline_mode/
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3783 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     7321 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 root         (0) root         (0)     5853 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3317 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     4535 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 root         (0) root         (0)     4103 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4462 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4468 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 root         (0) root         (0)     4276 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 root         (0) root         (0)     5343 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 root         (0) root         (0)     5560 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 root         (0) root         (0)     4397 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.998236 kynaylibs-1.7.3/ubotlibs/types/input_media/
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_media/input_media.py
+-rw-r--r--   0 root         (0) root         (0)     3230 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_video.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.998236 kynaylibs-1.7.3/ubotlibs/types/input_message_content/
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_message_content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_message_content/input_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:58.998236 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/animation.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/audio.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/dice.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/document.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/game.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/location.py
+-rw-r--r--   0 root         (0) root         (0)   148353 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/message.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/message_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     4220 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/photo.py
+-rw-r--r--   0 root         (0) root         (0)     7069 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/poll.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/poll_option.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/reaction.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/venue.py
+-rw-r--r--   0 root         (0) root         (0)     4357 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/video.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/video_note.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/voice.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 root         (0) root         (0)     6404 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/messages_and_media/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3806 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/object.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:07:59.002236 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32847 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)    20448 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_event.py
+-rw-r--r--   0 root         (0) root         (0)     5524 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 root         (0) root         (0)     9490 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 root         (0) root         (0)     4953 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/dialog.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/restriction.py
+-rw-r--r--   0 root         (0) root         (0)    13109 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/user.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 root         (0) root         (0)    10495 2023-05-21 22:07:41.000000 kynaylibs-1.7.3/ubotlibs/utils.py
```

### Comparing `kynaylibs-1.7.2/LICENSE` & `kynaylibs-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/NOTICE` & `kynaylibs-1.7.3/NOTICE`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/PKG-INFO` & `kynaylibs-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.7.2
+Version: 1.7.3
 Summary: ubotlibs - Telegram MTProto API Client Library for Python.
 Home-page: https://github.com/hitokizzy/ubotlibs
 Author: Hamba
 Author-email: tuyultermux777@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/iskandar777-dar/ubotlibs/issues
 Project-URL: Documentation, https://ubotlibs.tech
```

### Comparing `kynaylibs-1.7.2/README.md` & `kynaylibs-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/__init__.py` & `kynaylibs-1.7.3/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/api/__init__.py` & `kynaylibs-1.7.3/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/api/compiler.py` & `kynaylibs-1.7.3/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/api/source/auth_key.tl` & `kynaylibs-1.7.3/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/api/source/main_api.tl` & `kynaylibs-1.7.3/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/api/source/sys_msgs.tl` & `kynaylibs-1.7.3/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/api/template/combinator.txt` & `kynaylibs-1.7.3/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/api/template/type.txt` & `kynaylibs-1.7.3/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/errors/__init__.py` & `kynaylibs-1.7.3/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/errors/compiler.py` & `kynaylibs-1.7.3/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/errors/sort.py` & `kynaylibs-1.7.3/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/errors/source/400_BAD_REQUEST.tsv` & `kynaylibs-1.7.3/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/errors/source/401_UNAUTHORIZED.tsv` & `kynaylibs-1.7.3/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/errors/source/403_FORBIDDEN.tsv` & `kynaylibs-1.7.3/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `kynaylibs-1.7.3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `kynaylibs-1.7.3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-1.7.3/kynaylibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.7.2
+Version: 1.7.3
 Summary: ubotlibs - Telegram MTProto API Client Library for Python.
 Home-page: https://github.com/hitokizzy/ubotlibs
 Author: Hamba
 Author-email: tuyultermux777@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/iskandar777-dar/ubotlibs/issues
 Project-URL: Documentation, https://ubotlibs.tech
```

### Comparing `kynaylibs-1.7.2/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-1.7.3/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/setup.py` & `kynaylibs-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/__init__.py` & `kynaylibs-1.7.3/ubotlibs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import sys
 from datetime import datetime, timezone
 from typing import Dict, Optional, Union
 
-from config import CMD_HNDLR as cmds
 from pyrogram import Client, filters
 
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 BL_GCAST = [
     -1001599474353,
     -1001692751821,
     -1001473548283,
```

### Comparing `kynaylibs-1.7.2/ubotlibs/assistant.py` & `kynaylibs-1.7.3/ubotlibs/assistant.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/client.py` & `kynaylibs-1.7.3/ubotlibs/client.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/__init__.py` & `kynaylibs-1.7.3/ubotlibs/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/connection.py` & `kynaylibs-1.7.3/ubotlibs/connection/connection.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/transport/__init__.py` & `kynaylibs-1.7.3/ubotlibs/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/__init__.py` & `kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp.py` & `kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_abridged.py` & `kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_abridged_o.py` & `kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_full.py` & `kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_intermediate.py` & `kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/connection/transport/tcp/tcp_intermediate_o.py` & `kynaylibs-1.7.3/ubotlibs/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/crypto/__init__.py` & `kynaylibs-1.7.3/ubotlibs/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/crypto/aes.py` & `kynaylibs-1.7.3/ubotlibs/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/crypto/mtproto.py` & `kynaylibs-1.7.3/ubotlibs/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/crypto/prime.py` & `kynaylibs-1.7.3/ubotlibs/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/crypto/rsa.py` & `kynaylibs-1.7.3/ubotlibs/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/dispatcher.py` & `kynaylibs-1.7.3/ubotlibs/dispatcher.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/emoji.py` & `kynaylibs-1.7.3/ubotlibs/emoji.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/__init__.py` & `kynaylibs-1.7.3/ubotlibs/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/auto_name.py` & `kynaylibs-1.7.3/ubotlibs/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/chat_action.py` & `kynaylibs-1.7.3/ubotlibs/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/chat_event_action.py` & `kynaylibs-1.7.3/ubotlibs/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/chat_member_status.py` & `kynaylibs-1.7.3/ubotlibs/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/chat_members_filter.py` & `kynaylibs-1.7.3/ubotlibs/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/chat_type.py` & `kynaylibs-1.7.3/ubotlibs/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/message_entity_type.py` & `kynaylibs-1.7.3/ubotlibs/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/message_media_type.py` & `kynaylibs-1.7.3/ubotlibs/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/message_service_type.py` & `kynaylibs-1.7.3/ubotlibs/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/messages_filter.py` & `kynaylibs-1.7.3/ubotlibs/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/msg_types.py` & `kynaylibs-1.7.3/ubotlibs/enums/msg_types.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/next_code_type.py` & `kynaylibs-1.7.3/ubotlibs/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/parse_mode.py` & `kynaylibs-1.7.3/ubotlibs/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/poll_type.py` & `kynaylibs-1.7.3/ubotlibs/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/sent_code_type.py` & `kynaylibs-1.7.3/ubotlibs/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/enums/user_status.py` & `kynaylibs-1.7.3/ubotlibs/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/errors/__init__.py` & `kynaylibs-1.7.3/ubotlibs/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/errors/rpc_error.py` & `kynaylibs-1.7.3/ubotlibs/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/file_id.py` & `kynaylibs-1.7.3/ubotlibs/file_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/filters.py` & `kynaylibs-1.7.3/ubotlibs/filters.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/__init__.py` & `kynaylibs-1.7.3/ubotlibs/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/callback_query_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/chat_join_request_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/chat_member_updated_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/chosen_inline_result_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/conversation_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/conversation_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/deleted_messages_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/disconnect_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/edited_message_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/inline_query_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/message_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/poll_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/raw_update_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/handlers/user_status_handler.py` & `kynaylibs-1.7.3/ubotlibs/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/__init__.py` & `kynaylibs-1.7.3/ubotlibs/kynay/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/__init__.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/load.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/load.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/log.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/log.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/PyroHelpers.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/adminHelpers.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/ai.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/aiohttp_helper.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/basic.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/constants.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/db/__init__.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/db/permit.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/function.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/get_id.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/http.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/http.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/inline.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/interval.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/misc.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/parser.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/pilter.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/tools.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/unpack.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/kynay/nan/utils/utility.py` & `kynaylibs-1.7.3/ubotlibs/kynay/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/advanced/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/advanced/invoke.py` & `kynaylibs-1.7.3/ubotlibs/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/advanced/resolve_peer.py` & `kynaylibs-1.7.3/ubotlibs/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/advanced/save_file.py` & `kynaylibs-1.7.3/ubotlibs/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/accept_terms_of_service.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/check_password.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/connect.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/disconnect.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/get_password_hint.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/initialize.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/log_out.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/recover_password.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/resend_code.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/send_code.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/send_recovery_code.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/sign_in.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/sign_in_bot.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/sign_up.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/auth/terminate.py` & `kynaylibs-1.7.3/ubotlibs/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/answer_callback_query.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/answer_inline_query.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/answer_web_app_query.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/delete_bot_commands.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/get_bot_commands.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/get_bot_default_privileges.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/get_chat_menu_button.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/get_game_high_scores.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/get_inline_bot_results.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/request_callback_answer.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/send_game.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/send_inline_bot_result.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/set_bot_commands.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/set_bot_default_privileges.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/set_chat_menu_button.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/bots/set_game_score.py` & `kynaylibs-1.7.3/ubotlibs/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/add_chat_members.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/archive_chats.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/ban_chat_member.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/create_channel.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/create_group.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/create_supergroup.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/delete_channel.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/delete_chat_photo.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/delete_supergroup.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/delete_user_history.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_event_log.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_member.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_members.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_members_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_chat_online_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_dialogs.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_dialogs_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_nearby_chats.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/get_send_as_chats.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/join_chat.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/leave_chat.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/mark_chat_unread.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/pin_chat_message.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/promote_chat_member.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/restrict_chat_member.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_administrator_title.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_description.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_permissions.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_photo.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_protected_content.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_title.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_chat_username.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_send_as_chat.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/set_slow_mode.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/unarchive_chats.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/unban_chat_member.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/unpin_all_chat_messages.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/chats/unpin_chat_message.py` & `kynaylibs-1.7.3/ubotlibs/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/contacts/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/contacts/add_contact.py` & `kynaylibs-1.7.3/ubotlibs/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/contacts/delete_contacts.py` & `kynaylibs-1.7.3/ubotlibs/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/contacts/get_contacts.py` & `kynaylibs-1.7.3/ubotlibs/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/contacts/get_contacts_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/contacts/import_contacts.py` & `kynaylibs-1.7.3/ubotlibs/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_callback_query.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_chat_join_request.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_chat_member_updated.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_chosen_inline_result.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_deleted_messages.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_disconnect.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_edited_message.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_inline_query.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_message.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_poll.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_raw_update.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/decorators/on_user_status.py` & `kynaylibs-1.7.3/ubotlibs/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/approve_all_chat_join_requests.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/approve_chat_join_request.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/create_chat_invite_link.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/decline_all_chat_join_requests.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/decline_chat_join_request.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/delete_chat_admin_invite_links.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/delete_chat_invite_link.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/edit_chat_invite_link.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/export_chat_invite_link.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_admin_invite_links.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_admin_invite_links_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_admins_with_invite_links.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_invite_link.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_invite_link_joiners.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_invite_link_joiners_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/get_chat_join_requests.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/invite_links/revoke_chat_invite_link.py` & `kynaylibs-1.7.3/ubotlibs/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/copy_media_group.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/copy_message.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/delete_messages.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/download_media.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/edit_inline_caption.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/edit_inline_media.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/edit_inline_reply_markup.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/edit_inline_text.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/edit_message_caption.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/edit_message_media.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/edit_message_reply_markup.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/edit_message_text.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/forward_messages.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/get_chat_history.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/get_chat_history_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/get_custom_emoji_stickers.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/get_discussion_message.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/get_discussion_replies.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/get_discussion_replies_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/get_media_group.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/get_messages.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/inline_session.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/read_chat_history.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/retract_vote.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/search_global.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/search_global_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/search_messages.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/search_messages_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_animation.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_audio.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_cached_media.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_chat_action.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_contact.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_dice.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_document.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_location.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_media_group.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_message.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_photo.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_poll.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_reaction.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_sticker.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_venue.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_video.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_video_note.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/send_voice.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/stop_poll.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/stream_media.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/vote_poll.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/wait_for_callback_query.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/wait_for_callback_query.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/messages/wait_for_message.py` & `kynaylibs-1.7.3/ubotlibs/methods/messages/wait_for_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/password/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/password/change_cloud_password.py` & `kynaylibs-1.7.3/ubotlibs/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/password/enable_cloud_password.py` & `kynaylibs-1.7.3/ubotlibs/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/password/remove_cloud_password.py` & `kynaylibs-1.7.3/ubotlibs/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/block_user.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/delete_profile_photos.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/get_chat_photos.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/get_chat_photos_count.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/get_common_chats.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/get_default_emoji_statuses.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/get_me.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/get_users.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/set_emoji_status.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/set_profile_photo.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/set_username.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/unblock_user.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/users/update_profile.py` & `kynaylibs-1.7.3/ubotlibs/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/__init__.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/add_handler.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/compose.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/export_session_string.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/idle.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/remove_handler.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/restart.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/run.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/start.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/stop.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/methods/utilities/stop_transmission.py` & `kynaylibs-1.7.3/ubotlibs/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/mime_types.py` & `kynaylibs-1.7.3/ubotlibs/mime_types.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/parser/__init__.py` & `kynaylibs-1.7.3/ubotlibs/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/parser/html.py` & `kynaylibs-1.7.3/ubotlibs/parser/html.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/parser/markdown.py` & `kynaylibs-1.7.3/ubotlibs/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/parser/parser.py` & `kynaylibs-1.7.3/ubotlibs/parser/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/parser/utils.py` & `kynaylibs-1.7.3/ubotlibs/parser/utils.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/__init__.py` & `kynaylibs-1.7.3/ubotlibs/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/__init__.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/future_salt.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/future_salts.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/gzip_packed.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/list.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/message.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/msg_container.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/primitives/__init__.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/primitives/bool.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/primitives/bytes.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/primitives/double.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/primitives/int.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/primitives/string.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/primitives/vector.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/raw/core/tl_object.py` & `kynaylibs-1.7.3/ubotlibs/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/session/__init__.py` & `kynaylibs-1.7.3/ubotlibs/session/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/session/auth.py` & `kynaylibs-1.7.3/ubotlibs/session/auth.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/session/internals/__init__.py` & `kynaylibs-1.7.3/ubotlibs/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/session/internals/data_center.py` & `kynaylibs-1.7.3/ubotlibs/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/session/internals/msg_factory.py` & `kynaylibs-1.7.3/ubotlibs/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/session/internals/msg_id.py` & `kynaylibs-1.7.3/ubotlibs/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/session/internals/seq_no.py` & `kynaylibs-1.7.3/ubotlibs/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/session/session.py` & `kynaylibs-1.7.3/ubotlibs/session/session.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/storage/__init__.py` & `kynaylibs-1.7.3/ubotlibs/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/storage/file_storage.py` & `kynaylibs-1.7.3/ubotlibs/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/storage/memory_storage.py` & `kynaylibs-1.7.3/ubotlibs/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/storage/sqlite_storage.py` & `kynaylibs-1.7.3/ubotlibs/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/storage/storage.py` & `kynaylibs-1.7.3/ubotlibs/storage/storage.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/sync.py` & `kynaylibs-1.7.3/ubotlibs/sync.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/__init__.py` & `kynaylibs-1.7.3/ubotlibs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/authorization/__init__.py` & `kynaylibs-1.7.3/ubotlibs/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/authorization/sent_code.py` & `kynaylibs-1.7.3/ubotlibs/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/authorization/terms_of_service.py` & `kynaylibs-1.7.3/ubotlibs/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/__init__.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/bot_command_scope_default.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/callback_game.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/callback_query.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/force_reply.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/game_high_score.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/inline_keyboard_button.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/inline_keyboard_markup.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/keyboard_button.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/login_url.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/menu_button.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/menu_button_commands.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/menu_button_default.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/menu_button_web_app.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/reply_keyboard_markup.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/reply_keyboard_remove.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/sent_web_app_message.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/bots_and_keyboards/web_app_info.py` & `kynaylibs-1.7.3/ubotlibs/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/__init__.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/chosen_inline_result.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_animation.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_article.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_audio.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_animation.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_audio.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_document.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_photo.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_sticker.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_video.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_cached_voice.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_contact.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_document.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_location.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_photo.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_venue.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_video.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/inline_mode/inline_query_result_voice.py` & `kynaylibs-1.7.3/ubotlibs/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_media/__init__.py` & `kynaylibs-1.7.3/ubotlibs/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_media/input_media.py` & `kynaylibs-1.7.3/ubotlibs/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_animation.py` & `kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_audio.py` & `kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_document.py` & `kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_photo.py` & `kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_media/input_media_video.py` & `kynaylibs-1.7.3/ubotlibs/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_media/input_phone_contact.py` & `kynaylibs-1.7.3/ubotlibs/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_message_content/__init__.py` & `kynaylibs-1.7.3/ubotlibs/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_message_content/input_message_content.py` & `kynaylibs-1.7.3/ubotlibs/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/input_message_content/input_text_message_content.py` & `kynaylibs-1.7.3/ubotlibs/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/list.py` & `kynaylibs-1.7.3/ubotlibs/types/list.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/__init__.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/animation.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/audio.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/contact.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/dice.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/document.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/game.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/location.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/message.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/message_entity.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/message_reactions.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/photo.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/poll.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/poll_option.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/reaction.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/sticker.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/stripped_thumbnail.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/thumbnail.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/venue.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/video.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/video_note.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/voice.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/web_app_data.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/messages_and_media/web_page.py` & `kynaylibs-1.7.3/ubotlibs/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/object.py` & `kynaylibs-1.7.3/ubotlibs/types/object.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/update.py` & `kynaylibs-1.7.3/ubotlibs/types/update.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/__init__.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_admin_with_invite_links.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_event.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_event_filter.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_invite_link.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_join_request.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_joiner.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_member.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_member_updated.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_permissions.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_photo.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_preview.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_privileges.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/chat_reactions.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/dialog.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/emoji_status.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/invite_link_importer.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/restriction.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/user.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/video_chat_ended.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/video_chat_members_invited.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/video_chat_scheduled.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/types/user_and_chats/video_chat_started.py` & `kynaylibs-1.7.3/ubotlibs/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.2/ubotlibs/utils.py` & `kynaylibs-1.7.3/ubotlibs/utils.py`

 * *Files identical despite different names*

