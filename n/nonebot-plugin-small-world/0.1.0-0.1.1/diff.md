# Comparing `tmp/nonebot_plugin_small_world-0.1.0.tar.gz` & `tmp/nonebot_plugin_small_world-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_small_world-0.1.0.tar", last modified: Mon May 22 16:44:07 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "nonebot_plugin_small_world-0.1.1.tar", last modified: Mon May 22 17:08:23 2023, max compression
```

## Comparing `nonebot_plugin_small_world-0.1.0.tar` & `nonebot_plugin_small_world-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:40:24.000000 nonebot_plugin_small_world-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-22 16:40:47.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world/
-drwxrwxrwx   0        0        0        0 2023-05-22 16:40:50.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world/data/
--rwxrwxrwx   0        0        0 12001099 2023-05-19 09:40:33.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world/data/cards.json
--rwxrwxrwx   0        0        0     1146 2023-05-21 17:26:53.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world/name2id.py
--rwxrwxrwx   0        0        0     8872 2023-05-20 17:35:46.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:40:24.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world.egg-info/
--rwxrwxrwx   0        0        0        1 2023-05-22 16:31:27.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world.egg-info/dependency_links.txt
--rwxrwxrwx   0        0        0       73 2023-05-22 16:31:27.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world.egg-info/PKG-INFO
--rwxrwxrwx   0        0        0       32 2023-05-22 16:31:27.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world.egg-info/requires.txt
--rwxrwxrwx   0        0        0      340 2023-05-22 16:31:27.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world.egg-info/SOURCES.txt
--rwxrwxrwx   0        0        0       27 2023-05-22 16:31:27.000000 nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world.egg-info/top_level.txt
--rwxrwxrwx   0        0        0       73 2023-05-22 16:31:27.000000 nonebot_plugin_small_world-0.1.0/PKG-INFO
--rwxrwxrwx   0        0        0      133 2023-05-21 09:51:47.000000 nonebot_plugin_small_world-0.1.0/pyproject.toml
--rwxrwxrwx   0        0        0       42 2023-05-22 16:31:27.000000 nonebot_plugin_small_world-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 17:08:23.751208 nonebot_plugin_small_world-0.1.1/
+-rw-rw-rw-   0        0        0       56 2023-05-22 17:02:19.000000 nonebot_plugin_small_world-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0       73 2023-05-22 17:08:23.749210 nonebot_plugin_small_world-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 17:08:23.714956 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world/
+-rw-rw-rw-   0        0        0     8872 2023-05-20 17:35:46.000000 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:08:23.730199 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world/data/
+-rw-rw-rw-   0        0        0 12001099 2023-05-19 09:40:33.000000 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world/data/cards.json
+-rw-rw-rw-   0        0        0     1146 2023-05-21 17:26:53.000000 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world/name2id.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:08:23.728191 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world.egg-info/
+-rw-rw-rw-   0        0        0       73 2023-05-22 17:08:23.000000 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-22 17:08:23.000000 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 17:08:23.000000 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-22 17:08:23.000000 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-22 17:08:23.000000 nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      133 2023-05-22 17:07:37.000000 nonebot_plugin_small_world-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 17:08:23.751208 nonebot_plugin_small_world-0.1.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world/data/cards.json` & `nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world/data/cards.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world/name2id.py` & `nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world/name2id.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_small_world-0.1.0/nonebot_plugin_small_world/__init__.py` & `nonebot_plugin_small_world-0.1.1/nonebot_plugin_small_world/__init__.py`

 * *Files identical despite different names*

