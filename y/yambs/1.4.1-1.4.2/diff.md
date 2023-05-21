# Comparing `tmp/yambs-1.4.1.tar.gz` & `tmp/yambs-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.4.1.tar", last modified: Sun May 21 20:51:07 2023, max compression
+gzip compressed data, was "yambs-1.4.2.tar", last modified: Sun May 21 22:00:53 2023, max compression
```

## Comparing `yambs-1.4.1.tar` & `yambs-1.4.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.970376 yambs-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 20:50:02.000000 yambs-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-21 20:51:07.970376 yambs-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-21 20:50:02.000000 yambs-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-21 20:50:02.000000 yambs-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 20:51:07.970376 yambs-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-21 20:50:02.000000 yambs-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.966376 yambs-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-21 20:50:02.000000 yambs-1.4.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-21 20:50:02.000000 yambs-1.4.1/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.966376 yambs-1.4.1/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.966376 yambs-1.4.1/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.966376 yambs-1.4.1/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/config/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.966376 yambs-1.4.1/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.966376 yambs-1.4.1/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/includes/microchip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.970376 yambs-1.4.1/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.970376 yambs-1.4.1/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.970376 yambs-1.4.1/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/generate/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/generate/ninja.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.970376 yambs-1.4.1/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-21 20:50:02.000000 yambs-1.4.1/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:51:07.966376 yambs-1.4.1/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-21 20:51:07.000000 yambs-1.4.1/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-21 20:51:07.000000 yambs-1.4.1/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 20:51:07.000000 yambs-1.4.1/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-21 20:51:07.000000 yambs-1.4.1/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-21 20:51:07.000000 yambs-1.4.1/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 20:51:07.000000 yambs-1.4.1/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 21:59:45.000000 yambs-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-21 22:00:53.419499 yambs-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-21 21:59:45.000000 yambs-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-21 21:59:45.000000 yambs-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 22:00:53.419499 yambs-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-21 21:59:45.000000 yambs-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.415499 yambs-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-21 21:59:45.000000 yambs-1.4.2/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-21 21:59:45.000000 yambs-1.4.2/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.415499 yambs-1.4.2/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/config/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/includes/microchip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/generate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/generate/ninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.419499 yambs-1.4.2/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-21 21:59:45.000000 yambs-1.4.2/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:00:53.415499 yambs-1.4.2/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-21 22:00:53.000000 yambs-1.4.2/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-21 22:00:53.000000 yambs-1.4.2/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:00:53.000000 yambs-1.4.2/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-21 22:00:53.000000 yambs-1.4.2/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-21 22:00:53.000000 yambs-1.4.2/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 22:00:53.000000 yambs-1.4.2/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.4.1/LICENSE` & `yambs-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/PKG-INFO` & `yambs-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.4.1
+Version: 1.4.2
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
-    hash=2e388f2b5ac420fb7c63d634fad57093
+    hash=d66d7ab188c69e98ef4cfbd904223a7d
     =====================================
 -->
 
-# yambs ([1.4.1](https://pypi.org/project/yambs/))
+# yambs ([1.4.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.4.1/README.md` & `yambs-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=2e388f2b5ac420fb7c63d634fad57093
+    hash=d66d7ab188c69e98ef4cfbd904223a7d
     =====================================
 -->
 
