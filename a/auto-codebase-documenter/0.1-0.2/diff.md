# Comparing `tmp/auto-codebase-documenter-0.1.tar.gz` & `tmp/auto-codebase-documenter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-codebase-documenter-0.1.tar", last modified: Mon May 22 01:13:02 2023, max compression
+gzip compressed data, was "auto-codebase-documenter-0.2.tar", last modified: Mon May 22 01:24:41 2023, max compression
```

## Comparing `auto-codebase-documenter-0.1.tar` & `auto-codebase-documenter-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:13:02.657697 auto-codebase-documenter-0.1/
--rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.1/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      169 2023-05-22 01:13:02.657697 auto-codebase-documenter-0.1/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     8346 2023-05-22 00:14:55.000000 auto-codebase-documenter-0.1/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:13:02.657697 auto-codebase-documenter-0.1/auto_codebase_documenter/
--rw-r--r--   0 alex      (1000) alex      (1000)     5810 2023-05-22 01:04:32.000000 auto-codebase-documenter-0.1/auto_codebase_documenter/AutoCodebaseDocumenter.py
--rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 00:15:35.000000 auto-codebase-documenter-0.1/auto_codebase_documenter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.1/auto_codebase_documenter/default_ai_prompt.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:13:02.657697 auto-codebase-documenter-0.1/auto_codebase_documenter.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      169 2023-05-22 01:13:02.000000 auto-codebase-documenter-0.1/auto_codebase_documenter.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 01:13:02.000000 auto-codebase-documenter-0.1/auto_codebase_documenter.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 01:13:02.000000 auto-codebase-documenter-0.1/auto_codebase_documenter.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       80 2023-05-22 01:13:02.000000 auto-codebase-documenter-0.1/auto_codebase_documenter.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       21 2023-05-22 01:13:02.000000 auto-codebase-documenter-0.1/auto_codebase_documenter.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 01:13:02.000000 auto-codebase-documenter-0.1/auto_codebase_documenter.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 01:13:02.657697 auto-codebase-documenter-0.1/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      332 2023-05-22 00:20:02.000000 auto-codebase-documenter-0.1/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1096 2023-05-21 13:35:47.000000 auto-codebase-documenter-0.2/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      640 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     8346 2023-05-22 00:14:55.000000 auto-codebase-documenter-0.2/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/auto_codebase_documenter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     5810 2023-05-22 01:04:32.000000 auto-codebase-documenter-0.2/auto_codebase_documenter/AutoCodebaseDocumenter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       59 2023-05-22 00:15:35.000000 auto-codebase-documenter-0.2/auto_codebase_documenter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1494 2023-05-22 01:01:13.000000 auto-codebase-documenter-0.2/auto_codebase_documenter/default_ai_prompt.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      640 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      450 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       80 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       21 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       25 2023-05-22 01:24:41.000000 auto-codebase-documenter-0.2/auto_codebase_documenter.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-22 01:24:41.509654 auto-codebase-documenter-0.2/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      926 2023-05-22 01:19:57.000000 auto-codebase-documenter-0.2/setup.py
```

### Comparing `auto-codebase-documenter-0.1/LICENSE` & `auto-codebase-documenter-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.1/README.md` & `auto-codebase-documenter-0.2/README.md`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.1/auto_codebase_documenter/AutoCodebaseDocumenter.py` & `auto-codebase-documenter-0.2/auto_codebase_documenter/AutoCodebaseDocumenter.py`

 * *Files identical despite different names*

### Comparing `auto-codebase-documenter-0.1/auto_codebase_documenter/default_ai_prompt.py` & `auto-codebase-documenter-0.2/auto_codebase_documenter/default_ai_prompt.py`

 * *Files identical despite different names*

