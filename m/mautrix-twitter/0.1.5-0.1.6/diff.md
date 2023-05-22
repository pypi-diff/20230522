# Comparing `tmp/mautrix-twitter-0.1.5.tar.gz` & `tmp/mautrix-twitter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mautrix-twitter-0.1.5.tar", last modified: Tue Aug 23 20:44:36 2022, max compression
+gzip compressed data, was "mautrix-twitter-0.1.6.tar", last modified: Mon May 22 17:08:40 2023, max compression
```

## Comparing `mautrix-twitter-0.1.5.tar` & `mautrix-twitter-0.1.6.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.867659 mautrix-twitter-0.1.5/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/LICENSE
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       93 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/MANIFEST.in
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1991 2022-08-23 20:44:36.867659 mautrix-twitter-0.1.5/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1141 2022-05-19 19:51:42.000000 mautrix-twitter-0.1.5/README.md
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.863659 mautrix-twitter-0.1.5/mautrix_twitter/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       70 2022-08-23 20:44:09.000000 mautrix-twitter-0.1.5/mautrix_twitter/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3946 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/__main__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.863659 mautrix-twitter-0.1.5/mautrix_twitter/commands/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       68 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/commands/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3299 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/commands/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3100 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/commands/conn.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      276 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/commands/typehint.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4115 2022-07-06 16:01:26.000000 mautrix-twitter-0.1.5/mautrix_twitter/config.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.863659 mautrix-twitter-0.1.5/mautrix_twitter/db/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      413 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/db/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2601 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/db/message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4003 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/db/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3731 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/db/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4630 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/db/reaction.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4014 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/db/upgrade.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2975 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/db/user.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12363 2022-08-19 11:40:25.000000 mautrix-twitter-0.1.5/mautrix_twitter/example-config.yaml
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2676 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/formatter.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1438 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/get_version.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5473 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/matrix.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    44081 2022-07-13 20:26:23.000000 mautrix-twitter-0.1.5/mautrix_twitter/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8011 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    20847 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/user.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.863659 mautrix-twitter-0.1.5/mautrix_twitter/util/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/util/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1347 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/util/color_log.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      174 2022-08-23 20:44:36.000000 mautrix-twitter-0.1.5/mautrix_twitter/version.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.863659 mautrix-twitter-0.1.5/mautrix_twitter/web/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       46 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/web/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4533 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautrix_twitter/web/provisioning_api.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.863659 mautrix-twitter-0.1.5/mautrix_twitter.egg-info/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1991 2022-08-23 20:44:36.000000 mautrix-twitter-0.1.5/mautrix_twitter.egg-info/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1582 2022-08-23 20:44:36.000000 mautrix-twitter-0.1.5/mautrix_twitter.egg-info/SOURCES.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2022-08-23 20:44:36.000000 mautrix-twitter-0.1.5/mautrix_twitter.egg-info/dependency_links.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      349 2022-08-23 20:44:36.000000 mautrix-twitter-0.1.5/mautrix_twitter.egg-info/requires.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       26 2022-08-23 20:44:36.000000 mautrix-twitter-0.1.5/mautrix_twitter.egg-info/top_level.txt
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.867659 mautrix-twitter-0.1.5/mautwitdm/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       71 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5168 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/conversation.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1754 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/dispatcher.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2146 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/errors.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9601 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/poller.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5509 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/streamer.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7345 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/twitter.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-08-23 20:44:36.867659 mautrix-twitter-0.1.5/mautwitdm/types/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1084 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1787 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/conversation.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2583 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/entry.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1280 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4730 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/message_attachment.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1242 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/message_entity.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2288 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/reaction.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2340 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/response.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1184 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/stream_payload.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1030 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/user.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1115 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/types/util.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5094 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/mautwitdm/uploader.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      247 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/optional-requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      203 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/pyproject.toml
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      151 2022-08-22 13:08:40.000000 mautrix-twitter-0.1.5/requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2022-08-23 20:44:36.867659 mautrix-twitter-0.1.5/setup.cfg
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2064 2022-04-23 11:25:47.000000 mautrix-twitter-0.1.5/setup.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.077292 mautrix-twitter-0.1.6/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/LICENSE
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       93 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/MANIFEST.in
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1976 2023-05-22 17:08:40.077292 mautrix-twitter-0.1.6/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1140 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/README.md
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.073292 mautrix-twitter-0.1.6/mautrix_twitter/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       70 2023-05-22 17:08:13.000000 mautrix-twitter-0.1.6/mautrix_twitter/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4174 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/__main__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2901 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/backfill.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.073292 mautrix-twitter-0.1.6/mautrix_twitter/commands/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       68 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/commands/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3299 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/commands/auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3100 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/commands/conn.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      276 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/commands/typehint.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4453 2023-05-22 11:04:14.000000 mautrix-twitter-0.1.6/mautrix_twitter/config.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.073292 mautrix-twitter-0.1.6/mautrix_twitter/db/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      484 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/db/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2679 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/db/backfill.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3245 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/db/message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4177 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/db/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3448 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/db/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4506 2023-05-22 10:50:47.000000 mautrix-twitter-0.1.6/mautrix_twitter/db/reaction.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6819 2023-05-22 10:51:30.000000 mautrix-twitter-0.1.6/mautrix_twitter/db/upgrade.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2975 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/db/user.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    14895 2023-05-22 11:06:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/example-config.yaml
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2676 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/formatter.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1438 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/get_version.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5473 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/matrix.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    58222 2023-05-22 11:28:13.000000 mautrix-twitter-0.1.6/mautrix_twitter/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9161 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    24519 2023-05-22 10:50:47.000000 mautrix-twitter-0.1.6/mautrix_twitter/user.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.073292 mautrix-twitter-0.1.6/mautrix_twitter/util/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/util/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1347 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/util/color_log.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      174 2023-05-22 17:08:39.000000 mautrix-twitter-0.1.6/mautrix_twitter/version.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.073292 mautrix-twitter-0.1.6/mautrix_twitter/web/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       46 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/web/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4843 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautrix_twitter/web/provisioning_api.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.073292 mautrix-twitter-0.1.6/mautrix_twitter.egg-info/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1976 2023-05-22 17:08:40.000000 mautrix-twitter-0.1.6/mautrix_twitter.egg-info/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1641 2023-05-22 17:08:40.000000 mautrix-twitter-0.1.6/mautrix_twitter.egg-info/SOURCES.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2023-05-22 17:08:40.000000 mautrix-twitter-0.1.6/mautrix_twitter.egg-info/dependency_links.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      404 2023-05-22 17:08:40.000000 mautrix-twitter-0.1.6/mautrix_twitter.egg-info/requires.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       26 2023-05-22 17:08:40.000000 mautrix-twitter-0.1.6/mautrix_twitter.egg-info/top_level.txt
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.073292 mautrix-twitter-0.1.6/mautwitdm/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       71 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6159 2023-05-22 10:56:40.000000 mautrix-twitter-0.1.6/mautwitdm/conversation.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1754 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/dispatcher.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2161 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/errors.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    11936 2023-05-22 17:08:23.000000 mautrix-twitter-0.1.6/mautwitdm/poller.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5509 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/streamer.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     7345 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/twitter.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-22 17:08:40.077292 mautrix-twitter-0.1.6/mautwitdm/types/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1103 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/types/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1821 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/types/conversation.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2583 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/types/entry.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1400 2023-05-22 10:51:16.000000 mautrix-twitter-0.1.6/mautwitdm/types/message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4785 2023-05-22 10:51:11.000000 mautrix-twitter-0.1.6/mautwitdm/types/message_attachment.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1242 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/types/message_entity.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2882 2023-05-22 11:31:56.000000 mautrix-twitter-0.1.6/mautwitdm/types/reaction.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2537 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/types/response.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1184 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/types/stream_payload.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1030 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/types/user.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1115 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/mautwitdm/types/util.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5187 2023-05-22 10:57:25.000000 mautrix-twitter-0.1.6/mautwitdm/uploader.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      279 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/optional-requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      203 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/pyproject.toml
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      152 2023-05-22 17:06:58.000000 mautrix-twitter-0.1.6/requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2023-05-22 17:08:40.077292 mautrix-twitter-0.1.6/setup.cfg
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2064 2023-05-14 10:31:57.000000 mautrix-twitter-0.1.6/setup.py
```

### Comparing `mautrix-twitter-0.1.5/LICENSE` & `mautrix-twitter-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/PKG-INFO` & `mautrix-twitter-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 Metadata-Version: 2.1
 Name: mautrix-twitter
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Matrix-Twitter DM puppeting bridge.
 Home-page: https://github.com/mautrix/twitter
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: e2be
 Provides-Extra: metrics