-# yambs ([1.4.1](https://pypi.org/project/yambs/))
+# yambs ([1.4.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.4.1/pyproject.toml` & `yambs-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.4.1"
+version = "1.4.2"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.4.1/setup.py` & `yambs-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/tests/test_entry.py` & `yambs-1.4.2/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/app.py` & `yambs-1.4.2/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/commands/all.py` & `yambs-1.4.2/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/commands/gen.py` & `yambs-1.4.2/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/commands/uf2conv.py` & `yambs-1.4.2/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/config/__init__.py` & `yambs-1.4.2/yambs/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A module implementing a configuration interface for the package.
 """
 
 # built-in
 from pathlib import Path
-from typing import Any, Dict, Iterator, Tuple
+from typing import Any, Dict, Iterator, List, Tuple
 
 # third-party
 from vcorelib.dict import merge
 from vcorelib.dict.codec import BasicDictCodec as _BasicDictCodec
 from vcorelib.io import ARBITER as _ARBITER
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.paths import Pathlike, find_file
@@ -19,20 +19,33 @@
 from yambs.schemas import YambsDictCodec as _YambsDictCodec
 
 
 class Config(_YambsDictCodec, _BasicDictCodec):
     """The top-level configuration object for the package."""
 
     data: Dict[str, Any]
+    board_data: List[Board]
 
     def init(self, data: _JsonObject) -> None:
         """Initialize this instance."""
 
         self.data = data
         self.root = Path()
+        self._init_boards()
+
+        self.src_root = self.directory("src_root")
+        self.build_root = self.directory("build_root")
+
+    def _init_boards(self) -> None:
+        """Initialize board data."""
+
+        self.board_data = [
+            Board.from_dict(x, self.data["architectures"], self.data["chips"])
+            for x in self.data["boards"]
+        ]
 
     def directory(self, name: str, mkdir: bool = True) -> Path:
         """Get a configurable directory."""
 
         name_root = Path(str(self.data[name]))
         if not name_root.is_absolute():
             name_root = self.root.joinpath(name_root)
@@ -41,18 +54,16 @@
             name_root.mkdir(parents=True, exist_ok=True)
 
         return name_root
 
     def boards(self) -> Iterator[Tuple[Board, Dict[str, Any]]]:
         """Iterate over boards."""
 
-        for board in self.data["boards"]:
-            yield Board.from_dict(
-                board, self.data["architectures"], self.data["chips"]
-            ), board
+        for inst, board in zip(self.board_data, self.data["boards"]):
+            yield inst, board
 
 
 DEFAULT_CONFIG = f"{PKG_NAME}.yaml"
 
 
 def load(path: Pathlike = DEFAULT_CONFIG) -> Config:
     """Load a configuration."""
```

### Comparing `yambs-1.4.1/yambs/config/board.py` & `yambs-1.4.2/yambs/config/board.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     """A class representing a board's attributes."""
 
     name: str
     chip: Chip
     extra_cflags: List[str]
     targets: List[str]
     extra_dirs: List[str]
+    apps: Dict[str, Path]
 
     @property
     def build(self) -> Path:
         """Get a buld directory based on this board."""
         chip = self.chip
         return Path(
             chip.architecture.toolchain, chip.architecture.name, chip.cpu
@@ -75,8 +76,9 @@
 
         return Board(
             data["name"],
             Chip.from_dict(chip, chips[chip], architectures),
             data["extra_cflags"],
             data["targets"],
             data["extra_dirs"],
+            {},
         )
```

### Comparing `yambs-1.4.1/yambs/data/includes/chips.yaml` & `yambs-1.4.2/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/data/includes/infineon.yaml` & `yambs-1.4.2/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/data/includes/microchip.yaml` & `yambs-1.4.2/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/data/schemas/Chip.yaml` & `yambs-1.4.2/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/data/schemas/Config.yaml` & `yambs-1.4.2/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/data/templates/rules.ninja.j2` & `yambs-1.4.2/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/data/uf2families.json` & `yambs-1.4.2/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/entry.py` & `yambs-1.4.2/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/generate/architectures.py` & `yambs-1.4.2/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/generate/boards.py` & `yambs-1.4.2/yambs/generate/boards.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,24 +124,22 @@
     return all_srcs, app_srcs
 
 
 def generate(
     jinja: Environment,
     ninja_root: Path,
     config: Config,
-) -> Dict[str, Any]:
+) -> None:
     """Generate board-related ninja files."""
 
-    board_apps: Dict[str, Any] = {}
-
     # Render the board manifest and rules file.
     for template in ["all.ninja", "rules.ninja"]:
         render_template(jinja, ninja_root, template, config.data)
 
-    src_root = rel(config.directory("src_root"))
+    src_root = rel(config.src_root)
 
     # Keep track of all overall sources, so that no duplicate rules are
     # generated.
     global_sources: Set[Path] = set()
 
     for board, raw_data in config.boards():
         board_root = ninja_root.joinpath("boards", board.name)
@@ -159,20 +157,15 @@
         LOG.info(
             "(%s) Found %d sources and %d applications.",
             board.name,
             len(all_srcs),
             len(app_srcs),
         )
 
