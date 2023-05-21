# Comparing `tmp/mirror-tool-2023.5.tar.gz` & `tmp/mirror-tool-2023.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirror-tool-2023.5.tar", last modified: Sun May 21 23:43:52 2023, max compression
+gzip compressed data, was "mirror-tool-2023.5.21.tar", last modified: Sun May 21 23:50:38 2023, max compression
```

## Comparing `mirror-tool-2023.5.tar` & `mirror-tool-2023.5.21.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.277670 mirror-tool-2023.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 23:43:38.000000 mirror-tool-2023.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    51277 2023-05-21 23:43:52.277670 mirror-tool-2023.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-05-21 23:43:38.000000 mirror-tool-2023.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.273670 mirror-tool-2023.5/mirror_tool/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8164 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/git_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/git_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.277670 mirror-tool-2023.5/mirror_tool/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/ci_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/promote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.277670 mirror-tool-2023.5/mirror_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    51277 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-21 23:43:38.000000 mirror-tool-2023.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:43:52.277670 mirror-tool-2023.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.277670 mirror-tool-2023.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-21 23:43:38.000000 mirror-tool-2023.5/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:50:38.752239 mirror-tool-2023.5.21/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    51132 2023-05-21 23:50:38.752239 mirror-tool-2023.5.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:50:38.748239 mirror-tool-2023.5.21/mirror_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-21 23:50:38.000000 mirror-tool-2023.5.21/mirror_tool/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8164 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/git_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/git_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:50:38.752239 mirror-tool-2023.5.21/mirror_tool/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/gitlab/ci_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/gitlab/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/gitlab/promote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/gitlab/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/mirror_tool/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:50:38.748239 mirror-tool-2023.5.21/mirror_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    51132 2023-05-21 23:50:38.000000 mirror-tool-2023.5.21/mirror_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-21 23:50:38.000000 mirror-tool-2023.5.21/mirror_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:50:38.000000 mirror-tool-2023.5.21/mirror_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-21 23:50:38.000000 mirror-tool-2023.5.21/mirror_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 23:50:38.000000 mirror-tool-2023.5.21/mirror_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:50:38.752239 mirror-tool-2023.5.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:50:38.752239 mirror-tool-2023.5.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-21 23:50:22.000000 mirror-tool-2023.5.21/tests/test_import.py
```

### Comparing `mirror-tool-2023.5/LICENSE` & `mirror-tool-2023.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/PKG-INFO` & `mirror-tool-2023.5.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirror-tool
-Version: 2023.5
+Version: 2023.5.21
 Summary: A tool for managing git mirrors.
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,15 +684,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mirror-tool
 
 A tool for maintaining Git subtree mirrors.
 
-[![CI](https://github.com/rohanpm/mirror-tool/actions/workflows/ci.yml/badge.svg)](https://github.com/rohanpm/mirror-tool/actions/workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/mirror-tool)](https://pypi.org/pypi/mirror-tool) [![Docker Repository on Quay](https://quay.io/repository/rmcgover/mirror-tool/status "Docker Repository on Quay")](https://quay.io/repository/rmcgover/mirror-tool)
+[![PyPI](https://img.shields.io/pypi/v/mirror-tool)](https://pypi.org/pypi/mirror-tool) [![Docker Repository on Quay](https://quay.io/repository/rmcgover/mirror-tool/status "Docker Repository on Quay")](https://quay.io/repository/rmcgover/mirror-tool)
 
 <!--TOC-->
 
 - [mirror-tool](#mirror-tool)
   - [Installation](#installation)
   - [Usage](#usage)
     - [`mirror-tool validate-config`](#mirror-tool-validate-config)
```

### Comparing `mirror-tool-2023.5/README.md` & `mirror-tool-2023.5.21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # mirror-tool
 
 A tool for maintaining Git subtree mirrors.
 
-[![CI](https://github.com/rohanpm/mirror-tool/actions/workflows/ci.yml/badge.svg)](https://github.com/rohanpm/mirror-tool/actions/workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/mirror-tool)](https://pypi.org/pypi/mirror-tool) [![Docker Repository on Quay](https://quay.io/repository/rmcgover/mirror-tool/status "Docker Repository on Quay")](https://quay.io/repository/rmcgover/mirror-tool)
+[![PyPI](https://img.shields.io/pypi/v/mirror-tool)](https://pypi.org/pypi/mirror-tool) [![Docker Repository on Quay](https://quay.io/repository/rmcgover/mirror-tool/status "Docker Repository on Quay")](https://quay.io/repository/rmcgover/mirror-tool)
 
 <!--TOC-->
 
 - [mirror-tool](#mirror-tool)
   - [Installation](#installation)
   - [Usage](#usage)
     - [`mirror-tool validate-config`](#mirror-tool-validate-config)
```

### Comparing `mirror-tool-2023.5/mirror_tool/cmd.py` & `mirror-tool-2023.5.21/mirror_tool/cmd.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/mirror_tool/conf.py` & `mirror-tool-2023.5.21/mirror_tool/conf.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/mirror_tool/git_info.py` & `mirror-tool-2023.5.21/mirror_tool/git_info.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/mirror_tool/gitlab/ci_template.py` & `mirror-tool-2023.5.21/mirror_tool/gitlab/ci_template.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/mirror_tool/gitlab/common.py` & `mirror-tool-2023.5.21/mirror_tool/gitlab/common.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/mirror_tool/gitlab/promote.py` & `mirror-tool-2023.5.21/mirror_tool/gitlab/promote.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/mirror_tool/gitlab/update.py` & `mirror-tool-2023.5.21/mirror_tool/gitlab/update.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/mirror_tool/jinja.py` & `mirror-tool-2023.5.21/mirror_tool/jinja.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/mirror_tool.egg-info/PKG-INFO` & `mirror-tool-2023.5.21/mirror_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirror-tool
-Version: 2023.5
+Version: 2023.5.21
 Summary: A tool for managing git mirrors.
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,15 +684,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mirror-tool
 
 A tool for maintaining Git subtree mirrors.
 
-[![CI](https://github.com/rohanpm/mirror-tool/actions/workflows/ci.yml/badge.svg)](https://github.com/rohanpm/mirror-tool/actions/workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/mirror-tool)](https://pypi.org/pypi/mirror-tool) [![Docker Repository on Quay](https://quay.io/repository/rmcgover/mirror-tool/status "Docker Repository on Quay")](https://quay.io/repository/rmcgover/mirror-tool)
+[![PyPI](https://img.shields.io/pypi/v/mirror-tool)](https://pypi.org/pypi/mirror-tool) [![Docker Repository on Quay](https://quay.io/repository/rmcgover/mirror-tool/status "Docker Repository on Quay")](https://quay.io/repository/rmcgover/mirror-tool)
 
 <!--TOC-->
 
 - [mirror-tool](#mirror-tool)
   - [Installation](#installation)
   - [Usage](#usage)
     - [`mirror-tool validate-config`](#mirror-tool-validate-config)
```

### Comparing `mirror-tool-2023.5/mirror_tool.egg-info/SOURCES.txt` & `mirror-tool-2023.5.21/mirror_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mirror-tool-2023.5/pyproject.toml` & `mirror-tool-2023.5.21/pyproject.toml`

 * *Files identical despite different names*

