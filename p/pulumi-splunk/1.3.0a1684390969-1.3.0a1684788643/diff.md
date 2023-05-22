# Comparing `tmp/pulumi_splunk-1.3.0a1684390969.tar.gz` & `tmp/pulumi_splunk-1.3.0a1684788643.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_splunk-1.3.0a1684390969.tar", last modified: Thu May 18 06:32:06 2023, max compression
+gzip compressed data, was "pulumi_splunk-1.3.0a1684788643.tar", last modified: Mon May 22 20:54:50 2023, max compression
```

## Comparing `pulumi_splunk-1.3.0a1684390969.tar` & `pulumi_splunk-1.3.0a1684788643.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:32:06.799708 pulumi_splunk-1.3.0a1684390969/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-18 06:32:06.799708 pulumi_splunk-1.3.0a1684390969/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:32:06.799708 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    90731 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/admin_saml_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    38600 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/apps_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/authentication_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    45752 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/authorization_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:32:06.799708 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/configs_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/data_ui_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/generic_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/global_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   154784 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29483 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_tcp_cooked.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_tcp_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_tcp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_udp.py
--rw-r--r--   0 runner    (1001) docker     (123)    73136 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43975 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs_tcp_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    43421 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs_tcp_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31871 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    27807 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs_tcp_syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   499677 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/saved_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk/sh_indexes_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:32:06.799708 pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:32:06.799708 pulumi_splunk-1.3.0a1684390969/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-18 06:32:06.000000 pulumi_splunk-1.3.0a1684390969/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:54:50.238741 pulumi_splunk-1.3.0a1684788643/
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-22 20:54:50.238741 pulumi_splunk-1.3.0a1684788643/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:54:50.238741 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90731 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/admin_saml_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38600 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/apps_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/authentication_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45752 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/authorization_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:54:50.238741 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/configs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/data_ui_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/generic_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/global_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154784 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29483 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_tcp_cooked.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_tcp_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_tcp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73136 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43975 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs_tcp_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43421 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs_tcp_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31871 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27807 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs_tcp_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   506277 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/saved_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk/sh_indexes_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:54:50.238741 pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-22 20:54:50.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-22 20:54:50.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:54:50.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:54:50.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 20:54:50.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 20:54:50.000000 pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:54:50.238741 pulumi_splunk-1.3.0a1684788643/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 20:54:49.000000 pulumi_splunk-1.3.0a1684788643/setup.py
```

### Comparing `pulumi_splunk-1.3.0a1684390969/PKG-INFO` & `pulumi_splunk-1.3.0a1684788643/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1684390969
+Version: 1.3.0a1684788643
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi splunk
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-splunk/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-splunk/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fsplunk.svg)](https://www.npmjs.com/package/@pulumi/splunk)
 [![Python version](https://badge.fury.io/py/pulumi-splunk.svg)](https://pypi.org/project/pulumi-splunk)
 [![NuGet version](https://badge.fury.io/nu/pulumi.splunk.svg)](https://badge.fury.io/nu/pulumi.splunk)
```

### Comparing `pulumi_splunk-1.3.0a1684390969/README.md` & `pulumi_splunk-1.3.0a1684788643/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/__init__.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/_inputs.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/_utilities.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/admin_saml_groups.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/admin_saml_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/apps_local.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/apps_local.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/authentication_users.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/authentication_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/authorization_roles.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/authorization_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/config/vars.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/configs_conf.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/configs_conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,31 +17,27 @@
 class ConfigsConfArgs:
     def __init__(__self__, *,
                  acl: Optional[pulumi.Input['ConfigsConfAclArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  variables: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a ConfigsConf resource.
-        :param pulumi.Input['ConfigsConfAclArgs'] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] name: A '/' separated string consisting of {conf_file_name}/{stanza_name} ex. props/custom_stanza
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] variables: A map of key value pairs for a stanza.
         """
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if variables is not None:
             pulumi.set(__self__, "variables", variables)
 
     @property
     @pulumi.getter
     def acl(self) -> Optional[pulumi.Input['ConfigsConfAclArgs']]:
-        """
-        The app/user context that is the namespace for the resource
-        """
         return pulumi.get(self, "acl")
 
     @acl.setter
     def acl(self, value: Optional[pulumi.Input['ConfigsConfAclArgs']]):
         pulumi.set(self, "acl", value)
 
     @property
@@ -73,31 +69,27 @@
 class _ConfigsConfState:
     def __init__(__self__, *,
                  acl: Optional[pulumi.Input['ConfigsConfAclArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  variables: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering ConfigsConf resources.
-        :param pulumi.Input['ConfigsConfAclArgs'] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] name: A '/' separated string consisting of {conf_file_name}/{stanza_name} ex. props/custom_stanza
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] variables: A map of key value pairs for a stanza.
         """
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if variables is not None:
             pulumi.set(__self__, "variables", variables)
 
     @property
     @pulumi.getter
     def acl(self) -> Optional[pulumi.Input['ConfigsConfAclArgs']]:
-        """
-        The app/user context that is the namespace for the resource
-        """
         return pulumi.get(self, "acl")
 
     @acl.setter
     def acl(self, value: Optional[pulumi.Input['ConfigsConfAclArgs']]):
         pulumi.set(self, "acl", value)
 
     @property
@@ -149,15 +141,14 @@
             "disabled": "false",
             "custom_key": "value",
         })
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['ConfigsConfAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] name: A '/' separated string consisting of {conf_file_name}/{stanza_name} ex. props/custom_stanza
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] variables: A map of key value pairs for a stanza.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -226,15 +217,14 @@
         """
         Get an existing ConfigsConf resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['ConfigsConfAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] name: A '/' separated string consisting of {conf_file_name}/{stanza_name} ex. props/custom_stanza
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] variables: A map of key value pairs for a stanza.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ConfigsConfState.__new__(_ConfigsConfState)
 
@@ -242,17 +232,14 @@
         __props__.__dict__["name"] = name
         __props__.__dict__["variables"] = variables
         return ConfigsConf(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def acl(self) -> pulumi.Output['outputs.ConfigsConfAcl']:
-        """
-        The app/user context that is the namespace for the resource
-        """
         return pulumi.get(self, "acl")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         A '/' separated string consisting of {conf_file_name}/{stanza_name} ex. props/custom_stanza
```

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/data_ui_views.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/data_ui_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/generic_acl.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/generic_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/global_http_event_collector.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/global_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/indexes.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_http_event_collector.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_monitor.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_script.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_tcp_cooked.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_tcp_cooked.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_tcp_raw.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_tcp_raw.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_tcp_splunk_tcp_token.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_tcp_splunk_tcp_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_tcp_ssl.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_tcp_ssl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/inputs_udp.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/inputs_udp.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs_tcp_default.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs_tcp_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs_tcp_group.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs_tcp_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs_tcp_server.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs_tcp_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/outputs_tcp_syslog.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/outputs_tcp_syslog.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/provider.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/saved_searches.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/saved_searches.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
                  action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
                  action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_max_time: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_track_alert: Optional[pulumi.Input[bool]] = None,
                  action_populate_lookup_ttl: Optional[pulumi.Input[str]] = None,
@@ -225,14 +227,16 @@
         :param pulumi.Input[bool] action_email_width_sort_columns: Indicates whether columns should be sorted from least wide to most wide, left to right.Only valid if format=text.
         :param pulumi.Input[str] action_jira_service_desk_param_account: Jira Service Desk account name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_description: Jira issue description
         :param pulumi.Input[str] action_jira_service_desk_param_jira_issue_type: Jira issue type name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_priority: Jira priority of issue
         :param pulumi.Input[str] action_jira_service_desk_param_jira_project: Jira Project name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_summary: Jira issue title/summary
+        :param pulumi.Input[str] action_pagerduty_integration_url: The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        :param pulumi.Input[str] action_pagerduty_integration_url_override: The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[str] action_populate_lookup_command: The search command (or pipeline) which is responsible for executing the action.
         :param pulumi.Input[str] action_populate_lookup_dest: Lookup name of path of the lookup to populate
         :param pulumi.Input[str] action_populate_lookup_hostname: Sets the hostname used in the web link (url) sent in alert actions.This value accepts two forms: hostname (for example, splunkserver, splunkserver.example.com)\\n\\nprotocol://hostname:port (for example, http://splunkserver:8000, https://splunkserver.example.com:443)
         :param pulumi.Input[int] action_populate_lookup_max_results: Sets the maximum number of search results sent using alerts. Defaults to 100.
         :param pulumi.Input[int] action_populate_lookup_max_time: Valid values are: Integer[m|s|h|d]Sets the maximum amount of time the execution of an action takes before the action is aborted. Defaults to 5m.
         :param pulumi.Input[bool] action_populate_lookup_track_alert: Indicates whether the execution of this action signifies a trackable alert.
         :param pulumi.Input[str] action_populate_lookup_ttl: Valid values are Integer[p]Specifies the minimum time-to-live in seconds of the search artifacts if this action is triggered. If p follows Integer, then this specifies the number of scheduled periods. Defaults to 10p.
@@ -446,14 +450,18 @@
             pulumi.set(__self__, "action_jira_service_desk_param_jira_issue_type", action_jira_service_desk_param_jira_issue_type)
         if action_jira_service_desk_param_jira_priority is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_priority", action_jira_service_desk_param_jira_priority)
         if action_jira_service_desk_param_jira_project is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_project", action_jira_service_desk_param_jira_project)
         if action_jira_service_desk_param_jira_summary is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_summary", action_jira_service_desk_param_jira_summary)
+        if action_pagerduty_integration_url is not None:
+            pulumi.set(__self__, "action_pagerduty_integration_url", action_pagerduty_integration_url)
+        if action_pagerduty_integration_url_override is not None:
+            pulumi.set(__self__, "action_pagerduty_integration_url_override", action_pagerduty_integration_url_override)
         if action_populate_lookup_command is not None:
             pulumi.set(__self__, "action_populate_lookup_command", action_populate_lookup_command)
         if action_populate_lookup_dest is not None:
             pulumi.set(__self__, "action_populate_lookup_dest", action_populate_lookup_dest)
         if action_populate_lookup_hostname is not None:
             pulumi.set(__self__, "action_populate_lookup_hostname", action_populate_lookup_hostname)
         if action_populate_lookup_max_results is not None:
@@ -1302,14 +1310,38 @@
         return pulumi.get(self, "action_jira_service_desk_param_jira_summary")
 
     @action_jira_service_desk_param_jira_summary.setter
     def action_jira_service_desk_param_jira_summary(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "action_jira_service_desk_param_jira_summary", value)
 
     @property
+    @pulumi.getter(name="actionPagerdutyIntegrationUrl")
+    def action_pagerduty_integration_url(self) -> Optional[pulumi.Input[str]]:
+        """
+        The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_url")
+
+    @action_pagerduty_integration_url.setter
+    def action_pagerduty_integration_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_integration_url", value)
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationUrlOverride")
+    def action_pagerduty_integration_url_override(self) -> Optional[pulumi.Input[str]]:
+        """
+        The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_url_override")
+
+    @action_pagerduty_integration_url_override.setter
+    def action_pagerduty_integration_url_override(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_integration_url_override", value)
+
+    @property
     @pulumi.getter(name="actionPopulateLookupCommand")
     def action_populate_lookup_command(self) -> Optional[pulumi.Input[str]]:
         """
         The search command (or pipeline) which is responsible for executing the action.
         """
         return pulumi.get(self, "action_populate_lookup_command")
 
@@ -2605,14 +2637,16 @@
                  action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
                  action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup: Optional[pulumi.Input[bool]] = None,
                  action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_max_time: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_track_alert: Optional[pulumi.Input[bool]] = None,
@@ -2769,14 +2803,16 @@
         :param pulumi.Input[bool] action_email_width_sort_columns: Indicates whether columns should be sorted from least wide to most wide, left to right.Only valid if format=text.
         :param pulumi.Input[str] action_jira_service_desk_param_account: Jira Service Desk account name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_description: Jira issue description
         :param pulumi.Input[str] action_jira_service_desk_param_jira_issue_type: Jira issue type name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_priority: Jira priority of issue
         :param pulumi.Input[str] action_jira_service_desk_param_jira_project: Jira Project name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_summary: Jira issue title/summary
+        :param pulumi.Input[str] action_pagerduty_integration_url: The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        :param pulumi.Input[str] action_pagerduty_integration_url_override: The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[bool] action_populate_lookup: The state of the populate lookup action. Read-only attribute. Value ignored on POST. Use actions to specify a list of enabled actions. Defaults to 0.
         :param pulumi.Input[str] action_populate_lookup_command: The search command (or pipeline) which is responsible for executing the action.
         :param pulumi.Input[str] action_populate_lookup_dest: Lookup name of path of the lookup to populate
         :param pulumi.Input[str] action_populate_lookup_hostname: Sets the hostname used in the web link (url) sent in alert actions.This value accepts two forms: hostname (for example, splunkserver, splunkserver.example.com)\\n\\nprotocol://hostname:port (for example, http://splunkserver:8000, https://splunkserver.example.com:443)
         :param pulumi.Input[int] action_populate_lookup_max_results: Sets the maximum number of search results sent using alerts. Defaults to 100.
         :param pulumi.Input[int] action_populate_lookup_max_time: Valid values are: Integer[m|s|h|d]Sets the maximum amount of time the execution of an action takes before the action is aborted. Defaults to 5m.
         :param pulumi.Input[bool] action_populate_lookup_track_alert: Indicates whether the execution of this action signifies a trackable alert.
@@ -2996,14 +3032,18 @@
             pulumi.set(__self__, "action_jira_service_desk_param_jira_issue_type", action_jira_service_desk_param_jira_issue_type)
         if action_jira_service_desk_param_jira_priority is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_priority", action_jira_service_desk_param_jira_priority)
         if action_jira_service_desk_param_jira_project is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_project", action_jira_service_desk_param_jira_project)
         if action_jira_service_desk_param_jira_summary is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_summary", action_jira_service_desk_param_jira_summary)
+        if action_pagerduty_integration_url is not None:
+            pulumi.set(__self__, "action_pagerduty_integration_url", action_pagerduty_integration_url)
+        if action_pagerduty_integration_url_override is not None:
+            pulumi.set(__self__, "action_pagerduty_integration_url_override", action_pagerduty_integration_url_override)
         if action_populate_lookup is not None:
             pulumi.set(__self__, "action_populate_lookup", action_populate_lookup)
         if action_populate_lookup_command is not None:
             pulumi.set(__self__, "action_populate_lookup_command", action_populate_lookup_command)
         if action_populate_lookup_dest is not None:
             pulumi.set(__self__, "action_populate_lookup_dest", action_populate_lookup_dest)
         if action_populate_lookup_hostname is not None:
@@ -3862,14 +3902,38 @@
         return pulumi.get(self, "action_jira_service_desk_param_jira_summary")
 
     @action_jira_service_desk_param_jira_summary.setter
     def action_jira_service_desk_param_jira_summary(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "action_jira_service_desk_param_jira_summary", value)
 
     @property
+    @pulumi.getter(name="actionPagerdutyIntegrationUrl")
+    def action_pagerduty_integration_url(self) -> Optional[pulumi.Input[str]]:
+        """
+        The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_url")
+
+    @action_pagerduty_integration_url.setter
+    def action_pagerduty_integration_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_integration_url", value)
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationUrlOverride")
+    def action_pagerduty_integration_url_override(self) -> Optional[pulumi.Input[str]]:
+        """
+        The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_url_override")
+
+    @action_pagerduty_integration_url_override.setter
+    def action_pagerduty_integration_url_override(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_integration_url_override", value)
+
+    @property
     @pulumi.getter(name="actionPopulateLookup")
     def action_populate_lookup(self) -> Optional[pulumi.Input[bool]]:
         """
         The state of the populate lookup action. Read-only attribute. Value ignored on POST. Use actions to specify a list of enabled actions. Defaults to 0.
         """
         return pulumi.get(self, "action_populate_lookup")
 
@@ -5226,14 +5290,16 @@
                  action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
                  action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_max_time: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_track_alert: Optional[pulumi.Input[bool]] = None,
                  action_populate_lookup_ttl: Optional[pulumi.Input[str]] = None,
@@ -5417,14 +5483,16 @@
         :param pulumi.Input[bool] action_email_width_sort_columns: Indicates whether columns should be sorted from least wide to most wide, left to right.Only valid if format=text.
         :param pulumi.Input[str] action_jira_service_desk_param_account: Jira Service Desk account name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_description: Jira issue description
         :param pulumi.Input[str] action_jira_service_desk_param_jira_issue_type: Jira issue type name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_priority: Jira priority of issue
         :param pulumi.Input[str] action_jira_service_desk_param_jira_project: Jira Project name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_summary: Jira issue title/summary
+        :param pulumi.Input[str] action_pagerduty_integration_url: The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        :param pulumi.Input[str] action_pagerduty_integration_url_override: The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[str] action_populate_lookup_command: The search command (or pipeline) which is responsible for executing the action.
         :param pulumi.Input[str] action_populate_lookup_dest: Lookup name of path of the lookup to populate
         :param pulumi.Input[str] action_populate_lookup_hostname: Sets the hostname used in the web link (url) sent in alert actions.This value accepts two forms: hostname (for example, splunkserver, splunkserver.example.com)\\n\\nprotocol://hostname:port (for example, http://splunkserver:8000, https://splunkserver.example.com:443)
         :param pulumi.Input[int] action_populate_lookup_max_results: Sets the maximum number of search results sent using alerts. Defaults to 100.
         :param pulumi.Input[int] action_populate_lookup_max_time: Valid values are: Integer[m|s|h|d]Sets the maximum amount of time the execution of an action takes before the action is aborted. Defaults to 5m.
         :param pulumi.Input[bool] action_populate_lookup_track_alert: Indicates whether the execution of this action signifies a trackable alert.
         :param pulumi.Input[str] action_populate_lookup_ttl: Valid values are Integer[p]Specifies the minimum time-to-live in seconds of the search artifacts if this action is triggered. If p follows Integer, then this specifies the number of scheduled periods. Defaults to 10p.
@@ -5637,14 +5705,16 @@
                  action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
                  action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_max_time: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_track_alert: Optional[pulumi.Input[bool]] = None,
                  action_populate_lookup_ttl: Optional[pulumi.Input[str]] = None,
@@ -5803,14 +5873,16 @@
             __props__.__dict__["action_email_width_sort_columns"] = action_email_width_sort_columns
             __props__.__dict__["action_jira_service_desk_param_account"] = action_jira_service_desk_param_account
             __props__.__dict__["action_jira_service_desk_param_jira_description"] = action_jira_service_desk_param_jira_description
             __props__.__dict__["action_jira_service_desk_param_jira_issue_type"] = action_jira_service_desk_param_jira_issue_type
             __props__.__dict__["action_jira_service_desk_param_jira_priority"] = action_jira_service_desk_param_jira_priority
             __props__.__dict__["action_jira_service_desk_param_jira_project"] = action_jira_service_desk_param_jira_project
             __props__.__dict__["action_jira_service_desk_param_jira_summary"] = action_jira_service_desk_param_jira_summary
+            __props__.__dict__["action_pagerduty_integration_url"] = action_pagerduty_integration_url
+            __props__.__dict__["action_pagerduty_integration_url_override"] = action_pagerduty_integration_url_override
             __props__.__dict__["action_populate_lookup_command"] = action_populate_lookup_command
             __props__.__dict__["action_populate_lookup_dest"] = action_populate_lookup_dest
             __props__.__dict__["action_populate_lookup_hostname"] = action_populate_lookup_hostname
             __props__.__dict__["action_populate_lookup_max_results"] = action_populate_lookup_max_results
             __props__.__dict__["action_populate_lookup_max_time"] = action_populate_lookup_max_time
             __props__.__dict__["action_populate_lookup_track_alert"] = action_populate_lookup_track_alert
             __props__.__dict__["action_populate_lookup_ttl"] = action_populate_lookup_ttl
@@ -5978,14 +6050,16 @@
             action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
             action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+            action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
+            action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
             action_populate_lookup: Optional[pulumi.Input[bool]] = None,
             action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
             action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
             action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
             action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
             action_populate_lookup_max_time: Optional[pulumi.Input[int]] = None,
             action_populate_lookup_track_alert: Optional[pulumi.Input[bool]] = None,
@@ -6147,14 +6221,16 @@
         :param pulumi.Input[bool] action_email_width_sort_columns: Indicates whether columns should be sorted from least wide to most wide, left to right.Only valid if format=text.
         :param pulumi.Input[str] action_jira_service_desk_param_account: Jira Service Desk account name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_description: Jira issue description
         :param pulumi.Input[str] action_jira_service_desk_param_jira_issue_type: Jira issue type name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_priority: Jira priority of issue
         :param pulumi.Input[str] action_jira_service_desk_param_jira_project: Jira Project name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_summary: Jira issue title/summary
+        :param pulumi.Input[str] action_pagerduty_integration_url: The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        :param pulumi.Input[str] action_pagerduty_integration_url_override: The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[bool] action_populate_lookup: The state of the populate lookup action. Read-only attribute. Value ignored on POST. Use actions to specify a list of enabled actions. Defaults to 0.
         :param pulumi.Input[str] action_populate_lookup_command: The search command (or pipeline) which is responsible for executing the action.
         :param pulumi.Input[str] action_populate_lookup_dest: Lookup name of path of the lookup to populate
         :param pulumi.Input[str] action_populate_lookup_hostname: Sets the hostname used in the web link (url) sent in alert actions.This value accepts two forms: hostname (for example, splunkserver, splunkserver.example.com)\\n\\nprotocol://hostname:port (for example, http://splunkserver:8000, https://splunkserver.example.com:443)
         :param pulumi.Input[int] action_populate_lookup_max_results: Sets the maximum number of search results sent using alerts. Defaults to 100.
         :param pulumi.Input[int] action_populate_lookup_max_time: Valid values are: Integer[m|s|h|d]Sets the maximum amount of time the execution of an action takes before the action is aborted. Defaults to 5m.
         :param pulumi.Input[bool] action_populate_lookup_track_alert: Indicates whether the execution of this action signifies a trackable alert.
@@ -6324,14 +6400,16 @@
         __props__.__dict__["action_email_width_sort_columns"] = action_email_width_sort_columns
         __props__.__dict__["action_jira_service_desk_param_account"] = action_jira_service_desk_param_account
         __props__.__dict__["action_jira_service_desk_param_jira_description"] = action_jira_service_desk_param_jira_description
         __props__.__dict__["action_jira_service_desk_param_jira_issue_type"] = action_jira_service_desk_param_jira_issue_type
         __props__.__dict__["action_jira_service_desk_param_jira_priority"] = action_jira_service_desk_param_jira_priority
         __props__.__dict__["action_jira_service_desk_param_jira_project"] = action_jira_service_desk_param_jira_project
         __props__.__dict__["action_jira_service_desk_param_jira_summary"] = action_jira_service_desk_param_jira_summary
+        __props__.__dict__["action_pagerduty_integration_url"] = action_pagerduty_integration_url
+        __props__.__dict__["action_pagerduty_integration_url_override"] = action_pagerduty_integration_url_override
         __props__.__dict__["action_populate_lookup"] = action_populate_lookup
         __props__.__dict__["action_populate_lookup_command"] = action_populate_lookup_command
         __props__.__dict__["action_populate_lookup_dest"] = action_populate_lookup_dest
         __props__.__dict__["action_populate_lookup_hostname"] = action_populate_lookup_hostname
         __props__.__dict__["action_populate_lookup_max_results"] = action_populate_lookup_max_results
         __props__.__dict__["action_populate_lookup_max_time"] = action_populate_lookup_max_time
         __props__.__dict__["action_populate_lookup_track_alert"] = action_populate_lookup_track_alert
@@ -6867,14 +6945,30 @@
     def action_jira_service_desk_param_jira_summary(self) -> pulumi.Output[Optional[str]]:
         """
         Jira issue title/summary
         """
         return pulumi.get(self, "action_jira_service_desk_param_jira_summary")
 
     @property
+    @pulumi.getter(name="actionPagerdutyIntegrationUrl")
+    def action_pagerduty_integration_url(self) -> pulumi.Output[Optional[str]]:
+        """
+        The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_url")
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationUrlOverride")
+    def action_pagerduty_integration_url_override(self) -> pulumi.Output[Optional[str]]:
+        """
+        The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_url_override")
+
+    @property
     @pulumi.getter(name="actionPopulateLookup")
     def action_populate_lookup(self) -> pulumi.Output[bool]:
         """
         The state of the populate lookup action. Read-only attribute. Value ignored on POST. Use actions to specify a list of enabled actions. Defaults to 0.
         """
         return pulumi.get(self, "action_populate_lookup")
```

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk/sh_indexes_manager.py` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk/sh_indexes_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/PKG-INFO` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-splunk
-Version: 1.3.0a1684390969
+Version: 1.3.0a1684788643
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi splunk
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-splunk/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-splunk/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fsplunk.svg)](https://www.npmjs.com/package/@pulumi/splunk)
 [![Python version](https://badge.fury.io/py/pulumi-splunk.svg)](https://pypi.org/project/pulumi-splunk)
 [![NuGet version](https://badge.fury.io/nu/pulumi.splunk.svg)](https://badge.fury.io/nu/pulumi.splunk)
```

### Comparing `pulumi_splunk-1.3.0a1684390969/pulumi_splunk.egg-info/SOURCES.txt` & `pulumi_splunk-1.3.0a1684788643/pulumi_splunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1684390969/setup.py` & `pulumi_splunk-1.3.0a1684788643/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0a1684390969"
-PLUGIN_VERSION = "1.3.0-alpha.1684390969+7f7328cc"
+VERSION = "1.3.0a1684788643"
+PLUGIN_VERSION = "1.3.0-alpha.1684788643+8850b8e5"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'splunk', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "splunk Pulumi Package - Development Version"
 
 
 setup(name='pulumi_splunk',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing splunk cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

