# Comparing `tmp/pysen-plugins-2023.5.10.tar.gz` & `tmp/pysen-plugins-2023.5.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysen-plugins-2023.5.10.tar", last modified: Wed May 10 10:27:54 2023, max compression
+gzip compressed data, was "pysen-plugins-2023.5.22.tar", last modified: Mon May 22 03:36:17 2023, max compression
```

## Comparing `pysen-plugins-2023.5.10.tar` & `pysen-plugins-2023.5.22.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 10:27:54.770502 pysen-plugins-2023.5.10/
--rw-r--r--   0 root         (0) root         (0)     1081 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2246 2023-05-10 10:27:54.767169 pysen-plugins-2023.5.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/README.md
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 10:27:54.767169 pysen-plugins-2023.5.10/pysen_plugins/
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-10 10:27:38.000000 pysen-plugins-2023.5.10/pysen_plugins/_version.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/clang_format.py
--rw-r--r--   0 root         (0) root         (0)     3495 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/cmake_format.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/golint.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/goreturns.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/jq.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/mypy_init_check.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/mypy_simple.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/prettier.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 10:27:54.767169 pysen-plugins-2023.5.10/pysen_plugins/pylint/
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/pylint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/pylint/command.py
--rw-r--r--   0 root         (0) root         (0)      607 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/pylint/component.py
--rw-r--r--   0 root         (0) root         (0)      660 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/pylint/plugin.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/ruamel_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 10:27:54.767169 pysen-plugins-2023.5.10/pysen_plugins/ruff/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/ruff/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4732 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/ruff/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/ruff/preset.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/shellcheck.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/shfmt.py
--rw-r--r--   0 root         (0) root         (0)     2847 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/pysen_plugins/tidy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 10:27:54.767169 pysen-plugins-2023.5.10/pysen_plugins.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2246 2023-05-10 10:27:54.000000 pysen-plugins-2023.5.10/pysen_plugins.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-10 10:27:54.000000 pysen-plugins-2023.5.10/pysen_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 10:27:54.000000 pysen-plugins-2023.5.10/pysen_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-10 10:27:54.000000 pysen-plugins-2023.5.10/pysen_plugins.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-10 10:27:54.000000 pysen-plugins-2023.5.10/pysen_plugins.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 10:27:54.770502 pysen-plugins-2023.5.10/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-10 09:38:03.000000 pysen-plugins-2023.5.10/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/README.md
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.132679 pysen-plugins-2023.5.22/pysen_plugins/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-22 03:35:48.000000 pysen-plugins-2023.5.22/pysen_plugins/_version.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/clang_format.py
+-rw-r--r--   0 root         (0) root         (0)     3495 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/cmake_format.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/golint.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/goreturns.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/jq.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/mypy_init_check.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/mypy_simple.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/prettier.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/pysen_plugins/pylint/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/pylint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/pylint/command.py
+-rw-r--r--   0 root         (0) root         (0)      607 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/pylint/component.py
+-rw-r--r--   0 root         (0) root         (0)      660 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/pylint/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/ruamel_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/pysen_plugins/ruff/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/ruff/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4732 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/ruff/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/ruff/preset.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/shellcheck.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/shfmt.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/tidy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/pysen_plugins.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      852 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/setup.py
```

### Comparing `pysen-plugins-2023.5.10/LICENSE` & `pysen-plugins-2023.5.22/LICENSE`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/PKG-INFO` & `pysen-plugins-2023.5.22/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pysen-plugins
-Version: 2023.5.10
+Version: 2023.5.22
 Summary: Collection of pysen plugins
-Home-page: UNKNOWN
 Author: Toru Ogawa, Ryo Miyajima, Yuki Igarashi
 Author-email: ogawa@preferred.jp, ryo@preferred.jp, igarashi@preferred.jp
 License: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -67,9 +65,7 @@
 - TypeScript
   - [prettier](https://prettier.io) (lint, format)
 - XML
   - [tidy](http://www.html-tidy.org) (lint, format)
 - YAML
   - [prettier](https://prettier.io) (lint, format)
   - [ruamel_yaml](https://sourceforge.net/projects/ruamel-yaml) (lint, format)
-
-
```

### Comparing `pysen-plugins-2023.5.10/README.md` & `pysen-plugins-2023.5.22/README.md`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/__init__.py` & `pysen-plugins-2023.5.22/pysen_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/clang_format.py` & `pysen-plugins-2023.5.22/pysen_plugins/clang_format.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/cmake_format.py` & `pysen-plugins-2023.5.22/pysen_plugins/cmake_format.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/golint.py` & `pysen-plugins-2023.5.22/pysen_plugins/golint.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/goreturns.py` & `pysen-plugins-2023.5.22/pysen_plugins/goreturns.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/jq.py` & `pysen-plugins-2023.5.22/pysen_plugins/jq.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/mypy_init_check.py` & `pysen-plugins-2023.5.22/pysen_plugins/mypy_init_check.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/mypy_simple.py` & `pysen-plugins-2023.5.22/pysen_plugins/mypy_simple.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/prettier.py` & `pysen-plugins-2023.5.22/pysen_plugins/prettier.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/pylint/command.py` & `pysen-plugins-2023.5.22/pysen_plugins/pylint/command.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/pylint/component.py` & `pysen-plugins-2023.5.22/pysen_plugins/pylint/component.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/pylint/plugin.py` & `pysen-plugins-2023.5.22/pysen_plugins/pylint/plugin.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/ruamel_yaml.py` & `pysen-plugins-2023.5.22/pysen_plugins/ruamel_yaml.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/ruff/plugin.py` & `pysen-plugins-2023.5.22/pysen_plugins/ruff/plugin.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/ruff/preset.py` & `pysen-plugins-2023.5.22/pysen_plugins/ruff/preset.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/shellcheck.py` & `pysen-plugins-2023.5.22/pysen_plugins/shellcheck.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/shfmt.py` & `pysen-plugins-2023.5.22/pysen_plugins/shfmt.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins/tidy.py` & `pysen-plugins-2023.5.22/pysen_plugins/tidy.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/pysen_plugins.egg-info/PKG-INFO` & `pysen-plugins-2023.5.22/pysen_plugins.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pysen-plugins
-Version: 2023.5.10
+Version: 2023.5.22
 Summary: Collection of pysen plugins
-Home-page: UNKNOWN
 Author: Toru Ogawa, Ryo Miyajima, Yuki Igarashi
 Author-email: ogawa@preferred.jp, ryo@preferred.jp, igarashi@preferred.jp
 License: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -67,9 +65,7 @@
 - TypeScript
   - [prettier](https://prettier.io) (lint, format)
 - XML
   - [tidy](http://www.html-tidy.org) (lint, format)
 - YAML
   - [prettier](https://prettier.io) (lint, format)
   - [ruamel_yaml](https://sourceforge.net/projects/ruamel-yaml) (lint, format)
-
-
```

### Comparing `pysen-plugins-2023.5.10/pysen_plugins.egg-info/SOURCES.txt` & `pysen-plugins-2023.5.22/pysen_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.10/setup.py` & `pysen-plugins-2023.5.22/setup.py`

 * *Files identical despite different names*

