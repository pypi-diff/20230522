# Comparing `tmp/pulumi-remote-stack-0.1.5.tar.gz` & `tmp/pulumi-remote-stack-0.1.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi-remote-stack-0.1.5.tar", last modified: Mon May 22 14:13:23 2023, max compression
+gzip compressed data, was "pulumi-remote-stack-0.1.5.dev0.tar", last modified: Mon May 22 14:07:18 2023, max compression
```

## Comparing `pulumi-remote-stack-0.1.5.tar` & `pulumi-remote-stack-0.1.5.dev0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 beer      (1000) beer      (1000)        0 2023-05-22 14:13:23.986059 pulumi-remote-stack-0.1.5/
--rw-r--r--   0 beer      (1000) beer      (1000)    11357 2022-01-22 19:07:45.000000 pulumi-remote-stack-0.1.5/LICENSE
--rw-r--r--   0 beer      (1000) beer      (1000)      917 2023-05-22 14:13:23.986059 pulumi-remote-stack-0.1.5/PKG-INFO
--rw-r--r--   0 beer      (1000) beer      (1000)      393 2023-05-22 14:08:13.000000 pulumi-remote-stack-0.1.5/README.md
--rw-r--r--   0 beer      (1000) beer      (1000)      103 2021-09-16 16:49:56.000000 pulumi-remote-stack-0.1.5/pyproject.toml
--rw-r--r--   0 beer      (1000) beer      (1000)      672 2023-05-22 14:13:23.986059 pulumi-remote-stack-0.1.5/setup.cfg
-drwxr-xr-x   0 beer      (1000) beer      (1000)        0 2023-05-22 14:13:23.982725 pulumi-remote-stack-0.1.5/src/
-drwxr-xr-x   0 beer      (1000) beer      (1000)        0 2023-05-22 14:13:23.982725 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/
--rwxr-xr-x   0 beer      (1000) beer      (1000)       71 2021-12-02 20:02:07.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/__init__.py
--rwxr-xr-x   0 beer      (1000) beer      (1000)      789 2021-12-02 20:02:07.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/config.py
--rwxr-xr-x   0 beer      (1000) beer      (1000)     8667 2023-05-22 14:12:11.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/provider.py
--rwxr-xr-x   0 beer      (1000) beer      (1000)     1618 2021-12-02 20:02:07.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/remote_stack.py
--rwxr-xr-x   0 beer      (1000) beer      (1000)      682 2021-12-02 20:02:07.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/subprocess_run.py
-drwxr-xr-x   0 beer      (1000) beer      (1000)        0 2023-05-22 14:13:23.986059 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack.egg-info/
--rw-r--r--   0 beer      (1000) beer      (1000)      917 2023-05-22 14:13:23.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack.egg-info/PKG-INFO
--rw-r--r--   0 beer      (1000) beer      (1000)      418 2023-05-22 14:13:23.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack.egg-info/SOURCES.txt
--rw-r--r--   0 beer      (1000) beer      (1000)        1 2023-05-22 14:13:23.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack.egg-info/dependency_links.txt
--rw-r--r--   0 beer      (1000) beer      (1000)       20 2023-05-22 14:13:23.000000 pulumi-remote-stack-0.1.5/src/pulumi_remote_stack.egg-info/top_level.txt
+drwxr-xr-x   0 beer      (1000) beer      (1000)        0 2023-05-22 14:07:18.405510 pulumi-remote-stack-0.1.5.dev0/
+-rw-r--r--   0 beer      (1000) beer      (1000)    11357 2022-01-22 19:07:45.000000 pulumi-remote-stack-0.1.5.dev0/LICENSE
+-rw-r--r--   0 beer      (1000) beer      (1000)      691 2023-05-22 14:07:18.405510 pulumi-remote-stack-0.1.5.dev0/PKG-INFO
+-rw-r--r--   0 beer      (1000) beer      (1000)      162 2023-03-29 19:19:03.000000 pulumi-remote-stack-0.1.5.dev0/README.md
+-rw-r--r--   0 beer      (1000) beer      (1000)      103 2021-09-16 16:49:56.000000 pulumi-remote-stack-0.1.5.dev0/pyproject.toml
+-rw-r--r--   0 beer      (1000) beer      (1000)      677 2023-05-22 14:07:18.405510 pulumi-remote-stack-0.1.5.dev0/setup.cfg
+drwxr-xr-x   0 beer      (1000) beer      (1000)        0 2023-05-22 14:07:18.402176 pulumi-remote-stack-0.1.5.dev0/src/
+drwxr-xr-x   0 beer      (1000) beer      (1000)        0 2023-05-22 14:07:18.402176 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/
+-rwxr-xr-x   0 beer      (1000) beer      (1000)       71 2021-12-02 20:02:07.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/__init__.py
+-rwxr-xr-x   0 beer      (1000) beer      (1000)      789 2021-12-02 20:02:07.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/config.py
+-rwxr-xr-x   0 beer      (1000) beer      (1000)     8706 2023-05-22 14:04:38.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/provider.py
+-rwxr-xr-x   0 beer      (1000) beer      (1000)     1618 2021-12-02 20:02:07.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/remote_stack.py
+-rwxr-xr-x   0 beer      (1000) beer      (1000)      682 2021-12-02 20:02:07.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/subprocess_run.py
+drwxr-xr-x   0 beer      (1000) beer      (1000)        0 2023-05-22 14:07:18.405510 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack.egg-info/
+-rw-r--r--   0 beer      (1000) beer      (1000)      691 2023-05-22 14:07:18.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack.egg-info/PKG-INFO
+-rw-r--r--   0 beer      (1000) beer      (1000)      418 2023-05-22 14:07:18.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 beer      (1000) beer      (1000)        1 2023-05-22 14:07:18.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 beer      (1000) beer      (1000)       20 2023-05-22 14:07:18.000000 pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack.egg-info/top_level.txt
```

### Comparing `pulumi-remote-stack-0.1.5/LICENSE` & `pulumi-remote-stack-0.1.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pulumi-remote-stack-0.1.5/setup.cfg` & `pulumi-remote-stack-0.1.5.dev0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pulumi-remote-stack
-version = 0.1.5
+version = 0.1.5.dev0
 author = Jan Češpivo
 license_files = LICENSE
 author_email = developers@allusio.com
 description = Pulumi Remote Stack
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/pulumi-remote-stack
```

### Comparing `pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/config.py` & `pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/config.py`

 * *Files identical despite different names*

### Comparing `pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/provider.py` & `pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,16 @@
         else:
             stack = create_or_select_stack(**kwargs)
             _patch_get_all_config(project_name, stack)
             try:
                 stack.refresh_config()
             except CommandError as command_error:
                 command_result = command_error.args[0]
-                if 'error: no previous deployment' not in command_result:
+                stderr = command_result.stderr
+                if 'error: no previous deployment' not in stderr:
                     raise command_error
 
         stack_config = (
             {
                 key: _PulumiConfigValue(
                     value=config_value["value"],
                     secret=False,
```

### Comparing `pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/remote_stack.py` & `pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/remote_stack.py`

 * *Files identical despite different names*

### Comparing `pulumi-remote-stack-0.1.5/src/pulumi_remote_stack/subprocess_run.py` & `pulumi-remote-stack-0.1.5.dev0/src/pulumi_remote_stack/subprocess_run.py`

 * *Files identical despite different names*