-        # Keep track of each board's applications.
-        board_apps[board.name] = list(str(x) for x in app_srcs)
-
         # Write the application manifest.
         with board_root.joinpath("apps.ninja").open("w") as path_fd:
             for app_src in app_srcs:
-                write_link_line(path_fd, app_src, all_srcs, src_root)
+                write_link_line(path_fd, app_src, all_srcs, src_root, board)
 
             # Write the phony target.
             path_fd.write("# A target to build all applications." + linesep)
             write_phony(path_fd, app_srcs, src_root, board.name)
-
-    return board_apps
```

### Comparing `yambs-1.4.1/yambs/generate/chips.py` & `yambs-1.4.2/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/generate/common.py` & `yambs-1.4.2/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/generate/ninja.py` & `yambs-1.4.2/yambs/generate/ninja.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,47 +45,55 @@
 
 def write_continuation(stream: TextIO, offset: str) -> None:
     """Write a line continuation."""
     stream.write(" $" + linesep + offset)
 
 
 def write_link_line(
-    stream: TextIO, source: Path, all_srcs: Set[Path], base: Path
+    stream: TextIO, source: Path, all_srcs: Set[Path], base: Path, board: Board
 ) -> None:
     """
     Write a ninja configuration line for an application requiring linking.
     """
 
     source = source.relative_to(base)
 
-    elf = f"$build_dir/{source.with_suffix('.elf')}"
+    by_suffix = {
+        x: source.with_suffix(f".{x}")
+        for x in ["o", "elf", "bin", "hex", "dump", "uf2"]
+    }
+
+    elf = f"$build_dir/{by_suffix['elf']}"
     line = f"build {elf}: link "
     offset = " " * len(line)
-    stream.write(line + f"$build_dir/{source.with_suffix('.o')}")
+    stream.write(line + f"$build_dir/{by_suffix['o']}")
 
     for src in all_srcs:
         write_continuation(stream, offset)
         stream.write(f"$build_dir/{src.relative_to(base).with_suffix('.o')}")
     stream.write(linesep)
 
     # Add lines for creating binaries.
-    bin_path = f"$build_dir/{source.with_suffix('.bin')}"
-    stream.write(f"build {bin_path}: bin {elf}" + linesep)
+    stream.write(f"build $build_dir/{by_suffix['bin']}: bin {elf}" + linesep)
+
+    # Add an objdump target.
+    stream.write(f"build $build_dir/{by_suffix['dump']}: dump {elf}" + linesep)
 
     # Add an hex target.
-    hex_path = f"$build_dir/{source.with_suffix('.hex')}"
+    hex_path = f"$build_dir/{by_suffix['hex']}"
     stream.write(f"build {hex_path}: hex {elf}" + linesep)
 
-    # Add an objdump target.
-    dump_path = f"$build_dir/{source.with_suffix('.dump')}"
-    stream.write(f"build {dump_path}: dump {elf}" + linesep)
-
     # Add a uf2 target.
-    uf2_path = f"$build_dir/{source.with_suffix('.uf2')}"
-    stream.write(f"build {uf2_path}: uf2 {hex_path}" + linesep + linesep)
+    stream.write(f"build $build_dir/{by_suffix['uf2']}: uf2 {hex_path}")
+
+    stream.write(linesep + linesep)
+
+    # Add this application to the board's data structure.
+    out = by_suffix["elf"].with_suffix("")
+    board.apps[str(out)] = board.build.joinpath(out)
 
 
 def write_phony(
     stream: TextIO, app_srcs: Set[Path], base: Path, board: str
 ) -> None:
     """Write the phony target."""
```

### Comparing `yambs-1.4.1/yambs/generate/toolchains.py` & `yambs-1.4.2/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/schemas.py` & `yambs-1.4.2/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs/uf2/__init__.py` & `yambs-1.4.2/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.4.1/yambs.egg-info/PKG-INFO` & `yambs-1.4.2/yambs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.4.1
+Version: 1.4.2
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
-    hash=2e388f2b5ac420fb7c63d634fad57093
+    hash=d66d7ab188c69e98ef4cfbd904223a7d
     =====================================
 -->
 
-# yambs ([1.4.1](https://pypi.org/project/yambs/))
+# yambs ([1.4.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.4.1/yambs.egg-info/SOURCES.txt` & `yambs-1.4.2/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

