# Comparing `tmp/yambs-1.4.3.tar.gz` & `tmp/yambs-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.4.3.tar", last modified: Mon May 22 00:23:27 2023, max compression
+gzip compressed data, was "yambs-1.4.4.tar", last modified: Mon May 22 06:52:53 2023, max compression
```

## Comparing `yambs-1.4.3.tar` & `yambs-1.4.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.735551 yambs-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 00:22:18.000000 yambs-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-22 00:23:27.735551 yambs-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-22 00:22:18.000000 yambs-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-22 00:22:18.000000 yambs-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:23:27.735551 yambs-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 00:22:18.000000 yambs-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.727551 yambs-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 00:22:18.000000 yambs-1.4.3/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 00:22:18.000000 yambs-1.4.3/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.731551 yambs-1.4.3/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.731551 yambs-1.4.3/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.731551 yambs-1.4.3/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/config/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.731551 yambs-1.4.3/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.731551 yambs-1.4.3/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/includes/microchip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.731551 yambs-1.4.3/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.731551 yambs-1.4.3/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.735551 yambs-1.4.3/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/generate/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/generate/ninja.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.735551 yambs-1.4.3/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-22 00:22:18.000000 yambs-1.4.3/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:23:27.731551 yambs-1.4.3/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-22 00:23:27.000000 yambs-1.4.3/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-22 00:23:27.000000 yambs-1.4.3/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:23:27.000000 yambs-1.4.3/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 00:23:27.000000 yambs-1.4.3/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 00:23:27.000000 yambs-1.4.3/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 00:23:27.000000 yambs-1.4.3/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.295321 yambs-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 06:51:28.000000 yambs-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-22 06:52:53.295321 yambs-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-22 06:51:28.000000 yambs-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-22 06:51:28.000000 yambs-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:52:53.295321 yambs-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 06:51:28.000000 yambs-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.287321 yambs-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 06:51:28.000000 yambs-1.4.4/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 06:51:28.000000 yambs-1.4.4/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.291321 yambs-1.4.4/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.291321 yambs-1.4.4/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.291321 yambs-1.4.4/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/config/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.291321 yambs-1.4.4/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.291321 yambs-1.4.4/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/includes/microchip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.291321 yambs-1.4.4/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.295321 yambs-1.4.4/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.295321 yambs-1.4.4/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/generate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/generate/ninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.295321 yambs-1.4.4/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-22 06:51:28.000000 yambs-1.4.4/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:52:53.291321 yambs-1.4.4/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-22 06:52:53.000000 yambs-1.4.4/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-22 06:52:53.000000 yambs-1.4.4/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:52:53.000000 yambs-1.4.4/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 06:52:53.000000 yambs-1.4.4/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 06:52:53.000000 yambs-1.4.4/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 06:52:53.000000 yambs-1.4.4/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.4.3/LICENSE` & `yambs-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/PKG-INFO` & `yambs-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.4.3
+Version: 1.4.4
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=10c6b8348a72ce9ed5f13672daaa97b4
+    hash=a2579df1d732e7a3917254efbd2529ed
     =====================================
 -->
 
-# yambs ([1.4.3](https://pypi.org/project/yambs/))
+# yambs ([1.4.4](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.4.3/README.md` & `yambs-1.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=10c6b8348a72ce9ed5f13672daaa97b4
+    hash=a2579df1d732e7a3917254efbd2529ed
     =====================================
 -->
 
-# yambs ([1.4.3](https://pypi.org/project/yambs/))
+# yambs ([1.4.4](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.4.3/pyproject.toml` & `yambs-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.4.3"
+version = "1.4.4"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.4.3/setup.py` & `yambs-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/tests/test_entry.py` & `yambs-1.4.4/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/app.py` & `yambs-1.4.4/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/commands/all.py` & `yambs-1.4.4/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/commands/gen.py` & `yambs-1.4.4/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/commands/uf2conv.py` & `yambs-1.4.4/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/config/__init__.py` & `yambs-1.4.4/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/config/board.py` & `yambs-1.4.4/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/data/includes/chips.yaml` & `yambs-1.4.4/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/data/includes/infineon.yaml` & `yambs-1.4.4/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/data/includes/microchip.yaml` & `yambs-1.4.4/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/data/schemas/Chip.yaml` & `yambs-1.4.4/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/data/schemas/Config.yaml` & `yambs-1.4.4/yambs/data/schemas/Config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
   src_root:
     type: string
     default: src
 
   default_target:
     type: string
-    default: all_boards
+    default: all
 
   ninja_out:
     type: string
     default: ninja
 
   build_root:
     type: string
```

### Comparing `yambs-1.4.3/yambs/data/templates/rules.ninja.j2` & `yambs-1.4.4/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/data/uf2families.json` & `yambs-1.4.4/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/entry.py` & `yambs-1.4.4/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/generate/__init__.py` & `yambs-1.4.4/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/generate/architectures.py` & `yambs-1.4.4/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/generate/boards.py` & `yambs-1.4.4/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/generate/chips.py` & `yambs-1.4.4/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/generate/common.py` & `yambs-1.4.4/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/generate/ninja.py` & `yambs-1.4.4/yambs/generate/ninja.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/generate/toolchains.py` & `yambs-1.4.4/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/schemas.py` & `yambs-1.4.4/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs/uf2/__init__.py` & `yambs-1.4.4/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.3/yambs.egg-info/PKG-INFO` & `yambs-1.4.4/yambs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.4.3
+Version: 1.4.4
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=10c6b8348a72ce9ed5f13672daaa97b4
+    hash=a2579df1d732e7a3917254efbd2529ed
     =====================================
 -->
 
-# yambs ([1.4.3](https://pypi.org/project/yambs/))
+# yambs ([1.4.4](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.4.3/yambs.egg-info/SOURCES.txt` & `yambs-1.4.4/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

