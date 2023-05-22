# Comparing `tmp/ovos-microphone-plugin-arecord-0.0.0a1.tar.gz` & `tmp/ovos-microphone-plugin-arecord-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-microphone-plugin-arecord-0.0.0a1.tar", last modified: Fri May 19 23:59:50 2023, max compression
+gzip compressed data, was "ovos-microphone-plugin-arecord-0.0.0a2.tar", last modified: Mon May 22 16:01:53 2023, max compression
```

## Comparing `ovos-microphone-plugin-arecord-0.0.0a1.tar` & `ovos-microphone-plugin-arecord-0.0.0a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:59:50.159745 ovos-microphone-plugin-arecord-0.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-19 23:59:43.000000 ovos-microphone-plugin-arecord-0.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 23:59:43.000000 ovos-microphone-plugin-arecord-0.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 23:59:50.159745 ovos-microphone-plugin-arecord-0.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-19 23:59:43.000000 ovos-microphone-plugin-arecord-0.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:59:50.155745 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord/
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-19 23:59:43.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-19 23:59:46.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:59:50.155745 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 23:59:49.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-19 23:59:50.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:59:49.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-19 23:59:49.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 23:59:49.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 23:59:49.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:59:49.000000 ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:59:50.159745 ovos-microphone-plugin-arecord-0.0.0a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-05-19 23:59:43.000000 ovos-microphone-plugin-arecord-0.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:01:53.032493 ovos-microphone-plugin-arecord-0.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-22 16:01:41.000000 ovos-microphone-plugin-arecord-0.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 16:01:41.000000 ovos-microphone-plugin-arecord-0.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 16:01:53.032493 ovos-microphone-plugin-arecord-0.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-22 16:01:41.000000 ovos-microphone-plugin-arecord-0.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:01:53.028493 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord/
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-05-22 16:01:41.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-22 16:01:47.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:01:53.032493 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 16:01:52.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 16:01:53.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:01:52.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 16:01:52.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 16:01:52.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 16:01:52.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:01:52.000000 ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:01:53.032493 ovos-microphone-plugin-arecord-0.0.0a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-05-22 16:01:41.000000 ovos-microphone-plugin-arecord-0.0.0a2/setup.py
```

### Comparing `ovos-microphone-plugin-arecord-0.0.0a1/LICENSE` & `ovos-microphone-plugin-arecord-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-microphone-plugin-arecord-0.0.0a1/PKG-INFO` & `ovos-microphone-plugin-arecord-0.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-arecord
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A arecord microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-arecord
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone arecord
```

### Comparing `ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord/__init__.py` & `ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Copyright 2022 Mycroft AI Inc.
-#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
```

### Comparing `ovos-microphone-plugin-arecord-0.0.0a1/ovos_microphone_plugin_arecord.egg-info/PKG-INFO` & `ovos-microphone-plugin-arecord-0.0.0a2/ovos_microphone_plugin_arecord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-arecord
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A arecord microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-arecord
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone arecord
```

### Comparing `ovos-microphone-plugin-arecord-0.0.0a1/setup.py` & `ovos-microphone-plugin-arecord-0.0.0a2/setup.py`

 * *Files identical despite different names*