+Provides-Extra: sqlite
 License-File: LICENSE
 
 # mautrix-twitter
 ![Languages](https://img.shields.io/github/languages/top/mautrix/twitter.svg)
 [![License](https://img.shields.io/github/license/mautrix/twitter.svg)](LICENSE)
 [![Release](https://img.shields.io/github/release/mautrix/twitter/all.svg)](https://github.com/mautrix/twitter/releases)
 [![GitLab CI](https://mau.dev/mautrix/twitter/badges/master/pipeline.svg)](https://mau.dev/mautrix/twitter/container_registry)
 
 A Matrix-Twitter DM puppeting bridge.
 
-### Documentation
+## Documentation
 All setup and usage instructions are located on
 [docs.mau.fi](https://docs.mau.fi/bridges/python/twitter/index.html).
 Some quick links:
 
 * [Bridge setup](https://docs.mau.fi/bridges/python/setup.html?bridge=twitter)
   (or [with Docker](https://docs.mau.fi/bridges/general/docker-setup.html?bridge=twitter))
 * Basic usage: [Authentication](https://docs.mau.fi/bridges/python/twitter/authentication.html)
 
 ### Features & Roadmap
 [ROADMAP.md](https://github.com/mautrix/twitter/blob/master/ROADMAP.md)
 contains a general overview of what is supported by the bridge.
 
 ## Discussion
 Matrix room: [`#twitter:maunium.net`](https://matrix.to/#/#twitter:maunium.net)
-
-
```

### Comparing `mautrix-twitter-0.1.5/README.md` & `mautrix-twitter-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ![Languages](https://img.shields.io/github/languages/top/mautrix/twitter.svg)
 [![License](https://img.shields.io/github/license/mautrix/twitter.svg)](LICENSE)
 [![Release](https://img.shields.io/github/release/mautrix/twitter/all.svg)](https://github.com/mautrix/twitter/releases)
 [![GitLab CI](https://mau.dev/mautrix/twitter/badges/master/pipeline.svg)](https://mau.dev/mautrix/twitter/container_registry)
 
 A Matrix-Twitter DM puppeting bridge.
 
-### Documentation
+## Documentation
 All setup and usage instructions are located on
 [docs.mau.fi](https://docs.mau.fi/bridges/python/twitter/index.html).
 Some quick links:
 
 * [Bridge setup](https://docs.mau.fi/bridges/python/setup.html?bridge=twitter)
   (or [with Docker](https://docs.mau.fi/bridges/general/docker-setup.html?bridge=twitter))
 * Basic usage: [Authentication](https://docs.mau.fi/bridges/python/twitter/authentication.html)
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/__main__.py` & `mautrix-twitter-0.1.6/mautrix_twitter/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,37 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import Any
+import asyncio
 
 from mautrix.bridge import Bridge
 from mautrix.types import RoomID, UserID
+from mautrix.util import background_task
 
 from . import commands
+from .backfill import BackfillStatus
 from .config import Config
 from .db import init as init_db, upgrade_table
 from .matrix import MatrixHandler
 from .portal import Portal
 from .puppet import Puppet
 from .user import User
 from .version import linkified_version, version
 from .web import ProvisioningAPI
 
 
 class TwitterBridge(Bridge):
     module = "mautrix_twitter"
     name = "mautrix-twitter"
+    beeper_service_name = "twitter"
+    beeper_network_name = "twitter"
     command = "python -m mautrix-twitter"
     description = "A Matrix-Twitter DM puppeting bridge."
     repo_url = "https://github.com/mautrix/twitter"
     version = version
     markdown_version = linkified_version
     config_class = Config
     matrix_class = MatrixHandler
@@ -59,14 +64,15 @@
 
     async def start(self) -> None:
         self.add_startup_actions(User.init_cls(self))
         self.add_startup_actions(Puppet.init_cls(self))
         Portal.init_cls(self)
         if self.config["bridge.resend_bridge_info"]:
             self.add_startup_actions(self.resend_bridge_info())
+        background_task.create(BackfillStatus.backfill_loop())
         await super().start()
 
     def prepare_stop(self) -> None:
         self.add_shutdown_actions(user.stop() for user in User.by_twid.values())
         for puppet in Puppet.by_custom_mxid.values():
             puppet.stop()
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/commands/auth.py` & `mautrix-twitter-0.1.6/mautrix_twitter/commands/auth.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/commands/conn.py` & `mautrix-twitter-0.1.6/mautrix_twitter/commands/conn.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/config.py` & `mautrix-twitter-0.1.6/mautrix_twitter/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,34 +23,26 @@
 from mautrix.types import UserID
 from mautrix.util.config import ConfigUpdateHelper, ForbiddenDefault, ForbiddenKey
 
 Permissions = NamedTuple("Permissions", user=bool, admin=bool, level=str)
 
 
 class Config(BaseBridgeConfig):
-    def __getitem__(self, key: str) -> Any:
-        try:
-            return os.environ[f"MAUTRIX_TWITTER_{key.replace('.', '_').upper()}"]
-        except KeyError:
-            return super().__getitem__(key)
-
     @property
     def forbidden_defaults(self) -> list[ForbiddenDefault]:
         return [
             *super().forbidden_defaults,
             ForbiddenDefault("appservice.database", "postgres://username:password@hostname/db"),
             ForbiddenDefault("bridge.permissions", ForbiddenKey("example.com")),
         ]
 
     def do_update(self, helper: ConfigUpdateHelper) -> None:
         super().do_update(helper)
         copy, copy_dict, base = helper
 
-        copy("homeserver.asmux")
-
         copy("appservice.provisioning.enabled")
         copy("appservice.provisioning.prefix")
         copy("appservice.provisioning.shared_secret")
         if base["appservice.provisioning.shared_secret"] == "generate":
             base["appservice.provisioning.shared_secret"] = self._new_token()
 
         copy("metrics.enabled")
@@ -60,35 +52,46 @@
         copy("bridge.displayname_template")
 
         copy("bridge.displayname_max_length")
 
         copy("bridge.initial_conversation_sync")
         copy("bridge.sync_with_custom_puppets")
         copy("bridge.sync_direct_chat_list")
+        copy("bridge.low_quality_tag")
+        copy("bridge.low_quality_mute")
         copy("bridge.double_puppet_server_map")
         copy("bridge.double_puppet_allow_discovery")
         if self["bridge.login_shared_secret"]:
             base["bridge.login_shared_secret_map"] = {
                 base["homeserver.domain"]: self["bridge.login_shared_secret"]
             }
         else:
             copy("bridge.login_shared_secret_map")
         copy("bridge.federate_rooms")
         copy("bridge.backfill.invite_own_puppet")
         copy("bridge.backfill.initial_limit")
         copy("bridge.backfill.disable_notifications")
-        copy("bridge.private_chat_portal_meta")
+        copy("bridge.backfill.backwards")
+        if isinstance(self.get("bridge.private_chat_portal_meta", "default"), bool):
+            base["bridge.private_chat_portal_meta"] = (
+                "always" if self["bridge.private_chat_portal_meta"] else "default"
+            )
+        else:
+            copy("bridge.private_chat_portal_meta")
+            if base["bridge.private_chat_portal_meta"] not in ("default", "always", "never"):
+                base["bridge.private_chat_portal_meta"] = "default"
         copy("bridge.delivery_receipts")
         copy("bridge.delivery_error_reports")
         copy("bridge.message_status_events")
         copy("bridge.temporary_disconnect_notices")
         copy("bridge.disable_bridge_notices")
         copy("bridge.error_sleep")
         copy("bridge.max_poll_errors")
         copy("bridge.resend_bridge_info")
+        copy("bridge.caption_in_message")
 
         copy("bridge.command_prefix")
 
         copy_dict("bridge.permissions")
 
     def _get_permissions(self, key: str) -> Permissions:
         level = self["bridge.permissions"].get(key, "")
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/db/message.py` & `mautrix-twitter-0.1.6/mautrix_twitter/db/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,21 @@
     twid: int
     receiver: int
 
     async def insert(self) -> None:
         q = "INSERT INTO message (mxid, mx_room, twid, receiver) VALUES ($1, $2, $3, $4)"
         await self.db.execute(q, self.mxid, self.mx_room, self.twid, self.receiver)
 
+    async def upsert(self) -> None:
+        q = """
+            INSERT INTO message(mxid, mx_room, twid, receiver) VALUES($1, $2, $3, $4)
+            ON CONFLICT(twid, receiver) DO UPDATE SET twid=excluded.twid, receiver=excluded.receiver
+        """
+        await self.db.execute(q, self.mxid, self.mx_room, self.twid, self.receiver)
+
     async def delete(self) -> None:
         q = "DELETE FROM message WHERE twid=$1 AND receiver=$2"
         await self.db.execute(q, self.twid, self.receiver)
 
     @classmethod
     async def delete_all(cls, room_id: RoomID) -> None:
         await cls.db.execute("DELETE FROM message WHERE mx_room=$1", room_id)
@@ -59,13 +66,21 @@
         q = "SELECT mxid, mx_room, twid, receiver FROM message WHERE mx_room=$1 ORDER BY twid DESC LIMIT 1"
         row = await cls.db.fetchrow(q, mx_room)
         if not row:
             return None
         return cls(**row)
 
     @classmethod
+    async def get_first(cls, mx_room: RoomID) -> Message | None:
+        q = "SELECT mxid, mx_room, twid, receiver FROM message WHERE mx_room=$1 ORDER BY twid ASC LIMIT 1"
+        row = await cls.db.fetchrow(q, mx_room)
+        if not row:
+            return None
+        return cls(**row)
+
+    @classmethod
     async def get_by_twid(cls, twid: int, receiver: int = 0) -> Message | None:
         q = "SELECT mxid, mx_room, twid, receiver FROM message WHERE twid=$1 AND receiver=$2"
         row = await cls.db.fetchrow(q, twid, receiver)
         if not row:
             return None
         return cls(**row)
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/db/portal.py` & `mautrix-twitter-0.1.6/mautrix_twitter/db/portal.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,87 +34,89 @@
     twid: str
     receiver: int
     conv_type: ConversationType
     other_user: int | None
     mxid: RoomID | None
     name: str | None
     encrypted: bool
+    next_batch_id: str | None
 
     @property
     def _values(self):
         return (
             self.twid,
             self.receiver,
             self.conv_type.value,
             self.other_user,
             self.mxid,
             self.name,
             self.encrypted,
+            self.next_batch_id,
         )
 
     async def insert(self) -> None:
         q = (
-            "INSERT INTO portal (twid, receiver, conv_type, other_user, mxid, name, encrypted) "
-            "VALUES ($1, $2, $3, $4, $5, $6, $7)"
+            "INSERT INTO portal (twid, receiver, conv_type, other_user, mxid, name, encrypted, next_batch_id) "
+            "VALUES ($1, $2, $3, $4, $5, $6, $7, $8)"
         )
         await self.db.execute(q, *self._values)
 
     async def update(self) -> None:
         q = (
-            "UPDATE portal SET conv_type=$3, other_user=$4, mxid=$5, name=$6, encrypted=$7 "
+            "UPDATE portal SET conv_type=$3, other_user=$4, mxid=$5, name=$6, encrypted=$7, next_batch_id=$8 "
             "WHERE twid=$1 AND receiver=$2"
         )
         await self.db.execute(q, *self._values)
 
     @classmethod
     def _from_row(cls, row: asyncpg.Record) -> "Portal":
         data = {**row}
         return cls(conv_type=ConversationType(data.pop("conv_type")), **data)
 
     @classmethod
     async def get_by_mxid(cls, mxid: RoomID) -> Portal | None:
         q = (
-            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted "
+            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted, next_batch_id "
             "FROM portal WHERE mxid=$1"
         )
         row = await cls.db.fetchrow(q, mxid)
         if not row:
             return None
         return cls._from_row(row)
 
     @classmethod
     async def get_by_twid(cls, twid: str, receiver: int = 0) -> Portal | None:
         q = (
-            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted "
+            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted, next_batch_id "
             "FROM portal WHERE twid=$1 AND receiver=$2"
         )
         row = await cls.db.fetchrow(q, twid, receiver)
         if not row:
             return None
         return cls._from_row(row)
 
     @classmethod
     async def find_private_chats_of(cls, receiver: int) -> list[Portal]:
         q = (
-            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted FROM portal "
+            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted, next_batch_id FROM portal "
             "WHERE receiver=$1 AND conv_type='ONE_TO_ONE'"
         )
         rows = await cls.db.fetch(q, receiver)
         return [cls._from_row(row) for row in rows]
 
     @classmethod
     async def find_private_chats_with(cls, other_user: int) -> list[Portal]:
         q = (
-            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted FROM portal "
+            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted, next_batch_id FROM portal "
             "WHERE other_user=$1 AND conv_type='ONE_TO_ONE'"
         )
         rows = await cls.db.fetch(q, other_user)
         return [cls._from_row(row) for row in rows]
 
     @classmethod
     async def all_with_room(cls) -> list[Portal]:
         q = (
-            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted FROM portal "
+            "SELECT twid, receiver, conv_type, other_user, mxid, name, encrypted, next_batch_id FROM portal "
             "WHERE mxid IS NOT NULL"
         )
         rows = await cls.db.fetch(q)
         return [cls._from_row(row) for row in rows]
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/db/puppet.py` & `mautrix-twitter-0.1.6/mautrix_twitter/db/puppet.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,72 +39,68 @@
     is_registered: bool
 
     custom_mxid: UserID | None
     access_token: str | None
     next_batch: SyncToken | None
     base_url: URL | None
 
+    contact_info_set: bool
+
     @property
     def _values(self):
         return (
             self.twid,
             self.name,
             self.photo_url,
             self.photo_mxc,
             self.is_registered,
             self.custom_mxid,
             self.access_token,
             self.next_batch,
             str(self.base_url) if self.base_url else None,
+            self.contact_info_set,
         )
 
+    columns: ClassVar[str] = (
+        "twid, name, photo_url, photo_mxc, is_registered, custom_mxid, access_token, next_batch, "
+        "base_url, contact_info_set"
+    )
+
     async def insert(self) -> None:
-        q = (
-            "INSERT INTO puppet (twid, name, photo_url, photo_mxc, is_registered, custom_mxid,"
-            "                    access_token, next_batch, base_url) "
-            "VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9)"
-        )
+        q = f"""
+            INSERT INTO puppet ({self.columns})
+            VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10)
+        """
         await self.db.execute(q, *self._values)
 
     async def update(self) -> None:
-        q = (
-            "UPDATE puppet SET name=$2, photo_url=$3, photo_mxc=$4, is_registered=$5,"
-            "                  custom_mxid=$6, access_token=$7, next_batch=$8, base_url=$9 "
-            "WHERE twid=$1"
-        )
+        q = """
+            UPDATE puppet
+            SET name=$2, photo_url=$3, photo_mxc=$4, is_registered=$5, custom_mxid=$6,
+                access_token=$7, next_batch=$8, base_url=$9, contact_info_set=$10
+            WHERE twid=$1
+        """
         await self.db.execute(q, *self._values)
 
     @classmethod
     def _from_row(cls, row: asyncpg.Record) -> Puppet | None:
         if not row:
             return None
         data = {**row}
         base_url_str = data.pop("base_url")
         base_url = URL(base_url_str) if base_url_str is not None else None
         return cls(base_url=base_url, **data)
 
     @classmethod
     async def get_by_twid(cls, twid: int) -> Puppet | None:
-        q = (
-            "SELECT twid, name, photo_url, photo_mxc, is_registered,"
-            "       custom_mxid, access_token, next_batch, base_url "
-            "FROM puppet WHERE twid=$1"
-        )
+        q = f"SELECT {cls.columns} FROM puppet WHERE twid=$1"
         return cls._from_row(await cls.db.fetchrow(q, twid))
 
     @classmethod
     async def get_by_custom_mxid(cls, mxid: UserID) -> Puppet | None:
-        q = (
-            "SELECT twid, name, photo_url, photo_mxc, is_registered,"
-            "       custom_mxid, access_token, next_batch, base_url "
-            "FROM puppet WHERE custom_mxid=$1"
-        )
+        q = f"SELECT {cls.columns} FROM puppet WHERE custom_mxid=$1"
         return cls._from_row(await cls.db.fetchrow(q, mxid))
 
     @classmethod
     async def all_with_custom_mxid(cls) -> list[Puppet]:
-        q = (
-            "SELECT twid, name, photo_url, photo_mxc, is_registered,"
-            "       custom_mxid, access_token, next_batch, base_url "
-            "FROM puppet WHERE custom_mxid IS NOT NULL"
-        )
+        q = f"SELECT {cls.columns} FROM puppet WHERE custom_mxid IS NOT NULL"
         return [cls._from_row(row) for row in await cls.db.fetch(q)]
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/db/reaction.py` & `mautrix-twitter-0.1.6/mautrix_twitter/db/reaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,69 +32,67 @@
     db: ClassVar[Database] = fake_db
 
     mxid: EventID
     mx_room: RoomID
     tw_msgid: int
     tw_receiver: int
     tw_sender: int
-    reaction: ReactionKey
+    reaction: str
     tw_reaction_id: int
 
     async def insert(self) -> None:
         q = (
             "INSERT INTO reaction (mxid, mx_room, tw_msgid, tw_receiver, tw_sender, reaction, tw_reaction_id) "
             "VALUES ($1, $2, $3, $4, $5, $6, $7)"
         )
         await self.db.execute(
             q,
             self.mxid,
             self.mx_room,
             self.tw_msgid,
             self.tw_receiver,
             self.tw_sender,
-            self.reaction.value,
+            self.reaction,
             self.tw_reaction_id,
         )
 
     async def update_id(self, tw_reaction_id: int) -> None:
         q = (
             "UPDATE reaction SET tw_reaction_id=$1 "
             "WHERE tw_msgid=$4 AND tw_receiver=$5 AND tw_sender=$6"
         )
         await self.db.execute(q, tw_reaction_id, self.tw_msgid, self.tw_receiver, self.tw_sender)
 
     async def edit(
-        self, mx_room: RoomID, mxid: EventID, reaction: ReactionKey, tw_reaction_id: int | None
+        self, mx_room: RoomID, mxid: EventID, reaction: str, tw_reaction_id: int | None
     ) -> None:
         q = (
             "UPDATE reaction SET mxid=$1, mx_room=$2, reaction=$3, tw_reaction_id=$7 "
             "WHERE tw_msgid=$4 AND tw_receiver=$5 AND tw_sender=$6"
         )
         await self.db.execute(
             q,
             mxid,
             mx_room,
-            reaction.value,
+            reaction,
             self.tw_msgid,
             self.tw_receiver,
             self.tw_sender,
             tw_reaction_id,
         )
 
     async def delete(self) -> None:
         q = "DELETE FROM reaction WHERE tw_msgid=$1 AND tw_receiver=$2 AND tw_sender=$3"
         await self.db.execute(q, self.tw_msgid, self.tw_receiver, self.tw_sender)
 
     @classmethod
     def _from_row(cls, row: asyncpg.Record) -> Reaction | None:
         if not row:
             return None
-        data = {**row}
-        reaction = ReactionKey(data.pop("reaction"))
-        return cls(reaction=reaction, **data)
+        return cls(**row)
 
     @classmethod
     async def get_by_mxid(cls, mxid: EventID, mx_room: RoomID) -> Reaction | None:
         q = (
             "SELECT mxid, mx_room, tw_msgid, tw_receiver, tw_sender, reaction, tw_reaction_id "
             "FROM reaction WHERE mxid=$1 AND mx_room=$2"
         )
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/db/user.py` & `mautrix-twitter-0.1.6/mautrix_twitter/db/user.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/example-config.yaml` & `mautrix-twitter-0.1.6/mautrix_twitter/example-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,17 @@
     # The address that this appservice can use to connect to the homeserver.
     address: https://example.com
     # The domain of the homeserver (for MXIDs, etc).
     domain: example.com
     # Whether or not to verify the SSL certificate of the homeserver.
     # Only applies if address starts with https://
     verify_ssl: true
-    asmux: false
+    # What software is the homeserver running?
+    # Standard Matrix homeservers like Synapse, Dendrite and Conduit should just use "standard" here.
+    software: standard
     # Number of retries for all HTTP requests if the homeserver isn't reachable.
     http_retry_count: 4
     # The URL to push real-time bridge status to.
     # If set, the bridge will make POST requests to this URL whenever a user's Twitter connection state changes.
     # The bridge will use the appservice as_token to authorize requests.
     status_endpoint: null
     # Endpoint for reporting per-message status.
@@ -32,20 +34,26 @@
     # The hostname and port where this appservice should listen.
     hostname: 0.0.0.0
     port: 29327
     # The maximum body size of appservice API requests (from the homeserver) in mebibytes
     # Usually 1 is enough, but on high-traffic bridges you might need to increase this to avoid 413s
     max_body_size: 1
 
-    # The full URI to the database. Only Postgres is currently supported.
+    # The full URI to the database. SQLite and Postgres are supported.
+    # Format examples:
+    #   SQLite:   sqlite:///filename.db
+    #   Postgres: postgres://username:password@hostname/dbname
     database: postgres://username:password@hostname/db
-    # Additional arguments for asyncpg.create_pool()
+    # Additional arguments for asyncpg.create_pool() or sqlite3.connect()
     # https://magicstack.github.io/asyncpg/current/api/index.html#asyncpg.pool.create_pool
+    # https://docs.python.org/3/library/sqlite3.html#sqlite3.connect
+    # For sqlite, min_size is used as the connection thread pool size and max_size is ignored.
+    # Additionally, SQLite supports init_commands as an array of SQL queries to run on connect (e.g. to set PRAGMAs).
     database_opts:
-        min_size: 5
+        min_size: 1
         max_size: 10
 
     # Provisioning API part of the web server for automated portal creation and fetching information.
     # Used by things like mautrix-manager (https://github.com/tulir/mautrix-manager).
     provisioning:
         # Whether or not the provisioning API should be enabled.
         enabled: true
@@ -108,14 +116,19 @@
     # Whether or not to use /sync to get read receipts and typing notifications
     # when double puppeting is enabled
     sync_with_custom_puppets: false
     # Whether or not to update the m.direct account data event when double puppeting is enabled.
     # Note that updating the m.direct event is not atomic (except with mautrix-asmux)
     # and is therefore prone to race conditions.
     sync_direct_chat_list: false
+    # When using double puppeting, should low quality DMs be moved to a specific tag in Matrix?
+    # The low priority tag is `m.lowpriority`.
+    low_quality_tag: null
+    # When using double puppeting, mute low quality DMs (by changing the user's push rules)?
+    low_quality_mute: false
     # Allow using double puppeting from any server with a valid client .well-known file.
     double_puppet_allow_discovery: false
     # Servers to allow double puppeting from, even if double_puppet_allow_discovery is false.
     double_puppet_server_map:
         example.com: https://example.com
     # Shared secret for https://github.com/devture/matrix-synapse-shared-secret-auth
     #
@@ -141,28 +154,49 @@
         invite_own_puppet: true
         # Maximum number of messages to backfill initially.
         # Set to 0 to disable backfilling when creating portal.
         initial_limit: 0
         # If using double puppeting, should notifications be disabled
         # while the initial backfill is in progress?
         disable_notifications: false
+        # Backfill backwards after the initial batch (requires MSC2716 support on homeserver)
+        backwards: false
     # End-to-bridge encryption support options.
     #
     # See https://docs.mau.fi/bridges/general/end-to-bridge-encryption.html for more info.
     encryption:
         # Allow encryption, work in group chat rooms with e2ee enabled
         allow: false
         # Default to encryption, force-enable encryption in all portals the bridge creates
         # This will cause the bridge bot to be in private chats for the encryption to work properly.
         default: false
+        # Whether to use MSC2409/MSC3202 instead of /sync long polling for receiving encryption-related data.
+        appservice: false
         # Require encryption, drop any unencrypted messages.
         require: false
         # Enable key sharing? If enabled, key requests for rooms where users are in will be fulfilled.
         # You must use a client that supports requesting keys from other users to use this feature.
         allow_key_sharing: false
+        # Options for deleting megolm sessions from the bridge.
+        delete_keys:
+            # Beeper-specific: delete outbound sessions when hungryserv confirms
+            # that the user has uploaded the key to key backup.
+            delete_outbound_on_ack: false
+            # Don't store outbound sessions in the inbound table.
+            dont_store_outbound: false
+            # Ratchet megolm sessions forward after decrypting messages.
+            ratchet_on_decrypt: false
+            # Delete fully used keys (index >= max_messages) after decrypting messages.
+            delete_fully_used_on_decrypt: false
+            # Delete previous megolm sessions from same device when receiving a new one.
+            delete_prev_on_new_session: false
+            # Delete megolm sessions received from a device when the device is deleted.
+            delete_on_device_delete: false
+            # Periodically delete megolm sessions when 2x max_age has passed since receiving the session.
+            periodically_delete_expired: false
         # What level of device verification should be required from users?
         #
         # Valid levels:
         #   unverified - Send keys to all device in the room.
         #   cross-signed-untrusted - Require valid cross-signing, but trust all cross-signing keys.
         #   cross-signed-tofu - Require valid cross-signing, trust cross-signing keys on first use (and reject changes).
         #   cross-signed-verified - Require valid cross-signing, plus a valid user signature from the bridge bot.
@@ -190,17 +224,19 @@
             # as the default.
             milliseconds: 604800000
             # The maximum number of messages that should be sent with a given a
             # session before changing it. The Matrix spec recommends 100 as the
             # default.
             messages: 100
 
-    # Whether or not to explicitly set the avatar and room name for private
-    # chat portal rooms. This will be implicitly enabled if encryption.default is true.
-    private_chat_portal_meta: false
+    # Whether to explicitly set the avatar and room name for private chat portal rooms.
+    # If set to `default`, this will be enabled in encrypted rooms and disabled in unencrypted rooms.
+    # If set to `always`, all DM rooms will have explicit names and avatars set.
+    # If set to `never`, DM rooms will never have names and avatars set.
+    private_chat_portal_meta: default
     # Whether or not the bridge should send a read receipt from the bridge bot when a message has
     # been sent to Twitter.
     delivery_receipts: false
     # Whether or not delivery errors should be reported as messages in the Matrix room.
     delivery_error_reports: true
     # Whether the bridge should send the message status as a custom com.beeper.message_send_status event.
     message_status_events: false
@@ -213,14 +249,17 @@
     error_sleep: 5
     # Maximum number of polling errors before giving up. Set to -1 to retry forever.
     max_poll_errors: 12
     # Set this to true to tell the bridge to re-send m.bridge events to all rooms on the next run.
     # This field will automatically be changed back to false after it,
     # except if the config file is not writable.
     resend_bridge_info: false
+    # Send captions in the same message as images. This will send data compatible with MSC2530.
+    # This is currently not supported in most clients.
+    caption_in_message: false
 
     # The prefix for commands. Only required in non-management rooms.
     command_prefix: "!tw"
 
     # Permissions for using the bridge.
     # Permitted values:
     #       user - Use the bridge with puppeting.
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/formatter.py` & `mautrix-twitter-0.1.6/mautrix_twitter/formatter.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/get_version.py` & `mautrix-twitter-0.1.6/mautrix_twitter/get_version.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/matrix.py` & `mautrix-twitter-0.1.6/mautrix_twitter/matrix.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/portal.py` & `mautrix-twitter-0.1.6/mautrix_twitter/portal.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,75 +11,91 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, NamedTuple, cast
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Literal, NamedTuple, Tuple, cast
 from collections import deque
-from datetime import datetime
+from datetime import datetime, timedelta
 import asyncio
+import base64
+import hashlib
+import time
 
 from yarl import URL
 import magic
 
-from mautrix.appservice import AppService, IntentAPI
+from mautrix.appservice import DOUBLE_PUPPET_SOURCE_KEY, AppService, IntentAPI
 from mautrix.bridge import BasePortal, NotificationDisabler, async_getter_lock
 from mautrix.errors import MatrixError, MForbidden
 from mautrix.types import (
+    AudioInfo,
+    BatchSendEvent,
+    BatchSendStateEvent,
     BeeperMessageStatusEventContent,
     ContentURI,
     EncryptedFile,
     EventID,
     EventType,
     ImageInfo,
     MediaMessageEventContent,
+    Membership,
+    MemberStateEventContent,
     MessageEventContent,
     MessageStatus,
     MessageStatusReason,
     MessageType,
+    ReactionEventContent,
     RelatesTo,
     RelationType,
     RoomID,
     TextMessageEventContent,
     ThumbnailInfo,
     VideoInfo,
 )
+from mautrix.util import background_task, ffmpeg, variation_selector
 from mautrix.util.message_send_checkpoint import MessageSendCheckpointStatus
 from mautrix.util.simple_lock import SimpleLock
 from mautwitdm.types import (
     Conversation,
     ConversationType,
-    ImageBindingValue,
     MessageData,
     MessageEntry,
     Participant,
     ReactionCreateEntry,
-    ReactionDeleteEntry,
-    ReactionKey,
-    TimelineStatus,
     VideoVariant,
 )
 
-from . import matrix as m, puppet as p, user as u
+from . import backfill as b, matrix as m, puppet as p, user as u
 from .config import Config
-from .db import Message as DBMessage, Portal as DBPortal, Reaction as DBReaction
+from .db import (
+    BackfillStatus as DBBackfillStatus,
+    Message as DBMessage,
+    Portal as DBPortal,
+    Reaction as DBReaction,
+)
 from .formatter import twitter_to_matrix
 
 if TYPE_CHECKING:
     from .__main__ import TwitterBridge
 
 try:
     from mautrix.crypto.attachments import decrypt_attachment, encrypt_attachment
 except ImportError:
     encrypt_attachment = decrypt_attachment = None
 
 StateBridge = EventType.find("m.bridge", EventType.Class.STATE)
 StateHalfShotBridge = EventType.find("uk.half-shot.bridge", EventType.Class.STATE)
+StateMarker = EventType.find("org.matrix.msc2716.marker", EventType.Class.STATE)
+
+
+class UnsupportedAttachmentError(NotImplementedError):
+    pass
 
 
 class ReuploadedMediaInfo(NamedTuple):
     mxc: ContentURI | None
     decryption_info: EncryptedFile | None
     mime_type: str
     file_name: str
@@ -88,38 +104,48 @@
 
 class Portal(DBPortal, BasePortal):
     by_mxid: dict[RoomID, Portal] = {}
     by_twid: dict[tuple[str, int], Portal] = {}
     config: Config
     matrix: "m.MatrixHandler"
     az: AppService
-    private_chat_portal_meta: bool
+    private_chat_portal_meta: Literal["default", "always", "never"]
 
     _main_intent: IntentAPI | None
     _create_room_lock: asyncio.Lock
     backfill_lock: SimpleLock
     _msgid_dedup: deque[int]
     _reqid_dedup: set[str]
-    _reaction_dedup: deque[tuple[int, int, ReactionKey]]
+    _reaction_dedup: deque[tuple[int, int, str]]
 
     _main_intent: IntentAPI
     _last_participant_update: set[int]
     _reaction_lock: asyncio.Lock
 
     def __init__(
         self,
         twid: str,
         receiver: int,
         conv_type: ConversationType,
         other_user: int | None = None,
         mxid: RoomID | None = None,
         name: str | None = None,
         encrypted: bool = False,
+        next_batch_id: str | None = None,
     ) -> None:
-        super().__init__(twid, receiver, conv_type, other_user, mxid, name, encrypted)
+        super().__init__(
+            twid,
+            receiver,
+            conv_type,
+            other_user,
+            mxid,
+            name,
+            encrypted,
+            next_batch_id,
+        )
         self._create_room_lock = asyncio.Lock()
         self.log = self.log.getChild(twid)
         self._msgid_dedup = deque(maxlen=100)
         self._reaction_dedup = deque(maxlen=100)
         self._reqid_dedup = set()
         self._last_participant_update = set()
 
@@ -130,14 +156,22 @@
         self._reaction_lock = asyncio.Lock()
 
     @property
     def is_direct(self) -> bool:
         return self.conv_type == ConversationType.ONE_TO_ONE
 
     @property
+    def set_dm_room_metadata(self) -> bool:
+        return (
+            not self.is_direct
+            or self.private_chat_portal_meta == "always"
+            or (self.encrypted and self.private_chat_portal_meta != "never")
+        )
+
+    @property
     def main_intent(self) -> IntentAPI:
         if not self._main_intent:
             raise ValueError("Portal must be postinit()ed before main_intent can be used")
         return self._main_intent
 
     @classmethod
     def init_cls(cls, bridge: "TwitterBridge") -> None:
@@ -162,15 +196,15 @@
     async def _upsert_reaction(
         self,
         existing: DBReaction | None,
         intent: IntentAPI,
         mxid: EventID,
         message: DBMessage,
         sender: u.User | p.Puppet,
-        reaction: ReactionKey,
+        reaction: str,
         reaction_id: int | None = None,
     ) -> None:
         if existing:
             self.log.debug(
                 f"_upsert_reaction redacting {existing.mxid} and inserting {mxid}"
                 f" (message: {message.mxid})"
             )
@@ -203,15 +237,15 @@
         sender.send_remote_checkpoint(
             status=MessageSendCheckpointStatus.SUCCESS,
             event_id=event_id,
             room_id=self.mxid,
             event_type=event_type,
             message_type=msgtype,
         )
-        asyncio.create_task(self._send_message_status(event_id, err=None))
+        background_task.create(self._send_message_status(event_id, err=None))
         await self._send_delivery_receipt(event_id)
 
     async def _send_bridge_error(
         self,
         sender: u.User,
         err: Exception,
         event_id: EventID,
@@ -236,15 +270,15 @@
             await self._send_message(
                 self.main_intent,
                 TextMessageEventContent(
                     msgtype=MessageType.NOTICE,
                     body=f"\u26a0 Your {event_type_str} may not have been bridged: {str(err)}",
                 ),
             )
-        asyncio.create_task(self._send_message_status(event_id, err))
+        background_task.create(self._send_message_status(event_id, err))
 
     async def _send_message_status(self, event_id: EventID, err: Exception | None) -> None:
         if not self.config["bridge.message_status_events"]:
             return
         intent = self.az.intent if self.encrypted else self.main_intent
         status = BeeperMessageStatusEventContent(
             network=self.bridge_info_state_key,
@@ -254,19 +288,20 @@
             ),
         )
         if err:
             status.status = MessageStatus.RETRIABLE
             status.reason = MessageStatusReason.GENERIC_ERROR
             status.error = str(err)
             if isinstance(err, NotImplementedError):
+                if isinstance(err, UnsupportedAttachmentError):
+                    status.message = str(err)
                 status.status = MessageStatus.FAIL
                 status.reason = MessageStatusReason.UNSUPPORTED
         else:
             status.status = MessageStatus.SUCCESS
-        status.fill_legacy_booleans()
 
         await intent.send_message_event(
             room_id=self.mxid,
             event_type=EventType.BEEPER_MESSAGE_STATUS,
             content=status,
         )
 
@@ -300,55 +335,68 @@
         self._reqid_dedup.add(request_id)
         media_id = None
         if message.msgtype == MessageType.TEXT:
             text = message.body
         elif message.msgtype == MessageType.EMOTE:
             text = f"/me {message.body}"
         elif message.msgtype.is_media:
+            if message.msgtype != MessageType.IMAGE and message.msgtype != MessageType.VIDEO:
+                raise UnsupportedAttachmentError(
+                    "Non-image/video files are not supported by Twitter"
+                )
             if message.file and decrypt_attachment:
                 data = await self.main_intent.download_media(message.file.url)
                 data = decrypt_attachment(
                     data,
                     message.file.key.key,
                     message.file.hashes.get("sha256"),
                     message.file.iv,
                 )
             else:
                 data = await self.main_intent.download_media(message.url)
             mime_type = message.info.mimetype or magic.from_buffer(data, mime=True)
             upload_resp = await sender.client.upload(data, mime_type=mime_type)
             media_id = upload_resp.media_id
-            text = ""
+            filename = message.get("filename", None)
+            if filename and filename != message.body:
+                text = message.body
+            else:
+                text = ""
         else:
             raise NotImplementedError(f"unsupported msgtype '{message.msgtype.value}'")
+        reply_to = None
+        if message.get_reply_to():
+            reply_to_msg = await DBMessage.get_by_mxid(message.get_reply_to(), self.mxid)
+            if reply_to_msg:
+                reply_to = reply_to_msg.twid
         resp = await sender.client.conversation(self.twid).send(
-            text, media_id=media_id, request_id=request_id
+            text, media_id=media_id, request_id=request_id, reply_to_id=reply_to
         )
         resp_msg_id = int(resp.entries[0].message.id)
         self._msgid_dedup.appendleft(resp_msg_id)
         msg = DBMessage(mxid=event_id, mx_room=self.mxid, twid=resp_msg_id, receiver=self.receiver)
         await msg.insert()
         self._reqid_dedup.remove(request_id)
         self.log.debug(f"Handled Matrix message {event_id} -> {resp_msg_id}")
 
     async def handle_matrix_reaction(
-        self, sender: u.User, event_id: EventID, reacting_to: EventID, reaction_val: str
+        self, sender: u.User, event_id: EventID, reacting_to: EventID, reaction: str
     ) -> None:
         try:
-            await self._handle_matrix_reaction(sender, event_id, reacting_to, reaction_val)
+            await self._handle_matrix_reaction(sender, event_id, reacting_to, reaction)
         except Exception as e:
             self.log.exception(f"Failed to react to {event_id}")
             await self._send_bridge_error(sender, e, event_id, EventType.REACTION)
         else:
             await self._send_bridge_success(sender, event_id, EventType.REACTION)
 
     async def _handle_matrix_reaction(
-        self, sender: u.User, event_id: EventID, reacting_to: EventID, reaction_val: str
+        self, sender: u.User, event_id: EventID, reacting_to: EventID, reaction: str
     ) -> None:
-        reaction = ReactionKey.from_emoji(reaction_val)
+        reaction = variation_selector.remove(reaction)
         message = await DBMessage.get_by_mxid(reacting_to, self.mxid)
         if not message:
             raise NotImplementedError(f"Unknown reaction target event")
 
         async with self._reaction_lock:
             dedup_id = (message.twid, sender.twid, reaction)
             self._reaction_dedup.appendleft(dedup_id)
@@ -403,52 +451,89 @@
 
     # endregion
     # region Twitter event handling
 
     async def handle_twitter_message(
         self, source: u.User, sender: p.Puppet, message: MessageData, request_id: str
     ) -> None:
+        if await self._twitter_message_dedupe(request_id, int(message.id), message.sender_id):
+            await self._handle_deduplicated_twitter_message(
+                source, sender, message, int(message.id)
+            )
+
+    async def _twitter_message_dedupe(self, request_id: str, msg_id: int, sender_id: str) -> bool:
         if request_id in self._reqid_dedup:
             self.log.debug(
-                f"Ignoring message {message.id} by {message.sender_id}"
+                f"Ignoring message {msg_id} by {sender_id}"
                 " as it was sent by us (request_id in dedup queue)"
             )
-            return
-        msg_id = int(message.id)
+            return False
         if msg_id in self._msgid_dedup:
             self.log.debug(
-                f"Ignoring message {message.id} by {message.sender_id}"
+                f"Ignoring message {msg_id} by {sender_id}"
                 " as it was already handled (message.id in dedup queue)"
             )
-            return
+            return False
         self._msgid_dedup.appendleft(msg_id)
 
         if await DBMessage.get_by_twid(msg_id, self.receiver) is not None:
             self.log.debug(
-                f"Ignoring message {message.id} by {message.sender_id}"
+                f"Ignoring message {msg_id} by {sender_id}"
                 " as it was already handled (message.id found in database)"
             )
-            return
+            return False
 
-        await self._handle_deduplicated_twitter_message(source, sender, message, msg_id)
+        return True
 
-    async def _handle_deduplicated_twitter_message(
-        self, source: u.User, sender: p.Puppet, message: MessageData, msg_id: int
-    ) -> None:
+    def deterministic_event_id(self, msg_id: str, part: str) -> EventID:
+        hash_content = f"{self.mxid}/twitter/{msg_id}/{part}"
+        hashed = hashlib.sha256(hash_content.encode("utf-8")).digest()
+        b64hash = base64.urlsafe_b64encode(hashed).decode("utf-8").rstrip("=")
+        return EventID(f"${b64hash}:twitter.com")
+
+    async def _convert_twitter_message(
+        self, source: u.User, sender: p.Puppet, message: MessageData
+    ) -> list[MessageEventContent]:
+        converted = []
         intent = sender.intent_for(self)
-        event_id = None
+        if message.reply_data:
+            reply_to_msg = await DBMessage.get_by_twid(int(message.reply_data.id), self.receiver)
+        else:
+            reply_to_msg = None
+        media_content = None
         if message.attachment and message.attachment.media:
-            content = await self._handle_twitter_media(source, intent, message)
-            if content:
-                event_id = await self._send_message(intent, content, timestamp=message.time)
+            media_content = await self._handle_twitter_media(source, intent, message)
+            if media_content:
+                if reply_to_msg:
+                    media_content.set_reply(reply_to_msg.mxid)
+                converted.append(media_content)
         if message.text and not message.text.isspace():
-            content = await twitter_to_matrix(message)
-            content["com.beeper.linkpreviews"] = await self._twitter_preview_to_beeper(
+            text_content = await twitter_to_matrix(message)
+            text_content["com.beeper.linkpreviews"] = await self._twitter_preview_to_beeper(
                 source, intent, message
             )
+            if reply_to_msg:
+                text_content.set_reply(reply_to_msg.mxid)
+            if media_content and self.config["bridge.caption_in_message"]:
+                media_content["filename"] = media_content.body
+                media_content.body = text_content.body
+                if text_content.formatted_body:
+                    media_content["format"] = str(text_content.format)
+                    media_content["formatted_body"] = text_content.formatted_body
+            else:
+                converted.append(text_content)
+        return converted
+
+    async def _handle_deduplicated_twitter_message(
+        self, source: u.User, sender: p.Puppet, message: MessageData, msg_id: int
+    ) -> None:
+        intent = sender.intent_for(self)
+        event_id = None
+        converted = await self._convert_twitter_message(source, sender, message)
+        for content in converted:
             event_id = await self._send_message(intent, content, timestamp=message.time)
         if event_id:
             msg = DBMessage(
                 mxid=event_id,
                 mx_room=self.mxid,
                 twid=msg_id,
                 receiver=self.receiver,
@@ -567,22 +652,39 @@
             for variant in media.video_info.variants:
                 if (
                     not best_variant
                     or (variant.bitrate or 0) > (best_variant.bitrate or 0)
                     or self._is_better_mime(best_variant, variant)
                 ):
                     best_variant = variant
-            reuploaded_info = await self._reupload_twitter_media(source, best_variant.url, intent)
+            reuploaded_info = await self._reupload_twitter_media(
+                source, best_variant.url, intent, convert_to_audio=media.audio_only
+            )
         content = MediaMessageEventContent(
             body=reuploaded_info.file_name,
             url=reuploaded_info.mxc,
             file=reuploaded_info.decryption_info,
             external_url=media.media_url_https,
         )
-        if message.attachment.video or (
+        if message.attachment.video and message.attachment.video.audio_only:
+            content.msgtype = MessageType.AUDIO
+            content.info = AudioInfo(
+                mimetype=reuploaded_info.mime_type,
+                size=reuploaded_info.size,
+                duration=media.video_info.duration_millis or None,
+            )
+            content["org.matrix.msc1767.audio"] = (
+                {
+                    "duration": content.info.duration,
+                }
+                if content.info.duration
+                else {}
+            )
+            content["org.matrix.msc3245.voice"] = {}
+        elif message.attachment.video or (
             message.attachment.animated_gif and reuploaded_info.mime_type.startswith("video/")
         ):
             content.msgtype = MessageType.VIDEO
             content.info = VideoInfo(
                 mimetype=reuploaded_info.mime_type,
                 size=reuploaded_info.size,
                 width=media.original_info.width,
@@ -610,22 +712,34 @@
                 size=thumbnail_info.size,
                 width=media.original_info.width,
                 height=media.original_info.height,
             )
         # Remove the attachment link from message.text
         start, end = media.indices
         message.text = message.text[:start] + message.text[end:]
+        if message.entities and message.entities.urls:
+            message.entities.urls = [u for u in message.entities.urls if u.url != media.url]
         return content
 
     async def _reupload_twitter_media(
-        self, source: u.User, url: str, intent: IntentAPI
+        self, source: u.User, url: str, intent: IntentAPI, convert_to_audio: bool = False
     ) -> ReuploadedMediaInfo:
         file_name = URL(url).name
         data, mime_type = await source.client.download_media(url)
 
+        if convert_to_audio and (mime_type.startswith("video/") or mime_type.startswith("audio/")):
+            data = await ffmpeg.convert_bytes(
+                data,
+                ".ogg",
+                output_args=("-c:a", "libopus"),
+                input_mime=mime_type,
+            )
+            mime_type = "audio/ogg"
+            file_name += ".ogg"
+
         upload_mime_type = mime_type
         upload_file_name = file_name
         decryption_info = None
         if self.encrypted and encrypt_attachment:
             data, decryption_info = encrypt_attachment(data)
             upload_mime_type = "application/octet-stream"
             upload_file_name = None
@@ -643,46 +757,58 @@
 
         return ReuploadedMediaInfo(mxc, decryption_info, mime_type, file_name, len(data))
 
     async def handle_twitter_reaction_add(
         self,
         sender: p.Puppet,
         msg_id: int,
-        reaction: ReactionKey,
+        emoji: str,
         time: datetime,
         reaction_id: int,
     ) -> None:
         async with self._reaction_lock:
             # TODO update the database with the reaction_id of outgoing reactions
-            dedup_id = (msg_id, sender.twid, reaction)
+            dedup_id = (msg_id, sender.twid, emoji)
             if dedup_id in self._reaction_dedup:
+                self.log.debug(
+                    f"Ignoring duplicate reaction from {sender.twid} to {msg_id} (dedup queue)"
+                )
                 return
             self._reaction_dedup.appendleft(dedup_id)
 
         existing = await DBReaction.get_by_message_twid(msg_id, self.receiver, sender.twid)
-        if existing and existing.reaction == reaction:
+        if existing and existing.reaction == emoji:
             if not existing.tw_reaction_id:
                 await existing.update_id(reaction_id)
+            self.log.debug(
+                f"Ignoring duplicate reaction from {sender.twid} to {msg_id} (database)"
+            )
             return
 
         message = await DBMessage.get_by_twid(msg_id, self.receiver)
         if not message:
             self.log.debug(f"Ignoring reaction to unknown message {msg_id}")
             return
 
         intent = sender.intent_for(self)
-        mxid = await intent.react(message.mx_room, message.mxid, reaction.emoji, timestamp=time)
-        self.log.debug(f"{sender.twid} reacted to {message.mxid} -> {mxid}")
-        await self._upsert_reaction(existing, intent, mxid, message, sender, reaction, reaction_id)
+        mxid = await intent.react(
+            message.mx_room, message.mxid, variation_selector.add(emoji), timestamp=time
+        )
+        self.log.debug(f"{sender.twid} reacted to {msg_id}/{message.mxid} -> {mxid}")
+        await self._upsert_reaction(existing, intent, mxid, message, sender, emoji, reaction_id)
 
     async def handle_twitter_reaction_remove(
-        self, sender: p.Puppet, msg_id: int, key: ReactionKey
+        self, sender: p.Puppet, msg_id: int, emoji: str
     ) -> None:
         reaction = await DBReaction.get_by_message_twid(msg_id, self.receiver, sender.twid)
-        if reaction and reaction.reaction == key:
+        if reaction and reaction.reaction == emoji:
+            try:
+                self._reaction_dedup.remove((msg_id, sender.twid, emoji))
+            except ValueError:
+                pass
             try:
                 await sender.intent_for(self).redact(reaction.mx_room, reaction.mxid)
             except MForbidden:
                 await self.main_intent.redact(reaction.mx_room, reaction.mxid)
             await reaction.delete()
             self.log.debug(f"Removed {reaction} after Twitter removal")
 
@@ -706,47 +832,44 @@
 
     # endregion
     # region Updating portal info
 
     async def update_info(self, conv: Conversation) -> None:
         if self.conv_type == ConversationType.ONE_TO_ONE:
             if not self.other_user:
-                participant = next(
-                    pcp for pcp in conv.participants if int(pcp.user_id) != self.receiver
-                )
-                self.other_user = int(participant.user_id)
+                if len(conv.participants) == 1:
+                    self.other_user = int(conv.participants[0].user_id)
+                else:
+                    participant = next(
+                        pcp for pcp in conv.participants if int(pcp.user_id) != self.receiver
+                    )
+                    self.other_user = int(participant.user_id)
                 await self.update()
             puppet = await p.Puppet.get_by_twid(self.other_user)
             if not self._main_intent:
                 self._main_intent = puppet.default_mxid_intent
-            if self.encrypted or self.private_chat_portal_meta:
-                changed = await self._update_name(puppet.name)
-            else:
-                changed = False
+            changed = await self._update_name(puppet.name)
         else:
             changed = await self._update_name(conv.name)
         if changed:
             await self.update_bridge_info()
             await self.update()
         await self._update_participants(conv.participants)
 
     async def update_name(self, name: str) -> None:
-        if not self.encrypted and not self.private_chat_portal_meta:
-            return
-
         changed = await self._update_name(name)
 
         if changed:
             await self.update_bridge_info()
             await self.update()
 
     async def _update_name(self, name: str) -> bool:
         if self.name != name:
             self.name = name
-            if self.mxid:
+            if self.mxid and self.set_dm_room_metadata:
                 await self.main_intent.set_room_name(self.mxid, name)
             return True
         return False
 
     async def _update_participants(self, participants: list[Participant]) -> None:
         if not self.mxid:
             return
@@ -777,76 +900,125 @@
                     p.Puppet.get_mxid_from_id(twid),
                     reason="User had left this Twitter chat",
                 )
 
     # endregion
     # region Backfilling
 
-    async def backfill(self, source: u.User, is_initial: bool = False) -> None:
-        if not is_initial:
-            raise RuntimeError("Non-initial backfilling is not supported")
+    async def backfill(self, source: u.User, is_initial: bool = False) -> int:
         limit = self.config["bridge.backfill.initial_limit"]
         if limit == 0:
-            return
+            return 0
         elif limit < 0:
             limit = None
         with self.backfill_lock:
-            await self._backfill(source, limit)
+            return await self._backfill(source, limit, is_initial)
 
-    async def _backfill(self, source: u.User, limit: int) -> None:
-        self.log.debug("Backfilling history through %s", source.mxid)
+    async def _backfill(self, source: u.User, limit: int, is_initial: bool = False) -> int:
+        if is_initial:
+            self.log.debug("Backfilling initial batch through %s", source.mxid)
+        elif not self.config["bridge.backfill.backwards"]:
+            self.log.debug("Not backfilling history, disabled in config")
+            return 0
+        else:
+            self.log.debug("Backfilling history through %s", source.mxid)
+
+        first_message = await DBMessage.get_first(self.mxid)
+        max_id = None
+        if not is_initial:
+            if first_message is not None:
+                max_id = first_message.twid
+            else:
+                self.log.warn("Can't backfill without a first bridged message!")
+                raise b.NoFirstMessageException()
 
-        entries = await self._fetch_backfill_entries(source, limit)
+        mark_read, entries = await self._fetch_backfill_entries(source, limit, max_id)
         if not entries:
             self.log.debug("Didn't get any entries from server")
-            return
+            return 0
 
         self.log.debug("Got %d entries from server", len(entries))
 
-        backfill_leave = await self._invite_own_puppet_backfill(source)
-        async with NotificationDisabler(self.mxid, source):
-            for entry in reversed(entries):
-                await self._handle_backfill_entry(source, entry)
-        for intent in backfill_leave:
-            self.log.trace("Leaving room with %s post-backfill", intent.mxid)
-            await intent.leave_room(self.mxid)
-        self.log.info("Backfilled %d messages through %s", len(entries), source.mxid)
+        filled = 0
+        if self.config["bridge.backfill.backwards"]:
+            filled = await self._batch_handle_backfill(
+                source, reversed(entries), is_initial, mark_read
+            )
+        else:
+            backfill_leave = await self._invite_own_puppet_backfill(source)
+            async with NotificationDisabler(self.mxid, source):
+                for entry in reversed(entries):
+                    await self._handle_backfill_entry(source, entry)
+                    filled += 1
+            for intent in backfill_leave:
+                self.log.trace("Leaving room with %s post-backfill", intent.mxid)
+                await intent.leave_room(self.mxid)
+        self.log.info(
+            "Backfilled %d messages (%d events) through %s", len(entries), filled, source.mxid
+        )
+        return filled
 
     async def _fetch_backfill_entries(
-        self, source: u.User, limit: int
-    ) -> list[MessageEntry | ReactionCreateEntry]:
+        self, source: u.User, limit: int, max_id: int | None = None
+    ) -> tuple[bool, list[MessageEntry | ReactionCreateEntry]]:
         conv = source.client.conversation(self.twid)
         entries: list[MessageEntry | ReactionCreateEntry] = []
         message_count = 0
         self.log.debug("Fetching up to %d messages through %s", limit, source.twid)
         try:
-            max_id = None
+            mark_read = False
+            self.log.debug("Fetching with max_id %s", max_id)
+            resp = await conv.fetch(max_id=max_id)
+            resp_entries = (
+                list(filter(lambda x: x is not None, resp.entries))
+                if resp.entries is not None
+                else None
+            )
+            try:
+                if datetime.now() - timedelta(days=30) > datetime.fromtimestamp(
+                    resp.conversations[self.twid].sort_timestamp
+                ) or (
+                    resp_entries is not None
+                    and len(resp_entries) != 0
+                    and int(resp.conversations[self.twid].last_read_event_id)
+                    >= int(resp_entries[0].message.id)
+                ):
+                    mark_read = True
+            except:
+                mark_read = True
+
             while True:
-                resp = await conv.fetch(max_id=max_id)
-                max_id = resp.min_entry_id
-                for entry in resp.entries:
+                if resp_entries is None or len(resp_entries) == 0:
+                    break
+                for entry in resp_entries:
                     if entry and entry.message:
                         entries.append(entry.message)
                         message_count += 1
                         if entry.message.message_reactions:
                             entries += entry.message.message_reactions
                     if message_count >= limit:
                         break
                 if message_count >= limit:
                     self.log.debug("Got more messages than limit")
                     break
-                elif resp.status == TimelineStatus.AT_END:
-                    self.log.debug("Got all messages in conversation")
+
+                if resp.min_entry_id is None or resp.min_entry_id == max_id:
                     break
+                max_id = resp.min_entry_id
+                self.log.debug("Fetching more entries with max_id %s", max_id)
+                resp = await conv.fetch(max_id=max_id)
+
+            if len(entries) == 0:
+                return None, None
+            entries.sort(key=lambda ent: (ent.time, ent.id), reverse=True)
+            self.log.debug("Finished fetching entries")
+            return mark_read, entries
         except Exception:
             self.log.warning("Exception while fetching messages", exc_info=True)
-        if message_count != len(entries):
-            # Needs sorting to get reactions into correct place
-            entries.sort(key=lambda ent: (ent.time, ent.id), reverse=True)
-        return entries
+            return None, None
 
     async def _invite_own_puppet_backfill(self, source: u.User) -> set[IntentAPI]:
         backfill_leave = set()
         # TODO we should probably only invite the puppet when needed
         if self.config["bridge.backfill.invite_own_puppet"]:
             self.log.debug("Adding %s's default puppet to room for backfilling", source.mxid)
             sender = await p.Puppet.get_by_twid(source.twid)
@@ -859,17 +1031,168 @@
         self, source: u.User, entry: MessageEntry | ReactionCreateEntry
     ) -> None:
         sender = await p.Puppet.get_by_twid(int(entry.sender_id))
         if isinstance(entry, MessageEntry):
             await self.handle_twitter_message(source, sender, entry.message_data, entry.request_id)
         if isinstance(entry, ReactionCreateEntry):
             await self.handle_twitter_reaction_add(
-                sender, int(entry.message_id), entry.reaction_key, entry.time, int(entry.id)
+                sender, int(entry.message_id), entry.reaction_emoji, entry.time, int(entry.id)
             )
 
+    async def _batch_handle_backfill(
+        self,
+        source: u.User,
+        entries: list[MessageEntry | ReactionCreateEntry],
+        is_forward: bool,
+        mark_read: bool,
+    ) -> int:
+        events = []
+        twids = []
+        users_in_batch = set()
+        self.log.debug("Converting Twitter messages in batch")
+        for i, entry in enumerate(entries):
+            sender = await p.Puppet.get_by_twid(int(entry.sender_id))
+            users_in_batch.add(sender.mxid)
+            if isinstance(entry, MessageEntry):
+                msg_id = int(entry.message_data.id)
+                if await self._twitter_message_dedupe(
+                    entry.request_id, msg_id, entry.message_data.sender_id
+                ):
+                    converted = await self._convert_twitter_message(
+                        source, sender, entry.message_data
+                    )
+                    for i, content in enumerate(converted):
+                        event_type = EventType.ROOM_MESSAGE
+                        if self.encrypted and self.matrix.e2ee:
+                            event_type, content = await self.matrix.e2ee.encrypt(
+                                self.mxid, event_type, content
+                            )
+                        content[DOUBLE_PUPPET_SOURCE_KEY] = self.bridge.name
+                        e = BatchSendEvent(
+                            type=event_type,
+                            content=content,
+                            sender=sender.mxid,
+                            timestamp=int(entry.message_data.time.timestamp() * 1000),
+                        )
+                        if self.bridge.homeserver_software.is_hungry:
+                            e.event_id = self.deterministic_event_id(
+                                entry.id, "main" if i + 1 == len(converted) else str(i)
+                            )
+                        events.append(e)
+                        twids.append((msg_id, "message"))
+            elif (
+                isinstance(entry, ReactionCreateEntry)
+                and self.bridge.homeserver_software.is_hungry
+            ):
+                content = ReactionEventContent(
+                    relates_to=RelatesTo(
+                        rel_type=RelationType.ANNOTATION,
+                        event_id=self.deterministic_event_id(entry.message_id, "main"),
+                        key=entry.reaction_emoji,
+                    )
+                )
+                content[DOUBLE_PUPPET_SOURCE_KEY] = self.bridge.name
+                e = BatchSendEvent(
+                    type=EventType.REACTION,
+                    content=content,
+                    sender=sender.mxid,
+                    event_id=self.deterministic_event_id(entry.id, f"reaction{i}"),
+                    timestamp=int(entry.time.timestamp() * 1000),
+                )
+                events.append(e)
+                twids.append(
+                    (entry.id, "reaction", entry.message_id, entry.sender_id, entry.reaction_emoji)
+                )
+        if len(events) == 0:
+            self.log.warn("No bridgeable messages in backfill batch")
+            return 0
+
+        intent = self.main_intent
+
+        state_events_at_start = []
+        if not self.bridge.homeserver_software.is_hungry:
+            before_first_message_timestamp = events[0].timestamp - 1
+            self.log.debug("Adding member state events to batch")
+            for u in users_in_batch:
+                puppet = await self.bridge.get_puppet(u)
+                if puppet is None:
+                    self.log.warn("No puppet found for user %s while backfilling!", u)
+                    continue
+                state_events_at_start.append(
+                    BatchSendStateEvent(
+                        type=EventType.ROOM_MEMBER,
+                        content=MemberStateEventContent(
+                            Membership.INVITE, avatar_url=puppet.photo_mxc, displayname=puppet.name
+                        ),
+                        sender=intent.mxid,
+                        timestamp=before_first_message_timestamp,
+                        state_key=u,
+                    )
+                )
+                state_events_at_start.append(
+                    BatchSendStateEvent(
+                        type=EventType.ROOM_MEMBER,
+                        content=MemberStateEventContent(
+                            Membership.JOIN, avatar_url=puppet.photo_mxc, displayname=puppet.name
+                        ),
+                        sender=u,
+                        timestamp=before_first_message_timestamp,
+                        state_key=u,
+                    )
+                )
+
+        first_event = None
+        if not is_forward:
+            first_event = await DBMessage.get_first(self.mxid)
+            if first_event is None:
+                raise b.NoFirstMessageException
+            else:
+                first_event = first_event.mxid
+        self.log.debug("Sending batch send request")
+        resp = await intent.batch_send(
+            self.mxid,
+            first_event,
+            batch_id=None if is_forward else self.next_batch_id,
+            events=events,
+            state_events_at_start=state_events_at_start,
+            beeper_new_messages=is_forward,
+            beeper_mark_read_by=source.mxid if mark_read else None,
+        )
+        if resp.base_insertion_event_id is not None:
+            self.log.debug("Sending msc2716 insertion marker event")
+            await self.main_intent.send_state_event(
+                self.mxid,
+                StateMarker,
+                {
+                    "org.matrix.msc2716.marker.insertion": resp.base_insertion_event_id,
+                    "com.beeper.timestamp": int(time.time() * 1000),
+                },
+                state_key=resp.base_insertion_event_id,
+            )
+
+        for i, event_id in enumerate(resp.event_ids):
+            if twids[i][1] == "message":
+                msg = DBMessage(event_id, self.mxid, twids[i][0], self.receiver)
+                await msg.upsert()
+            elif twids[i][1] == "reaction" and self.bridge.homeserver_software.is_hungry:
+                reaction = DBReaction(
+                    mxid=event_id,
+                    mx_room=self.mxid,
+                    tw_msgid=twids[i][2],
+                    tw_receiver=self.receiver,
+                    tw_sender=twids[i][3],
+                    reaction=twids[i][4],
+                    tw_reaction_id=twids[i][0],
+                )
+                await reaction.insert()
+        self.next_batch_id = resp.next_batch_id
+        await self.update()
+
+        return len(events)
+
     # endregion
     # region Bridge info state event
 
     @property
     def bridge_info_state_key(self) -> str:
         return f"net.maunium.twitter://twitter/{self.twid}"
 
@@ -948,15 +1271,14 @@
 
     async def _create_matrix_room(self, source: u.User, info: Conversation) -> RoomID | None:
         if self.mxid:
             await self._update_matrix_room(source, info)
             return self.mxid
         await self.update_info(info)
         self.log.debug("Creating Matrix room")
-        name: str | None = None
         initial_state = [
             {
                 "type": str(StateBridge),
                 "state_key": self.bridge_info_state_key,
                 "content": self.bridge_info,
             },
             {
@@ -973,25 +1295,23 @@
                 {
                     "type": "m.room.encryption",
                     "content": self.get_encryption_state_event_json(),
                 }
             )
             if self.is_direct:
                 invites.append(self.az.bot_mxid)
-        if self.encrypted or self.private_chat_portal_meta or not self.is_direct:
-            name = self.name
 
         # We lock backfill lock here so any messages that come between the room being created
         # and the initial backfill finishing wouldn't be bridged before the backfill messages.
         with self.backfill_lock:
             creation_content = {}
             if not self.config["bridge.federate_rooms"]:
                 creation_content["m.federate"] = False
             self.mxid = await self.main_intent.create_room(
-                name=name,
+                name=self.name if self.set_dm_room_metadata else None,
                 is_direct=self.is_direct,
                 initial_state=initial_state,
                 invitees=invites,
                 creation_content=creation_content,
             )
             if not self.mxid:
                 raise Exception("Failed to create room: no mxid returned")
@@ -1010,36 +1330,50 @@
 
             puppet = await p.Puppet.get_by_custom_mxid(source.mxid)
             if puppet:
                 try:
                     await puppet.intent.join_room_by_id(self.mxid)
                     if self.is_direct:
                         await source.update_direct_chats({self.main_intent.mxid: [self.mxid]})
+                    if self.config["bridge.low_quality_tag"]:
+                        await source.tag_room(
+                            puppet,
+                            self,
+                            self.config["bridge.low_quality_tag"],
+                            info.low_quality == True,
+                        )
+                    if self.config["bridge.low_quality_mute"]:
+                        await source.set_muted(puppet, self, info.low_quality == True)
                 except MatrixError:
                     self.log.debug(
                         "Failed to join custom puppet into newly created portal", exc_info=True
                     )
 
             if not info.trusted:
                 msg = "This is a message request. Replying here will accept the request."
                 if info.low_quality:
                     msg += ' Note: Twitter has marked this as a "low quality" message.'
                 await self.main_intent.send_notice(self.mxid, msg)
 
             try:
-                await self.backfill(source, is_initial=True)
+                await self._enqueue_backfills(source)
             except Exception:
                 self.log.exception("Failed to backfill new portal")
 
             # Update participants again after backfill to sync read receipts
             self._last_participant_update = set()
             await self._update_participants(info.participants)
 
         return self.mxid
 
+    async def _enqueue_backfills(self, source: u.User) -> None:
+        state = DBBackfillStatus(self.twid, self.receiver, source.twid, False, 0, 0)
+        await state.insert()
+        await b.BackfillStatus.recheck()
+
     # endregion
     # region Database getters
 
     async def postinit(self) -> None:
         self.by_twid[(self.twid, self.receiver)] = self
         if self.mxid:
             self.by_mxid[self.mxid] = self
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/puppet.py` & `mautrix-twitter-0.1.6/mautrix_twitter/puppet.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 class Puppet(DBPuppet, BasePuppet):
     by_twid: dict[int, Puppet] = {}
     by_custom_mxid: dict[UserID, Puppet] = {}
     hs_domain: str
     mxid_template: SimpleTemplate[int]
 
+    bridge: TwitterBridge
     config: Config
 
     default_mxid_intent: IntentAPI
     default_mxid: UserID
 
     def __init__(
         self,
@@ -53,34 +54,37 @@
         photo_url: str | None = None,
         photo_mxc: ContentURI | None = None,
         is_registered: bool = False,
         custom_mxid: UserID | None = None,
         access_token: str | None = None,
         next_batch: SyncToken | None = None,
         base_url: URL | None = None,
+        contact_info_set: bool = False,
     ) -> None:
         super().__init__(
             twid=twid,
             name=name,
             photo_url=photo_url,
             photo_mxc=photo_mxc,
             is_registered=is_registered,
             custom_mxid=custom_mxid,
             access_token=access_token,
             next_batch=next_batch,
             base_url=base_url,
+            contact_info_set=contact_info_set,
         )
         self.log = self.log.getChild(str(twid))
 
         self.default_mxid = self.get_mxid_from_id(twid)
         self.default_mxid_intent = self.az.intent.user(self.default_mxid)
         self.intent = self._fresh_intent()
 
     @classmethod
     def init_cls(cls, bridge: "TwitterBridge") -> AsyncIterable[Awaitable[None]]:
+        cls.bridge = bridge
         cls.config = bridge.config
         cls.loop = bridge.loop
         cls.mx = bridge.matrix
         cls.az = bridge.az
         cls.hs_domain = cls.config["homeserver.domain"]
         cls.mxid_template = SimpleTemplate(
             cls.config["bridge.username_template"],
@@ -106,20 +110,45 @@
         if portal.other_user == self.twid or (
             self.config["bridge.backfill.invite_own_puppet"] and portal.backfill_lock.locked
         ):
             return self.default_mxid_intent
         return self.intent
 
     async def update_info(self, info: User) -> None:
-        update = False
+        update = await self._update_contact_info(info)
         update = await self._update_name(info) or update
-        update = await self._update_avatar(info.profile_image_url_https) or update
+        try:
+            update = await self._update_avatar(info.profile_image_url_https) or update
+        except Exception:
+            self.log.exception("Error updating avatar from {info.profile_image_url_https}")
         if update:
             await self.update()
 
+    async def _update_contact_info(self, info: User) -> bool:
+        if not self.bridge.homeserver_software.is_hungry:
+            return False
+
+        if self.contact_info_set:
+            return False
+
+        try:
+            await self.default_mxid_intent.beeper_update_profile(
+                {
+                    "com.beeper.bridge.identifiers": [f"twitter:{info.screen_name}"],
+                    "com.beeper.bridge.remote_id": str(info.id),
+                    "com.beeper.bridge.service": self.bridge.beeper_service_name,
+                    "com.beeper.bridge.network": self.bridge.beeper_network_name,
+                }
+            )
+            self.contact_info_set = True
+        except Exception:
+            self.log.exception("Error updating contact info")
+            self.contact_info_set = False
+        return True
+
     @classmethod
     def _get_displayname(cls, info: User) -> str:
         return cls.config["bridge.displayname_template"].format(
             displayname=info.name, id=info.id, username=info.screen_name
         )
 
     async def _update_name(self, info: User) -> bool:
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/user.py` & `mautrix-twitter-0.1.6/mautrix_twitter/user.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,29 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, AsyncGenerator, AsyncIterable, Awaitable, cast
 import asyncio
 import logging
 
+from mautrix.appservice import DOUBLE_PUPPET_SOURCE_KEY
 from mautrix.bridge import BaseUser, async_getter_lock
-from mautrix.types import EventID, MessageType, RoomID, TextMessageEventContent, UserID
+from mautrix.errors import MNotFound
+from mautrix.types import (
+    EventID,
+    MessageType,
+    PushActionType,
+    PushRuleKind,
+    PushRuleScope,
+    RoomID,
+    RoomTagInfo,
+    TextMessageEventContent,
+    UserID,
+)
+from mautrix.util import background_task
 from mautrix.util.bridge_state import BridgeState, BridgeStateEvent
 from mautrix.util.opt_prometheus import Gauge, Summary, async_time
 from mautwitdm import TwitterAPI
 from mautwitdm.errors import TwitterAuthError, TwitterError
 from mautwitdm.poller import PollingErrored, PollingErrorResolved, PollingStarted, PollingStopped
 from mautwitdm.types import (
     Conversation,
@@ -211,16 +224,16 @@
         await self.update()
 
         self._intentional_stop = False
         if self.poll_cursor:
             self.log.debug("Poll cursor set, starting polling right away (not initial syncing)")
             self.client.start_polling()
         else:
-            asyncio.create_task(self._try_initial_sync())
-        asyncio.create_task(self._try_sync_puppet(user_info))
+            background_task.create(self._try_initial_sync())
+        background_task.create(self._try_sync_puppet(user_info))
 
     async def fill_bridge_state(self, state: BridgeState) -> None:
         await super().fill_bridge_state(state)
         if self.twid:
             state.remote_id = str(self.twid)
             puppet = await pu.Puppet.get_by_twid(self.twid)
             state.remote_name = puppet.name
@@ -292,19 +305,29 @@
                 event_id = await self.az.intent.send_message(await self.get_notice_room(), content)
         except Exception:
             self.log.warning("Failed to send bridge notice", exc_info=True)
         return edit or event_id
 
     async def on_error(self, evt: PollingErrored) -> None:
         if evt.fatal:
-            await self.send_bridge_notice(
-                f"Fatal error while polling Twitter: {evt.error}",
-                state_event=BridgeStateEvent.UNKNOWN_ERROR,
-                important=evt.fatal,
-            )
+            if isinstance(evt.error, TwitterAuthError):
+                await self.push_bridge_state(
+                    BridgeStateEvent.BAD_CREDENTIALS,
+                    error="twitter-auth-error",
+                    message=evt.error.message,
+                )
+                await self.send_bridge_notice(
+                    f"Auth error while polling Twitter: {evt.error}", important=True
+                )
+            else:
+                await self.send_bridge_notice(
+                    f"Fatal error while polling Twitter: {evt.error}",
+                    state_event=BridgeStateEvent.UNKNOWN_ERROR,
+                    important=evt.fatal,
+                )
         elif evt.count == 1 and self.config["bridge.temporary_disconnect_notices"]:
             await self.send_bridge_notice(
                 f"Error while polling Twitter: {evt.error}\nThe bridge will keep retrying.",
                 state_event=BridgeStateEvent.TRANSIENT_DISCONNECT,
             )
         else:
             state_event = (
@@ -355,30 +378,76 @@
 
     async def sync(self) -> None:
         await self.push_bridge_state(BridgeStateEvent.BACKFILLING)
         resp = await self.client.inbox_initial_state(set_poll_cursor=False)
         if not self.poll_cursor:
             self.poll_cursor = resp.cursor
         self.client.poll_cursor = self.poll_cursor
+        self.log.debug("Fetching all trusted conversations...")
+        conversations, users = await self.client.all_trusted_conversations()
         limit = self.config["bridge.initial_conversation_sync"]
         conversations = sorted(
-            resp.conversations.values(), key=lambda conv: conv.sort_timestamp, reverse=True
+            conversations.values(), key=lambda conv: conv.sort_timestamp, reverse=True
         )
+        self.log.info("Got %d conversations (sync limit %d)", len(conversations), limit)
         if limit < 0:
             limit = len(conversations)
-        for user in resp.users.values():
+        for _, user in users.items():
             await self.handle_user_update(user)
         index = 0
         for conversation in conversations:
-            create_portal = index < limit and conversation.trusted
-            if create_portal:
-                index += 1
-            await self.handle_conversation_update(conversation, create_portal=create_portal)
+            self.log.info(
+                "Syncing conversation %s (%d of %d)", conversation.conversation_id, index, limit
+            )
+            try:
+                create_portal = index < limit and conversation.trusted
+                if create_portal:
+                    index += 1
+                await self.handle_conversation_update(conversation, create_portal=create_portal)
+            except Exception:
+                self.log.exception(
+                    "Error while syncing conversation %s!", conversation.conversation_id
+                )
         await self.update_direct_chats()
 
+    async def tag_room(self, puppet: pu.Puppet, portal: po.Portal, tag: str, active: bool) -> None:
+        if not tag or not portal or not portal.mxid:
+            return
+        tag_info = await puppet.intent.get_room_tag(portal.mxid, tag)
+        if active and tag_info is None:
+            tag_info = RoomTagInfo(order=0.5)
+            tag_info[DOUBLE_PUPPET_SOURCE_KEY] = self.bridge.name
+            self.log.debug(f"Adding tag {tag} to {portal.mxid}/{portal.twid}")
+            await puppet.intent.set_room_tag(portal.mxid, tag, tag_info)
+        elif (
+            not active and tag_info and tag_info.get(DOUBLE_PUPPET_SOURCE_KEY) == self.bridge.name
+        ):
+            self.log.debug(f"Removing tag {tag} from {portal.mxid}/{portal.twid}")
+            await puppet.intent.remove_room_tag(portal.mxid, tag)
+
+    async def set_muted(self, puppet: pu.Puppet, portal: po.Portal, muted: bool) -> None:
+        if not portal or not portal.mxid:
+            return
+        if muted:
+            self.log.debug(f"Muting {portal.mxid}/{portal.twid}")
+            await puppet.intent.set_push_rule(
+                PushRuleScope.GLOBAL,
+                PushRuleKind.ROOM,
+                portal.mxid,
+                actions=[PushActionType.DONT_NOTIFY],
+            )
+        else:
+            try:
+                await puppet.intent.remove_push_rule(
+                    PushRuleScope.GLOBAL, PushRuleKind.ROOM, portal.mxid
+                )
+                self.log.debug(f"Unmuted {portal.mxid}/{portal.twid}")
+            except MNotFound:
+                pass
+
     async def get_info(self) -> TwitterUser:
         settings = await self.client.get_settings()
         self.username = settings["screen_name"]
         return (await self.client.lookup_users(usernames=[self.username]))[0]
 
     async def stop(self) -> None:
         if self.client:
@@ -415,52 +484,67 @@
     async def handle_conversation_update(
         self, evt: Conversation, create_portal: bool = False
     ) -> None:
         portal = await po.Portal.get_by_twid(
             evt.conversation_id, receiver=self.twid, conv_type=evt.type
         )
         if not portal.mxid:
+            self.log.debug("Conversation %s doesn't have MXID!", evt.conversation_id)
             if create_portal:
+                self.log.debug("Creating Matrix room...")
                 await portal.create_matrix_room(self, evt)
         else:
             # We don't want to do the invite_user and such things each time conversation info
             # comes down polling, so if the room already exists, only call .update_info()
             await portal.update_info(evt)
+            puppet = await pu.Puppet.get_by_custom_mxid(self.mxid)
+            if puppet:
+                if self.config["bridge.low_quality_tag"]:
+                    self.log.debug("Tagging room if low-quality")
+                    await self.tag_room(
+                        puppet,
+                        portal,
+                        self.config["bridge.low_quality_tag"],
+                        evt.low_quality == True,
+                    )
+                if self.config["bridge.low_quality_mute"] and evt.low_quality:
+                    await self.set_muted(puppet, portal, True)
 
     @async_time(METRIC_USER_UPDATE)
     async def handle_user_update(self, user: TwitterUser) -> None:
         puppet = await pu.Puppet.get_by_twid(user.id)
         await puppet.update_info(user)
 
     @async_time(METRIC_MESSAGE)
     async def handle_message(self, evt: MessageEntry) -> None:
         portal = await po.Portal.get_by_twid(
             evt.conversation_id, receiver=self.twid, conv_type=evt.conversation.type
         )
         if not portal.mxid:
             await portal.create_matrix_room(self, evt.conversation)
         sender = await pu.Puppet.get_by_twid(int(evt.message_data.sender_id))
+        await portal.backfill_lock.wait(f"{evt.message_data.sender_id}/{evt.message_data.id}")
         await portal.handle_twitter_message(self, sender, evt.message_data, evt.request_id)
 
     @async_time(METRIC_REACTION)
     async def handle_reaction(self, evt: ReactionCreateEntry | ReactionDeleteEntry) -> None:
         portal = await po.Portal.get_by_twid(
             evt.conversation_id, receiver=self.twid, conv_type=evt.conversation.type
         )
         if not portal.mxid:
             self.log.debug(f"Ignoring reaction in conversation {evt.conversation_id} with no room")
             return
         puppet = await pu.Puppet.get_by_twid(int(evt.sender_id))
         if isinstance(evt, ReactionCreateEntry):
             await portal.handle_twitter_reaction_add(
-                puppet, int(evt.message_id), evt.reaction_key, evt.time, int(evt.id)
+                puppet, int(evt.message_id), evt.reaction_emoji, evt.time, int(evt.id)
             )
         else:
             await portal.handle_twitter_reaction_remove(
-                puppet, int(evt.message_id), evt.reaction_key
+                puppet, int(evt.message_id), evt.reaction_emoji
             )
 
     @async_time(METRIC_RECEIPT)
     async def handle_receipt(self, evt: ConversationReadEntry) -> None:
         portal = await po.Portal.get_by_twid(
             evt.conversation_id, receiver=self.twid, conv_type=evt.conversation.type
         )
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/util/color_log.py` & `mautrix-twitter-0.1.6/mautrix_twitter/util/color_log.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter/web/provisioning_api.py` & `mautrix-twitter-0.1.6/mautrix_twitter/web/provisioning_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import json
 import logging
 
 from aiohttp import web
 
 from mautrix.types import UserID
 from mautrix.util.logging import TraceLogger
+from mautwitdm.errors import TwitterError
 
 from .. import user as u
 
 
 class ProvisioningAPI:
     log: TraceLogger = logging.getLogger("mau.web.provisioning")
     app: web.Application
@@ -104,16 +105,21 @@
             auth_token = data["auth_token"]
             csrf_token = data["csrf_token"]
         except KeyError:
             raise web.HTTPBadRequest(body='{"error": "Missing keys"}', headers=self._headers)
 
         try:
             await user.locked_connect(auth_token=auth_token, csrf_token=csrf_token)
+        except TwitterError as e:
+            self.log.debug("Failed to log in with TwitterError", exc_info=True)
+            raise web.HTTPUnauthorized(
+                body=json.dumps({"error": e.message}), headers=self._headers
+            )
         except Exception:
-            self.log.debug("Failed to log in", exc_info=True)
+            self.log.debug("Failed to log in with generic Exception", exc_info=True)
             raise web.HTTPUnauthorized(
                 body='{"error": "Twitter authorization failed"}', headers=self._headers
             )
         return web.Response(body="{}", status=200, headers=self._headers)
 
     async def logout(self, request: web.Request) -> web.Response:
         user = await self.check_token(request)
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter.egg-info/PKG-INFO` & `mautrix-twitter-0.1.6/mautrix_twitter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 Metadata-Version: 2.1
 Name: mautrix-twitter
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Matrix-Twitter DM puppeting bridge.
 Home-page: https://github.com/mautrix/twitter
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: e2be
 Provides-Extra: metrics
+Provides-Extra: sqlite
 License-File: LICENSE
 
 # mautrix-twitter
 ![Languages](https://img.shields.io/github/languages/top/mautrix/twitter.svg)
 [![License](https://img.shields.io/github/license/mautrix/twitter.svg)](LICENSE)
 [![Release](https://img.shields.io/github/release/mautrix/twitter/all.svg)](https://github.com/mautrix/twitter/releases)
 [![GitLab CI](https://mau.dev/mautrix/twitter/badges/master/pipeline.svg)](https://mau.dev/mautrix/twitter/container_registry)
 
 A Matrix-Twitter DM puppeting bridge.
 
-### Documentation
+## Documentation
 All setup and usage instructions are located on
 [docs.mau.fi](https://docs.mau.fi/bridges/python/twitter/index.html).
 Some quick links:
 
 * [Bridge setup](https://docs.mau.fi/bridges/python/setup.html?bridge=twitter)
   (or [with Docker](https://docs.mau.fi/bridges/general/docker-setup.html?bridge=twitter))
 * Basic usage: [Authentication](https://docs.mau.fi/bridges/python/twitter/authentication.html)
 
 ### Features & Roadmap
 [ROADMAP.md](https://github.com/mautrix/twitter/blob/master/ROADMAP.md)
 contains a general overview of what is supported by the bridge.
 
 ## Discussion
 Matrix room: [`#twitter:maunium.net`](https://matrix.to/#/#twitter:maunium.net)
-
-
```

### Comparing `mautrix-twitter-0.1.5/mautrix_twitter.egg-info/SOURCES.txt` & `mautrix-twitter-0.1.6/mautrix_twitter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 optional-requirements.txt
 pyproject.toml
 requirements.txt
 setup.py
 mautrix_twitter/__init__.py
 mautrix_twitter/__main__.py
+mautrix_twitter/backfill.py
 mautrix_twitter/config.py
 mautrix_twitter/example-config.yaml
 mautrix_twitter/formatter.py
 mautrix_twitter/get_version.py
 mautrix_twitter/matrix.py
 mautrix_twitter/portal.py
 mautrix_twitter/puppet.py
@@ -22,14 +23,15 @@
 mautrix_twitter.egg-info/requires.txt
 mautrix_twitter.egg-info/top_level.txt
 mautrix_twitter/commands/__init__.py
 mautrix_twitter/commands/auth.py
 mautrix_twitter/commands/conn.py
 mautrix_twitter/commands/typehint.py
 mautrix_twitter/db/__init__.py
+mautrix_twitter/db/backfill.py
 mautrix_twitter/db/message.py
 mautrix_twitter/db/portal.py
 mautrix_twitter/db/puppet.py
 mautrix_twitter/db/reaction.py
 mautrix_twitter/db/upgrade.py
 mautrix_twitter/db/user.py
 mautrix_twitter/util/__init__.py
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/conversation.py` & `mautrix-twitter-0.1.6/mautwitdm/conversation.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,23 +44,27 @@
         async with self.api.http.post(self.api_url / "accept.json", headers=self.api.headers) as r:
             await check_error(r)
 
     async def send(
         self,
         text: str,
         media_id: str | int | None = None,
+        voice_message: bool = False,
+        reply_to_id: str | int | None = None,
         request_id: UUID | str | None = None,
     ) -> SendResponse:
         """
         Send a message to this conversation.
 
         Args:
             text: The text to send. May be an empty string if only sending media.
             media_id: The media ID to send. Use :meth:`TwitterUploader.upload` to upload media and
                 get a media ID.
+            voice_message: Whether the media message is a voice message.
+            reply_to_id: ID of message to reply to.
             request_id: The transaction ID for this request. It will be included in the message
                 when polling and can be used for deduplication. If not provided, one will be
                 automatically created using :meth:`TwitterAPI.new_request_id`
 
         Returns:
             The send response from the server.
         """
@@ -68,52 +72,68 @@
             **self.api.poll_params,
             "text": text,
             "conversation_id": self.id,
             "recipient_ids": "false",
             "request_id": str(request_id or self.api.new_request_id()),
         }
         url = self.api.dm_url / "new.json"
+        if reply_to_id:
+            data["reply_to_dm_id"] = reply_to_id
         if media_id:
             data["media_id"] = str(media_id)
+            if voice_message:
+                data["audio_only_media_attachment"] = True
         async with self.api.http.post(url, data=data, headers=self.api.headers) as resp:
             resp_data = await check_error(resp)
             return SendResponse.deserialize(resp_data)
 
-    async def react(self, message_id: str | int, key: ReactionKey) -> None:
+    @staticmethod
+    def _reaction_key_to_params(emoji: str) -> dict[str, str]:
+        key = ReactionKey.from_emoji(emoji)
+        if key == ReactionKey.EMOJI:
+            return {
+                "emoji_reaction": emoji,
+                "reaction_key": str(key),
+            }
+        else:
+            return {
+                "reaction_key": str(key),
+            }
+
+    async def react(self, message_id: str | int, emoji: str) -> None:
         """
         React to a message. Reacting to the same message multiple times will override earlier
         reactions.
 
         Args:
             message_id: The message ID to react to.
-            key: The reaction itself.
+            emoji: The reaction itself.
         """
-        url = (self.api.dm_url / "reaction" / "new.json").with_query(
-            {
-                "reaction_key": str(key),
-                "conversation_id": self.id,
-                "dm_id": str(message_id),
-            }
-        )
+        query = {
+            "conversation_id": self.id,
+            "dm_id": str(message_id),
+            **self._reaction_key_to_params(emoji),
+        }
+        url = (self.api.dm_url / "reaction" / "new.json").with_query(query)
         async with self.api.http.post(url, headers=self.api.headers) as resp:
             await check_error(resp)
 
-    async def delete_reaction(self, message_id: str | int, key: ReactionKey) -> None:
+    async def delete_reaction(self, message_id: str | int, emoji: str) -> None:
         """
         Delete an earlier reaction.
 
         Args:
             message_id: The message ID to react to.
-            key: The reaction itself.
+            emoji: The reaction itself.
         """
         url = (self.api.dm_url / "reaction" / "delete.json").with_query(
             {
-                "reaction_key": str(key),
                 "conversation_id": self.id,
                 "dm_id": str(message_id),
+                **self._reaction_key_to_params(emoji),
             }
         )
         async with self.api.http.post(url, headers=self.api.headers) as resp:
             await check_error(resp)
 
     async def fetch(self, max_id: str | None = None) -> FetchConversationResponse:
         """
@@ -131,8 +151,15 @@
             "include_conversation_info": "true",
         }
         req = (self.api.dm_url / "conversation" / f"{self.id}.json").with_query(query)
         if max_id:
             req = req.update_query({"max_id": max_id})
         async with self.api.http.get(req, headers=self.api.headers) as resp:
             resp_data = await check_error(resp)
-        return FetchConversationResponse.deserialize(resp_data["conversation_timeline"])
+        data = resp_data["conversation_timeline"]
+        if "entries" not in data:
+            data["entries"] = None
+        if "min_entry_id" not in data:
+            data["min_entry_id"] = None
+        if "max_entry_id" not in data:
+            data["max_entry_id"] = None
+        return FetchConversationResponse.deserialize(data)
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/dispatcher.py` & `mautrix-twitter-0.1.6/mautwitdm/dispatcher.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautwitdm/errors.py` & `mautrix-twitter-0.1.6/mautwitdm/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,10 +64,10 @@
         code = error["code"]
         message = error["message"]
     except (KeyError, IndexError):
         resp.raise_for_status()
         raise
     if code == 88:
         raise RateLimitError(code, message, resp.headers)
-    elif code == 32:
+    elif code in (32, 63, 64, 326):
         raise TwitterAuthError(code, message)
     raise TwitterError(code, message)
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/poller.py` & `mautrix-twitter-0.1.6/mautwitdm/poller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 # Copyright (c) 2022 Tulir Asokan
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
+from typing import Dict
 import asyncio
 import logging
 import time
 
 from aiohttp import ClientSession
 from attr import dataclass
 from yarl import URL
 
 from . import conversation as c
 from .dispatcher import TwitterDispatcher
-from .errors import RateLimitError, check_error
-from .types import InitialStateResponse, PollResponse
+from .errors import RateLimitError, TwitterAuthError, check_error
+from .types import (
+    Conversation,
+    InboxTimeline,
+    InitialStateResponse,
+    PollResponse,
+    TimelineStatus,
+    User,
+)
 
 
 class PollingStarted:
     pass
 
 
 class PollingStopped:
@@ -98,14 +106,65 @@
             "include_can_media_tag": "1",
             "include_ext_alt_text": "1",
             "include_ext_has_nft_avatar": "1",
             "skip_status": "1",
             **self.poll_params,
         }
 
+    async def all_trusted_conversations(
+        self,
+    ) -> tuple[Dict[str, Conversation], Dict[str, User]]:
+        """
+        Get all trusted conversations from the inbox (using pagination).
+
+        Returns:
+            Dictionary containing all conversations, keyed by their ID.
+        """
+        initial_state = await self.inbox_initial_state(set_poll_cursor=False)
+        conversations = initial_state.conversations
+        users = initial_state.users
+
+        if initial_state.inbox_timelines.trusted.status == TimelineStatus.AT_END:
+            return conversations, users
+
+        min_entry_id = initial_state.inbox_timelines.trusted.min_entry_id
+
+        while True:
+            self.log.debug("Not at end, fetching more conversations with max_id %s", min_entry_id)
+            inbox_timeline = await self.inbox_timeline("trusted", min_entry_id)
+
+            if inbox_timeline.conversations is not None:
+                conversations = {**conversations, **inbox_timeline.conversations}
+
+            if inbox_timeline.users is not None:
+                users = {**users, **inbox_timeline.users}
+
+            if inbox_timeline.status == TimelineStatus.AT_END:
+                return conversations, users
+
+            if inbox_timeline.min_entry_id is not None:
+                min_entry_id = inbox_timeline.min_entry_id
+            else:
+                return conversations, users
+
+    async def inbox_timeline(self, inbox: str, max_id: str) -> InboxTimeline:
+        """
+        Gets a page of DMs from one of the possible inbox timelines.
+
+        Returns:
+            The response data from the server.
+        """
+        url = (self.dm_url / "inbox_timeline" / f"{inbox}.json").with_query(
+            {**self.full_state_params, "max_id": max_id}
+        )
+        async with self.http.get(url, headers=self.headers) as resp:
+            data = await check_error(resp)
+            response = InboxTimeline.deserialize(data["inbox_timeline"])
+            return response
+
     async def inbox_initial_state(self, set_poll_cursor: bool = True) -> InitialStateResponse:
         """
         Get the initial DM inbox state, including conversations, user profiles and some messages.
 
         This also gets the initial :attr:`poll_cursor` value.
 
         Returns:
@@ -162,14 +221,17 @@
                 :class:`asyncio.CancelledError` will not be raised in any case.
         """
         try:
             await self._poll_forever()
         except asyncio.CancelledError:
             self.log.debug("Polling stopped")
             await self.dispatch(PollingStopped())
+        except TwitterAuthError as e:
+            self.log.exception("Auth error while polling")
+            await self.dispatch(PollingErrored(e, fatal=True, count=0))
         except Exception as e:
             await self.dispatch(PollingErrored(e, fatal=True, count=0))
             self.log.exception("Fatal error while polling")
             if raise_exceptions:
                 raise
 
     async def dispatch_all(self, resp: PollResponse | InitialStateResponse) -> None:
@@ -209,25 +271,27 @@
         errors = 0
         while True:
             try:
                 resp = await self._poll_once()
             except RateLimitError as e:
                 sleep = e.reset - int(time.time())
                 self.log.warning(
-                    f"Got rate limit until {e.reset} while polling, " f"waiting {sleep} seconds"
+                    f"Got rate limit until {e.reset} while polling, waiting {sleep} seconds"
                 )
                 if self.poll_sleep < 8:
                     self.poll_sleep += 1
                     self.log.debug(f"Increased poll sleep to {self.poll_sleep}")
                 await asyncio.sleep(sleep)
                 continue
+            except TwitterAuthError:
+                raise
             except Exception as e:
                 if errors > self.max_poll_errors > 0:
                     self.log.debug(
-                        f"Error count ({errors}) exceeded maximum, " f"raising error as fatal"
+                        f"Error count ({errors}) exceeded maximum, raising error as fatal"
                     )
                     raise
                 errors += 1
                 sleep = min(15 * 60, self.error_sleep * errors)
                 self.log.warning(f"Error while polling, retrying in {sleep}s", exc_info=True)
                 await self.dispatch(PollingErrored(e, fatal=False, count=errors))
                 await asyncio.sleep(sleep)
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/streamer.py` & `mautrix-twitter-0.1.6/mautwitdm/streamer.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautwitdm/twitter.py` & `mautrix-twitter-0.1.6/mautwitdm/twitter.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/__init__.py` & `mautrix-twitter-0.1.6/mautwitdm/types/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     MessageEntitySimple,
     MessageEntityURL,
     MessageEntityUserMention,
 )
 from .reaction import ReactionCreateEntry, ReactionDeleteEntry, ReactionKey
 from .response import (
     FetchConversationResponse,
+    InboxTimeline,
     InitialStateResponse,
     MediaUploadResponse,
     PollResponse,
     SendResponse,
     TimelineStatus,
 )
 from .stream_payload import DMTypingEvent, DMUpdateEvent, StreamEvent
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/conversation.py` & `mautrix-twitter-0.1.6/mautwitdm/types/conversation.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 @dataclass
 class Conversation(SerializableAttrs):
     conversation_id: str
     type: ConversationType
     participants: List[Participant]
     notifications_disabled: bool
     mention_notifications_disabled: bool
-    trusted: bool
-    low_quality: bool
+    trusted: Optional[bool] = None
+    low_quality: Optional[bool] = None
 
     sort_event_id: Optional[str] = None
     sort_timestamp: StringTimestamp = datetime.fromtimestamp(0)
 
     # These are present in some responses
     min_entry_id: Optional[str] = None
     max_entry_id: Optional[str] = None
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/entry.py` & `mautrix-twitter-0.1.6/mautwitdm/types/entry.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/message.py` & `mautrix-twitter-0.1.6/mautwitdm/types/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 from typing import List, Optional
 
 from attr import dataclass
+import attr
 
 from mautrix.types import SerializableAttrs
 
 from .conversation import Conversation
 from .message_attachment import MessageAttachment
 from .message_entity import MessageEntities
 from .reaction import ReactionCreateEntry
@@ -22,14 +23,19 @@
     time: StringTimestamp
     sender_id: str
     text: str
     recipient_id: Optional[str] = None
     conversation_id: Optional[str] = None
     entities: Optional[MessageEntities] = None
     attachment: Optional[MessageAttachment] = None
+    reply_data: Optional["MessageData"] = None
+
+
+# Resolve reply_data field
+attr.resolve_types(MessageData)
 
 
 @dataclass
 class MessageEntry(SerializableAttrs):
     id: str
     time: StringTimestamp
     conversation_id: str
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/message_attachment.py` & `mautrix-twitter-0.1.6/mautwitdm/types/message_attachment.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     url: str
     display_url: str
     expanded_url: str
     type: str
     sizes: Dict[str, ImageSizeInfo]
     original_info: OriginalImageSizeInfo
     video_info: Optional[VideoInfo] = None
+    audio_only: Optional[bool] = None
 
 
 @dataclass
 class ImageBindingValue(SerializableAttrs):
     url: str
     width: int
     height: int
@@ -81,15 +82,15 @@
 @dataclass
 class ImageColorBindingValue(SerializableAttrs):
     palette: List[ImageColor]
 
 
 @dataclass
 class CardBindingValue(SerializableAttrs):
-    type: str
+    type: Optional[str] = None
     string_value: Optional[str] = None
     image_value: Optional[ImageBindingValue] = None
     image_color_value: Optional[ImageColorBindingValue] = None
     scribe_key: Optional[str] = None
 
 
 @dataclass
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/message_entity.py` & `mautrix-twitter-0.1.6/mautwitdm/types/message_entity.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/reaction.py` & `mautrix-twitter-0.1.6/mautwitdm/types/reaction.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # Copyright (c) 2020 Tulir Asokan
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 from attr import dataclass
 
 from mautrix.types import SerializableAttrs, SerializableEnum
+from mautrix.util import variation_selector
 
 from .conversation import Conversation
 from .util import StringTimestamp
 
 
 class ReactionKey(SerializableEnum):
     FUNNY = "funny"  # 😂
     SURPRISED = "surprised"  # 😲
     SAD = "sad"  # 😢
     LIKE = "like"  # ❤
     EXCITED = "excited"  # 🔥
     AGREE = "agree"  # 👍
     DISAGREE = "disagree"  # 👎
+    EMOJI = "emoji"  # arbitrary emoji
 
     @property
     def emoji(self) -> str:
         return _key_to_emoji[self]
 
     @classmethod
-    def from_emoji(cls, emoji: str) -> "ReactionKey":
+    def from_emoji(cls, emoji: str) -> Union["ReactionKey", str]:
         try:
             return _emoji_to_key[emoji.rstrip("\uFE0F")]
         except KeyError:
-            raise NotImplementedError(f"Unsupported reaction emoji {emoji}")
+            return ReactionKey.EMOJI
 
 
 _key_to_emoji: Dict[ReactionKey, str] = {
     ReactionKey.FUNNY: "\U0001F602",
     ReactionKey.SURPRISED: "\U0001F632",
     ReactionKey.SAD: "\U0001F622",
     ReactionKey.LIKE: "\u2764\uFE0F",
@@ -60,23 +62,40 @@
 class ReactionCreateEntry(SerializableAttrs):
     id: str
     time: StringTimestamp
     conversation_id: str
     message_id: str
     reaction_key: ReactionKey
     sender_id: str
+    emoji_reaction: Optional[str] = None
     affects_sort: Optional[bool] = None
+    request_id: Optional[str] = None
 
     conversation: Optional[Conversation] = None
 
+    @property
+    def reaction_emoji(self) -> str:
+        if self.reaction_key == ReactionKey.EMOJI:
+            return self.emoji_reaction
+        return self.reaction_key.emoji
+
 
 @dataclass
 class ReactionDeleteEntry(SerializableAttrs):
     id: str
     time: StringTimestamp
     conversation_id: str
     message_id: str
     reaction_key: ReactionKey
+    emoji_reaction: str
     sender_id: str
     affects_sort: Optional[bool] = None
 
     conversation: Optional[Conversation] = None
+
+    @property
+    def reaction_emoji(self) -> str:
+        if self.reaction_key == ReactionKey.EMOJI:
+            emoji = self.emoji_reaction
+        else:
+            emoji = self.reaction_key.emoji
+        return variation_selector.remove(emoji)
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/response.py` & `mautrix-twitter-0.1.6/mautwitdm/types/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     users: Dict[str, User]
     conversations: Optional[Dict[str, Conversation]] = None
 
 
 @dataclass
 class FetchConversationResponse(SerializableAttrs):
     status: TimelineStatus
-    min_entry_id: str
-    max_entry_id: str
-    entries: List[Entry]
     users: Dict[str, User]
+    min_entry_id: Optional[str] = None
+    max_entry_id: Optional[str] = None
+    entries: Optional[List[Entry]] = None
     conversations: Optional[Dict[str, Conversation]] = None
 
 
 @dataclass
 class PollResponse(SerializableAttrs):
     cursor: str
     last_seen_event_id: str
@@ -46,14 +46,17 @@
     conversations: Optional[Dict[str, Conversation]] = None
 
 
 @dataclass
 class InboxTimeline(SerializableAttrs):
     status: TimelineStatus
     min_entry_id: Optional[str] = None
+    entries: Optional[List[Entry]] = None
+    users: Optional[Dict[str, User]] = None
+    conversations: Optional[Dict[str, Conversation]] = None
 
 
 @dataclass
 class InboxTimelines(SerializableAttrs):
     trusted: InboxTimeline
     untrusted: InboxTimeline
     untrusted_low_quality: InboxTimeline
```

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/stream_payload.py` & `mautrix-twitter-0.1.6/mautwitdm/types/stream_payload.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/user.py` & `mautrix-twitter-0.1.6/mautwitdm/types/user.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautwitdm/types/util.py` & `mautrix-twitter-0.1.6/mautwitdm/types/util.py`

 * *Files identical despite different names*

### Comparing `mautrix-twitter-0.1.5/mautwitdm/uploader.py` & `mautrix-twitter-0.1.6/mautwitdm/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,24 +72,26 @@
             self.log.debug(f"Finished uploading {media_id}, but server is still processing it")
             check_after = processing_info.get("check_after_secs", 1)
             return await self._wait_processing(media_id, check_after)
         self.log.debug(f"Finished uploading {media_id}")
         return MediaUploadResponse.deserialize(resp_data)
 
     async def upload(
-        self, data: bytes = None, url: str = None, mime_type: str = None
+        self, data: bytes = None, url: str = None, mime_type: str = None, is_audio: bool = False
     ) -> MediaUploadResponse:
         if mime_type == "image/gif":
             category = "dm_gif"
             size_limit = 15 * 1024 * 1024
         elif mime_type.startswith("image/"):
             category = "dm_image"
             size_limit = 5 * 1024 * 1024
         elif mime_type.startswith("video/"):
             category = "dm_video"
+            if is_audio:
+                category = "dm_audio_video"
             size_limit = 15 * 1024 * 1024
         else:
             raise NotImplementedError(f"Unsupported mime type {mime_type}")
         if len(data) > size_limit:
             raise NotImplementedError("File too big")
         init_req = {
             "command": "INIT",
```

### Comparing `mautrix-twitter-0.1.5/setup.py` & `mautrix-twitter-0.1.6/setup.py`

 * *Files identical despite different names*

