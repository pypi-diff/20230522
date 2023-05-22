# Comparing `tmp/enkanetwork.py-1.4.2.tar.gz` & `tmp/enkanetwork.py-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkanetwork.py-1.4.2.tar", last modified: Wed Mar 22 11:31:32 2023, max compression
+gzip compressed data, was "enkanetwork.py-1.4.4.tar", last modified: Mon May 22 15:17:51 2023, max compression
```

## Comparing `enkanetwork.py-1.4.2.tar` & `enkanetwork.py-1.4.4.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-03-22 11:31:32.214790 enkanetwork.py-1.4.2/
--rw-r--r--   0 m307       (501) staff       (20)     1045 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/LICENSE
--rw-r--r--   0 m307       (501) staff       (20)       36 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/MANIFEST.in
--rw-r--r--   0 m307       (501) staff       (20)    19271 2023-03-22 11:31:32.214312 enkanetwork.py-1.4.2/PKG-INFO
--rw-r--r--   0 m307       (501) staff       (20)    18717 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/README.md
-drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-03-22 11:31:32.174681 enkanetwork.py-1.4.2/enkanetwork/
--rw-r--r--   0 m307       (501) staff       (20)     1415 2023-03-22 11:31:07.000000 enkanetwork.py-1.4.2/enkanetwork/__init__.py
-drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-03-22 11:31:32.164672 enkanetwork.py-1.4.2/enkanetwork/assets/
-drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-03-22 11:31:32.183142 enkanetwork.py-1.4.2/enkanetwork/assets/data/
--rw-r--r--   0 m307       (501) staff       (20)    52146 2023-03-20 09:05:20.000000 enkanetwork.py-1.4.2/enkanetwork/assets/data/artifact_props.json
--rw-r--r--   0 m307       (501) staff       (20)    35758 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/data/characters.json
--rw-r--r--   0 m307       (501) staff       (20)    40251 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/data/constellations.json
--rw-r--r--   0 m307       (501) staff       (20)     2188 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/data/costumes.json
--rw-r--r--   0 m307       (501) staff       (20)    42594 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/data/namecards.json
--rw-r--r--   0 m307       (501) staff       (20)    67438 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/data/skills.json
-drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-03-22 11:31:32.200127 enkanetwork.py-1.4.2/enkanetwork/assets/langs/
--rw-r--r--   0 m307       (501) staff       (20)    27473 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/langs/artifact_sets.json
--rw-r--r--   0 m307       (501) staff       (20)  2344125 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/langs/artifacts.json
--rw-r--r--   0 m307       (501) staff       (20)    27496 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/langs/characters.json
--rw-r--r--   0 m307       (501) staff       (20)   248584 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/langs/constellations.json
--rw-r--r--   0 m307       (501) staff       (20)    28787 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/langs/fight_props.json
--rw-r--r--   0 m307       (501) staff       (20)    96697 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/langs/namecards.json
--rw-r--r--   0 m307       (501) staff       (20)   253964 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/langs/skills.json
--rw-r--r--   0 m307       (501) staff       (20)    98669 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/assets/langs/weapons.json
--rw-r--r--   0 m307       (501) staff       (20)     7582 2023-03-20 09:32:59.000000 enkanetwork.py-1.4.2/enkanetwork/assets.py
--rw-r--r--   0 m307       (501) staff       (20)      645 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/cache.py
--rw-r--r--   0 m307       (501) staff       (20)    12742 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/client.py
--rw-r--r--   0 m307       (501) staff       (20)      798 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/config.py
--rw-r--r--   0 m307       (501) staff       (20)     1059 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/enum.py
--rw-r--r--   0 m307       (501) staff       (20)     1501 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/exception.py
--rw-r--r--   0 m307       (501) staff       (20)     7157 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/http.py
-drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-03-22 11:31:32.212211 enkanetwork.py-1.4.2/enkanetwork/model/
--rw-r--r--   0 m307       (501) staff       (20)      137 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/model/__init__.py
--rw-r--r--   0 m307       (501) staff       (20)     4173 2023-03-20 09:29:19.000000 enkanetwork.py-1.4.2/enkanetwork/model/assets.py
--rw-r--r--   0 m307       (501) staff       (20)     1935 2023-03-20 09:50:59.000000 enkanetwork.py-1.4.2/enkanetwork/model/base.py
--rw-r--r--   0 m307       (501) staff       (20)     1147 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/model/build.py
--rw-r--r--   0 m307       (501) staff       (20)     5133 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/model/character.py
--rw-r--r--   0 m307       (501) staff       (20)     5610 2023-03-20 09:51:59.000000 enkanetwork.py-1.4.2/enkanetwork/model/equipments.py
--rw-r--r--   0 m307       (501) staff       (20)      307 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/model/hoyos.py
--rw-r--r--   0 m307       (501) staff       (20)     3751 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/model/players.py
--rw-r--r--   0 m307       (501) staff       (20)      346 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/model/profile.py
--rw-r--r--   0 m307       (501) staff       (20)     7763 2023-03-20 08:38:11.000000 enkanetwork.py-1.4.2/enkanetwork/model/stats.py
--rw-r--r--   0 m307       (501) staff       (20)      293 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/model/utils.py
--rw-r--r--   0 m307       (501) staff       (20)     1313 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/tools.py
-drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-03-22 11:31:32.213555 enkanetwork.py-1.4.2/enkanetwork/types/
--rw-r--r--   0 m307       (501) staff       (20)      153 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/types/__init__.py
--rw-r--r--   0 m307       (501) staff       (20)     1157 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/types/enkanetwork.py
--rw-r--r--   0 m307       (501) staff       (20)     3012 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/enkanetwork/utils.py
-drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-03-22 11:31:32.179180 enkanetwork.py-1.4.2/enkanetwork.py.egg-info/
--rw-r--r--   0 m307       (501) staff       (20)    19271 2023-03-22 11:31:32.000000 enkanetwork.py-1.4.2/enkanetwork.py.egg-info/PKG-INFO
--rw-r--r--   0 m307       (501) staff       (20)     1389 2023-03-22 11:31:32.000000 enkanetwork.py-1.4.2/enkanetwork.py.egg-info/SOURCES.txt
--rw-r--r--   0 m307       (501) staff       (20)        1 2023-03-22 11:31:32.000000 enkanetwork.py-1.4.2/enkanetwork.py.egg-info/dependency_links.txt
--rw-r--r--   0 m307       (501) staff       (20)       28 2023-03-22 11:31:32.000000 enkanetwork.py-1.4.2/enkanetwork.py.egg-info/requires.txt
--rw-r--r--   0 m307       (501) staff       (20)       12 2023-03-22 11:31:32.000000 enkanetwork.py-1.4.2/enkanetwork.py.egg-info/top_level.txt
--rw-r--r--   0 m307       (501) staff       (20)       38 2023-03-22 11:31:32.214914 enkanetwork.py-1.4.2/setup.cfg
--rw-r--r--   0 m307       (501) staff       (20)     1032 2023-03-20 07:45:12.000000 enkanetwork.py-1.4.2/setup.py
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.987055 enkanetwork.py-1.4.4/
+-rw-r--r--   0 m307       (501) staff       (20)     1045 2022-12-01 04:18:44.000000 enkanetwork.py-1.4.4/LICENSE
+-rw-r--r--   0 m307       (501) staff       (20)       36 2022-12-01 04:18:44.000000 enkanetwork.py-1.4.4/MANIFEST.in
+-rw-r--r--   0 m307       (501) staff       (20)    19241 2023-05-22 15:17:51.986758 enkanetwork.py-1.4.4/PKG-INFO
+-rw-r--r--   0 m307       (501) staff       (20)    18724 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/README.md
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.961665 enkanetwork.py-1.4.4/enkanetwork/
+-rw-r--r--   0 m307       (501) staff       (20)     1415 2023-05-22 15:14:47.000000 enkanetwork.py-1.4.4/enkanetwork/__init__.py
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.957087 enkanetwork.py-1.4.4/enkanetwork/assets/
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.965583 enkanetwork.py-1.4.4/enkanetwork/assets/data/
+-rw-r--r--   0 m307       (501) staff       (20)    52146 2023-05-22 14:57:24.000000 enkanetwork.py-1.4.4/enkanetwork/assets/data/artifact_props.json
+-rw-r--r--   0 m307       (501) staff       (20)    36667 2023-05-22 14:57:24.000000 enkanetwork.py-1.4.4/enkanetwork/assets/data/characters.json
+-rw-r--r--   0 m307       (501) staff       (20)    42032 2023-05-22 14:57:24.000000 enkanetwork.py-1.4.4/enkanetwork/assets/data/constellations.json
+-rw-r--r--   0 m307       (501) staff       (20)     2188 2023-05-22 14:57:24.000000 enkanetwork.py-1.4.4/enkanetwork/assets/data/costumes.json
+-rw-r--r--   0 m307       (501) staff       (20)    45149 2023-05-22 14:57:24.000000 enkanetwork.py-1.4.4/enkanetwork/assets/data/namecards.json
+-rw-r--r--   0 m307       (501) staff       (20)    69333 2023-05-22 14:57:24.000000 enkanetwork.py-1.4.4/enkanetwork/assets/data/skills.json
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.979257 enkanetwork.py-1.4.4/enkanetwork/assets/langs/
+-rw-r--r--   0 m307       (501) staff       (20)    28607 2023-05-22 14:57:49.000000 enkanetwork.py-1.4.4/enkanetwork/assets/langs/artifact_sets.json
+-rw-r--r--   0 m307       (501) staff       (20)  2383280 2023-05-22 14:57:49.000000 enkanetwork.py-1.4.4/enkanetwork/assets/langs/artifacts.json
+-rw-r--r--   0 m307       (501) staff       (20)    28278 2023-05-22 14:57:49.000000 enkanetwork.py-1.4.4/enkanetwork/assets/langs/characters.json
+-rw-r--r--   0 m307       (501) staff       (20)   259644 2023-05-22 14:57:49.000000 enkanetwork.py-1.4.4/enkanetwork/assets/langs/constellations.json
+-rw-r--r--   0 m307       (501) staff       (20)    29675 2023-05-22 14:57:49.000000 enkanetwork.py-1.4.4/enkanetwork/assets/langs/fight_props.json
+-rw-r--r--   0 m307       (501) staff       (20)   102542 2023-05-22 14:57:49.000000 enkanetwork.py-1.4.4/enkanetwork/assets/langs/namecards.json
+-rw-r--r--   0 m307       (501) staff       (20)   261913 2023-05-22 14:57:49.000000 enkanetwork.py-1.4.4/enkanetwork/assets/langs/skills.json
+-rw-r--r--   0 m307       (501) staff       (20)    99218 2023-05-22 14:57:49.000000 enkanetwork.py-1.4.4/enkanetwork/assets/langs/weapons.json
+-rw-r--r--   0 m307       (501) staff       (20)     7582 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/assets.py
+-rw-r--r--   0 m307       (501) staff       (20)      645 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/cache.py
+-rw-r--r--   0 m307       (501) staff       (20)    12742 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/client.py
+-rw-r--r--   0 m307       (501) staff       (20)      798 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/config.py
+-rw-r--r--   0 m307       (501) staff       (20)     1059 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/enum.py
+-rw-r--r--   0 m307       (501) staff       (20)     1501 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/exception.py
+-rw-r--r--   0 m307       (501) staff       (20)     7157 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/http.py
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.985383 enkanetwork.py-1.4.4/enkanetwork/model/
+-rw-r--r--   0 m307       (501) staff       (20)      137 2022-12-01 04:18:44.000000 enkanetwork.py-1.4.4/enkanetwork/model/__init__.py
+-rw-r--r--   0 m307       (501) staff       (20)     4173 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/model/assets.py
+-rw-r--r--   0 m307       (501) staff       (20)     1935 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/model/base.py
+-rw-r--r--   0 m307       (501) staff       (20)     1147 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/model/build.py
+-rw-r--r--   0 m307       (501) staff       (20)     5133 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/model/character.py
+-rw-r--r--   0 m307       (501) staff       (20)     5610 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/model/equipments.py
+-rw-r--r--   0 m307       (501) staff       (20)      307 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/model/hoyos.py
+-rw-r--r--   0 m307       (501) staff       (20)     3751 2022-12-09 06:01:27.000000 enkanetwork.py-1.4.4/enkanetwork/model/players.py
+-rw-r--r--   0 m307       (501) staff       (20)      346 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/model/profile.py
+-rw-r--r--   0 m307       (501) staff       (20)     7763 2022-12-01 04:18:44.000000 enkanetwork.py-1.4.4/enkanetwork/model/stats.py
+-rw-r--r--   0 m307       (501) staff       (20)      293 2022-12-01 04:18:44.000000 enkanetwork.py-1.4.4/enkanetwork/model/utils.py
+-rw-r--r--   0 m307       (501) staff       (20)     1313 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/tools.py
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.986012 enkanetwork.py-1.4.4/enkanetwork/types/
+-rw-r--r--   0 m307       (501) staff       (20)      153 2022-12-01 04:18:44.000000 enkanetwork.py-1.4.4/enkanetwork/types/__init__.py
+-rw-r--r--   0 m307       (501) staff       (20)     1157 2022-12-01 04:18:44.000000 enkanetwork.py-1.4.4/enkanetwork/types/enkanetwork.py
+-rw-r--r--   0 m307       (501) staff       (20)     3012 2023-05-22 14:56:01.000000 enkanetwork.py-1.4.4/enkanetwork/utils.py
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.962893 enkanetwork.py-1.4.4/enkanetwork.py.egg-info/
+-rw-r--r--   0 m307       (501) staff       (20)    19241 2023-05-22 15:17:51.000000 enkanetwork.py-1.4.4/enkanetwork.py.egg-info/PKG-INFO
+-rw-r--r--   0 m307       (501) staff       (20)     1407 2023-05-22 15:17:51.000000 enkanetwork.py-1.4.4/enkanetwork.py.egg-info/SOURCES.txt
+-rw-r--r--   0 m307       (501) staff       (20)        1 2023-05-22 15:17:51.000000 enkanetwork.py-1.4.4/enkanetwork.py.egg-info/dependency_links.txt
+-rw-r--r--   0 m307       (501) staff       (20)       28 2023-05-22 15:17:51.000000 enkanetwork.py-1.4.4/enkanetwork.py.egg-info/requires.txt
+-rw-r--r--   0 m307       (501) staff       (20)       12 2023-05-22 15:17:51.000000 enkanetwork.py-1.4.4/enkanetwork.py.egg-info/top_level.txt
+-rw-r--r--   0 m307       (501) staff       (20)       38 2023-05-22 15:17:51.987122 enkanetwork.py-1.4.4/setup.cfg
+-rw-r--r--   0 m307       (501) staff       (20)     1032 2022-12-20 10:49:22.000000 enkanetwork.py-1.4.4/setup.py
+drwxr-xr-x   0 m307       (501) staff       (20)        0 2023-05-22 15:17:51.986237 enkanetwork.py-1.4.4/test/
+-rw-r--r--   0 m307       (501) staff       (20)      556 2023-02-16 15:49:48.000000 enkanetwork.py-1.4.4/test/test.test.py
```

### Comparing `enkanetwork.py-1.4.2/LICENSE` & `enkanetwork.py-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/PKG-INFO` & `enkanetwork.py-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: enkanetwork.py
-Version: 1.4.2
+Version: 1.4.4
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/mrwan200/EnkaNetwork.py
 Author: M-307
 Author-email: me@m307.dev
-License: UNKNOWN
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -73,15 +71,15 @@
 
 async def main():
     async with client:
         data = await client.fetch_user(843715177)
         print("=== Player Info ===")
         print(f"Nickname: {data.player.nickname}")
         print(f"Level: {data.player.level}")
-        print(f"Icon: {data.player.icon.url}")
+        print(f"Icon: {data.player.avatar.icon.url}")
         print(f"Signature: {data.player.signature}")
         print(f"Achievement: {data.player.achievement}")
         print(f"Abyss floor: {data.player.abyss_floor} - {data.player.abyss_room}")
         print(f"Cache timeout: {data.ttl}")
 
 asyncio.run(main())
 ```
@@ -435,9 +433,7 @@
 # LICENSE
 
 [MIT License](./LICENSE)
 
 ![Keqing](https://c.tenor.com/MnkpnVCLcb0AAAAC/keqing-dance.gif)
 
 [Picture by KKOMDASTRO](https://twitter.com/KKOMDASTRO)
-
-
```

### Comparing `enkanetwork.py-1.4.2/README.md` & `enkanetwork.py-1.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 async def main():
     async with client:
         data = await client.fetch_user(843715177)
         print("=== Player Info ===")
         print(f"Nickname: {data.player.nickname}")
         print(f"Level: {data.player.level}")
-        print(f"Icon: {data.player.icon.url}")
+        print(f"Icon: {data.player.avatar.icon.url}")
         print(f"Signature: {data.player.signature}")
         print(f"Achievement: {data.player.achievement}")
         print(f"Abyss floor: {data.player.abyss_floor} - {data.player.abyss_room}")
         print(f"Cache timeout: {data.ttl}")
 
 asyncio.run(main())
 ```
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/__init__.py` & `enkanetwork.py-1.4.4/enkanetwork/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE."""
 
 __title__ = 'enkanetwork.py'
 __author__ = 'M-307'
-__version__ = '1.4.2'
+__version__ = '1.4.4'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022-present M-307'
 
 
 from .client import *
 from .exception import *
 from .model import *
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/data/artifact_props.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/data/artifact_props.json`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/data/characters.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/data/characters.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'10000081'": "OrderedDict([('nameTextMapHash', 466355514), ('iconName', 'UI_AvatarIcon_Kaveh'), "*

 * *               "('sideIconName', 'UI_AvatarIcon_Side_Kaveh'), ('qualityType', 'QUALITY_PURPLE'), "*

 * *               "('costElemType', 'Grass'), ('skills', [10811, 10812, 10815]), ('talents', [811, "*

 * *               '812, 813, 814, 815, 816])])',*

 * * "'10000082'": "OrderedDict([('nameTextMapHash', 2984815066), ('iconName', "*

 * *               "'UI_AvatarIcon_Baizhuer'), ('sideIconName', 'UI_AvatarIcon_Side_Baizhuer'),  […]*

```diff
@@ -1540,9 +1540,49 @@
             801,
             802,
             803,
             804,
             805,
             806
         ]
+    },
+    "10000081": {
+        "costElemType": "Grass",
+        "iconName": "UI_AvatarIcon_Kaveh",
+        "nameTextMapHash": 466355514,
+        "qualityType": "QUALITY_PURPLE",
+        "sideIconName": "UI_AvatarIcon_Side_Kaveh",
+        "skills": [
+            10811,
+            10812,
+            10815
+        ],
+        "talents": [
+            811,
+            812,
+            813,
+            814,
+            815,
+            816
+        ]
+    },
+    "10000082": {
+        "costElemType": "Grass",
+        "iconName": "UI_AvatarIcon_Baizhuer",
+        "nameTextMapHash": 2984815066,
+        "qualityType": "QUALITY_ORANGE",
+        "sideIconName": "UI_AvatarIcon_Side_Baizhuer",
+        "skills": [
+            10821,
+            10822,
+            10825
+        ],
+        "talents": [
+            821,
+            822,
+            823,
+            824,
+            825,
+            826
+        ]
     }
 }
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/data/constellations.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/data/constellations.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9577464788732394%*

 * *Differences: {"'611'": "OrderedDict([('nameTextMapHash', 3502158873), ('icon', 'UI_Talent_S_Momoka_01')])",*

 * * "'612'": "OrderedDict([('nameTextMapHash', 3954516065), ('icon', 'UI_Talent_S_Momoka_02')])",*

 * * "'613'": "OrderedDict([('nameTextMapHash', 3397892401), ('icon', 'UI_Talent_U_Momoka_01')])",*

 * * "'614'": "OrderedDict([('nameTextMapHash', 3551684865), ('icon', 'UI_Talent_S_Momoka_04')])",*

 * * "'615'": "OrderedDict([('nameTextMapHash', 34942769), ('icon', 'UI_Talent_U_Momoka_02')])",*

 * * "'616'": "OrderedDict([('nameTextMapHa […]*

```diff
@@ -1123,14 +1123,38 @@
         "icon": "UI_Talent_U_Yelan_02",
         "nameTextMapHash": 2362082321
     },
     "606": {
         "icon": "UI_Talent_S_Yelan_04",
         "nameTextMapHash": 1272265729
     },
+    "611": {
+        "icon": "UI_Talent_S_Momoka_01",
+        "nameTextMapHash": 3502158873
+    },
+    "612": {
+        "icon": "UI_Talent_S_Momoka_02",
+        "nameTextMapHash": 3954516065
+    },
+    "613": {
+        "icon": "UI_Talent_U_Momoka_01",
+        "nameTextMapHash": 3397892401
+    },
+    "614": {
+        "icon": "UI_Talent_S_Momoka_04",
+        "nameTextMapHash": 3551684865
+    },
+    "615": {
+        "icon": "UI_Talent_U_Momoka_02",
+        "nameTextMapHash": 34942769
+    },
+    "616": {
+        "icon": "UI_Talent_S_Momoka_03",
+        "nameTextMapHash": 2439940993
+    },
     "621": {
         "icon": "UI_Talent_S_Aloy_Lock",
         "nameTextMapHash": 1426348289
     },
     "622": {
         "icon": "UI_Talent_S_Aloy_Lock",
         "nameTextMapHash": 3468411401
@@ -1603,14 +1627,62 @@
         "icon": "UI_Talent_U_Mika_02",
         "nameTextMapHash": 101621505
     },
     "806": {
         "icon": "UI_Talent_S_Mika_04",
         "nameTextMapHash": 1784924817
     },
+    "811": {
+        "icon": "UI_Talent_S_Kaveh_01",
+        "nameTextMapHash": 3110332641
+    },
+    "812": {
+        "icon": "UI_Talent_S_Kaveh_02",
+        "nameTextMapHash": 20172977
+    },
+    "813": {
+        "icon": "UI_Talent_U_Kaveh_02",
+        "nameTextMapHash": 2730015409
+    },
+    "814": {
+        "icon": "UI_Talent_S_Kaveh_03",
+        "nameTextMapHash": 2860814489
+    },
+    "815": {
+        "icon": "UI_Talent_U_Kaveh_01",
+        "nameTextMapHash": 1755584449
+    },
+    "816": {
+        "icon": "UI_Talent_S_Kaveh_04",
+        "nameTextMapHash": 2892000521
+    },
+    "821": {
+        "icon": "UI_Talent_S_Baizhuer_01",
+        "nameTextMapHash": 858748369
+    },
+    "822": {
+        "icon": "UI_Talent_S_Baizhuer_02",
+        "nameTextMapHash": 1849398401
+    },
+    "823": {
+        "icon": "UI_Talent_U_Baizhuer_01",
+        "nameTextMapHash": 2410139081
+    },
+    "824": {
+        "icon": "UI_Talent_S_Baizhuer_03",
+        "nameTextMapHash": 4262913073
+    },
+    "825": {
+        "icon": "UI_Talent_U_Baizhuer_02",
+        "nameTextMapHash": 63855777
+    },
+    "826": {
+        "icon": "UI_Talent_S_Baizhuer_04",
+        "nameTextMapHash": 1293460177
+    },
     "91": {
         "icon": "UI_Talent_S_PlayerRock_01",
         "nameTextMapHash": 3120087313
     },
     "92": {
         "icon": "UI_Talent_S_PlayerRock_02",
         "nameTextMapHash": 1377520009
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/data/costumes.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/data/costumes.json`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/data/namecards.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/data/namecards.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9433962264150944%*

 * *Differences: {"'210155'": "OrderedDict([('nameTextMapHash', 2816803308), ('icon', 'UI_NameCardIcon_Baizhuer'), "*

 * *             "('picPath', ['UI_NameCardPic_Baizhuer_Alpha', 'UI_NameCardPic_Baizhuer_P']), "*

 * *             "('rankLevel', 4), ('materialType', 'MATERIAL_NAMECARD')])",*

 * * "'210156'": "OrderedDict([('nameTextMapHash', 2684456012), ('icon', 'UI_NameCardIcon_Kaveh'), "*

 * *             "('picPath', ['UI_NameCardPic_Kaveh_Alpha', 'UI_NameCardPic_Kaveh_P']), ('rankLevel', "*

 * *             "4), ('materialType', 'MATERIAL_NA […]*

```diff
@@ -1494,9 +1494,99 @@
         "materialType": "MATERIAL_NAMECARD",
         "nameTextMapHash": 893197700,
         "picPath": [
             "UI_NameCardPic_Bp22_P_Alpha",
             "UI_NameCardPic_Bp22_P"
         ],
         "rankLevel": 4
+    },
+    "210155": {
+        "icon": "UI_NameCardIcon_Baizhuer",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 2816803308,
+        "picPath": [
+            "UI_NameCardPic_Baizhuer_Alpha",
+            "UI_NameCardPic_Baizhuer_P"
+        ],
+        "rankLevel": 4
+    },
+    "210156": {
+        "icon": "UI_NameCardIcon_Kaveh",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 2684456012,
+        "picPath": [
+            "UI_NameCardPic_Kaveh_Alpha",
+            "UI_NameCardPic_Kaveh_P"
+        ],
+        "rankLevel": 4
+    },
+    "210157": {
+        "icon": "UI_NameCardIcon_Xm4",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 370573972,
+        "picPath": [
+            "UI_NameCardPic_Xm4_Alpha",
+            "UI_NameCardPic_Xm4_P"
+        ],
+        "rankLevel": 4
+    },
+    "210158": {
+        "icon": "UI_NameCardIcon_Tzz7",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 110943356,
+        "picPath": [
+            "UI_NameCardPic_Tzz7_Alpha",
+            "UI_NameCardPic_Tzz7_P"
+        ],
+        "rankLevel": 4
+    },
+    "210159": {
+        "icon": "UI_NameCardIcon_Vasara",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 1790614036,
+        "picPath": [
+            "UI_NameCardPic_Vasara_Alpha",
+            "UI_NameCardPic_Vasara_P"
+        ],
+        "rankLevel": 4
+    },
+    "210160": {
+        "icon": "UI_NameCardIcon_OfferingPari",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 3159539884,
+        "picPath": [
+            "UI_NameCardPic_OfferingPari_Alpha",
+            "UI_NameCardPic_OfferingPari_P"
+        ],
+        "rankLevel": 4
+    },
+    "210161": {
+        "icon": "UI_NameCardIcon_Bp23",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 641457676,
+        "picPath": [
+            "UI_NameCardPic_Bp23_Alpha",
+            "UI_NameCardPic_Bp23_P"
+        ],
+        "rankLevel": 4
+    },
+    "210162": {
+        "icon": "UI_NameCardIcon_Kirara",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 2371279924,
+        "picPath": [
+            "UI_NameCardPic_Kirara_Alpha",
+            "UI_NameCardPic_Kirara_P"
+        ],
+        "rankLevel": 4
+    },
+    "210163": {
+        "icon": "UI_NameCardIcon_Bp24",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 252168660,
+        "picPath": [
+            "UI_NameCardPic_Bp24_Alpha",
+            "UI_NameCardPic_Bp24_P"
+        ],
+        "rankLevel": 4
     }
 }
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/data/skills.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/data/skills.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9652509652509652%*

 * *Differences: {"'10611'": "OrderedDict([('nameTextMapHash', 2089915453), ('skillIcon', 'Skill_A_01'), "*

 * *            "('proudSkillGroupId', 6131)])",*

 * * "'10612'": "OrderedDict([('nameTextMapHash', 3512914781), ('skillIcon', 'Skill_S_Momoka_01'), "*

 * *            "('proudSkillGroupId', 6132)])",*

 * * "'10613'": "OrderedDict([('nameTextMapHash', 451737061), ('skillIcon', 'Skill_S_Momoka_02'), "*

 * *            "('proudSkillGroupId', '')])",*

 * * "'10615'": "OrderedDict([('nameTextMapHash', 2543392221), ('skillIcon', 'Skill_E_Momoka_01'), " […]*

```diff
@@ -155,19 +155,14 @@
         "skillIcon": "Skill_A_01"
     },
     "100541": {
         "nameTextMapHash": 3198281757,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_01"
     },
-    "100542": {
-        "nameTextMapHash": 3565118517,
-        "proudSkillGroupId": "",
-        "skillIcon": "Skill_A_01"
-    },
     "100543": {
         "nameTextMapHash": 3283214237,
         "proudSkillGroupId": 730,
         "skillIcon": "Skill_A_01"
     },
     "100544": {
         "nameTextMapHash": 895313525,
@@ -200,19 +195,14 @@
         "skillIcon": "Skill_A_01"
     },
     "100551": {
         "nameTextMapHash": 2463434149,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_01"
     },
-    "100552": {
-        "nameTextMapHash": 299520933,
-        "proudSkillGroupId": "",
-        "skillIcon": "Skill_A_01"
-    },
     "100553": {
         "nameTextMapHash": 2182891949,
         "proudSkillGroupId": 731,
         "skillIcon": "Skill_A_01"
     },
     "100554": {
         "nameTextMapHash": 1522492485,
@@ -1260,14 +1250,34 @@
         "skillIcon": "Skill_S_Yelan_02"
     },
     "10610": {
         "nameTextMapHash": 4098371861,
         "proudSkillGroupId": 6039,
         "skillIcon": "Skill_E_Yelan_01"
     },
+    "10611": {
+        "nameTextMapHash": 2089915453,
+        "proudSkillGroupId": 6131,
+        "skillIcon": "Skill_A_01"
+    },
+    "10612": {
+        "nameTextMapHash": 3512914781,
+        "proudSkillGroupId": 6132,
+        "skillIcon": "Skill_S_Momoka_01"
+    },
+    "10613": {
+        "nameTextMapHash": 451737061,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_S_Momoka_02"
+    },
+    "10615": {
+        "nameTextMapHash": 2543392221,
+        "proudSkillGroupId": 6139,
+        "skillIcon": "Skill_E_Momoka_01"
+    },
     "10621": {
         "nameTextMapHash": 2994648485,
         "proudSkillGroupId": 6231,
         "skillIcon": "Skill_A_02"
     },
     "10622": {
         "nameTextMapHash": 1871687965,
@@ -1655,14 +1665,44 @@
         "skillIcon": "Skill_S_Mika_01"
     },
     "10805": {
         "nameTextMapHash": 3170404421,
         "proudSkillGroupId": 8039,
         "skillIcon": "Skill_E_Mika_01"
     },
+    "10811": {
+        "nameTextMapHash": 2101931541,
+        "proudSkillGroupId": 8131,
+        "skillIcon": "Skill_A_04"
+    },
+    "10812": {
+        "nameTextMapHash": 4260508917,
+        "proudSkillGroupId": 8132,
+        "skillIcon": "Skill_S_Kaveh_01"
+    },
+    "10815": {
+        "nameTextMapHash": 1210107733,
+        "proudSkillGroupId": 8139,
+        "skillIcon": "Skill_E_Kaveh_01"
+    },
+    "10821": {
+        "nameTextMapHash": 2662918965,
+        "proudSkillGroupId": 8231,
+        "skillIcon": "Skill_A_Catalyst_MD"
+    },
+    "10822": {
+        "nameTextMapHash": 2409917,
+        "proudSkillGroupId": 8232,
+        "skillIcon": "Skill_S_Baizhuer_01"
+    },
+    "10825": {
+        "nameTextMapHash": 3249611093,
+        "proudSkillGroupId": 8239,
+        "skillIcon": "Skill_E_Baizhuer_01"
+    },
     "11301": {
         "nameTextMapHash": 3802462781,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_02"
     },
     "11302": {
         "nameTextMapHash": 2467360621,
@@ -2005,14 +2045,29 @@
         "skillIcon": "Skill_LanV3_Icon05"
     },
     "20345": {
         "nameTextMapHash": 1316655253,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_PacMan"
     },
+    "20350": {
+        "nameTextMapHash": 3206240077,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_E_Klee_01"
+    },
+    "20351": {
+        "nameTextMapHash": 2174036525,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_E_Klee_01"
+    },
+    "20352": {
+        "nameTextMapHash": 1538181693,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_Fishing_Bait"
+    },
     "20400": {
         "nameTextMapHash": 2657714069,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Seeker_A_01"
     },
     "20401": {
         "nameTextMapHash": 66214933,
@@ -2410,14 +2465,19 @@
         "skillIcon": "Skill_A_Catalyst_MD"
     },
     "5060010": {
         "nameTextMapHash": 289877085,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_02"
     },
+    "5061010": {
+        "nameTextMapHash": 1011789509,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_A_01"
+    },
     "5062010": {
         "nameTextMapHash": 1225242717,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_02"
     },
     "5063010": {
         "nameTextMapHash": 1461236069,
@@ -2504,9 +2564,19 @@
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_04"
     },
     "5080010": {
         "nameTextMapHash": 886703661,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_03"
+    },
+    "5081010": {
+        "nameTextMapHash": 331663653,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_A_04"
+    },
+    "5082010": {
+        "nameTextMapHash": 3734682949,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_A_Catalyst_MD"
     }
 }
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/langs/artifact_sets.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/langs/artifact_sets.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9604575163398693%*

 * *Differences: {"'1925210475'": "OrderedDict([('FR', 'Rêve de la nymphe'), ('JP', '水仙の夢'), ('CHT', '水仙之夢'), "*

 * *                 '(\'ID\', "Nymph\'s Dream"), (\'CHS\', \'水仙之梦\'), (\'VI\', \'Giấc Mộng Thủy '*

 * *                 'Tiên\'), (\'ES\', \'Sueño de la Ninfa\'), (\'TH\', "Nymph\'s Dream"), (\'TR\', '*

 * *                 "'Nergisin Rüyası'), ('KR', '님프의 꿈'), ('DE', 'Traum der Narzisse'), ('RU', 'Сон "*

 * *                 'нимфы\'), (\'IT\', \'Sogno della ninfa\'), (\'EN\', "Nymph\'s Dream"), (\'PT\', '*

 * *                 "'Sonho […]*

```diff
@@ -318,14 +318,31 @@
         "KR": "\ub1cc\uba85\uc744 \ud3c9\uc815\ud55c \uc874\uc790",
         "PT": "Lan\u00e7ador de Trov\u00f5es",
         "RU": "\u0423\u0441\u043c\u0438\u0440\u044f\u044e\u0449\u0438\u0439 \u0433\u0440\u043e\u043c",
         "TH": "Thundersoother",
         "TR": "Y\u0131ld\u0131r\u0131m Terbiyecisi",
         "VI": "T\u00f4n Gi\u1ea3 Tr\u1ea7m L\u1eb7ng"
     },
+    "1925210475": {
+        "CHS": "\u6c34\u4ed9\u4e4b\u68a6",
+        "CHT": "\u6c34\u4ed9\u4e4b\u5922",
+        "DE": "Traum der Narzisse",
+        "EN": "Nymph's Dream",
+        "ES": "Sue\u00f1o de la Ninfa",
+        "FR": "R\u00eave de la nymphe",
+        "ID": "Nymph's Dream",
+        "IT": "Sogno della ninfa",
+        "JP": "\u6c34\u4ed9\u306e\u5922",
+        "KR": "\ub2d8\ud504\uc758 \uafc8",
+        "PT": "Sonho da Ninfa",
+        "RU": "\u0421\u043e\u043d \u043d\u0438\u043c\u0444\u044b",
+        "TH": "Nymph's Dream",
+        "TR": "Nergisin R\u00fcyas\u0131",
+        "VI": "Gi\u1ea5c M\u1ed9ng Th\u1ee7y Ti\u00ean"
+    },
     "2040573235": {
         "CHS": "\u60a0\u53e4\u7684\u78d0\u5ca9",
         "CHT": "\u60a0\u53e4\u7684\u78d0\u5ca9",
         "DE": "Archaischer Fels",
         "EN": "Archaic Petra",
         "ES": "Petra Arcaica",
         "FR": "Roche ancienne",
@@ -403,14 +420,31 @@
         "KR": "\uc808\uc5f0\uc758 \uae30\uce58",
         "PT": "Selo da Insula\u00e7\u00e3o",
         "RU": "\u042d\u043c\u0431\u043b\u0435\u043c\u0430 \u0440\u0430\u0441\u0441\u0435\u0447\u0451\u043d\u043d\u043e\u0439 \u0441\u0443\u0434\u044c\u0431\u044b",
         "TH": "Emblem of Severed Fate",
         "TR": "Par\u00e7alanan Kader Amblemi",
         "VI": "D\u1ea5u \u1ea4n Ng\u0103n C\u00e1ch"
     },
+    "235897163": {
+        "CHS": "\u82b1\u6d77\u7518\u9732\u4e4b\u5149",
+        "CHT": "\u82b1\u6d77\u7518\u9732\u4e4b\u5149",
+        "DE": "Licht der Vourukasha-Oase",
+        "EN": "Vourukasha's Glow",
+        "ES": "Fulgor de Vurukasha",
+        "FR": "Lueur du vourukasha",
+        "ID": "Vourukasha's Glow",
+        "IT": "Bagliore di Vourukasha",
+        "JP": "\u82b1\u6d77\u7518\u9732\u306e\u5149",
+        "KR": "\uac10\ub85c\ube5b \uaf43\ubc14\ub2e4",
+        "PT": "Brilho Vourukasha",
+        "RU": "\u0421\u0438\u044f\u043d\u0438\u0435 \u0412\u0443\u0440\u0443\u043a\u0430\u0448\u0438",
+        "TH": "Vourukasha's Glow",
+        "TR": "Vourukasha'n\u0131n Par\u0131lt\u0131s\u0131",
+        "VI": "V\u1ea7ng S\u00e1ng Vourukasha"
+    },
     "2364208851": {
         "CHS": "\u884c\u8005\u4e4b\u5fc3",
         "CHT": "\u884c\u8005\u4e4b\u5fc3",
         "DE": "Fernweh",
         "EN": "Resolution of Sojourner",
         "ES": "Coraz\u00f3n del Viajero",
         "FR": "C\u0153ur du Voyageur",
@@ -703,15 +737,15 @@
         "EN": "Shimenawa's Reminiscence",
         "ES": "Reminiscencia de la Purificaci\u00f3n",
         "FR": "R\u00e9miniscence nostalgique",
         "ID": "Shimenawa's Reminiscence",
         "IT": "Reminiscenza di Shimenawa",
         "JP": "\u8ffd\u61b6\u306e\u3057\u3081\u7e04",
         "KR": "\ucd94\uc5b5\uc758 \uc2dc\uba54\ub098\uc640",
-        "PT": "Reminesc\u00eancia Nost\u00e1lgica",
+        "PT": "Reminisc\u00eancia Nost\u00e1lgica",
         "RU": "\u0412\u043e\u0441\u043f\u043e\u043c\u0438\u043d\u0430\u043d\u0438\u044f \u0421\u0438\u043c\u044d\u043d\u0430\u0432\u044b",
         "TH": "Shimenawa's Reminiscence",
         "TR": "Shimenawa'n\u0131n Hat\u0131ras\u0131",
         "VI": "D\u00f2ng H\u1ed3i \u1ee8c B\u1ea5t T\u1eadn"
     },
     "4145306051": {
         "CHS": "\u9970\u91d1\u4e4b\u68a6",
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/langs/artifacts.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/langs/artifacts.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9842602308499475%*

 * *Differences: {"'1000397964'": "OrderedDict([('FR', 'Monocle de dragon démoniaque'), ('JP', '悪龍の片眼鏡'), ('CHT', "*

 * *                 '\'惡龍的單片鏡\'), (\'ID\', "Fell Dragon\'s Monocle"), (\'CHS\', \'恶龙的单片镜\'), (\'VI\', '*

 * *                 "'Kính Mắt Của Ác Long'), ('ES', 'Monóculo del Dragón Protervo'), ('TH', "*

 * *                 '"Fell Dragon\'s Monocle"), (\'TR\', \'Uğursuz Ejderin Gözlüğü\'), (\'KR\', \'악룡의 '*

 * *                 "단안경'), ('DE', 'Monokel des bösen Drachen'), ('RU', 'Монокль свирепого дракона'), "*

 * *                 ' […]*

```diff
@@ -1,8 +1,25 @@
 {
+    "1000397964": {
+        "CHS": "\u6076\u9f99\u7684\u5355\u7247\u955c",
+        "CHT": "\u60e1\u9f8d\u7684\u55ae\u7247\u93e1",
+        "DE": "Monokel des b\u00f6sen Drachen",
+        "EN": "Fell Dragon's Monocle",
+        "ES": "Mon\u00f3culo del Drag\u00f3n Protervo",
+        "FR": "Monocle de dragon d\u00e9moniaque",
+        "ID": "Fell Dragon's Monocle",
+        "IT": "Monocolo del drago caduto",
+        "JP": "\u60aa\u9f8d\u306e\u7247\u773c\u93e1",
+        "KR": "\uc545\ub8e1\uc758 \ub2e8\uc548\uacbd",
+        "PT": "Mon\u00f3culo do Drag\u00e3o Maligno",
+        "RU": "\u041c\u043e\u043d\u043e\u043a\u043b\u044c \u0441\u0432\u0438\u0440\u0435\u043f\u043e\u0433\u043e \u0434\u0440\u0430\u043a\u043e\u043d\u0430",
+        "TH": "Fell Dragon's Monocle",
+        "TR": "U\u011fursuz Ejderin G\u00f6zl\u00fc\u011f\u00fc",
+        "VI": "K\u00ednh M\u1eaft C\u1ee7a \u00c1c Long"
+    },
     "1000741724": {
         "CHS": "\u4e50\u56e2\u7684\u6668\u5149",
         "CHT": "\u6a02\u5718\u7684\u6668\u5149",
         "DE": "Morgenlicht des Ensembles",
         "EN": "Troupe's Dawnlight",
         "ES": "Luz Matinal de la Orquesta",
         "FR": "Aube de l'orchestre",
@@ -386,14 +403,31 @@
         "KR": "\ubb34\uc778\uc758 \ub450\uac74",
         "PT": "Bandana de Artista Marcial",
         "RU": "\u041f\u043e\u0432\u044f\u0437\u043a\u0430 \u0432\u043e\u0438\u043d\u0430",
         "TH": "Martial Artist's Bandana",
         "TR": "D\u00f6v\u00fc\u015f Ustas\u0131n\u0131n Bandanas\u0131",
         "VI": "Kh\u0103n V\u00f5 Nh\u00e2n"
     },
+    "1023372020": {
+        "CHS": "\u52c7\u8005\u4eec\u7684\u8336\u4f1a",
+        "CHT": "\u52c7\u8005\u5011\u7684\u8336\u6703",
+        "DE": "Teegesellschaft der Tapferen",
+        "EN": "Heroes' Tea Party",
+        "ES": "Fiesta del T\u00e9 de la Valent\u00eda",
+        "FR": "Go\u00fbter des h\u00e9ros",
+        "ID": "Heroes' Tea Party",
+        "IT": "Un t\u00e8 con gli eroi",
+        "JP": "\u52c7\u8005\u305f\u3061\u306e\u304a\u8336\u4f1a",
+        "KR": "\uc6a9\uc790\ub4e4\uc758 \ud2f0\ud0c0\uc784",
+        "PT": "Festa de Ch\u00e1 dos Her\u00f3is",
+        "RU": "\u0427\u0430\u0435\u043f\u0438\u0442\u0438\u0435 \u0433\u0435\u0440\u043e\u0435\u0432",
+        "TH": "Heroes' Tea Party",
+        "TR": "Kahramanlar\u0131n \u00c7ay Partisi",
+        "VI": "Ti\u1ec7c Tr\u00e0 C\u00e1c D\u0169ng S\u0129"
+    },
     "1024337420": {
         "CHS": "\u4e0d\u52a8\u7384\u77f3\u4e4b\u76f8",
         "CHT": "\u4e0d\u52d5\u7384\u77f3\u4e4b\u76f8",
         "DE": "Maske des starren Gesteins",
         "EN": "Mask of Solitude Basalt",
         "ES": "M\u00e1scara de Basalto Inerte",
         "FR": "Masque en basalte inerte",
@@ -539,14 +573,31 @@
         "KR": "\uae30\uc801\uc758 \uc794",
         "PT": "C\u00e1lice do Milagre",
         "RU": "\u0427\u0430\u0448\u043a\u0430 \u043c\u0430\u043b\u0435\u043d\u044c\u043a\u043e\u0433\u043e \u0447\u0443\u0434\u0430",
         "TH": "Tiny Miracle's Goblet",
         "TR": "K\u00fc\u00e7\u00fck Mucizenin Kadehi",
         "VI": "Ly K\u1ef3 T\u00edch"
     },
+    "103062540": {
+        "CHS": "\u6076\u9f99\u7684\u5355\u7247\u955c",
+        "CHT": "\u60e1\u9f8d\u7684\u55ae\u7247\u93e1",
+        "DE": "Monokel des b\u00f6sen Drachen",
+        "EN": "Fell Dragon's Monocle",
+        "ES": "Mon\u00f3culo del Drag\u00f3n Protervo",
+        "FR": "Monocle de dragon d\u00e9moniaque",
+        "ID": "Fell Dragon's Monocle",
+        "IT": "Monocolo del drago caduto",
+        "JP": "\u60aa\u9f8d\u306e\u7247\u773c\u93e1",
+        "KR": "\uc545\ub8e1\uc758 \ub2e8\uc548\uacbd",
+        "PT": "Mon\u00f3culo do Drag\u00e3o Maligno",
+        "RU": "\u041c\u043e\u043d\u043e\u043a\u043b\u044c \u0441\u0432\u0438\u0440\u0435\u043f\u043e\u0433\u043e \u0434\u0440\u0430\u043a\u043e\u043d\u0430",
+        "TH": "Fell Dragon's Monocle",
+        "TR": "U\u011fursuz Ejderin G\u00f6zl\u00fc\u011f\u00fc",
+        "VI": "K\u00ednh M\u1eaft C\u1ee7a \u00c1c Long"
+    },
     "1030810684": {
         "CHS": "\u67d3\u8840\u9a91\u58eb\u4e4b\u676f",
         "CHT": "\u67d3\u8840\u9a0e\u58eb\u4e4b\u676f",
         "DE": "Kelch des Blutbefleckten",
         "EN": "Bloodstained Chevalier's Goblet",
         "ES": "C\u00e1liz del Caballero Sanguinario",
         "FR": "Coupe du chevalier ensanglant\u00e9e",
@@ -3599,14 +3650,31 @@
         "KR": "\ub208\ubc2d \uc18d\uc758 \uae43\ud138",
         "PT": "Pena da Neve",
         "RU": "\u041f\u0435\u0440\u043e \u0441\u043d\u0435\u0436\u043d\u044b\u0445 \u0440\u0430\u0432\u043d\u0438\u043d",
         "TH": "Plume of Snow",
         "TR": "Kar T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 D\u01b0\u1edbi Tuy\u1ebft"
     },
+    "1201323332": {
+        "CHS": "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6",
+        "CHT": "\u4e45\u9060\u82b1\u843d\u4e4b\u6642",
+        "DE": "Uralter Abschied",
+        "EN": "Ancient Abscission",
+        "ES": "Marchitamiento de Anta\u00f1o",
+        "FR": "Abscission ancienne",
+        "ID": "Ancient Abscission",
+        "IT": "Escissione ancestrale",
+        "JP": "\u4e45\u9060\u843d\u82b1\u306e\u6642",
+        "KR": "\uba3c \uc61b\ub0a0 \uaf43\uc774 \uc9c8 \ubb34\ub835",
+        "PT": "Abscis\u00e3o Antiga",
+        "RU": "\u0414\u0440\u0435\u0432\u043d\u0435\u0435 \u0443\u0432\u044f\u0434\u0430\u043d\u0438\u0435",
+        "TH": "Ancient Abscission",
+        "TR": "Ge\u00e7mi\u015fin Yaprak D\u00f6k\u00fcmleri",
+        "VI": "Th\u1eddi Kh\u1eafc X\u01b0a C\u1ed5"
+    },
     "120343020": {
         "CHS": "\u534e\u9986\u4e4b\u7fbd",
         "CHT": "\u83ef\u9928\u4e4b\u7fbd",
         "DE": "Feder der Opulenz",
         "EN": "Plume of Luxury",
         "ES": "Pluma de la Opulencia",
         "FR": "Plume d'opulence",
@@ -4313,14 +4381,31 @@
         "KR": "\ub9c8\ub140\uc758 \uc5fc\ud654 \uaf43",
         "PT": "Flor de Labareda da Bruxa",
         "RU": "\u0412\u0435\u0434\u044c\u043c\u0438\u043d \u043e\u0433\u043d\u0435\u043d\u043d\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a",
         "TH": "Witch's Flower of Blaze",
         "TR": "Cad\u0131n\u0131n Alev \u00c7i\u00e7e\u011fi",
         "VI": "Hoa L\u1eeda C\u1ee7a Ma N\u1eef"
     },
+    "1251573836": {
+        "CHS": "\u65c5\u9014\u4e2d\u7684\u9c9c\u82b1",
+        "CHT": "\u65c5\u9014\u4e2d\u7684\u9bae\u82b1",
+        "DE": "Blume auf der Reise",
+        "EN": "Odyssean Flower",
+        "ES": "Flor del Periplo",
+        "FR": "Fleur odyss\u00e9enne",
+        "ID": "Odyssean Flower",
+        "IT": "Fiore odisseico",
+        "JP": "\u65c5\u4e2d\u306e\u82b1",
+        "KR": "\uc5ec\uc815 \uc911\uc758 \uaf43",
+        "PT": "Flor da Jornada",
+        "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0441\u0442\u0440\u0430\u043d\u0441\u0442\u0432\u0438\u0439",
+        "TH": "Odyssean Flower",
+        "TR": "Yolculuk \u00c7i\u00e7e\u011fi",
+        "VI": "Hoa T\u01b0\u01a1i Tr\u00ean L\u1eef Tr\u00ecnh"
+    },
     "1251916452": {
         "CHS": "\u6e38\u533b\u7684\u6000\u949f",
         "CHT": "\u904a\u91ab\u7684\u61f7\u9418",
         "DE": "Wanderarzt-Taschenuhr",
         "EN": "Traveling Doctor's Pocket Watch",
         "ES": "Reloj de Bolsillo de la M\u00e9dica Itinerante",
         "FR": "Montre de poche du M\u00e9decin itin\u00e9rant",
@@ -4381,14 +4466,31 @@
         "KR": "\uc6a9\uc0ac\uc758 \ud6c8\uc7a5",
         "PT": "Medalha do Valente",
         "RU": "\u0411\u0440\u043e\u0448\u044c \u0445\u0440\u0430\u0431\u0440\u0435\u0446\u0430",
         "TH": "Medal of The Brave",
         "TR": "Cesurlar\u0131n Madalyas\u0131",
         "VI": "Huy Ch\u01b0\u01a1ng D\u0169ng S\u0129"
     },
+    "1255686932": {
+        "CHS": "\u6c34\u4ed9\u7684\u65f6\u65f6\u523b\u523b",
+        "CHT": "\u6c34\u4ed9\u7684\u6642\u6642\u523b\u523b",
+        "DE": "Best\u00e4ndigkeit der Narzisse",
+        "EN": "Nymph's Constancy",
+        "ES": "Asiduidad de las Ninfas",
+        "FR": "Constance de la nymphe",
+        "ID": "Nymph's Constancy",
+        "IT": "Fedelt\u00e0 della ninfa",
+        "JP": "\u6c34\u4ed9\u306e\u4e00\u77ac\u4e00\u77ac",
+        "KR": "\ub2d8\ud504\uc758 \uc2dc\uc2dc\uac01\uac01",
+        "PT": "Ninfas Eternas",
+        "RU": "\u041f\u043e\u0441\u0442\u043e\u044f\u043d\u0441\u0442\u0432\u043e \u043d\u0438\u043c\u0444\u044b",
+        "TH": "Nymph's Constancy",
+        "TR": "Nergisin Daimiyeti",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a Th\u1ee7y Ti\u00ean"
+    },
     "1257751660": {
         "CHS": "\u5b88\u79d8\u7684\u9b54\u74f6",
         "CHT": "\u5b88\u79d8\u7684\u9b54\u74f6",
         "DE": "Zauberflasche des Geheimnisbewahrers",
         "EN": "Secret-Keeper's Magic Bottle",
         "ES": "Frasco M\u00e1gico de la Confidencia",
         "FR": "Bouteille magique du gardien du secret",
@@ -6064,14 +6166,31 @@
         "KR": "\uc6a9\uc0ac\uc758 \uae30\ub300",
         "PT": "Esperan\u00e7a do Valente",
         "RU": "\u041d\u0430\u0434\u0435\u0436\u0434\u044b \u0445\u0440\u0430\u0431\u0440\u0435\u0446\u0430",
         "TH": "Prospect of the Brave",
         "TR": "Cesurlar\u0131n Aray\u0131\u015f\u0131",
         "VI": "S\u1ef1 Mong \u0110\u1ee3i C\u1ee7a D\u0169ng S\u0129"
     },
+    "1352276684": {
+        "CHS": "\u65e0\u8fb9\u9163\u4e50\u4e4b\u7b75",
+        "CHT": "\u7121\u908a\u9163\u6a02\u4e4b\u7b75",
+        "DE": "Festessen der grenzenlosen Freude",
+        "EN": "Feast of Boundless Joy",
+        "ES": "Fest\u00edn del J\u00fabilo Inconmensurable",
+        "FR": "Festin de joie sans bornes",
+        "ID": "Feast of Boundless Joy",
+        "IT": "Banchetto della gioia infinita",
+        "JP": "\u559c\u697d\u7121\u9650\u306e\u5bb4",
+        "KR": "\ub05d\uc5c6\ub294 \ud5a5\ub77d\uc758 \uc5f0\ud68c",
+        "PT": "C\u00e1lice do Festival Alegre",
+        "RU": "\u041f\u0438\u0440 \u043d\u0435\u043e\u0431\u0443\u0437\u0434\u0430\u043d\u043d\u043e\u0433\u043e \u0432\u0435\u0441\u0435\u043b\u044c\u044f",
+        "TH": "Feast of Boundless Joy",
+        "TR": "Sonsuz Sevin\u00e7 \u015eenli\u011fi",
+        "VI": "B\u1eefa Ti\u1ec7c Vui V\u00f4 B\u1edd"
+    },
     "1353039908": {
         "CHS": "\u68a6\u4e2d\u7684\u94c1\u82b1",
         "CHT": "\u5922\u4e2d\u7684\u9435\u82b1",
         "DE": "Metallbl\u00fcte im Traum",
         "EN": "Dreaming Steelbloom",
         "ES": "Flor de Metal On\u00edrica",
         "FR": "Fleur d'acier r\u00eaveuse",
@@ -7509,14 +7628,31 @@
         "KR": "\ub1cc\uc815\uc758 \uc2dc\uacc4",
         "PT": "Rel\u00f3gio do Trov\u00e3o",
         "RU": "\u041f\u0435\u0441\u043e\u0447\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u0433\u0440\u043e\u043c\u0430",
         "TH": "Hourglass of Thunder",
         "TR": "Y\u0131ld\u0131r\u0131m Saati",
         "VI": "Th\u1eddi Gian L\u00f4i \u0110\u00ecnh"
     },
+    "1433962852": {
+        "CHS": "\u65e0\u8fb9\u9163\u4e50\u4e4b\u7b75",
+        "CHT": "\u7121\u908a\u9163\u6a02\u4e4b\u7b75",
+        "DE": "Festessen der grenzenlosen Freude",
+        "EN": "Feast of Boundless Joy",
+        "ES": "Fest\u00edn del J\u00fabilo Inconmensurable",
+        "FR": "Festin de joie sans bornes",
+        "ID": "Feast of Boundless Joy",
+        "IT": "Banchetto della gioia infinita",
+        "JP": "\u559c\u697d\u7121\u9650\u306e\u5bb4",
+        "KR": "\ub05d\uc5c6\ub294 \ud5a5\ub77d\uc758 \uc5f0\ud68c",
+        "PT": "C\u00e1lice do Festival Alegre",
+        "RU": "\u041f\u0438\u0440 \u043d\u0435\u043e\u0431\u0443\u0437\u0434\u0430\u043d\u043d\u043e\u0433\u043e \u0432\u0435\u0441\u0435\u043b\u044c\u044f",
+        "TH": "Feast of Boundless Joy",
+        "TR": "Sonsuz Sevin\u00e7 \u015eenli\u011fi",
+        "VI": "B\u1eefa Ti\u1ec7c Vui V\u00f4 B\u1edd"
+    },
     "1434913164": {
         "CHS": "\u9970\u91d1\u80f8\u82b1",
         "CHT": "\u98fe\u91d1\u80f8\u82b1",
         "DE": "Vergoldete Brosche",
         "EN": "Gilded Corsage",
         "ES": "Broche Dorado",
         "FR": "Broche plaqu\u00e9e",
@@ -11300,14 +11436,31 @@
         "KR": "\uad50\uad00\uc758 \ud68c\uc911\uc2dc\uacc4",
         "PT": "Rel\u00f3gio de Bolso de Instrutor",
         "RU": "\u041a\u0430\u0440\u043c\u0430\u043d\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u0438\u043d\u0441\u0442\u0440\u0443\u043a\u0442\u043e\u0440\u0430",
         "TH": "Instructor's Pocket Watch",
         "TR": "E\u011fitmenin Cep Saati",
         "VI": "\u0110\u1ed3ng H\u1ed3 Gi\u00e1o Quan"
     },
+    "1663575524": {
+        "CHS": "\u7426\u8272\u7075\u5f69\u4e4b\u7fbd",
+        "CHT": "\u7426\u8272\u9748\u5f69\u4e4b\u7fbd",
+        "DE": "Bezaubernde Feder",
+        "EN": "Vibrant Pinion",
+        "ES": "Pluma Crom\u00e1tica",
+        "FR": "Penne vibrante",
+        "ID": "Vibrant Pinion",
+        "IT": "Penna dalle tinte vivaci",
+        "JP": "\u970a\u5f69\u5947\u9e97\u306e\u7fbd",
+        "KR": "\uc601\ub871\ud55c \uc625\ube5b \uae43\ud138",
+        "PT": "Pluma do Cristal Reluzente",
+        "RU": "\u0421\u0430\u043c\u043e\u0446\u0432\u0435\u0442\u043d\u043e\u0435 \u043f\u0435\u0440\u043e",
+        "TH": "Vibrant Pinion",
+        "TR": "Alacal\u0131 T\u00fcy",
+        "VI": "L\u00f4ng V\u0169 \u00c1nh S\u1eafc M\u00e0u"
+    },
     "1665536940": {
         "CHS": "\u5b97\u5ba4\u9762\u5177",
         "CHT": "\u5b97\u5ba4\u9762\u5177",
         "DE": "K\u00f6nigliche Maske",
         "EN": "Royal Masque",
         "ES": "M\u00e1scara Real",
         "FR": "Masque du Noble",
@@ -13561,14 +13714,31 @@
         "KR": "\uc7a5\uc218\uc758 \ud22c\uad6c",
         "PT": "Capacete do Comandante",
         "RU": "\u0414\u0440\u0435\u0432\u043d\u0438\u0439 \u0448\u043b\u0435\u043c \u0433\u0435\u043d\u0435\u0440\u0430\u043b\u0430",
         "TH": "General's Ancient Helm",
         "TR": "Kadim General Mi\u011fferi",
         "VI": "N\u00f3n Nguy\u00ean So\u00e1i"
     },
+    "1808154372": {
+        "CHS": "\u6076\u9f99\u7684\u5355\u7247\u955c",
+        "CHT": "\u60e1\u9f8d\u7684\u55ae\u7247\u93e1",
+        "DE": "Monokel des b\u00f6sen Drachen",
+        "EN": "Fell Dragon's Monocle",
+        "ES": "Mon\u00f3culo del Drag\u00f3n Protervo",
+        "FR": "Monocle de dragon d\u00e9moniaque",
+        "ID": "Fell Dragon's Monocle",
+        "IT": "Monocolo del drago caduto",
+        "JP": "\u60aa\u9f8d\u306e\u7247\u773c\u93e1",
+        "KR": "\uc545\ub8e1\uc758 \ub2e8\uc548\uacbd",
+        "PT": "Mon\u00f3culo do Drag\u00e3o Maligno",
+        "RU": "\u041c\u043e\u043d\u043e\u043a\u043b\u044c \u0441\u0432\u0438\u0440\u0435\u043f\u043e\u0433\u043e \u0434\u0440\u0430\u043a\u043e\u043d\u0430",
+        "TH": "Fell Dragon's Monocle",
+        "TR": "U\u011fursuz Ejderin G\u00f6zl\u00fc\u011f\u00fc",
+        "VI": "K\u00ednh M\u1eaft C\u1ee7a \u00c1c Long"
+    },
     "1808344828": {
         "CHS": "\u5b97\u5ba4\u4e4b\u82b1",
         "CHT": "\u5b97\u5ba4\u4e4b\u82b1",
         "DE": "K\u00f6nigliche Blume",
         "EN": "Royal Flora",
         "ES": "Flora Real",
         "FR": "Fleur du Noble",
@@ -14224,14 +14394,31 @@
         "KR": "\ub5a0\ub3cc\uc774 \uc758\uc0ac\uc758 \ub450\uac74",
         "PT": "Len\u00e7o do Doutor Viajante",
         "RU": "\u041f\u043b\u0430\u0442\u043e\u043a \u0446\u0435\u043b\u0438\u0442\u0435\u043b\u044f",
         "TH": "Traveling Doctor's Handkerchief",
         "TR": "Gezgin Doktorun Mendili",
         "VI": "Kh\u0103n Th\u1ea7y Thu\u1ed1c"
     },
+    "1849454924": {
+        "CHS": "\u7075\u5149\u6e90\u8d77\u4e4b\u854a",
+        "CHT": "\u9748\u5149\u6e90\u8d77\u4e4b\u854a",
+        "DE": "Staubblatt Khvarenas Herkunft",
+        "EN": "Stamen of Khvarena's Origin",
+        "ES": "Estambre Primordial de la Jvarena",
+        "FR": "\u00c9tamine de l'origine de la khvarena",
+        "ID": "Stamen of Khvarena's Origin",
+        "IT": "Stame della Genesi di Khvarena",
+        "JP": "\u970a\u5149\u8d77\u6e90\u306e\u854a",
+        "KR": "\ud06c\ubc14\ub808\ub098 \uae30\uc6d0\uc758 \uaf43\uc220",
+        "PT": "Estame Primordial de Khvarena",
+        "RU": "\u0422\u044b\u0447\u0438\u043d\u043a\u0430 \u0438\u0441\u0442\u043e\u043a\u0430 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Stamen of Khvarena's Origin",
+        "TR": "Khvarena'n\u0131n K\u00f6keninin Tomurcu\u011fu",
+        "VI": "Nh\u1ee5y Hoa Khvarena Kh\u1edfi Nguy\u00ean"
+    },
     "1850111036": {
         "CHS": "\u505c\u6446\u4e4b\u523b",
         "CHT": "\u505c\u64fa\u4e4b\u523b",
         "DE": "Uhr des Stillstands",
         "EN": "Moment of Cessation",
         "ES": "Momento de Cese",
         "FR": "Fig\u00e9 dans le temps",
@@ -17386,14 +17573,31 @@
         "KR": "\uc0d8\ubb3c\uc758 \ucc3b\uc794",
         "PT": "C\u00e1lice da Fonte",
         "RU": "\u0427\u0430\u0448\u0430 \u0438\u0441\u0442\u043e\u043a\u0430",
         "TH": "Chalice of the Font",
         "TR": "P\u0131narlar\u0131n Kadehi",
         "VI": "Ch\u00e9n N\u01b0\u1edbc Th\u00e1nh"
     },
+    "203252716": {
+        "CHS": "\u6c34\u4ed9\u7684\u65f6\u65f6\u523b\u523b",
+        "CHT": "\u6c34\u4ed9\u7684\u6642\u6642\u523b\u523b",
+        "DE": "Best\u00e4ndigkeit der Narzisse",
+        "EN": "Nymph's Constancy",
+        "ES": "Asiduidad de las Ninfas",
+        "FR": "Constance de la nymphe",
+        "ID": "Nymph's Constancy",
+        "IT": "Fedelt\u00e0 della ninfa",
+        "JP": "\u6c34\u4ed9\u306e\u4e00\u77ac\u4e00\u77ac",
+        "KR": "\ub2d8\ud504\uc758 \uc2dc\uc2dc\uac01\uac01",
+        "PT": "Ninfas Eternas",
+        "RU": "\u041f\u043e\u0441\u0442\u043e\u044f\u043d\u0441\u0442\u0432\u043e \u043d\u0438\u043c\u0444\u044b",
+        "TH": "Nymph's Constancy",
+        "TR": "Nergisin Daimiyeti",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a Th\u1ee7y Ti\u00ean"
+    },
     "2034328036": {
         "CHS": "\u8d4c\u5f92\u7684\u80f8\u82b1",
         "CHT": "\u8ced\u5f92\u7684\u80f8\u82b1",
         "DE": "Gl\u00fccksspielbrosche",
         "EN": "Gambler's Brooch",
         "ES": "Broche de la Jugadora",
         "FR": "Broche du Parieur",
@@ -19851,14 +20055,31 @@
         "KR": "\uc61b \ubc97\uc758 \ub9c8\uc74c",
         "PT": "Cora\u00e7\u00e3o de Camaradagem",
         "RU": "\u0421\u0435\u0440\u0434\u0446\u0435 \u0442\u043e\u0432\u0430\u0440\u0438\u0449\u0435\u0441\u0442\u0432\u0430",
         "TH": "Heart of Comradeship",
         "TR": "Yolda\u015fl\u0131k Kalbi",
         "VI": "Tr\u00e1i Tim C\u1ee7a C\u1ed1 Nh\u00e2n"
     },
+    "2192067188": {
+        "CHS": "\u7075\u5149\u6e90\u8d77\u4e4b\u854a",
+        "CHT": "\u9748\u5149\u6e90\u8d77\u4e4b\u854a",
+        "DE": "Staubblatt Khvarenas Herkunft",
+        "EN": "Stamen of Khvarena's Origin",
+        "ES": "Estambre Primordial de la Jvarena",
+        "FR": "\u00c9tamine de l'origine de la khvarena",
+        "ID": "Stamen of Khvarena's Origin",
+        "IT": "Stame della Genesi di Khvarena",
+        "JP": "\u970a\u5149\u8d77\u6e90\u306e\u854a",
+        "KR": "\ud06c\ubc14\ub808\ub098 \uae30\uc6d0\uc758 \uaf43\uc220",
+        "PT": "Estame Primordial de Khvarena",
+        "RU": "\u0422\u044b\u0447\u0438\u043d\u043a\u0430 \u0438\u0441\u0442\u043e\u043a\u0430 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Stamen of Khvarena's Origin",
+        "TR": "Khvarena'n\u0131n K\u00f6keninin Tomurcu\u011fu",
+        "VI": "Nh\u1ee5y Hoa Khvarena Kh\u1edfi Nguy\u00ean"
+    },
     "219231412": {
         "CHS": "\u590f\u796d\u4e4b\u82b1",
         "CHT": "\u590f\u796d\u4e4b\u82b1",
         "DE": "Sommerfestbrosche",
         "EN": "Summer Night's Bloom",
         "ES": "Flor de la Noche de Verano",
         "FR": "Fleur de la nuit d'\u00e9t\u00e9",
@@ -21857,14 +22078,31 @@
         "KR": "\uc655\uc2e4\uc758 \uc740\ud56d\uc544\ub9ac",
         "PT": "Urna de Prata Real",
         "RU": "\u041a\u043e\u0440\u043e\u043b\u0435\u0432\u0441\u043a\u0430\u044f \u0441\u0435\u0440\u0435\u0431\u0440\u044f\u043d\u0430\u044f \u0444\u043b\u044f\u0436\u043a\u0430",
         "TH": "Royal Silver Urn",
         "TR": "Kraliyet G\u00fcm\u00fc\u015f Vazosu",
         "VI": "B\u00ecnh B\u1ea1c T\u00f4ng Th\u1ea5t"
     },
+    "2330924084": {
+        "CHS": "\u7075\u5149\u6e90\u8d77\u4e4b\u854a",
+        "CHT": "\u9748\u5149\u6e90\u8d77\u4e4b\u854a",
+        "DE": "Staubblatt Khvarenas Herkunft",
+        "EN": "Stamen of Khvarena's Origin",
+        "ES": "Estambre Primordial de la Jvarena",
+        "FR": "\u00c9tamine de l'origine de la khvarena",
+        "ID": "Stamen of Khvarena's Origin",
+        "IT": "Stame della Genesi di Khvarena",
+        "JP": "\u970a\u5149\u8d77\u6e90\u306e\u854a",
+        "KR": "\ud06c\ubc14\ub808\ub098 \uae30\uc6d0\uc758 \uaf43\uc220",
+        "PT": "Estame Primordial de Khvarena",
+        "RU": "\u0422\u044b\u0447\u0438\u043d\u043a\u0430 \u0438\u0441\u0442\u043e\u043a\u0430 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Stamen of Khvarena's Origin",
+        "TR": "Khvarena'n\u0131n K\u00f6keninin Tomurcu\u011fu",
+        "VI": "Nh\u1ee5y Hoa Khvarena Kh\u1edfi Nguy\u00ean"
+    },
     "233094236": {
         "CHS": "\u590f\u796d\u4e4b\u82b1",
         "CHT": "\u590f\u796d\u4e4b\u82b1",
         "DE": "Sommerfestbrosche",
         "EN": "Summer Night's Bloom",
         "ES": "Flor de la Noche de Verano",
         "FR": "Fleur de la nuit d'\u00e9t\u00e9",
@@ -23591,14 +23829,31 @@
         "KR": "\uc5ec\ub984 \ucd95\uc81c\uc758 \ubb3c\ud48d\uc120",
         "PT": "Bal\u00f5es de \u00c1gua do Festival de Ver\u00e3o",
         "RU": "\u0428\u0430\u0440 \u0440\u0430\u0432\u043d\u043e\u0434\u0435\u043d\u0441\u0442\u0432\u0438\u044f",
         "TH": "Summer Night's Waterballoon",
         "TR": "Yaz Gecesi Su Balonu",
         "VI": "Ly Ng\u1ecdc L\u1ec5 T\u1ebf M\u00f9a H\u00e8"
     },
+    "2431631004": {
+        "CHS": "\u7075\u5149\u6e90\u8d77\u4e4b\u854a",
+        "CHT": "\u9748\u5149\u6e90\u8d77\u4e4b\u854a",
+        "DE": "Staubblatt Khvarenas Herkunft",
+        "EN": "Stamen of Khvarena's Origin",
+        "ES": "Estambre Primordial de la Jvarena",
+        "FR": "\u00c9tamine de l'origine de la khvarena",
+        "ID": "Stamen of Khvarena's Origin",
+        "IT": "Stame della Genesi di Khvarena",
+        "JP": "\u970a\u5149\u8d77\u6e90\u306e\u854a",
+        "KR": "\ud06c\ubc14\ub808\ub098 \uae30\uc6d0\uc758 \uaf43\uc220",
+        "PT": "Estame Primordial de Khvarena",
+        "RU": "\u0422\u044b\u0447\u0438\u043d\u043a\u0430 \u0438\u0441\u0442\u043e\u043a\u0430 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Stamen of Khvarena's Origin",
+        "TR": "Khvarena'n\u0131n K\u00f6keninin Tomurcu\u011fu",
+        "VI": "Nh\u1ee5y Hoa Khvarena Kh\u1edfi Nguy\u00ean"
+    },
     "2432236732": {
         "CHS": "\u661f\u7f57\u572d\u74a7\u4e4b\u6677",
         "CHT": "\u661f\u7f85\u572d\u74a7\u4e4b\u6677",
         "DE": "Sonnenuhr der d\u00fcsteren Jade",
         "EN": "Sundial of Enduring Jade",
         "ES": "Reloj de Sol de Jade Sempiterno",
         "FR": "Cadran du jade immuable",
@@ -24611,14 +24866,31 @@
         "KR": "\uc720\ubc30\uc790\uc758 \ud68c\uc911\uc2dc\uacc4",
         "PT": "Rel\u00f3gio de Bolso do Exilado",
         "RU": "\u041a\u0430\u0440\u043c\u0430\u043d\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u0438\u0437\u0433\u043d\u0430\u043d\u043d\u0438\u043a\u0430",
         "TH": "Exile's Pocket Watch",
         "TR": "S\u00fcrg\u00fcn\u00fcn Cep Saati",
         "VI": "\u0110\u1ed3ng H\u1ed3 K\u1ebb L\u01b0u \u0110\u00e0y"
     },
+    "2497187284": {
+        "CHS": "\u65e0\u8fb9\u9163\u4e50\u4e4b\u7b75",
+        "CHT": "\u7121\u908a\u9163\u6a02\u4e4b\u7b75",
+        "DE": "Festessen der grenzenlosen Freude",
+        "EN": "Feast of Boundless Joy",
+        "ES": "Fest\u00edn del J\u00fabilo Inconmensurable",
+        "FR": "Festin de joie sans bornes",
+        "ID": "Feast of Boundless Joy",
+        "IT": "Banchetto della gioia infinita",
+        "JP": "\u559c\u697d\u7121\u9650\u306e\u5bb4",
+        "KR": "\ub05d\uc5c6\ub294 \ud5a5\ub77d\uc758 \uc5f0\ud68c",
+        "PT": "C\u00e1lice do Festival Alegre",
+        "RU": "\u041f\u0438\u0440 \u043d\u0435\u043e\u0431\u0443\u0437\u0434\u0430\u043d\u043d\u043e\u0433\u043e \u0432\u0435\u0441\u0435\u043b\u044c\u044f",
+        "TH": "Feast of Boundless Joy",
+        "TR": "Sonsuz Sevin\u00e7 \u015eenli\u011fi",
+        "VI": "B\u1eefa Ti\u1ec7c Vui V\u00f4 B\u1edd"
+    },
     "2501899244": {
         "CHS": "\u6d41\u653e\u8005\u4e4b\u676f",
         "CHT": "\u6d41\u653e\u8005\u4e4b\u676f",
         "DE": "Kelch des Verbannten",
         "EN": "Exile's Goblet",
         "ES": "C\u00e1liz del Exiliado",
         "FR": "Coupe de l'Exil\u00e9",
@@ -24662,14 +24934,31 @@
         "KR": "\uc655\uc2e4\uc758 \uae43\ud138",
         "PT": "Pena Real",
         "RU": "\u041a\u043e\u0440\u043e\u043b\u0435\u0432\u0441\u043a\u043e\u0435 \u043f\u0435\u0440\u043e",
         "TH": "Royal Plume",
         "TR": "Kraliyet T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 T\u00f4ng Th\u1ea5t"
     },
+    "2503679772": {
+        "CHS": "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6",
+        "CHT": "\u4e45\u9060\u82b1\u843d\u4e4b\u6642",
+        "DE": "Uralter Abschied",
+        "EN": "Ancient Abscission",
+        "ES": "Marchitamiento de Anta\u00f1o",
+        "FR": "Abscission ancienne",
+        "ID": "Ancient Abscission",
+        "IT": "Escissione ancestrale",
+        "JP": "\u4e45\u9060\u843d\u82b1\u306e\u6642",
+        "KR": "\uba3c \uc61b\ub0a0 \uaf43\uc774 \uc9c8 \ubb34\ub835",
+        "PT": "Abscis\u00e3o Antiga",
+        "RU": "\u0414\u0440\u0435\u0432\u043d\u0435\u0435 \u0443\u0432\u044f\u0434\u0430\u043d\u0438\u0435",
+        "TH": "Ancient Abscission",
+        "TR": "Ge\u00e7mi\u015fin Yaprak D\u00f6k\u00fcmleri",
+        "VI": "Th\u1eddi Kh\u1eafc X\u01b0a C\u1ed5"
+    },
     "2506859148": {
         "CHS": "\u6d41\u653e\u8005\u4e4b\u676f",
         "CHT": "\u6d41\u653e\u8005\u4e4b\u676f",
         "DE": "Kelch des Verbannten",
         "EN": "Exile's Goblet",
         "ES": "C\u00e1liz del Exiliado",
         "FR": "Coupe de l'Exil\u00e9",
@@ -24968,14 +25257,31 @@
         "KR": "\uc6d4\ub140\uc758 \uc0c9\ucc44",
         "PT": "Esplendor da Dama da Lua",
         "RU": "\u0412\u0435\u043b\u0438\u043a\u043e\u043b\u0435\u043f\u0438\u0435 \u0410\u0439-\u0425\u0430\u043d\u0443\u043c",
         "TH": "Ay-Khanoum's Myriad",
         "TR": "Ay-Khanoum Enginli\u011fi",
         "VI": "Mu\u00f4n S\u1eafc C\u1ee7a Ay-Khanoum"
     },
+    "2527776044": {
+        "CHS": "\u52c7\u8005\u4eec\u7684\u8336\u4f1a",
+        "CHT": "\u52c7\u8005\u5011\u7684\u8336\u6703",
+        "DE": "Teegesellschaft der Tapferen",
+        "EN": "Heroes' Tea Party",
+        "ES": "Fiesta del T\u00e9 de la Valent\u00eda",
+        "FR": "Go\u00fbter des h\u00e9ros",
+        "ID": "Heroes' Tea Party",
+        "IT": "Un t\u00e8 con gli eroi",
+        "JP": "\u52c7\u8005\u305f\u3061\u306e\u304a\u8336\u4f1a",
+        "KR": "\uc6a9\uc790\ub4e4\uc758 \ud2f0\ud0c0\uc784",
+        "PT": "Festa de Ch\u00e1 dos Her\u00f3is",
+        "RU": "\u0427\u0430\u0435\u043f\u0438\u0442\u0438\u0435 \u0433\u0435\u0440\u043e\u0435\u0432",
+        "TH": "Heroes' Tea Party",
+        "TR": "Kahramanlar\u0131n \u00c7ay Partisi",
+        "VI": "Ti\u1ec7c Tr\u00e0 C\u00e1c D\u0169ng S\u0129"
+    },
     "2527845844": {
         "CHS": "\u4e50\u56e2\u7684\u6668\u5149",
         "CHT": "\u6a02\u5718\u7684\u6668\u5149",
         "DE": "Morgenlicht des Ensembles",
         "EN": "Troupe's Dawnlight",
         "ES": "Luz Matinal de la Orquesta",
         "FR": "Aube de l'orchestre",
@@ -26447,14 +26753,31 @@
         "KR": "\uc655\uc2e4\uc758 \uc740\ud56d\uc544\ub9ac",
         "PT": "Urna de Prata Real",
         "RU": "\u041a\u043e\u0440\u043e\u043b\u0435\u0432\u0441\u043a\u0430\u044f \u0441\u0435\u0440\u0435\u0431\u0440\u044f\u043d\u0430\u044f \u0444\u043b\u044f\u0436\u043a\u0430",
         "TH": "Royal Silver Urn",
         "TR": "Kraliyet G\u00fcm\u00fc\u015f Vazosu",
         "VI": "B\u00ecnh B\u1ea1c T\u00f4ng Th\u1ea5t"
     },
+    "2606766532": {
+        "CHS": "\u7426\u8272\u7075\u5f69\u4e4b\u7fbd",
+        "CHT": "\u7426\u8272\u9748\u5f69\u4e4b\u7fbd",
+        "DE": "Bezaubernde Feder",
+        "EN": "Vibrant Pinion",
+        "ES": "Pluma Crom\u00e1tica",
+        "FR": "Penne vibrante",
+        "ID": "Vibrant Pinion",
+        "IT": "Penna dalle tinte vivaci",
+        "JP": "\u970a\u5f69\u5947\u9e97\u306e\u7fbd",
+        "KR": "\uc601\ub871\ud55c \uc625\ube5b \uae43\ud138",
+        "PT": "Pluma do Cristal Reluzente",
+        "RU": "\u0421\u0430\u043c\u043e\u0446\u0432\u0435\u0442\u043d\u043e\u0435 \u043f\u0435\u0440\u043e",
+        "TH": "Vibrant Pinion",
+        "TR": "Alacal\u0131 T\u00fcy",
+        "VI": "L\u00f4ng V\u0169 \u00c1nh S\u1eafc M\u00e0u"
+    },
     "2609690236": {
         "CHS": "\u6e38\u533b\u7684\u94f6\u83b2",
         "CHT": "\u904a\u91ab\u7684\u9280\u84ee",
         "DE": "Wanderarztanemone",
         "EN": "Traveling Doctor's Silver Lotus",
         "ES": "Loto de Plata de la M\u00e9dica Itinerante",
         "FR": "An\u00e9mone du M\u00e9decin itin\u00e9rant",
@@ -28895,14 +29218,31 @@
         "KR": "\uae30\uc801\uc758 \ubaa8\ub798",
         "PT": "Ampulheta do Milagre",
         "RU": "\u041f\u0435\u0441\u043e\u0447\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u043c\u0430\u043b\u0435\u043d\u044c\u043a\u043e\u0433\u043e \u0447\u0443\u0434\u0430",
         "TH": "Tiny Miracle's Hourglass",
         "TR": "K\u00fc\u00e7\u00fck Mucizenin Kum Saati",
         "VI": "C\u00e1t K\u1ef3 T\u00edch"
     },
+    "2762923908": {
+        "CHS": "\u6c34\u4ed9\u7684\u65f6\u65f6\u523b\u523b",
+        "CHT": "\u6c34\u4ed9\u7684\u6642\u6642\u523b\u523b",
+        "DE": "Best\u00e4ndigkeit der Narzisse",
+        "EN": "Nymph's Constancy",
+        "ES": "Asiduidad de las Ninfas",
+        "FR": "Constance de la nymphe",
+        "ID": "Nymph's Constancy",
+        "IT": "Fedelt\u00e0 della ninfa",
+        "JP": "\u6c34\u4ed9\u306e\u4e00\u77ac\u4e00\u77ac",
+        "KR": "\ub2d8\ud504\uc758 \uc2dc\uc2dc\uac01\uac01",
+        "PT": "Ninfas Eternas",
+        "RU": "\u041f\u043e\u0441\u0442\u043e\u044f\u043d\u0441\u0442\u0432\u043e \u043d\u0438\u043c\u0444\u044b",
+        "TH": "Nymph's Constancy",
+        "TR": "Nergisin Daimiyeti",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a Th\u1ee7y Ti\u00ean"
+    },
     "2764088564": {
         "CHS": "\u5b66\u58eb\u7684\u58a8\u676f",
         "CHT": "\u5b78\u58eb\u7684\u58a8\u676f",
         "DE": "Gelehrten-Tintenfass",
         "EN": "Scholar's Ink Cup",
         "ES": "Tintero de la Erudita",
         "FR": "Coupe de l'\u00c9rudit",
@@ -30765,14 +31105,31 @@
         "KR": "\ubd81\ud48d\uc758 \uc794",
         "PT": "C\u00e1lice do Vento do Norte",
         "RU": "\u041a\u0443\u0431\u043e\u043a \u0441\u0435\u0432\u0435\u0440\u043d\u044b\u0445 \u0432\u0435\u0442\u0440\u043e\u0432",
         "TH": "Goblet of Aquilo",
         "TR": "Poyraz Kadehi",
         "VI": "Ly B\u1eafc Phong"
     },
+    "2870671908": {
+        "CHS": "\u7426\u8272\u7075\u5f69\u4e4b\u7fbd",
+        "CHT": "\u7426\u8272\u9748\u5f69\u4e4b\u7fbd",
+        "DE": "Bezaubernde Feder",
+        "EN": "Vibrant Pinion",
+        "ES": "Pluma Crom\u00e1tica",
+        "FR": "Penne vibrante",
+        "ID": "Vibrant Pinion",
+        "IT": "Penna dalle tinte vivaci",
+        "JP": "\u970a\u5f69\u5947\u9e97\u306e\u7fbd",
+        "KR": "\uc601\ub871\ud55c \uc625\ube5b \uae43\ud138",
+        "PT": "Pluma do Cristal Reluzente",
+        "RU": "\u0421\u0430\u043c\u043e\u0446\u0432\u0435\u0442\u043d\u043e\u0435 \u043f\u0435\u0440\u043e",
+        "TH": "Vibrant Pinion",
+        "TR": "Alacal\u0131 T\u00fcy",
+        "VI": "L\u00f4ng V\u0169 \u00c1nh S\u1eafc M\u00e0u"
+    },
     "2871785892": {
         "CHS": "\u9ad8\u5929\u7684\u98ce\u4e4b\u4e3b\u6c99",
         "CHT": "\u9ad8\u5929\u7684\u98a8\u4e4b\u4e3b\u6c99",
         "DE": "Sand der himmlischen Winde",
         "EN": "Lord of Wind over Firmament's Hourglass",
         "ES": "Arena del Se\u00f1or de los Vientos Celestiales",
         "FR": "Sable des Vents c\u00e9lestes",
@@ -32907,14 +33264,31 @@
         "KR": "\ud559\uc0ac\uc758 \uae43\ud39c",
         "PT": "Caneta de Pena de Estudioso",
         "RU": "\u041f\u0435\u0440\u043e \u0443\u0447\u0451\u043d\u043e\u0433\u043e",
         "TH": "Scholar's Quill Pen",
         "TR": "Alimin T\u00fcy Kalemi",
         "VI": "B\u00fat L\u00f4ng H\u1ecdc S\u0129"
     },
+    "300735980": {
+        "CHS": "\u574f\u5deb\u5e08\u7684\u7fbd\u6756",
+        "CHT": "\u58de\u5deb\u5e2b\u7684\u7fbd\u6756",
+        "DE": "Feder des b\u00f6sen Magiers",
+        "EN": "Wicked Mage's Plumule",
+        "ES": "Pluma del Brujo Mal\u00e9fico",
+        "FR": "Plumule de mage malsain",
+        "ID": "Wicked Mage's Plumule",
+        "IT": "Plumula del mago perfido",
+        "JP": "\u60aa\u3057\u304d\u9b54\u6cd5\u4f7f\u3044\u306e\u7fbd\u6756",
+        "KR": "\ub098\uc05c \ub9c8\ubc95\uc0ac\uc758 \uae43\ud138 \uc9c0\ud321\uc774",
+        "PT": "Pluma do Feiticeiro Mal\u00e9fico",
+        "RU": "\u041f\u0435\u0440\u043e \u0437\u043b\u043e\u0433\u043e \u043c\u0430\u0433\u0430",
+        "TH": "Wicked Mage's Plumule",
+        "TR": "Zalim B\u00fcy\u00fcc\u00fcn\u00fcn T\u00fcy\u00fc",
+        "VI": "L\u00f4ng T\u01a1 \u00c1c Ph\u00f9 Th\u1ee7y"
+    },
     "3007893084": {
         "CHS": "\u6b66\u4eba\u7684\u5934\u5dfe",
         "CHT": "\u6b66\u4eba\u7684\u982d\u5dfe",
         "DE": "Kampfk\u00fcnstler-Kopftuch",
         "EN": "Martial Artist's Bandana",
         "ES": "Bandana del Artista Marcial",
         "FR": "Bandeau de l'Artiste martial",
@@ -33434,14 +33808,31 @@
         "KR": "\ud5d8\ud55c \uc0b0\ubd09\uc6b0\ub9ac\uc758 \ub0a0\uac1c",
         "PT": "Asas do Pico da Montanha",
         "RU": "\u041f\u0435\u0440\u043e \u0437\u0443\u0431\u0447\u0430\u0442\u044b\u0445 \u043f\u0438\u043a\u043e\u0432",
         "TH": "Feather of Jagged Peaks",
         "TR": "Sarp Zirve T\u00fcy\u00fc",
         "VI": "C\u00e1nh Th\u00e1i S\u01a1n"
     },
+    "3044050628": {
+        "CHS": "\u65c5\u9014\u4e2d\u7684\u9c9c\u82b1",
+        "CHT": "\u65c5\u9014\u4e2d\u7684\u9bae\u82b1",
+        "DE": "Blume auf der Reise",
+        "EN": "Odyssean Flower",
+        "ES": "Flor del Periplo",
+        "FR": "Fleur odyss\u00e9enne",
+        "ID": "Odyssean Flower",
+        "IT": "Fiore odisseico",
+        "JP": "\u65c5\u4e2d\u306e\u82b1",
+        "KR": "\uc5ec\uc815 \uc911\uc758 \uaf43",
+        "PT": "Flor da Jornada",
+        "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0441\u0442\u0440\u0430\u043d\u0441\u0442\u0432\u0438\u0439",
+        "TH": "Odyssean Flower",
+        "TR": "Yolculuk \u00c7i\u00e7e\u011fi",
+        "VI": "Hoa T\u01b0\u01a1i Tr\u00ean L\u1eef Tr\u00ecnh"
+    },
     "304581284": {
         "CHS": "\u660e\u5a01\u4e4b\u9561",
         "CHT": "\u660e\u5a01\u4e4b\u9414",
         "DE": "Prunkvolles Stichblatt",
         "EN": "Magnificent Tsuba",
         "ES": "Guardamano del Honor",
         "FR": "Tsuba magnifique",
@@ -36868,14 +37259,31 @@
         "KR": "\ud654\ub824\ud55c \ud22c\uad6c",
         "PT": "Capacete Ornamentado",
         "RU": "\u0423\u043a\u0440\u0430\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u0430\u0431\u0443\u0442\u043e",
         "TH": "Ornate Kabuto",
         "TR": "\u0130\u015flemeli Kabuto",
         "VI": "N\u00f3n Hoa M\u1ef9"
     },
+    "3259345068": {
+        "CHS": "\u7075\u5149\u660e\u70c1\u4e4b\u5fc3",
+        "CHT": "\u9748\u5149\u660e\u720d\u4e4b\u5fc3",
+        "DE": "Herz khvarenaischer Brillianz",
+        "EN": "Heart of Khvarena's Brilliance",
+        "ES": "Coraz\u00f3n Refulgente de la Jvarena",
+        "FR": "C\u0153ur de la brillance de la khvarena",
+        "ID": "Heart of Khvarena's Brilliance",
+        "IT": "Fulgore del Cuore di Khvarena",
+        "JP": "\u970a\u5149\u660e\u6ec5\u306e\u5fc3",
+        "KR": "\ud06c\ubc14\ub808\ub098\uc758 \ub208\ubd80\uc2e0 \uc2ec\uc7a5",
+        "PT": "Cora\u00e7\u00e3o do Brilho de Khvarena",
+        "RU": "\u0421\u0435\u0440\u0434\u0446\u0435 \u0441\u0432\u0435\u0442\u043e\u0437\u0430\u0440\u043d\u043e\u0441\u0442\u0438 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Heart of Khvarena's Brilliance",
+        "TR": "Khvarena'n\u0131n \u0130hti\u015fam\u0131n\u0131n Kalbi",
+        "VI": "Tr\u00e1i Tim Khvarena Huy Ho\u00e0ng"
+    },
     "3260967780": {
         "CHS": "\u5f02\u56fd\u4e4b\u76cf",
         "CHT": "\u7570\u570b\u4e4b\u76de",
         "DE": "Kelch der Fremde",
         "EN": "Goblet of the Sojourner",
         "ES": "C\u00e1liz Extranjero",
         "FR": "Calice du Voyageur",
@@ -37650,14 +38058,31 @@
         "KR": "\uc804\ud22c\uad11\uc758 \ud574\uace8\uc794",
         "PT": "Ta\u00e7a de Ossos de Berserker",
         "RU": "\u041a\u043e\u0441\u0442\u044f\u043d\u043e\u0439 \u043a\u0443\u0431\u043e\u043a \u0431\u0435\u0440\u0441\u0435\u0440\u043a\u0430",
         "TH": "Berserker's Bone Goblet",
         "TR": "Vah\u015fi Sava\u015f\u00e7\u0131 Kemik Kadehi",
         "VI": "Ly X\u01b0\u01a1ng Cu\u1ed3ng Chi\u1ebfn"
     },
+    "331647924": {
+        "CHS": "\u7075\u5149\u660e\u70c1\u4e4b\u5fc3",
+        "CHT": "\u9748\u5149\u660e\u720d\u4e4b\u5fc3",
+        "DE": "Herz khvarenaischer Brillianz",
+        "EN": "Heart of Khvarena's Brilliance",
+        "ES": "Coraz\u00f3n Refulgente de la Jvarena",
+        "FR": "C\u0153ur de la brillance de la khvarena",
+        "ID": "Heart of Khvarena's Brilliance",
+        "IT": "Fulgore del Cuore di Khvarena",
+        "JP": "\u970a\u5149\u660e\u6ec5\u306e\u5fc3",
+        "KR": "\ud06c\ubc14\ub808\ub098\uc758 \ub208\ubd80\uc2e0 \uc2ec\uc7a5",
+        "PT": "Cora\u00e7\u00e3o do Brilho de Khvarena",
+        "RU": "\u0421\u0435\u0440\u0434\u0446\u0435 \u0441\u0432\u0435\u0442\u043e\u0437\u0430\u0440\u043d\u043e\u0441\u0442\u0438 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Heart of Khvarena's Brilliance",
+        "TR": "Khvarena'n\u0131n \u0130hti\u015fam\u0131n\u0131n Kalbi",
+        "VI": "Tr\u00e1i Tim Khvarena Huy Ho\u00e0ng"
+    },
     "3317425324": {
         "CHS": "\u89d2\u6597\u58eb\u7684\u5e0c\u5180",
         "CHT": "\u89d2\u9b25\u58eb\u7684\u5e0c\u5180",
         "DE": "Zuversicht des Gladiators",
         "EN": "Gladiator's Longing",
         "ES": "Esperanza del Gladiador",
         "FR": "Espoir du Gladiateur",
@@ -39520,14 +39945,31 @@
         "KR": "\ucd95\uc0ac\uc758 \uc99d\uba85",
         "PT": "S\u00edmbolo da Oferenda",
         "RU": "\u0421\u0438\u043c\u0432\u043e\u043b \u043f\u043e\u0434\u043d\u043e\u0448\u0435\u043d\u0438\u044f",
         "TH": "Symbol of Feliciation",
         "TR": "Ayin Simgesi",
         "VI": "Ch\u1ee9ng Nh\u1eadn T\u00e1n D\u01b0\u01a1ng"
     },
+    "3429117468": {
+        "CHS": "\u52c7\u8005\u4eec\u7684\u8336\u4f1a",
+        "CHT": "\u52c7\u8005\u5011\u7684\u8336\u6703",
+        "DE": "Teegesellschaft der Tapferen",
+        "EN": "Heroes' Tea Party",
+        "ES": "Fiesta del T\u00e9 de la Valent\u00eda",
+        "FR": "Go\u00fbter des h\u00e9ros",
+        "ID": "Heroes' Tea Party",
+        "IT": "Un t\u00e8 con gli eroi",
+        "JP": "\u52c7\u8005\u305f\u3061\u306e\u304a\u8336\u4f1a",
+        "KR": "\uc6a9\uc790\ub4e4\uc758 \ud2f0\ud0c0\uc784",
+        "PT": "Festa de Ch\u00e1 dos Her\u00f3is",
+        "RU": "\u0427\u0430\u0435\u043f\u0438\u0442\u0438\u0435 \u0433\u0435\u0440\u043e\u0435\u0432",
+        "TH": "Heroes' Tea Party",
+        "TR": "Kahramanlar\u0131n \u00c7ay Partisi",
+        "VI": "Ti\u1ec7c Tr\u00e0 C\u00e1c D\u0169ng S\u0129"
+    },
     "3429892020": {
         "CHS": "\u9152\u6e0d\u8239\u5e3d",
         "CHT": "\u9152\u6f2c\u8239\u5e3d",
         "DE": "Weinverschmierte Kapit\u00e4nsm\u00fctze",
         "EN": "Wine-Stained Tricorne",
         "ES": "Gorro de Capit\u00e1n Manchado de Vino",
         "FR": "Calot tach\u00e9 de vin",
@@ -41016,14 +41458,31 @@
         "KR": "\uac80\ud22c\uc0ac\uc758 \ud76c\ub9dd",
         "PT": "Esperan\u00e7a do Gladiador",
         "RU": "\u0421\u0442\u0440\u0435\u043c\u043b\u0435\u043d\u0438\u0435 \u0433\u043b\u0430\u0434\u0438\u0430\u0442\u043e\u0440\u0430",
         "TH": "Gladiator's Longing",
         "TR": "Gladyat\u00f6r\u00fcn \u00d6zlemi",
         "VI": "Hy V\u1ecdng C\u1ee7a Gi\u00e1c \u0110\u1ea5u S\u0129"
     },
+    "3506136420": {
+        "CHS": "\u6076\u9f99\u7684\u5355\u7247\u955c",
+        "CHT": "\u60e1\u9f8d\u7684\u55ae\u7247\u93e1",
+        "DE": "Monokel des b\u00f6sen Drachen",
+        "EN": "Fell Dragon's Monocle",
+        "ES": "Mon\u00f3culo del Drag\u00f3n Protervo",
+        "FR": "Monocle de dragon d\u00e9moniaque",
+        "ID": "Fell Dragon's Monocle",
+        "IT": "Monocolo del drago caduto",
+        "JP": "\u60aa\u9f8d\u306e\u7247\u773c\u93e1",
+        "KR": "\uc545\ub8e1\uc758 \ub2e8\uc548\uacbd",
+        "PT": "Mon\u00f3culo do Drag\u00e3o Maligno",
+        "RU": "\u041c\u043e\u043d\u043e\u043a\u043b\u044c \u0441\u0432\u0438\u0440\u0435\u043f\u043e\u0433\u043e \u0434\u0440\u0430\u043a\u043e\u043d\u0430",
+        "TH": "Fell Dragon's Monocle",
+        "TR": "U\u011fursuz Ejderin G\u00f6zl\u00fc\u011f\u00fc",
+        "VI": "K\u00ednh M\u1eaft C\u1ee7a \u00c1c Long"
+    },
     "3506972524": {
         "CHS": "\u6d41\u653e\u8005\u5934\u51a0",
         "CHT": "\u6d41\u653e\u8005\u982d\u51a0",
         "DE": "Haarreif des Verbannten",
         "EN": "Exile's Circlet",
         "ES": "Diadema del Exiliado",
         "FR": "Diad\u00e8me de l'Exil\u00e9",
@@ -41203,14 +41662,31 @@
         "KR": "\ubb34\uc778\uc758 \ubd89\uc740 \uaf43",
         "PT": "Flor Vermelha de Artista Marcial",
         "RU": "\u0410\u043b\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a \u0432\u043e\u0438\u043d\u0430",
         "TH": "Martial Artist's Red Flower",
         "TR": "D\u00f6v\u00fc\u015f Ustas\u0131n\u0131n K\u0131rm\u0131z\u0131 \u00c7i\u00e7e\u011fi",
         "VI": "Hoa V\u00f5 Nh\u00e2n"
     },
+    "3516718308": {
+        "CHS": "\u7075\u5149\u660e\u70c1\u4e4b\u5fc3",
+        "CHT": "\u9748\u5149\u660e\u720d\u4e4b\u5fc3",
+        "DE": "Herz khvarenaischer Brillianz",
+        "EN": "Heart of Khvarena's Brilliance",
+        "ES": "Coraz\u00f3n Refulgente de la Jvarena",
+        "FR": "C\u0153ur de la brillance de la khvarena",
+        "ID": "Heart of Khvarena's Brilliance",
+        "IT": "Fulgore del Cuore di Khvarena",
+        "JP": "\u970a\u5149\u660e\u6ec5\u306e\u5fc3",
+        "KR": "\ud06c\ubc14\ub808\ub098\uc758 \ub208\ubd80\uc2e0 \uc2ec\uc7a5",
+        "PT": "Cora\u00e7\u00e3o do Brilho de Khvarena",
+        "RU": "\u0421\u0435\u0440\u0434\u0446\u0435 \u0441\u0432\u0435\u0442\u043e\u0437\u0430\u0440\u043d\u043e\u0441\u0442\u0438 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Heart of Khvarena's Brilliance",
+        "TR": "Khvarena'n\u0131n \u0130hti\u015fam\u0131n\u0131n Kalbi",
+        "VI": "Tr\u00e1i Tim Khvarena Huy Ho\u00e0ng"
+    },
     "3516962580": {
         "CHS": "\u6e21\u706b\u8005\u7684\u714e\u71ac",
         "CHT": "\u6e21\u706b\u8005\u7684\u714e\u71ac",
         "DE": "M\u00fchsal des Laval\u00e4ufers",
         "EN": "Lavawalker's Torment",
         "ES": "Tormento del Corredor de Lava",
         "FR": "Tourment du Marcheur du feu",
@@ -41781,14 +42257,31 @@
         "KR": "\uc81c\ub8b0\uc758 \uad00",
         "PT": "Coroa do Ritual Electro",
         "RU": "\u0422\u0438\u0430\u0440\u0430 \u0433\u0440\u043e\u043c\u0430",
         "TH": "Tiara of Thunder",
         "TR": "Y\u0131ld\u0131r\u0131m Tac\u0131",
         "VI": "N\u00f3n T\u1ebf L\u00f4i"
     },
+    "3545354476": {
+        "CHS": "\u7426\u8272\u7075\u5f69\u4e4b\u7fbd",
+        "CHT": "\u7426\u8272\u9748\u5f69\u4e4b\u7fbd",
+        "DE": "Bezaubernde Feder",
+        "EN": "Vibrant Pinion",
+        "ES": "Pluma Crom\u00e1tica",
+        "FR": "Penne vibrante",
+        "ID": "Vibrant Pinion",
+        "IT": "Penna dalle tinte vivaci",
+        "JP": "\u970a\u5f69\u5947\u9e97\u306e\u7fbd",
+        "KR": "\uc601\ub871\ud55c \uc625\ube5b \uae43\ud138",
+        "PT": "Pluma do Cristal Reluzente",
+        "RU": "\u0421\u0430\u043c\u043e\u0446\u0432\u0435\u0442\u043d\u043e\u0435 \u043f\u0435\u0440\u043e",
+        "TH": "Vibrant Pinion",
+        "TR": "Alacal\u0131 T\u00fcy",
+        "VI": "L\u00f4ng V\u0169 \u00c1nh S\u1eafc M\u00e0u"
+    },
     "354590484": {
         "CHS": "\u6218\u72c2\u7684\u9b3c\u9762",
         "CHT": "\u6230\u72c2\u7684\u9b3c\u9762",
         "DE": "Furchteinfl\u00f6\u00dfende Berserkermaske",
         "EN": "Berserker's Battle Mask",
         "ES": "M\u00e1scara de Batalla del Berserker",
         "FR": "Masque du Berserker",
@@ -42869,14 +43362,31 @@
         "KR": "\uc720\ubc30\uc790\uc758 \uc794",
         "PT": "C\u00e1lice do Exilado",
         "RU": "\u041a\u0443\u0431\u043e\u043a \u0438\u0437\u0433\u043d\u0430\u043d\u043d\u0438\u043a\u0430",
         "TH": "Exile's Goblet",
         "TR": "S\u00fcrg\u00fcn\u00fcn Kadehi",
         "VI": "Ly K\u1ebb L\u01b0u \u0110\u00e0y"
     },
+    "3623460348": {
+        "CHS": "\u52c7\u8005\u4eec\u7684\u8336\u4f1a",
+        "CHT": "\u52c7\u8005\u5011\u7684\u8336\u6703",
+        "DE": "Teegesellschaft der Tapferen",
+        "EN": "Heroes' Tea Party",
+        "ES": "Fiesta del T\u00e9 de la Valent\u00eda",
+        "FR": "Go\u00fbter des h\u00e9ros",
+        "ID": "Heroes' Tea Party",
+        "IT": "Un t\u00e8 con gli eroi",
+        "JP": "\u52c7\u8005\u305f\u3061\u306e\u304a\u8336\u4f1a",
+        "KR": "\uc6a9\uc790\ub4e4\uc758 \ud2f0\ud0c0\uc784",
+        "PT": "Festa de Ch\u00e1 dos Her\u00f3is",
+        "RU": "\u0427\u0430\u0435\u043f\u0438\u0442\u0438\u0435 \u0433\u0435\u0440\u043e\u0435\u0432",
+        "TH": "Heroes' Tea Party",
+        "TR": "Kahramanlar\u0131n \u00c7ay Partisi",
+        "VI": "Ti\u1ec7c Tr\u00e0 C\u00e1c D\u0169ng S\u0129"
+    },
     "3625596140": {
         "CHS": "\u67d3\u8840\u7684\u94c1\u5047\u9762",
         "CHT": "\u67d3\u8840\u7684\u9435\u5047\u9762",
         "DE": "Eisenmaske des Blutbefleckten",
         "EN": "Bloodstained Iron Mask",
         "ES": "M\u00e1scara de Hierro Sanguinaria",
         "FR": "Masque de fer ensanglant\u00e9",
@@ -45334,14 +45844,31 @@
         "KR": "\uc9c4\uc8fc\uc758 \uc694\ub78c",
         "PT": "Jaula de P\u00e9rola",
         "RU": "\u0416\u0435\u043c\u0447\u0443\u0436\u043d\u0430\u044f \u043a\u043b\u0435\u0442\u043a\u0430",
         "TH": "Pearl Cage",
         "TR": "\u0130nci Kafesi",
         "VI": "L\u1ed3ng Tr\u00e2n Ch\u00e2u"
     },
+    "3785534860": {
+        "CHS": "\u65e0\u8fb9\u9163\u4e50\u4e4b\u7b75",
+        "CHT": "\u7121\u908a\u9163\u6a02\u4e4b\u7b75",
+        "DE": "Festessen der grenzenlosen Freude",
+        "EN": "Feast of Boundless Joy",
+        "ES": "Fest\u00edn del J\u00fabilo Inconmensurable",
+        "FR": "Festin de joie sans bornes",
+        "ID": "Feast of Boundless Joy",
+        "IT": "Banchetto della gioia infinita",
+        "JP": "\u559c\u697d\u7121\u9650\u306e\u5bb4",
+        "KR": "\ub05d\uc5c6\ub294 \ud5a5\ub77d\uc758 \uc5f0\ud68c",
+        "PT": "C\u00e1lice do Festival Alegre",
+        "RU": "\u041f\u0438\u0440 \u043d\u0435\u043e\u0431\u0443\u0437\u0434\u0430\u043d\u043d\u043e\u0433\u043e \u0432\u0435\u0441\u0435\u043b\u044c\u044f",
+        "TH": "Feast of Boundless Joy",
+        "TR": "Sonsuz Sevin\u00e7 \u015eenli\u011fi",
+        "VI": "B\u1eefa Ti\u1ec7c Vui V\u00f4 B\u1edd"
+    },
     "3786003004": {
         "CHS": "\u52c7\u58eb\u7684\u575a\u6bc5",
         "CHT": "\u52c7\u58eb\u7684\u5805\u6bc5",
         "DE": "Entschlossenheit des Recken",
         "EN": "Fortitude of the Brave",
         "ES": "Determinaci\u00f3n del Guerrero",
         "FR": "Pers\u00e9v\u00e9rance du Brave",
@@ -45674,14 +46201,31 @@
         "KR": "\uc81c\uc218\uc758 \uad00",
         "PT": "Coroa do Ritual Hydro",
         "RU": "\u0422\u0438\u0430\u0440\u0430 \u0432\u043e\u0434\u044b",
         "TH": "Tiara of Torrents",
         "TR": "Sa\u011fanak Tac\u0131",
         "VI": "N\u00f3n T\u1ebf Th\u1ee7y"
     },
+    "380912396": {
+        "CHS": "\u65e0\u8fb9\u9163\u4e50\u4e4b\u7b75",
+        "CHT": "\u7121\u908a\u9163\u6a02\u4e4b\u7b75",
+        "DE": "Festessen der grenzenlosen Freude",
+        "EN": "Feast of Boundless Joy",
+        "ES": "Fest\u00edn del J\u00fabilo Inconmensurable",
+        "FR": "Festin de joie sans bornes",
+        "ID": "Feast of Boundless Joy",
+        "IT": "Banchetto della gioia infinita",
+        "JP": "\u559c\u697d\u7121\u9650\u306e\u5bb4",
+        "KR": "\ub05d\uc5c6\ub294 \ud5a5\ub77d\uc758 \uc5f0\ud68c",
+        "PT": "C\u00e1lice do Festival Alegre",
+        "RU": "\u041f\u0438\u0440 \u043d\u0435\u043e\u0431\u0443\u0437\u0434\u0430\u043d\u043d\u043e\u0433\u043e \u0432\u0435\u0441\u0435\u043b\u044c\u044f",
+        "TH": "Feast of Boundless Joy",
+        "TR": "Sonsuz Sevin\u00e7 \u015eenli\u011fi",
+        "VI": "B\u1eefa Ti\u1ec7c Vui V\u00f4 B\u1edd"
+    },
     "3809216908": {
         "CHS": "\u6b66\u4eba\u7684\u6c34\u6f0f",
         "CHT": "\u6b66\u4eba\u7684\u6c34\u6f0f",
         "DE": "Kampfk\u00fcnstler-Wasseruhr",
         "EN": "Martial Artist's Water Hourglass",
         "ES": "Reloj de Agua del Artista Marcial",
         "FR": "Sablier d'eau de l'Artiste martial",
@@ -46252,14 +46796,31 @@
         "KR": "\uc720\ubc30\uc790\uc758 \uba38\ub9ac\uc7a5\uc2dd",
         "PT": "Grinalda do Exilado",
         "RU": "\u041a\u043e\u0440\u043e\u043d\u0430 \u0438\u0437\u0433\u043d\u0430\u043d\u043d\u0438\u043a\u0430",
         "TH": "Exile's Circlet",
         "TR": "S\u00fcrg\u00fcn\u00fcn Tac\u0131",
         "VI": "V\u01b0\u01a1ng Mi\u1ec7n K\u1ebb L\u01b0u \u0110\u00e0y"
     },
+    "384586580": {
+        "CHS": "\u6c34\u4ed9\u7684\u65f6\u65f6\u523b\u523b",
+        "CHT": "\u6c34\u4ed9\u7684\u6642\u6642\u523b\u523b",
+        "DE": "Best\u00e4ndigkeit der Narzisse",
+        "EN": "Nymph's Constancy",
+        "ES": "Asiduidad de las Ninfas",
+        "FR": "Constance de la nymphe",
+        "ID": "Nymph's Constancy",
+        "IT": "Fedelt\u00e0 della ninfa",
+        "JP": "\u6c34\u4ed9\u306e\u4e00\u77ac\u4e00\u77ac",
+        "KR": "\ub2d8\ud504\uc758 \uc2dc\uc2dc\uac01\uac01",
+        "PT": "Ninfas Eternas",
+        "RU": "\u041f\u043e\u0441\u0442\u043e\u044f\u043d\u0441\u0442\u0432\u043e \u043d\u0438\u043c\u0444\u044b",
+        "TH": "Nymph's Constancy",
+        "TR": "Nergisin Daimiyeti",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a Th\u1ee7y Ti\u00ean"
+    },
     "3846460172": {
         "CHS": "\u96f7\u4e91\u4e4b\u7b3c",
         "CHT": "\u96f7\u96f2\u4e4b\u7c60",
         "DE": "Blitzwolkenk\u00e4fig",
         "EN": "Storm Cage",
         "ES": "Inrou de la Tempestad",
         "FR": "Inro de la temp\u00eate",
@@ -47034,14 +47595,31 @@
         "KR": "\uc18c\ubb34\uc758 \uae43\ud138",
         "PT": "Pena Brilhante Marcial",
         "RU": "\u0411\u043e\u0435\u0432\u043e\u0435 \u043f\u0435\u0440\u043e \u043a\u043e\u043c\u0430\u043d\u0434\u0438\u0440\u0430",
         "TH": "Ceremonial War-Plume",
         "TR": "Merasim Sava\u015f T\u00fcy\u00fc",
         "VI": "Chi\u00eau V\u00f5 Linh V\u0169"
     },
+    "3883964132": {
+        "CHS": "\u7075\u5149\u6e90\u8d77\u4e4b\u854a",
+        "CHT": "\u9748\u5149\u6e90\u8d77\u4e4b\u854a",
+        "DE": "Staubblatt Khvarenas Herkunft",
+        "EN": "Stamen of Khvarena's Origin",
+        "ES": "Estambre Primordial de la Jvarena",
+        "FR": "\u00c9tamine de l'origine de la khvarena",
+        "ID": "Stamen of Khvarena's Origin",
+        "IT": "Stame della Genesi di Khvarena",
+        "JP": "\u970a\u5149\u8d77\u6e90\u306e\u854a",
+        "KR": "\ud06c\ubc14\ub808\ub098 \uae30\uc6d0\uc758 \uaf43\uc220",
+        "PT": "Estame Primordial de Khvarena",
+        "RU": "\u0422\u044b\u0447\u0438\u043d\u043a\u0430 \u0438\u0441\u0442\u043e\u043a\u0430 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Stamen of Khvarena's Origin",
+        "TR": "Khvarena'n\u0131n K\u00f6keninin Tomurcu\u011fu",
+        "VI": "Nh\u1ee5y Hoa Khvarena Kh\u1edfi Nguy\u00ean"
+    },
     "3884482180": {
         "CHS": "\u5b88\u62a4\u5ea7\u949f",
         "CHT": "\u5b88\u8b77\u5ea7\u9418",
         "DE": "W\u00e4chtertischuhr",
         "EN": "Guardian's Clock",
         "ES": "Reloj del Guardi\u00e1n",
         "FR": "Horloge du Gardien",
@@ -47425,14 +48003,31 @@
         "KR": "\ud589\uc6b4\uc544\uc758 \ubaa8\ub798\uc2dc\uacc4",
         "PT": "Ampulheta do Sortudo",
         "RU": "\u041f\u0435\u0441\u043e\u0447\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u0432\u0435\u0437\u0443\u043d\u0447\u0438\u043a\u0430",
         "TH": "Lucky Dog's Hourglass",
         "TR": "Baht\u0131 A\u00e7\u0131\u011f\u0131n Kum Saati",
         "VI": "\u0110\u1ed3ng H\u1ed3 C\u00e1t May M\u1eafn"
     },
+    "3907730572": {
+        "CHS": "\u574f\u5deb\u5e08\u7684\u7fbd\u6756",
+        "CHT": "\u58de\u5deb\u5e2b\u7684\u7fbd\u6756",
+        "DE": "Feder des b\u00f6sen Magiers",
+        "EN": "Wicked Mage's Plumule",
+        "ES": "Pluma del Brujo Mal\u00e9fico",
+        "FR": "Plumule de mage malsain",
+        "ID": "Wicked Mage's Plumule",
+        "IT": "Plumula del mago perfido",
+        "JP": "\u60aa\u3057\u304d\u9b54\u6cd5\u4f7f\u3044\u306e\u7fbd\u6756",
+        "KR": "\ub098\uc05c \ub9c8\ubc95\uc0ac\uc758 \uae43\ud138 \uc9c0\ud321\uc774",
+        "PT": "Pluma do Feiticeiro Mal\u00e9fico",
+        "RU": "\u041f\u0435\u0440\u043e \u0437\u043b\u043e\u0433\u043e \u043c\u0430\u0433\u0430",
+        "TH": "Wicked Mage's Plumule",
+        "TR": "Zalim B\u00fcy\u00fcc\u00fcn\u00fcn T\u00fcy\u00fc",
+        "VI": "L\u00f4ng T\u01a1 \u00c1c Ph\u00f9 Th\u1ee7y"
+    },
     "3908539236": {
         "CHS": "\u6218\u72c2\u7684\u9b3c\u9762",
         "CHT": "\u6230\u72c2\u7684\u9b3c\u9762",
         "DE": "Furchteinfl\u00f6\u00dfende Berserkermaske",
         "EN": "Berserker's Battle Mask",
         "ES": "M\u00e1scara de Batalla del Berserker",
         "FR": "Masque du Berserker",
@@ -47901,14 +48496,31 @@
         "KR": "\ubaa8\ud5d8\uac00\uc758 \uaf41\uc9c0 \uae43\ud138",
         "PT": "Pena de Cauda de Aventureiro",
         "RU": "\u041f\u0435\u0440\u043e \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044f \u043f\u0440\u0438\u043a\u043b\u044e\u0447\u0435\u043d\u0438\u0439",
         "TH": "Adventurer's Tail Feather",
         "TR": "Macerac\u0131n\u0131n Kuyruk T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 Nh\u00e0 M\u1ea1o Hi\u1ec3m"
     },
+    "3941697284": {
+        "CHS": "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6",
+        "CHT": "\u4e45\u9060\u82b1\u843d\u4e4b\u6642",
+        "DE": "Uralter Abschied",
+        "EN": "Ancient Abscission",
+        "ES": "Marchitamiento de Anta\u00f1o",
+        "FR": "Abscission ancienne",
+        "ID": "Ancient Abscission",
+        "IT": "Escissione ancestrale",
+        "JP": "\u4e45\u9060\u843d\u82b1\u306e\u6642",
+        "KR": "\uba3c \uc61b\ub0a0 \uaf43\uc774 \uc9c8 \ubb34\ub835",
+        "PT": "Abscis\u00e3o Antiga",
+        "RU": "\u0414\u0440\u0435\u0432\u043d\u0435\u0435 \u0443\u0432\u044f\u0434\u0430\u043d\u0438\u0435",
+        "TH": "Ancient Abscission",
+        "TR": "Ge\u00e7mi\u015fin Yaprak D\u00f6k\u00fcmleri",
+        "VI": "Th\u1eddi Kh\u1eafc X\u01b0a C\u1ed5"
+    },
     "3941984964": {
         "CHS": "\u89d2\u6597\u58eb\u7684\u5e0c\u5180",
         "CHT": "\u89d2\u9b25\u58eb\u7684\u5e0c\u5180",
         "DE": "Zuversicht des Gladiators",
         "EN": "Gladiator's Longing",
         "ES": "Esperanza del Gladiador",
         "FR": "Espoir du Gladiateur",
@@ -47986,14 +48598,31 @@
         "KR": "\ud589\uc6b4\uc544\uc758 \uc740\uad00",
         "PT": "Grinalda de Prata do Sortudo",
         "RU": "\u0421\u0435\u0440\u0435\u0431\u0440\u044f\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430 \u0432\u0435\u0437\u0443\u043d\u0447\u0438\u043a\u0430",
         "TH": "Lucky Dog's Silver Circlet",
         "TR": "Baht\u0131 A\u00e7\u0131\u011f\u0131n G\u00fcm\u00fc\u015f Tac\u0131",
         "VI": "V\u00f2ng B\u1ea1c May M\u1eafn"
     },
+    "3947874620": {
+        "CHS": "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6",
+        "CHT": "\u4e45\u9060\u82b1\u843d\u4e4b\u6642",
+        "DE": "Uralter Abschied",
+        "EN": "Ancient Abscission",
+        "ES": "Marchitamiento de Anta\u00f1o",
+        "FR": "Abscission ancienne",
+        "ID": "Ancient Abscission",
+        "IT": "Escissione ancestrale",
+        "JP": "\u4e45\u9060\u843d\u82b1\u306e\u6642",
+        "KR": "\uba3c \uc61b\ub0a0 \uaf43\uc774 \uc9c8 \ubb34\ub835",
+        "PT": "Abscis\u00e3o Antiga",
+        "RU": "\u0414\u0440\u0435\u0432\u043d\u0435\u0435 \u0443\u0432\u044f\u0434\u0430\u043d\u0438\u0435",
+        "TH": "Ancient Abscission",
+        "TR": "Ge\u00e7mi\u015fin Yaprak D\u00f6k\u00fcmleri",
+        "VI": "Th\u1eddi Kh\u1eafc X\u01b0a C\u1ed5"
+    },
     "3949402716": {
         "CHS": "\u7eef\u82b1\u4e4b\u58f6",
         "CHT": "\u7dcb\u82b1\u4e4b\u58fa",
         "DE": "Krug mit dunkelroten Blumen",
         "EN": "Scarlet Vessel",
         "ES": "C\u00e1liz Escarlata",
         "FR": "Gourde pourpre",
@@ -48564,14 +49193,31 @@
         "KR": "\uc625\uc758 \uc78e",
         "PT": "Folha de Jade",
         "RU": "\u041d\u0435\u0444\u0440\u0438\u0442\u043e\u0432\u044b\u0439 \u043b\u0438\u0441\u0442\u043e\u043a",
         "TH": "Jade Leaf",
         "TR": "Ye\u015fim Yaprak",
         "VI": "L\u00e1 B\u00edch Ng\u1ecdc"
     },
+    "3980097148": {
+        "CHS": "\u7075\u5149\u660e\u70c1\u4e4b\u5fc3",
+        "CHT": "\u9748\u5149\u660e\u720d\u4e4b\u5fc3",
+        "DE": "Herz khvarenaischer Brillianz",
+        "EN": "Heart of Khvarena's Brilliance",
+        "ES": "Coraz\u00f3n Refulgente de la Jvarena",
+        "FR": "C\u0153ur de la brillance de la khvarena",
+        "ID": "Heart of Khvarena's Brilliance",
+        "IT": "Fulgore del Cuore di Khvarena",
+        "JP": "\u970a\u5149\u660e\u6ec5\u306e\u5fc3",
+        "KR": "\ud06c\ubc14\ub808\ub098\uc758 \ub208\ubd80\uc2e0 \uc2ec\uc7a5",
+        "PT": "Cora\u00e7\u00e3o do Brilho de Khvarena",
+        "RU": "\u0421\u0435\u0440\u0434\u0446\u0435 \u0441\u0432\u0435\u0442\u043e\u0437\u0430\u0440\u043d\u043e\u0441\u0442\u0438 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Heart of Khvarena's Brilliance",
+        "TR": "Khvarena'n\u0131n \u0130hti\u015fam\u0131n\u0131n Kalbi",
+        "VI": "Tr\u00e1i Tim Khvarena Huy Ho\u00e0ng"
+    },
     "3980175540": {
         "CHS": "\u6d41\u653e\u8005\u5934\u51a0",
         "CHT": "\u6d41\u653e\u8005\u982d\u51a0",
         "DE": "Haarreif des Verbannten",
         "EN": "Exile's Circlet",
         "ES": "Diadema del Exiliado",
         "FR": "Diad\u00e8me de l'Exil\u00e9",
@@ -49057,14 +49703,31 @@
         "KR": "\ubd88\ud0c0\uc624\ub974\ub294 \ub9c8\ub140 \ubaa8\uc790",
         "PT": "Chap\u00e9u Abrasador da Bruxa",
         "RU": "\u0422\u043b\u0435\u044e\u0449\u0430\u044f \u0432\u0435\u0434\u044c\u043c\u0438\u043d\u0430 \u0448\u043b\u044f\u043f\u0430",
         "TH": "Witch's Scorching Hat",
         "TR": "Cad\u0131n\u0131n Yak\u0131c\u0131 \u015eapkas\u0131",
         "VI": "N\u00f3n Ma N\u1eef Lo L\u1eafng"
     },
+    "4012105332": {
+        "CHS": "\u6076\u9f99\u7684\u5355\u7247\u955c",
+        "CHT": "\u60e1\u9f8d\u7684\u55ae\u7247\u93e1",
+        "DE": "Monokel des b\u00f6sen Drachen",
+        "EN": "Fell Dragon's Monocle",
+        "ES": "Mon\u00f3culo del Drag\u00f3n Protervo",
+        "FR": "Monocle de dragon d\u00e9moniaque",
+        "ID": "Fell Dragon's Monocle",
+        "IT": "Monocolo del drago caduto",
+        "JP": "\u60aa\u9f8d\u306e\u7247\u773c\u93e1",
+        "KR": "\uc545\ub8e1\uc758 \ub2e8\uc548\uacbd",
+        "PT": "Mon\u00f3culo do Drag\u00e3o Maligno",
+        "RU": "\u041c\u043e\u043d\u043e\u043a\u043b\u044c \u0441\u0432\u0438\u0440\u0435\u043f\u043e\u0433\u043e \u0434\u0440\u0430\u043a\u043e\u043d\u0430",
+        "TH": "Fell Dragon's Monocle",
+        "TR": "U\u011fursuz Ejderin G\u00f6zl\u00fc\u011f\u00fc",
+        "VI": "K\u00ednh M\u1eaft C\u1ee7a \u00c1c Long"
+    },
     "401341236": {
         "CHS": "\u8fdc\u65b9\u7684\u5c11\u5973\u4e4b\u5fc3",
         "CHT": "\u9060\u65b9\u7684\u5c11\u5973\u4e4b\u5fc3",
         "DE": "Kindlichkeit der Maid",
         "EN": "Maiden's Distant Love",
         "ES": "Coraz\u00f3n Distante de la Doncella",
         "FR": "C\u0153ur lointain de la Demoiselle",
@@ -49601,14 +50264,31 @@
         "KR": "\ub3c4\uae08 \ube0c\ub85c\uce58",
         "PT": "Broche Dourado",
         "RU": "\u041f\u043e\u0437\u043e\u043b\u043e\u0447\u0435\u043d\u043d\u0430\u044f \u0431\u0440\u043e\u0448\u044c",
         "TH": "Gilded Corsage",
         "TR": "Yald\u0131zl\u0131 Bro\u015f",
         "VI": "Hoa C\u00e0i V\u00e0ng"
     },
+    "4050236044": {
+        "CHS": "\u574f\u5deb\u5e08\u7684\u7fbd\u6756",
+        "CHT": "\u58de\u5deb\u5e2b\u7684\u7fbd\u6756",
+        "DE": "Feder des b\u00f6sen Magiers",
+        "EN": "Wicked Mage's Plumule",
+        "ES": "Pluma del Brujo Mal\u00e9fico",
+        "FR": "Plumule de mage malsain",
+        "ID": "Wicked Mage's Plumule",
+        "IT": "Plumula del mago perfido",
+        "JP": "\u60aa\u3057\u304d\u9b54\u6cd5\u4f7f\u3044\u306e\u7fbd\u6756",
+        "KR": "\ub098\uc05c \ub9c8\ubc95\uc0ac\uc758 \uae43\ud138 \uc9c0\ud321\uc774",
+        "PT": "Pluma do Feiticeiro Mal\u00e9fico",
+        "RU": "\u041f\u0435\u0440\u043e \u0437\u043b\u043e\u0433\u043e \u043c\u0430\u0433\u0430",
+        "TH": "Wicked Mage's Plumule",
+        "TR": "Zalim B\u00fcy\u00fcc\u00fcn\u00fcn T\u00fcy\u00fc",
+        "VI": "L\u00f4ng T\u01a1 \u00c1c Ph\u00f9 Th\u1ee7y"
+    },
     "4050689028": {
         "CHS": "\u6d41\u653e\u8005\u4e4b\u7fbd",
         "CHT": "\u6d41\u653e\u8005\u4e4b\u7fbd",
         "DE": "Feder des Verbannten",
         "EN": "Exile's Feather",
         "ES": "Pluma del Exiliado",
         "FR": "Plume de l'Exil\u00e9",
@@ -50706,14 +51386,31 @@
         "KR": "\ud589\uc6b4\uc544\uc758 \ub124 \uc78e \ud074\ub85c\ubc84",
         "PT": "Flor Verde do Sortudo",
         "RU": "\u041a\u043b\u0435\u0432\u0435\u0440 \u0432\u0435\u0437\u0443\u043d\u0447\u0438\u043a\u0430",
         "TH": "Lucky Dog's Clover",
         "TR": "Baht\u0131 A\u00e7\u0131\u011f\u0131n Yoncas\u0131",
         "VI": "Hoa May M\u1eafn"
     },
+    "4114550212": {
+        "CHS": "\u7075\u5149\u660e\u70c1\u4e4b\u5fc3",
+        "CHT": "\u9748\u5149\u660e\u720d\u4e4b\u5fc3",
+        "DE": "Herz khvarenaischer Brillianz",
+        "EN": "Heart of Khvarena's Brilliance",
+        "ES": "Coraz\u00f3n Refulgente de la Jvarena",
+        "FR": "C\u0153ur de la brillance de la khvarena",
+        "ID": "Heart of Khvarena's Brilliance",
+        "IT": "Fulgore del Cuore di Khvarena",
+        "JP": "\u970a\u5149\u660e\u6ec5\u306e\u5fc3",
+        "KR": "\ud06c\ubc14\ub808\ub098\uc758 \ub208\ubd80\uc2e0 \uc2ec\uc7a5",
+        "PT": "Cora\u00e7\u00e3o do Brilho de Khvarena",
+        "RU": "\u0421\u0435\u0440\u0434\u0446\u0435 \u0441\u0432\u0435\u0442\u043e\u0437\u0430\u0440\u043d\u043e\u0441\u0442\u0438 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Heart of Khvarena's Brilliance",
+        "TR": "Khvarena'n\u0131n \u0130hti\u015fam\u0131n\u0131n Kalbi",
+        "VI": "Tr\u00e1i Tim Khvarena Huy Ho\u00e0ng"
+    },
     "4116721580": {
         "CHS": "\u6218\u72c2\u7684\u9aa8\u676f",
         "CHT": "\u6230\u72c2\u7684\u9aa8\u676f",
         "DE": "Berserkertrinkhorn",
         "EN": "Berserker's Bone Goblet",
         "ES": "C\u00e1liz de Hueso del Berserker",
         "FR": "Coupe du Berserker",
@@ -51845,14 +52542,31 @@
         "KR": "\ube59\ud558\uc758 \uc655\uad00",
         "PT": "Coroa Glacial",
         "RU": "\u041a\u043e\u0440\u043e\u043d\u0430 \u043c\u0451\u0440\u0437\u043b\u044b\u0445 \u0440\u0435\u043a",
         "TH": "Crown of Glacier",
         "TR": "Buzul Tac\u0131",
         "VI": "N\u00f3n B\u0103ng Gi\u00e1"
     },
+    "4184215908": {
+        "CHS": "\u65c5\u9014\u4e2d\u7684\u9c9c\u82b1",
+        "CHT": "\u65c5\u9014\u4e2d\u7684\u9bae\u82b1",
+        "DE": "Blume auf der Reise",
+        "EN": "Odyssean Flower",
+        "ES": "Flor del Periplo",
+        "FR": "Fleur odyss\u00e9enne",
+        "ID": "Odyssean Flower",
+        "IT": "Fiore odisseico",
+        "JP": "\u65c5\u4e2d\u306e\u82b1",
+        "KR": "\uc5ec\uc815 \uc911\uc758 \uaf43",
+        "PT": "Flor da Jornada",
+        "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0441\u0442\u0440\u0430\u043d\u0441\u0442\u0432\u0438\u0439",
+        "TH": "Odyssean Flower",
+        "TR": "Yolculuk \u00c7i\u00e7e\u011fi",
+        "VI": "Hoa T\u01b0\u01a1i Tr\u00ean L\u1eef Tr\u00ecnh"
+    },
     "4184793308": {
         "CHS": "\u662d\u6b66\u7fce\u7fbd",
         "CHT": "\u662d\u6b66\u7fce\u7fbd",
         "DE": "Bekundungsfeder",
         "EN": "Ceremonial War-Plume",
         "ES": "Pluma de Guerra Ceremonial",
         "FR": "Plume de guerre du Commandant",
@@ -52083,14 +52797,31 @@
         "KR": "\ucd08\uc6d4\uc758 \uc794",
         "PT": "Ta\u00e7a da Supera\u00e7\u00e3o",
         "RU": "\u041f\u0440\u0435\u0432\u043e\u0441\u0445\u043e\u0434\u044f\u0449\u0430\u044f \u0447\u0430\u0448\u0430",
         "TH": "Surpassing Cup",
         "TR": "\u00dcst\u00fcn Kadeh",
         "VI": "Ly Si\u00eau Vi\u1ec7t"
     },
+    "4194054668": {
+        "CHS": "\u65c5\u9014\u4e2d\u7684\u9c9c\u82b1",
+        "CHT": "\u65c5\u9014\u4e2d\u7684\u9bae\u82b1",
+        "DE": "Blume auf der Reise",
+        "EN": "Odyssean Flower",
+        "ES": "Flor del Periplo",
+        "FR": "Fleur odyss\u00e9enne",
+        "ID": "Odyssean Flower",
+        "IT": "Fiore odisseico",
+        "JP": "\u65c5\u4e2d\u306e\u82b1",
+        "KR": "\uc5ec\uc815 \uc911\uc758 \uaf43",
+        "PT": "Flor da Jornada",
+        "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0441\u0442\u0440\u0430\u043d\u0441\u0442\u0432\u0438\u0439",
+        "TH": "Odyssean Flower",
+        "TR": "Yolculuk \u00c7i\u00e7e\u011fi",
+        "VI": "Hoa T\u01b0\u01a1i Tr\u00ean L\u1eef Tr\u00ecnh"
+    },
     "4195498252": {
         "CHS": "\u6559\u5b98\u7684\u6000\u8868",
         "CHT": "\u6559\u5b98\u7684\u61f7\u9336",
         "DE": "Ausbilderstoppuhr",
         "EN": "Instructor's Pocket Watch",
         "ES": "Reloj de Bolsillo del Instructor",
         "FR": "Montre de poche de l'Instructeur",
@@ -53579,14 +54310,31 @@
         "KR": "\uc720\ubc30\uc790\uc758 \uae43\ud138",
         "PT": "Pena do Exilado",
         "RU": "\u041f\u0435\u0440\u043e \u0438\u0437\u0433\u043d\u0430\u043d\u043d\u0438\u043a\u0430",
         "TH": "Exile's Feather",
         "TR": "S\u00fcrg\u00fcn\u00fcn T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 K\u1ebb L\u01b0u \u0110\u00e0y"
     },
+    "4276188444": {
+        "CHS": "\u65c5\u9014\u4e2d\u7684\u9c9c\u82b1",
+        "CHT": "\u65c5\u9014\u4e2d\u7684\u9bae\u82b1",
+        "DE": "Blume auf der Reise",
+        "EN": "Odyssean Flower",
+        "ES": "Flor del Periplo",
+        "FR": "Fleur odyss\u00e9enne",
+        "ID": "Odyssean Flower",
+        "IT": "Fiore odisseico",
+        "JP": "\u65c5\u4e2d\u306e\u82b1",
+        "KR": "\uc5ec\uc815 \uc911\uc758 \uaf43",
+        "PT": "Flor da Jornada",
+        "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0441\u0442\u0440\u0430\u043d\u0441\u0442\u0432\u0438\u0439",
+        "TH": "Odyssean Flower",
+        "TR": "Yolculuk \u00c7i\u00e7e\u011fi",
+        "VI": "Hoa T\u01b0\u01a1i Tr\u00ean L\u1eef Tr\u00ecnh"
+    },
     "4277189252": {
         "CHS": "\u662d\u6b66\u7fce\u7fbd",
         "CHT": "\u662d\u6b66\u7fce\u7fbd",
         "DE": "Bekundungsfeder",
         "EN": "Ceremonial War-Plume",
         "ES": "Pluma de Guerra Ceremonial",
         "FR": "Plume de guerre du Commandant",
@@ -53885,14 +54633,31 @@
         "KR": "\ud589\uc6b4\uc544\uc758 \uc740\uad00",
         "PT": "Grinalda de Prata do Sortudo",
         "RU": "\u0421\u0435\u0440\u0435\u0431\u0440\u044f\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430 \u0432\u0435\u0437\u0443\u043d\u0447\u0438\u043a\u0430",
         "TH": "Lucky Dog's Silver Circlet",
         "TR": "Baht\u0131 A\u00e7\u0131\u011f\u0131n G\u00fcm\u00fc\u015f Tac\u0131",
         "VI": "V\u00f2ng B\u1ea1c May M\u1eafn"
     },
+    "433775532": {
+        "CHS": "\u52c7\u8005\u4eec\u7684\u8336\u4f1a",
+        "CHT": "\u52c7\u8005\u5011\u7684\u8336\u6703",
+        "DE": "Teegesellschaft der Tapferen",
+        "EN": "Heroes' Tea Party",
+        "ES": "Fiesta del T\u00e9 de la Valent\u00eda",
+        "FR": "Go\u00fbter des h\u00e9ros",
+        "ID": "Heroes' Tea Party",
+        "IT": "Un t\u00e8 con gli eroi",
+        "JP": "\u52c7\u8005\u305f\u3061\u306e\u304a\u8336\u4f1a",
+        "KR": "\uc6a9\uc790\ub4e4\uc758 \ud2f0\ud0c0\uc784",
+        "PT": "Festa de Ch\u00e1 dos Her\u00f3is",
+        "RU": "\u0427\u0430\u0435\u043f\u0438\u0442\u0438\u0435 \u0433\u0435\u0440\u043e\u0435\u0432",
+        "TH": "Heroes' Tea Party",
+        "TR": "Kahramanlar\u0131n \u00c7ay Partisi",
+        "VI": "Ti\u1ec7c Tr\u00e0 C\u00e1c D\u0169ng S\u0129"
+    },
     "433808380": {
         "CHS": "\u96ea\u85cf\u4e4b\u7fbd",
         "CHT": "\u96ea\u85cf\u4e4b\u7fbd",
         "DE": "Vereiste Feder",
         "EN": "Plume of Snow",
         "ES": "Pluma de Nieve",
         "FR": "Plume de neige",
@@ -54242,14 +55007,31 @@
         "KR": "\uc81c\ud654\uc758 \uad00",
         "PT": "Coroa do Ritual Pyro",
         "RU": "\u0422\u0438\u0430\u0440\u0430 \u043e\u0433\u043d\u044f",
         "TH": "Tiara of Flame",
         "TR": "Alev Tac\u0131",
         "VI": "N\u00f3n T\u1ebf L\u1eeda"
     },
+    "4580908": {
+        "CHS": "\u7075\u5149\u660e\u70c1\u4e4b\u5fc3",
+        "CHT": "\u9748\u5149\u660e\u720d\u4e4b\u5fc3",
+        "DE": "Herz khvarenaischer Brillianz",
+        "EN": "Heart of Khvarena's Brilliance",
+        "ES": "Coraz\u00f3n Refulgente de la Jvarena",
+        "FR": "C\u0153ur de la brillance de la khvarena",
+        "ID": "Heart of Khvarena's Brilliance",
+        "IT": "Fulgore del Cuore di Khvarena",
+        "JP": "\u970a\u5149\u660e\u6ec5\u306e\u5fc3",
+        "KR": "\ud06c\ubc14\ub808\ub098\uc758 \ub208\ubd80\uc2e0 \uc2ec\uc7a5",
+        "PT": "Cora\u00e7\u00e3o do Brilho de Khvarena",
+        "RU": "\u0421\u0435\u0440\u0434\u0446\u0435 \u0441\u0432\u0435\u0442\u043e\u0437\u0430\u0440\u043d\u043e\u0441\u0442\u0438 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Heart of Khvarena's Brilliance",
+        "TR": "Khvarena'n\u0131n \u0130hti\u015fam\u0131n\u0131n Kalbi",
+        "VI": "Tr\u00e1i Tim Khvarena Huy Ho\u00e0ng"
+    },
     "458374260": {
         "CHS": "\u5317\u98ce\u4e4b\u76cf",
         "CHT": "\u5317\u98a8\u4e4b\u76de",
         "DE": "Kelch des Aquilo",
         "EN": "Goblet of Aquilo",
         "ES": "C\u00e1liz de Aquilo",
         "FR": "Coupe aquilon",
@@ -55075,14 +55857,31 @@
         "KR": "\ubaa8\ud5d8\uac00\uc758 \uba38\ub9ac\ub760",
         "PT": "Bandana de Aventureiro",
         "RU": "\u041f\u043e\u0432\u044f\u0437\u043a\u0430 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044f \u043f\u0440\u0438\u043a\u043b\u044e\u0447\u0435\u043d\u0438\u0439",
         "TH": "Adventurer's Bandana",
         "TR": "Macerac\u0131n\u0131n Bandanas\u0131",
         "VI": "Kh\u0103n Nh\u00e0 M\u1ea1o Hi\u1ec3m"
     },
+    "509533780": {
+        "CHS": "\u574f\u5deb\u5e08\u7684\u7fbd\u6756",
+        "CHT": "\u58de\u5deb\u5e2b\u7684\u7fbd\u6756",
+        "DE": "Feder des b\u00f6sen Magiers",
+        "EN": "Wicked Mage's Plumule",
+        "ES": "Pluma del Brujo Mal\u00e9fico",
+        "FR": "Plumule de mage malsain",
+        "ID": "Wicked Mage's Plumule",
+        "IT": "Plumula del mago perfido",
+        "JP": "\u60aa\u3057\u304d\u9b54\u6cd5\u4f7f\u3044\u306e\u7fbd\u6756",
+        "KR": "\ub098\uc05c \ub9c8\ubc95\uc0ac\uc758 \uae43\ud138 \uc9c0\ud321\uc774",
+        "PT": "Pluma do Feiticeiro Mal\u00e9fico",
+        "RU": "\u041f\u0435\u0440\u043e \u0437\u043b\u043e\u0433\u043e \u043c\u0430\u0433\u0430",
+        "TH": "Wicked Mage's Plumule",
+        "TR": "Zalim B\u00fcy\u00fcc\u00fcn\u00fcn T\u00fcy\u00fc",
+        "VI": "L\u00f4ng T\u01a1 \u00c1c Ph\u00f9 Th\u1ee7y"
+    },
     "511805676": {
         "CHS": "\u67d3\u8840\u9a91\u58eb\u4e4b\u676f",
         "CHT": "\u67d3\u8840\u9a0e\u58eb\u4e4b\u676f",
         "DE": "Kelch des Blutbefleckten",
         "EN": "Bloodstained Chevalier's Goblet",
         "ES": "C\u00e1liz del Caballero Sanguinario",
         "FR": "Coupe du chevalier ensanglant\u00e9e",
@@ -56163,14 +56962,31 @@
         "KR": "\ud589\uc6b4\uc544\uc758 \ub124 \uc78e \ud074\ub85c\ubc84",
         "PT": "Flor Verde do Sortudo",
         "RU": "\u041a\u043b\u0435\u0432\u0435\u0440 \u0432\u0435\u0437\u0443\u043d\u0447\u0438\u043a\u0430",
         "TH": "Lucky Dog's Clover",
         "TR": "Baht\u0131 A\u00e7\u0131\u011f\u0131n Yoncas\u0131",
         "VI": "Hoa May M\u1eafn"
     },
+    "569289700": {
+        "CHS": "\u6c34\u4ed9\u7684\u65f6\u65f6\u523b\u523b",
+        "CHT": "\u6c34\u4ed9\u7684\u6642\u6642\u523b\u523b",
+        "DE": "Best\u00e4ndigkeit der Narzisse",
+        "EN": "Nymph's Constancy",
+        "ES": "Asiduidad de las Ninfas",
+        "FR": "Constance de la nymphe",
+        "ID": "Nymph's Constancy",
+        "IT": "Fedelt\u00e0 della ninfa",
+        "JP": "\u6c34\u4ed9\u306e\u4e00\u77ac\u4e00\u77ac",
+        "KR": "\ub2d8\ud504\uc758 \uc2dc\uc2dc\uac01\uac01",
+        "PT": "Ninfas Eternas",
+        "RU": "\u041f\u043e\u0441\u0442\u043e\u044f\u043d\u0441\u0442\u0432\u043e \u043d\u0438\u043c\u0444\u044b",
+        "TH": "Nymph's Constancy",
+        "TR": "Nergisin Daimiyeti",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a Th\u1ee7y Ti\u00ean"
+    },
     "56995820": {
         "CHS": "\u8d1f\u7cbe\u901a",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "\u8d1f\u7cbe\u901a",
@@ -57081,14 +57897,31 @@
         "KR": "\uc218\ud638\uc758 \ud0c1\uc0c1\uc2dc\uacc4",
         "PT": "Rel\u00f3gio do Guarda",
         "RU": "\u0427\u0430\u0441\u044b \u0437\u0430\u0449\u0438\u0442\u043d\u0438\u043a\u0430",
         "TH": "Guardian's Clock",
         "TR": "Muhaf\u0131z Saati",
         "VI": "\u0110\u1ed3ng H\u1ed3 Th\u1ee7 H\u1ed9"
     },
+    "613773908": {
+        "CHS": "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6",
+        "CHT": "\u4e45\u9060\u82b1\u843d\u4e4b\u6642",
+        "DE": "Uralter Abschied",
+        "EN": "Ancient Abscission",
+        "ES": "Marchitamiento de Anta\u00f1o",
+        "FR": "Abscission ancienne",
+        "ID": "Ancient Abscission",
+        "IT": "Escissione ancestrale",
+        "JP": "\u4e45\u9060\u843d\u82b1\u306e\u6642",
+        "KR": "\uba3c \uc61b\ub0a0 \uaf43\uc774 \uc9c8 \ubb34\ub835",
+        "PT": "Abscis\u00e3o Antiga",
+        "RU": "\u0414\u0440\u0435\u0432\u043d\u0435\u0435 \u0443\u0432\u044f\u0434\u0430\u043d\u0438\u0435",
+        "TH": "Ancient Abscission",
+        "TR": "Ge\u00e7mi\u015fin Yaprak D\u00f6k\u00fcmleri",
+        "VI": "Th\u1eddi Kh\u1eafc X\u01b0a C\u1ed5"
+    },
     "613933276": {
         "CHS": "\u662d\u6b66\u7fce\u7fbd",
         "CHT": "\u662d\u6b66\u7fce\u7fbd",
         "DE": "Bekundungsfeder",
         "EN": "Ceremonial War-Plume",
         "ES": "Pluma de Guerra Ceremonial",
         "FR": "Plume de guerre du Commandant",
@@ -57472,14 +58305,31 @@
         "KR": "\uc704\uc554 \ubc18\uc11d\uc758 \uc220\uc794",
         "PT": "Ta\u00e7a do Escultor de Pedra",
         "RU": "\u041a\u0443\u0431\u043e\u043a \u0438\u0437 \u0440\u0435\u0437\u043d\u043e\u0433\u043e \u043a\u0430\u043c\u043d\u044f",
         "TH": "Goblet of Chiseled Crag",
         "TR": "Yal\u00e7\u0131n Kayal\u0131k Kadehi",
         "VI": "Ly Ng\u1ecdc B\u00e0n Th\u1ea1ch"
     },
+    "63248004": {
+        "CHS": "\u6c34\u4ed9\u7684\u65f6\u65f6\u523b\u523b",
+        "CHT": "\u6c34\u4ed9\u7684\u6642\u6642\u523b\u523b",
+        "DE": "Best\u00e4ndigkeit der Narzisse",
+        "EN": "Nymph's Constancy",
+        "ES": "Asiduidad de las Ninfas",
+        "FR": "Constance de la nymphe",
+        "ID": "Nymph's Constancy",
+        "IT": "Fedelt\u00e0 della ninfa",
+        "JP": "\u6c34\u4ed9\u306e\u4e00\u77ac\u4e00\u77ac",
+        "KR": "\ub2d8\ud504\uc758 \uc2dc\uc2dc\uac01\uac01",
+        "PT": "Ninfas Eternas",
+        "RU": "\u041f\u043e\u0441\u0442\u043e\u044f\u043d\u0441\u0442\u0432\u043e \u043d\u0438\u043c\u0444\u044b",
+        "TH": "Nymph's Constancy",
+        "TR": "Nergisin Daimiyeti",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a Th\u1ee7y Ti\u00ean"
+    },
     "633132620": {
         "CHS": "\u6b66\u4eba\u7684\u6c34\u6f0f",
         "CHT": "\u6b66\u4eba\u7684\u6c34\u6f0f",
         "DE": "Kampfk\u00fcnstler-Wasseruhr",
         "EN": "Martial Artist's Water Hourglass",
         "ES": "Reloj de Agua del Artista Marcial",
         "FR": "Sablier d'eau de l'Artiste martial",
@@ -57863,14 +58713,31 @@
         "KR": "\uc804\ud22c\uad11\uc758 \uc7a5\ubbf8",
         "PT": "Rosa de Berserker",
         "RU": "\u0420\u043e\u0437\u0430 \u0431\u0435\u0440\u0441\u0435\u0440\u043a\u0430",
         "TH": "Berserker's Rose",
         "TR": "Vah\u015fi Sava\u015f\u00e7\u0131 G\u00fcl\u00fc",
         "VI": "T\u01b0\u1eddng Vi Cu\u1ed3ng Chi\u1ebfn"
     },
+    "654492908": {
+        "CHS": "\u52c7\u8005\u4eec\u7684\u8336\u4f1a",
+        "CHT": "\u52c7\u8005\u5011\u7684\u8336\u6703",
+        "DE": "Teegesellschaft der Tapferen",
+        "EN": "Heroes' Tea Party",
+        "ES": "Fiesta del T\u00e9 de la Valent\u00eda",
+        "FR": "Go\u00fbter des h\u00e9ros",
+        "ID": "Heroes' Tea Party",
+        "IT": "Un t\u00e8 con gli eroi",
+        "JP": "\u52c7\u8005\u305f\u3061\u306e\u304a\u8336\u4f1a",
+        "KR": "\uc6a9\uc790\ub4e4\uc758 \ud2f0\ud0c0\uc784",
+        "PT": "Festa de Ch\u00e1 dos Her\u00f3is",
+        "RU": "\u0427\u0430\u0435\u043f\u0438\u0442\u0438\u0435 \u0433\u0435\u0440\u043e\u0435\u0432",
+        "TH": "Heroes' Tea Party",
+        "TR": "Kahramanlar\u0131n \u00c7ay Partisi",
+        "VI": "Ti\u1ec7c Tr\u00e0 C\u00e1c D\u0169ng S\u0129"
+    },
     "65507964": {
         "CHS": "\u5947\u8ff9\u8033\u5760",
         "CHT": "\u5947\u8e5f\u8033\u589c",
         "DE": "Wunderohrh\u00e4nger",
         "EN": "Tiny Miracle's Earrings",
         "ES": "Aretes del Milagro",
         "FR": "Boucles d'oreilles du Miracle",
@@ -57914,14 +58781,31 @@
         "KR": "\uc57c\uc0dd\ud654 \uae30\uc5b5 \uc18d\uc758 \ud478\ub978 \ub4e4\ud310",
         "PT": "Lembran\u00e7a de Flores Silvestres",
         "RU": "\u0412\u043e\u0441\u043f\u043e\u043c\u0438\u043d\u0430\u043d\u0438\u044f \u043e\u0431 \u0438\u0437\u0443\u043c\u0440\u0443\u0434\u043d\u044b\u0445 \u043b\u0443\u0433\u0430\u0445",
         "TH": "In Rememberance of Viridescent Field",
         "TR": "Ye\u015fil Tarlalar\u0131n Hat\u0131ras\u0131",
         "VI": "Hoa K\u00fd \u1ee8c \u0110\u1ed3ng Xanh"
     },
+    "657472556": {
+        "CHS": "\u7075\u5149\u6e90\u8d77\u4e4b\u854a",
+        "CHT": "\u9748\u5149\u6e90\u8d77\u4e4b\u854a",
+        "DE": "Staubblatt Khvarenas Herkunft",
+        "EN": "Stamen of Khvarena's Origin",
+        "ES": "Estambre Primordial de la Jvarena",
+        "FR": "\u00c9tamine de l'origine de la khvarena",
+        "ID": "Stamen of Khvarena's Origin",
+        "IT": "Stame della Genesi di Khvarena",
+        "JP": "\u970a\u5149\u8d77\u6e90\u306e\u854a",
+        "KR": "\ud06c\ubc14\ub808\ub098 \uae30\uc6d0\uc758 \uaf43\uc220",
+        "PT": "Estame Primordial de Khvarena",
+        "RU": "\u0422\u044b\u0447\u0438\u043d\u043a\u0430 \u0438\u0441\u0442\u043e\u043a\u0430 \u0425\u0432\u0430\u0440\u043d\u044b",
+        "TH": "Stamen of Khvarena's Origin",
+        "TR": "Khvarena'n\u0131n K\u00f6keninin Tomurcu\u011fu",
+        "VI": "Nh\u1ee5y Hoa Khvarena Kh\u1edfi Nguy\u00ean"
+    },
     "658212884": {
         "CHS": "\u671d\u9732\u4e4b\u65f6",
         "CHT": "\u671d\u9732\u4e4b\u6642",
         "DE": "Augenblick des Morgentaus",
         "EN": "Morning Dew's Moment",
         "ES": "Reloj de la Transitoriedad",
         "FR": "Horloge de l'aube",
@@ -58968,14 +59852,31 @@
         "KR": "\ud589\uc6b4\uc544\uc758 \uc794",
         "PT": "C\u00e1lice do Sortudo",
         "RU": "\u041a\u0443\u0431\u043e\u043a \u0432\u0435\u0437\u0443\u043d\u0447\u0438\u043a\u0430",
         "TH": "Lucky Dog's Goblet",
         "TR": "Baht\u0131 A\u00e7\u0131\u011f\u0131n Kadehi",
         "VI": "Ly May M\u1eafn"
     },
+    "708144612": {
+        "CHS": "\u65e0\u8fb9\u9163\u4e50\u4e4b\u7b75",
+        "CHT": "\u7121\u908a\u9163\u6a02\u4e4b\u7b75",
+        "DE": "Festessen der grenzenlosen Freude",
+        "EN": "Feast of Boundless Joy",
+        "ES": "Fest\u00edn del J\u00fabilo Inconmensurable",
+        "FR": "Festin de joie sans bornes",
+        "ID": "Feast of Boundless Joy",
+        "IT": "Banchetto della gioia infinita",
+        "JP": "\u559c\u697d\u7121\u9650\u306e\u5bb4",
+        "KR": "\ub05d\uc5c6\ub294 \ud5a5\ub77d\uc758 \uc5f0\ud68c",
+        "PT": "C\u00e1lice do Festival Alegre",
+        "RU": "\u041f\u0438\u0440 \u043d\u0435\u043e\u0431\u0443\u0437\u0434\u0430\u043d\u043d\u043e\u0433\u043e \u0432\u0435\u0441\u0435\u043b\u044c\u044f",
+        "TH": "Feast of Boundless Joy",
+        "TR": "Sonsuz Sevin\u00e7 \u015eenli\u011fi",
+        "VI": "B\u1eefa Ti\u1ec7c Vui V\u00f4 B\u1edd"
+    },
     "708364340": {
         "CHS": "\u5b66\u58eb\u7684\u4e66\u7b7e",
         "CHT": "\u5b78\u58eb\u7684\u66f8\u7c64",
         "DE": "Gelehrtenlesezeichen",
         "EN": "Scholar's Bookmark",
         "ES": "Marcap\u00e1ginas de la Erudita",
         "FR": "Marque-page de l'\u00c9rudit",
@@ -59121,14 +60022,31 @@
         "KR": "\ub9c8\ub140\uc758 \ud30c\uba78\uc758 \uc2dc\uac04",
         "PT": "Fim dos Tempos da Bruxa",
         "RU": "\u0412\u0435\u0434\u044c\u043c\u0438\u043d \u043f\u043e\u0441\u043b\u0435\u0434\u043d\u0438\u0439 \u0447\u0430\u0441",
         "TH": "Witch's End Time",
         "TR": "Cad\u0131n\u0131n Kum Saati",
         "VI": "Th\u1eddi Gian Ma N\u1eef B\u00f9ng N\u1ed5"
     },
+    "716215164": {
+        "CHS": "\u574f\u5deb\u5e08\u7684\u7fbd\u6756",
+        "CHT": "\u58de\u5deb\u5e2b\u7684\u7fbd\u6756",
+        "DE": "Feder des b\u00f6sen Magiers",
+        "EN": "Wicked Mage's Plumule",
+        "ES": "Pluma del Brujo Mal\u00e9fico",
+        "FR": "Plumule de mage malsain",
+        "ID": "Wicked Mage's Plumule",
+        "IT": "Plumula del mago perfido",
+        "JP": "\u60aa\u3057\u304d\u9b54\u6cd5\u4f7f\u3044\u306e\u7fbd\u6756",
+        "KR": "\ub098\uc05c \ub9c8\ubc95\uc0ac\uc758 \uae43\ud138 \uc9c0\ud321\uc774",
+        "PT": "Pluma do Feiticeiro Mal\u00e9fico",
+        "RU": "\u041f\u0435\u0440\u043e \u0437\u043b\u043e\u0433\u043e \u043c\u0430\u0433\u0430",
+        "TH": "Wicked Mage's Plumule",
+        "TR": "Zalim B\u00fcy\u00fcc\u00fcn\u00fcn T\u00fcy\u00fc",
+        "VI": "L\u00f4ng T\u01a1 \u00c1c Ph\u00f9 Th\u1ee7y"
+    },
     "717092700": {
         "CHS": "\u8d4c\u5f92\u7684\u7fbd\u9970",
         "CHT": "\u8ced\u5f92\u7684\u7fbd\u98fe",
         "DE": "Gl\u00fccksspiel-Federschmuck",
         "EN": "Gambler's Feather Accessory",
         "ES": "Pluma de la Jugadora",
         "FR": "Plume du Parieur",
@@ -59359,14 +60277,31 @@
         "KR": "\uae30\uc801\uc758 \uc794",
         "PT": "C\u00e1lice do Milagre",
         "RU": "\u0427\u0430\u0448\u043a\u0430 \u043c\u0430\u043b\u0435\u043d\u044c\u043a\u043e\u0433\u043e \u0447\u0443\u0434\u0430",
         "TH": "Tiny Miracle's Goblet",
         "TR": "K\u00fc\u00e7\u00fck Mucizenin Kadehi",
         "VI": "Ly K\u1ef3 T\u00edch"
     },
+    "732107228": {
+        "CHS": "\u7426\u8272\u7075\u5f69\u4e4b\u7fbd",
+        "CHT": "\u7426\u8272\u9748\u5f69\u4e4b\u7fbd",
+        "DE": "Bezaubernde Feder",
+        "EN": "Vibrant Pinion",
+        "ES": "Pluma Crom\u00e1tica",
+        "FR": "Penne vibrante",
+        "ID": "Vibrant Pinion",
+        "IT": "Penna dalle tinte vivaci",
+        "JP": "\u970a\u5f69\u5947\u9e97\u306e\u7fbd",
+        "KR": "\uc601\ub871\ud55c \uc625\ube5b \uae43\ud138",
+        "PT": "Pluma do Cristal Reluzente",
+        "RU": "\u0421\u0430\u043c\u043e\u0446\u0432\u0435\u0442\u043d\u043e\u0435 \u043f\u0435\u0440\u043e",
+        "TH": "Vibrant Pinion",
+        "TR": "Alacal\u0131 T\u00fcy",
+        "VI": "L\u00f4ng V\u0169 \u00c1nh S\u1eafc M\u00e0u"
+    },
     "73409068": {
         "CHS": "\u5b97\u5ba4\u9762\u5177",
         "CHT": "\u5b97\u5ba4\u9762\u5177",
         "DE": "K\u00f6nigliche Maske",
         "EN": "Royal Masque",
         "ES": "M\u00e1scara Real",
         "FR": "Masque du Noble",
@@ -60175,14 +61110,31 @@
         "KR": "\uc18c\ub140\uc758 \uc9e7\uc740 \ud589\ubcf5",
         "PT": "Juventude Passageira da Donzela",
         "RU": "\u0423\u0445\u043e\u0434\u044f\u0449\u0430\u044f \u043c\u043e\u043b\u043e\u0434\u043e\u0441\u0442\u044c \u044e\u043d\u043e\u0439 \u0434\u0435\u0432\u044b",
         "TH": "Maiden's Passing Youth",
         "TR": "Han\u0131m\u0131n Kaybolan Gen\u00e7li\u011fi",
         "VI": "Th\u1eddi Gian Ch\u1edd \u0110\u1ee3i C\u1ee7a Thi\u1ebfu N\u1eef"
     },
+    "773257660": {
+        "CHS": "\u65c5\u9014\u4e2d\u7684\u9c9c\u82b1",
+        "CHT": "\u65c5\u9014\u4e2d\u7684\u9bae\u82b1",
+        "DE": "Blume auf der Reise",
+        "EN": "Odyssean Flower",
+        "ES": "Flor del Periplo",
+        "FR": "Fleur odyss\u00e9enne",
+        "ID": "Odyssean Flower",
+        "IT": "Fiore odisseico",
+        "JP": "\u65c5\u4e2d\u306e\u82b1",
+        "KR": "\uc5ec\uc815 \uc911\uc758 \uaf43",
+        "PT": "Flor da Jornada",
+        "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0441\u0442\u0440\u0430\u043d\u0441\u0442\u0432\u0438\u0439",
+        "TH": "Odyssean Flower",
+        "TR": "Yolculuk \u00c7i\u00e7e\u011fi",
+        "VI": "Hoa T\u01b0\u01a1i Tr\u00ean L\u1eef Tr\u00ecnh"
+    },
     "774066284": {
         "CHS": "\u6d41\u653e\u8005\u5934\u51a0",
         "CHT": "\u6d41\u653e\u8005\u982d\u51a0",
         "DE": "Haarreif des Verbannten",
         "EN": "Exile's Circlet",
         "ES": "Diadema del Exiliado",
         "FR": "Diad\u00e8me de l'Exil\u00e9",
@@ -60787,14 +61739,31 @@
         "KR": "\ubb34\uc778\uc758 \ubb3c\uc2dc\uacc4",
         "PT": "Ampulheta de Artista Marcial",
         "RU": "\u0412\u043e\u0434\u044f\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u0432\u043e\u0438\u043d\u0430",
         "TH": "Martial Artist's Water Hourglass",
         "TR": "D\u00f6v\u00fc\u015f Ustas\u0131n\u0131n Su Saati",
         "VI": "\u0110\u1ed3ng H\u1ed3 N\u01b0\u1edbc V\u00f5 Nh\u00e2n"
     },
+    "808016300": {
+        "CHS": "\u574f\u5deb\u5e08\u7684\u7fbd\u6756",
+        "CHT": "\u58de\u5deb\u5e2b\u7684\u7fbd\u6756",
+        "DE": "Feder des b\u00f6sen Magiers",
+        "EN": "Wicked Mage's Plumule",
+        "ES": "Pluma del Brujo Mal\u00e9fico",
+        "FR": "Plumule de mage malsain",
+        "ID": "Wicked Mage's Plumule",
+        "IT": "Plumula del mago perfido",
+        "JP": "\u60aa\u3057\u304d\u9b54\u6cd5\u4f7f\u3044\u306e\u7fbd\u6756",
+        "KR": "\ub098\uc05c \ub9c8\ubc95\uc0ac\uc758 \uae43\ud138 \uc9c0\ud321\uc774",
+        "PT": "Pluma do Feiticeiro Mal\u00e9fico",
+        "RU": "\u041f\u0435\u0440\u043e \u0437\u043b\u043e\u0433\u043e \u043c\u0430\u0433\u0430",
+        "TH": "Wicked Mage's Plumule",
+        "TR": "Zalim B\u00fcy\u00fcc\u00fcn\u00fcn T\u00fcy\u00fc",
+        "VI": "L\u00f4ng T\u01a1 \u00c1c Ph\u00f9 Th\u1ee7y"
+    },
     "808388524": {
         "CHS": "\u91d1\u94dc\u65f6\u6677",
         "CHT": "\u91d1\u9285\u6642\u6677",
         "DE": "Kupferne Sonnenuhr",
         "EN": "Orichalceous Time-Dial",
         "ES": "Reloj de Sol de Oricalco",
         "FR": "Cadran solaire dor\u00e9",
@@ -61994,14 +62963,31 @@
         "KR": "\uc774\ubcc4\uc758 \ubaa8\uc790",
         "PT": "Coroa da Despedida",
         "RU": "\u0412\u0435\u043d\u043e\u043a \u0440\u0430\u0441\u0441\u0442\u0430\u0432\u0430\u043d\u0438\u044f",
         "TH": "Crown of Parting",
         "TR": "Ayr\u0131l\u0131k Tac\u0131",
         "VI": "Chi\u1ebfc N\u00f3n T\u1eeb Bi\u1ec7t"
     },
+    "884302492": {
+        "CHS": "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6",
+        "CHT": "\u4e45\u9060\u82b1\u843d\u4e4b\u6642",
+        "DE": "Uralter Abschied",
+        "EN": "Ancient Abscission",
+        "ES": "Marchitamiento de Anta\u00f1o",
+        "FR": "Abscission ancienne",
+        "ID": "Ancient Abscission",
+        "IT": "Escissione ancestrale",
+        "JP": "\u4e45\u9060\u843d\u82b1\u306e\u6642",
+        "KR": "\uba3c \uc61b\ub0a0 \uaf43\uc774 \uc9c8 \ubb34\ub835",
+        "PT": "Abscis\u00e3o Antiga",
+        "RU": "\u0414\u0440\u0435\u0432\u043d\u0435\u0435 \u0443\u0432\u044f\u0434\u0430\u043d\u0438\u0435",
+        "TH": "Ancient Abscission",
+        "TR": "Ge\u00e7mi\u015fin Yaprak D\u00f6k\u00fcmleri",
+        "VI": "Th\u1eddi Kh\u1eafc X\u01b0a C\u1ed5"
+    },
     "885000396": {
         "CHS": "\u5192\u9669\u5bb6\u5934\u5e26",
         "CHT": "\u5192\u96aa\u5bb6\u982d\u5e36",
         "DE": "Kopftuch eines Abenteurers",
         "EN": "Adventurer's Bandana",
         "ES": "Bandana del Aventurero",
         "FR": "Bandeau de l'Aventurier",
@@ -62470,14 +63456,31 @@
         "KR": "\ud589\uc6b4\uc544\uc758 \uc740\uad00",
         "PT": "Grinalda de Prata do Sortudo",
         "RU": "\u0421\u0435\u0440\u0435\u0431\u0440\u044f\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430 \u0432\u0435\u0437\u0443\u043d\u0447\u0438\u043a\u0430",
         "TH": "Lucky Dog's Silver Circlet",
         "TR": "Baht\u0131 A\u00e7\u0131\u011f\u0131n G\u00fcm\u00fc\u015f Tac\u0131",
         "VI": "V\u00f2ng B\u1ea1c May M\u1eafn"
     },
+    "906667788": {
+        "CHS": "\u6076\u9f99\u7684\u5355\u7247\u955c",
+        "CHT": "\u60e1\u9f8d\u7684\u55ae\u7247\u93e1",
+        "DE": "Monokel des b\u00f6sen Drachen",
+        "EN": "Fell Dragon's Monocle",
+        "ES": "Mon\u00f3culo del Drag\u00f3n Protervo",
+        "FR": "Monocle de dragon d\u00e9moniaque",
+        "ID": "Fell Dragon's Monocle",
+        "IT": "Monocolo del drago caduto",
+        "JP": "\u60aa\u9f8d\u306e\u7247\u773c\u93e1",
+        "KR": "\uc545\ub8e1\uc758 \ub2e8\uc548\uacbd",
+        "PT": "Mon\u00f3culo do Drag\u00e3o Maligno",
+        "RU": "\u041c\u043e\u043d\u043e\u043a\u043b\u044c \u0441\u0432\u0438\u0440\u0435\u043f\u043e\u0433\u043e \u0434\u0440\u0430\u043a\u043e\u043d\u0430",
+        "TH": "Fell Dragon's Monocle",
+        "TR": "U\u011fursuz Ejderin G\u00f6zl\u00fc\u011f\u00fc",
+        "VI": "K\u00ednh M\u1eaft C\u1ee7a \u00c1c Long"
+    },
     "907000716": {
         "CHS": "\u6218\u72c2\u7684\u65f6\u8ba1",
         "CHT": "\u6230\u72c2\u7684\u6642\u8a08",
         "DE": "Berserkersanduhr",
         "EN": "Berserker's Timepiece",
         "ES": "Reloj del Berserker",
         "FR": "Sablier du Berserker",
@@ -63303,14 +64306,31 @@
         "KR": "\ud604\uba85\uc758 \uc8fc\uae30",
         "PT": "Momento de Sabedoria",
         "RU": "\u0427\u0430\u0441 \u043e\u0441\u043c\u044b\u0441\u043b\u0435\u043d\u0438\u044f",
         "TH": "A Time of Insight",
         "TR": "Bilgelik Devri",
         "VI": "Th\u1eddi H\u1ea1n C\u1ee7a Hi\u1ec1n Tr\u00ed"
     },
+    "960910716": {
+        "CHS": "\u7426\u8272\u7075\u5f69\u4e4b\u7fbd",
+        "CHT": "\u7426\u8272\u9748\u5f69\u4e4b\u7fbd",
+        "DE": "Bezaubernde Feder",
+        "EN": "Vibrant Pinion",
+        "ES": "Pluma Crom\u00e1tica",
+        "FR": "Penne vibrante",
+        "ID": "Vibrant Pinion",
+        "IT": "Penna dalle tinte vivaci",
+        "JP": "\u970a\u5f69\u5947\u9e97\u306e\u7fbd",
+        "KR": "\uc601\ub871\ud55c \uc625\ube5b \uae43\ud138",
+        "PT": "Pluma do Cristal Reluzente",
+        "RU": "\u0421\u0430\u043c\u043e\u0446\u0432\u0435\u0442\u043d\u043e\u0435 \u043f\u0435\u0440\u043e",
+        "TH": "Vibrant Pinion",
+        "TR": "Alacal\u0131 T\u00fcy",
+        "VI": "L\u00f4ng V\u0169 \u00c1nh S\u1eafc M\u00e0u"
+    },
     "962538140": {
         "CHS": "\u4e50\u56e2\u7684\u6668\u5149",
         "CHT": "\u6a02\u5718\u7684\u6668\u5149",
         "DE": "Morgenlicht des Ensembles",
         "EN": "Troupe's Dawnlight",
         "ES": "Luz Matinal de la Orquesta",
         "FR": "Aube de l'orchestre",
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/langs/characters.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/langs/characters.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'2984815066'": "OrderedDict([('FR', 'Baizhu'), ('JP', '白朮'), ('CHT', '白朮'), ('ID', 'Baizhu'), "*

 * *                 "('CHS', '白术'), ('VI', 'Baizhu'), ('ES', 'Baizhu'), ('TH', 'Baizhu'), ('TR', "*

 * *                 "'Baizhu'), ('KR', '백출'), ('DE', 'Baizhu'), ('RU', 'Бай Чжу'), ('IT', 'Baizhu'), "*

 * *                 "('EN', 'Baizhu'), ('PT', 'Baizhu')])",*

 * * "'466355514'": "OrderedDict([('FR', 'Kaveh'), ('JP', 'カーヴェ'), ('CHT', '卡維'), ('ID', 'Kaveh'), "*

 * *                "('CHS', '卡维'), ('VI', 'Kaveh'), ('ES', 'Kaveh') […]*

```diff
@@ -522,14 +522,31 @@
         "KR": "\ucf5c\ub808\uc774",
         "PT": "Collei",
         "RU": "\u041a\u043e\u043b\u043b\u0435\u0438",
         "TH": "Collei",
         "TR": "Collei",
         "VI": "Collei"
     },
+    "2984815066": {
+        "CHS": "\u767d\u672f",
+        "CHT": "\u767d\u672e",
+        "DE": "Baizhu",
+        "EN": "Baizhu",
+        "ES": "Baizhu",
+        "FR": "Baizhu",
+        "ID": "Baizhu",
+        "IT": "Baizhu",
+        "JP": "\u767d\u672e",
+        "KR": "\ubc31\ucd9c",
+        "PT": "Baizhu",
+        "RU": "\u0411\u0430\u0439 \u0427\u0436\u0443",
+        "TH": "Baizhu",
+        "TR": "Baizhu",
+        "VI": "Baizhu"
+    },
     "3024507506": {
         "CHS": "\u96f7\u7535\u5c06\u519b",
         "CHT": "\u96f7\u96fb\u5c07\u8ecd",
         "DE": "Shougun Raiden",
         "EN": "Raiden Shogun",
         "ES": "Shogun Raiden",
         "FR": "Shogun Raiden",
@@ -1015,14 +1032,31 @@
         "KR": "\uc2e0\uc5fc",
         "PT": "Xinyan",
         "RU": "\u0421\u0438\u043d\u044c \u042f\u043d\u044c",
         "TH": "Xinyan",
         "TR": "Xinyan",
         "VI": "Xinyan"
     },
+    "466355514": {
+        "CHS": "\u5361\u7ef4",
+        "CHT": "\u5361\u7dad",
+        "DE": "Kaveh",
+        "EN": "Kaveh",
+        "ES": "Kaveh",
+        "FR": "Kaveh",
+        "ID": "Kaveh",
+        "IT": "Kaveh",
+        "JP": "\u30ab\u30fc\u30f4\u30a7",
+        "KR": "\uce74\ubca0",
+        "PT": "Kaveh",
+        "RU": "\u041a\u0430\u0432\u0435\u0445",
+        "TH": "Kaveh",
+        "TR": "Kaveh",
+        "VI": "Kaveh"
+    },
     "646032090": {
         "CHS": "\u9e7f\u91ce\u9662\u5e73\u85cf",
         "CHT": "\u9e7f\u91ce\u9662\u5e73\u85cf",
         "DE": "Shikanoin Heizou",
         "EN": "Shikanoin Heizou",
         "ES": "Shikanoin Heizou",
         "FR": "Shikanoin Heizou",
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/langs/constellations.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/langs/constellations.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.957472613458529%*

 * *Differences: {"'1293460177'": "OrderedDict([('FR', 'Purification du qi'), ('JP', '真邪離合'), ('CHT', '真邪合離'), "*

 * *                 "('ID', 'Elimination of Malicious Qi'), ('CHS', '真邪合离'), ('VI', 'Chân Tà Hợp "*

 * *                 "Ly'), ('ES', 'Disipación del chi maligno'), ('TH', 'Elimination of Malicious "*

 * *                 "Qi'), ('TR', 'Negatif Çi Arındırma'), ('KR', '병과 건강'), ('DE', 'Austreibung "*

 * *                 "negativer Energie'), ('RU', 'Устранение зловредной энергии'), ('IT', 'Rimozione "*

 * *                 "del qi mal […]*

```diff
@@ -522,14 +522,31 @@
         "KR": "\ubb34\ud55c\uc758 \uc804\uae30\ud68c\ub85c",
         "PT": "Circuito Infinito",
         "RU": "\u0417\u0430\u043c\u044b\u043a\u0430\u043d\u0438\u0435 \u0446\u0435\u043f\u0438",
         "TH": "Infinite Circuit",
         "TR": "Sonsuz Devre",
         "VI": "\u0110\u01b0\u1eddng \u0110i\u1ec7n V\u00f4 H\u1ea1n"
     },
+    "1293460177": {
+        "CHS": "\u771f\u90aa\u5408\u79bb",
+        "CHT": "\u771f\u90aa\u5408\u96e2",
+        "DE": "Austreibung negativer Energie",
+        "EN": "Elimination of Malicious Qi",
+        "ES": "Disipaci\u00f3n del chi maligno",
+        "FR": "Purification du qi",
+        "ID": "Elimination of Malicious Qi",
+        "IT": "Rimozione del qi maligno",
+        "JP": "\u771f\u90aa\u96e2\u5408",
+        "KR": "\ubcd1\uacfc \uac74\uac15",
+        "PT": "Elimina\u00e7\u00e3o de Qi Malicioso",
+        "RU": "\u0423\u0441\u0442\u0440\u0430\u043d\u0435\u043d\u0438\u0435 \u0437\u043b\u043e\u0432\u0440\u0435\u0434\u043d\u043e\u0439 \u044d\u043d\u0435\u0440\u0433\u0438\u0438",
+        "TH": "Elimination of Malicious Qi",
+        "TR": "Negatif \u00c7i Ar\u0131nd\u0131rma",
+        "VI": "Ch\u00e2n T\u00e0 H\u1ee3p Ly"
+    },
     "1318685825": {
         "CHS": "\u670d\u81ba\u8a93\u7981\u606a\u5b88\u65e0\u5931",
         "CHT": "\u670d\u81ba\u8a93\u7981\u606a\u5b88\u7121\u5931",
         "DE": "Dem Eid treu ergeben",
         "EN": "An Oath Abiding",
         "ES": "Juramento inquebrantable",
         "FR": "Liant serment de respect",
@@ -596,15 +613,15 @@
     },
     "1377520009": {
         "CHS": "\u4e0d\u7a33\u7684\u7194\u5ca9",
         "CHT": "\u4e0d\u7a69\u7684\u7194\u5ca9",
         "DE": "Instabiler Kern",
         "EN": "Rockcore Meltdown",
         "ES": "Fusi\u00f3n de lava",
-        "FR": "Enfondrement de lave",
+        "FR": "Effondrement de lave",
         "ID": "Rockcore Meltdown",
         "IT": "Fusione esplosiva",
         "JP": "\u4e0d\u7a4f\u306a\u6eb6\u5ca9",
         "KR": "\ubd88\uc548\uc815\ud55c \uc6a9\uc554",
         "PT": "Pedra Derretida",
         "RU": "\u041f\u043b\u0430\u0432\u043b\u0435\u043d\u0438\u0435 \u043a\u0430\u043c\u0435\u043d\u043d\u043e\u0433\u043e \u044f\u0434\u0440\u0430",
         "TH": "Rockcore Meltdown",
@@ -908,15 +925,15 @@
         "ES": "Sangre excelente",
         "FR": "Lign\u00e9e de l'excellence",
         "ID": "Excellent Blood",
         "IT": "Lignaggio d'eccellenza",
         "JP": "\u512a\u308c\u305f\u8840\u7b4b",
         "KR": "\uac78\ucd9c\ud55c \ud608\ud1b5",
         "PT": "Sangue Excelente",
-        "RU": "\u0418\u0437\u043c\u043e\u0440\u043e\u0437\u044c",
+        "RU": "\u041f\u0440\u0435\u0432\u043e\u0441\u0445\u043e\u0434\u043d\u0430\u044f \u043a\u0440\u043e\u0432\u044c",
         "TH": "Excellent Blood",
         "TR": "Kusursuz Kan",
         "VI": "Huy\u1ebft M\u1ea1ch \u01afu Vi\u1ec7t"
     },
     "1479737849": {
         "CHS": "\u6781\u6076\u6280\u00b7\u5929\u4f7f\u706d\u5c3d",
         "CHT": "\u6975\u60e1\u6280\u00b7\u5929\u4f7f\u6ec5\u76e1",
@@ -1457,14 +1474,31 @@
         "KR": "\uac00\uc2e0\uc758 \uc624\ub79c \uacc4\ud68d",
         "PT": "Plano a Longo Prazo",
         "RU": "\u0414\u043e\u043b\u0433\u043e\u0441\u0440\u043e\u0447\u043d\u044b\u0439 \u043f\u043b\u0430\u043d",
         "TH": "Long-Term Planning",
         "TR": "Uzun Vadeli Planlama",
         "VI": "M\u01b0u K\u1ebf C\u1ee7a Gia Th\u1ea7n"
     },
+    "1755584449": {
+        "CHS": "\u5723\u53e4\u7684\u5e93\u85cf",
+        "CHT": "\u8056\u53e4\u7684\u5eab\u85cf",
+        "DE": "Sch\u00e4tze von Bonkhanak",
+        "EN": "Treasures of Bonkhanak",
+        "ES": "Galer\u00eda sagrada",
+        "FR": "Entreposage du saint ancien",
+        "ID": "Treasures of Bonkhanak",
+        "IT": "Tesori della Bonkhanak",
+        "JP": "\u8056\u306a\u308b\u30ab\u30fc\u30d0",
+        "KR": "\ub099\uc250 \ub85c\uc2a4\ud0d0\uc758 \uc2e0\uc804",
+        "PT": "Tesouros Sagrados",
+        "RU": "\u0421\u043e\u043a\u0440\u043e\u0432\u0438\u0449\u0430 \u0411\u043e\u043d-\u0425\u0430\u043d\u0430\u043a",
+        "TH": "Treasures of Bonkhanak",
+        "TR": "Bonkhanak'\u0131n Hazineleri",
+        "VI": "Kho T\u00e0ng Bonkhanak"
+    },
     "1768747369": {
         "CHS": "\u6700\u4e0d\u5b89\u795e\u6674\u53c8\u590d\u96e8",
         "CHT": "\u6700\u4e0d\u5b89\u795e\u6674\u53c8\u5fa9\u96e8",
         "DE": "Wetterwechsel",
         "EN": "Ominous Rainfall",
         "ES": "Mal presagio",
         "FR": "Sombres auspices",
@@ -1593,14 +1627,31 @@
         "KR": "\uc9c4\ub9ac\ub85c \ud1b5\ud558\ub294 \uae38",
         "PT": "Ess\u00eancia da Verdade",
         "RU": "\u0414\u0438\u0432\u043d\u044b\u0439 \u043f\u0443\u0442\u044c \u0438\u0441\u0442\u0438\u043d\u044b",
         "TH": "The Wondrous Path of Truth",
         "TR": "Ger\u00e7e\u011fin Harika Yolu",
         "VI": "\u0110\u01b0\u1eddng Ch\u00e2n L\u00fd K\u1ef3 Di\u1ec7u"
     },
+    "1849398401": {
+        "CHS": "\u52a8\u9759\u7cbe\u660e",
+        "CHT": "\u52d5\u975c\u7cbe\u660e",
+        "DE": "Flink und geschickt",
+        "EN": "Incisive Discernment",
+        "ES": "Discernimiento maestro",
+        "FR": "Discernement incisif",
+        "ID": "Incisive Discernment",
+        "IT": "Discernimento accurato",
+        "JP": "\u8108\u7d61\u660e\u54f2",
+        "KR": "\ud658\uc790 \uc9c4\ub2e8",
+        "PT": "Discernimento Incisivo",
+        "RU": "\u041e\u0441\u0442\u0440\u0430\u044f \u043f\u0440\u043e\u043d\u0438\u0446\u0430\u0442\u0435\u043b\u044c\u043d\u043e\u0441\u0442\u044c",
+        "TH": "Incisive Discernment",
+        "TR": "Hassas Muhakeme",
+        "VI": "\u0110\u1ed9ng T\u0129nh Tinh Minh"
+    },
     "1859111849": {
         "CHS": "\u91ca\u51cc\u548f\u51b0",
         "CHT": "\u91cb\u51cc\u8a60\u51b0",
         "DE": "Gesang der Eiszapfen",
         "EN": "Ice Unleashed",
         "ES": "Ventisca desatada",
         "FR": "Glace d\u00e9cha\u00een\u00e9e",
@@ -1865,14 +1916,31 @@
         "KR": "\uc9c4\ub9ac \ucd94\uad6c",
         "PT": "Busca pela Verdade",
         "RU": "\u0418\u0441\u0442\u0438\u043d\u0430 \u043b\u044e\u0431\u044b\u043c \u043f\u0443\u0442\u0451\u043c",
         "TH": "Truth by Any Means",
         "TR": "Ne Olursa Olsun Ger\u00e7ek",
         "VI": "S\u1ef1 Th\u1eadt B\u1eb1ng M\u1ecdi C\u00e1ch"
     },
+    "20172977": {
+        "CHS": "\u5fa1\u9a7f\u7684\u5f84\u8ff9",
+        "CHT": "\u5fa1\u9a5b\u7684\u5f91\u8de1",
+        "DE": "Erhabene Stra\u00dfen",
+        "EN": "Grace of Royal Roads",
+        "ES": "Camino del Gran Tronco",
+        "FR": "Gr\u00e2ce du sentier royal",
+        "ID": "Grace of Royal Roads",
+        "IT": "Grazia delle vie reali",
+        "JP": "\u30ad\u30e3\u30e9\u30d0\u30f3\u30b5\u30e9\u30a4\u306e\u8f4d",
+        "KR": "\uce74\ub77c\ubc18\uc0ac\ub77c\uc758 \uae38",
+        "PT": "A Grande Estrada",
+        "RU": "\u0418\u0437\u044f\u0449\u0435\u0441\u0442\u0432\u043e \u043a\u043e\u0440\u043e\u043b\u0435\u0432\u0441\u043a\u0438\u0445 \u043f\u0443\u0442\u0435\u0439",
+        "TH": "Grace of Royal Roads",
+        "TR": "Kral Yolunun \u0130hti\u015fam\u0131",
+        "VI": "\u0110\u1ea1i L\u1ed9 Th\u00eanh Thang"
+    },
     "202198665": {
         "CHS": "\u9769\u65b0\u7684\u65cb\u98ce",
         "CHT": "\u9769\u65b0\u7684\u65cb\u98a8",
         "DE": "Aufsteigender Wind",
         "EN": "Uprising Whirlwind",
         "ES": "Torbellino ascendente",
         "FR": "Tornade de la r\u00e9bellion",
@@ -2562,14 +2630,31 @@
         "KR": "\uc6b0\uc5f0\ud788 \ud53c\uc6b4 \uaf43",
         "PT": "Admira\u00e7\u00e3o das Flores",
         "RU": "\u0421\u043e\u0437\u0435\u0440\u0446\u0430\u043d\u0438\u0435 \u0446\u0432\u0435\u0442\u043e\u0432",
         "TH": "To Admire the Flowers",
         "TR": "\u00c7i\u00e7eklerin Seyri",
         "VI": "V\u00f4 \u00dd Th\u01b0\u1edfng Hoa"
     },
+    "2410139081": {
+        "CHS": "\u516b\u6b63\u5b9a\u6c14",
+        "CHT": "\u516b\u6b63\u5b9a\u6c23",
+        "DE": "Alle Symptome stabilisiert",
+        "EN": "All Aspects Stabilized",
+        "ES": "Homeostasis omn\u00edmoda",
+        "FR": "Stabilisation compl\u00e8te",
+        "ID": "All Aspects Stabilized",
+        "IT": "Tutti gli aspetti stabilizzati",
+        "JP": "\u516b\u6b63\u4e4b\u6c17",
+        "KR": "\uae30\uc6b4 \uc548\uc815",
+        "PT": "Estabilidade Total",
+        "RU": "\u0421\u0442\u0430\u0431\u0438\u043b\u0438\u0437\u0430\u0446\u0438\u044f \u0432\u043e\u0441\u044c\u043c\u0438 \u0430\u0441\u043f\u0435\u043a\u0442\u043e\u0432",
+        "TH": "All Aspects Stabilized",
+        "TR": "T\u00fcm De\u011ferler Stabil",
+        "VI": "B\u00e1t Ch\u00ednh \u0110\u1ecbnh Kh\u00ed"
+    },
     "2414003921": {
         "CHS": "\u6b66\u706b\u6025\u70f9",
         "CHT": "\u6b66\u706b\u6025\u70f9",
         "DE": "Scharf angebraten",
         "EN": "Deepfry",
         "ES": "Que quede bien frito",
         "FR": "Saut\u00e9 profond",
@@ -2630,14 +2715,31 @@
         "KR": "\ud53c\uc5b4\ub09c \ud64d\ub828",
         "PT": "Flor de L\u00f3tus Carmesim",
         "RU": "\u0426\u0432\u0435\u0442\u0435\u043d\u0438\u0435 \u043a\u0440\u0430\u0441\u043d\u043e\u0433\u043e \u043b\u043e\u0442\u043e\u0441\u0430",
         "TH": "Crimson Lotus Bloom",
         "TR": "K\u0131z\u0131l Nil\u00fcfer \u00c7i\u00e7e\u011fi",
         "VI": "Sen H\u1ed3ng Ch\u1edbm N\u1edf"
     },
+    "2439940993": {
+        "CHS": "\u6cbf\u9014\u767e\u666f\u4f1a\u5fc3",
+        "CHT": "\u6cbf\u9014\u767e\u666f\u6703\u5fc3",
+        "DE": "Unz\u00e4hlige Sehensw\u00fcrdigkeiten",
+        "EN": "Countless Sights to See",
+        "ES": "Infinidad paisaj\u00edstica",
+        "FR": "Myriade de curiosit\u00e9s en chemin",
+        "ID": "Countless Sights to See",
+        "IT": "Panorami infiniti",
+        "JP": "\u9053\u4e2d\u767e\u666f\u5fc3\u5f97\u305f\u308a",
+        "KR": "\ubc30\uc1a1 \uc911\uc758 \uacbd\uce58",
+        "PT": "Infinitas Paisagens no Caminho",
+        "RU": "\u0421\u043e\u0442\u043d\u0438 \u043f\u0435\u0439\u0437\u0430\u0436\u0435\u0439",
+        "TH": "Countless Sights to See",
+        "TR": "G\u00f6r\u00fclecek Say\u0131s\u0131z Manzara",
+        "VI": "L\u01b0u L\u1ea1i C\u1ea3nh S\u1eafc"
+    },
     "2443947665": {
         "CHS": "\u5f00\u62d3\u7684\u5fc3\u9b42",
         "CHT": "\u958b\u62d3\u7684\u5fc3\u9b42",
         "DE": "Entdeckergeist",
         "EN": "True Explorer",
         "ES": "Explorador verdadero",
         "FR": "Ouverture d'\u00e2me",
@@ -2854,15 +2956,15 @@
         "TH": "Dance of Suigetsu",
         "TR": "Suigetsu Dans\u0131",
         "VI": "Gian Th\u1ee7y Nguy\u1ec7t"
     },
     "2594998721": {
         "CHS": "\u65a9\u94c1\u65ad\u91d1",
         "CHT": "\u65ac\u9435\u65b7\u91d1",
-        "DE": "Stahlbrecher",
+        "DE": "Stahlbrecherin",
         "EN": "Steelbreaker",
         "ES": "Asoladora del acero",
         "FR": "Brise-acier",
         "ID": "Steelbreaker",
         "IT": "Spezzacciaio",
         "JP": "\u65ac\u9244\u65ad\u91d1",
         "KR": "\uac15\ucca0 \uc808\ub2e8",
@@ -3079,15 +3181,15 @@
     "2696040833": {
         "CHS": "\u5e84\u8c10\u5e76\u4e3e",
         "CHT": "\u838a\u8ae7\u4e26\u8209",
         "DE": "Gemeinsame Unternehmung",
         "EN": "Decorous Harmony",
         "ES": "Armon\u00eda y decoro",
         "FR": "Harmonie esth\u00e9tique",
-        "ID": "Decorous Harmony",
+        "ID": "Hiasan yang Harmonis",
         "IT": "Armonia e decoro",
         "JP": "\u8358\u8ae7\u4f75\u6301",
         "KR": "\uc7a5\uc5c4\ud558\uace0 \uc775\uc0b4\uc2a4\ub7ec\uc6b4 \ub178\ub7ab\uc18c\ub9ac",
         "PT": "Harmonia e Decoro",
         "RU": "\u0413\u0430\u0440\u043c\u043e\u043d\u0438\u0447\u043d\u043e\u0435 \u0440\u0430\u0437\u0432\u0438\u0442\u0438\u0435",
         "TH": "Decorous Harmony",
         "TR": "Zarif Bir Ahenk",
@@ -3140,14 +3242,31 @@
         "KR": "\uac70\uc6b8 \uc18d\uc758 \uc790\ud0dc",
         "PT": "Reflexo Gracioso",
         "RU": "\u041a\u0451\u043a\u0430 \u0444\u0443\u0441\u0438",
         "TH": "Kyouka Fuushi",
         "TR": "Kyouka Fuushi",
         "VI": "Kyouka Fuushi"
     },
+    "2730015409": {
+        "CHS": "\u91d1\u5854\u7684\u9999\u732e",
+        "CHT": "\u91d1\u5854\u7684\u9999\u737b",
+        "DE": "Opfergabe von Dur Untash",
+        "EN": "Profferings of Dur Untash",
+        "ES": "Oblaci\u00f3n de Dur Untash",
+        "FR": "Encens de la tour d'or",
+        "ID": "Profferings of Dur Untash",
+        "IT": "Profferte di Dur Untash",
+        "JP": "\u30b8\u30c3\u30b0\u30e9\u30c8\u3078\u306e\u4f9b\u7269",
+        "KR": "\ub450\ub974 \uc6b4\ud0c0\uc2dc\uc758 \uc81c\ubb3c",
+        "PT": "Oferenda da Torre Dourada",
+        "RU": "\u041f\u043e\u0434\u043d\u043e\u0448\u0435\u043d\u0438\u044f \u0414\u0443\u0440-\u0423\u043d\u0442\u0430\u0448",
+        "TH": "Profferings of Dur Untash",
+        "TR": "Dur Untash'\u0131n Arma\u011fan\u0131",
+        "VI": "T\u1ebf L\u1ec5 Dur Untash"
+    },
     "2730852953": {
         "CHS": "\u4e4c\u773c",
         "CHT": "\u70cf\u773c",
         "DE": "Kr\u00e4henauge",
         "EN": "Crow's Eye",
         "ES": "Ojo corvino",
         "FR": "\u0152il de corbeau",
@@ -3293,14 +3412,31 @@
         "KR": "\ucc22\uc5b4\ubc1c\uae30\ub294 \ud654\uc5fc \ubc1c\ud1b1",
         "PT": "Corte das Garras Incandescentes",
         "RU": "\u0420\u0430\u0437\u0440\u044b\u0432\u0430\u044e\u0449\u0438\u0435 \u043e\u0433\u043d\u0435\u043d\u043d\u044b\u0435 \u043a\u043e\u0433\u0442\u0438",
         "TH": "The Burning Claws Cleaving",
         "TR": "Par\u00e7alay\u0131c\u0131 Alevli Pen\u00e7e",
         "VI": "M\u00f3ng Vu\u1ed1t L\u1eeda C\u00e0n Qu\u00e9t"
     },
+    "2860814489": {
+        "CHS": "\u767e\u67f1\u7684\u9163\u5bb4",
+        "CHT": "\u767e\u67f1\u7684\u9163\u5bb4",
+        "DE": "Festmahl von Apadana",
+        "EN": "Feast of Apadana",
+        "ES": "Fest\u00edn hip\u00f3stilo",
+        "FR": "Banquet des cent piliers",
+        "ID": "Feast of Apadana",
+        "IT": "Banchetto dell'Apadana",
+        "JP": "\u30a2\u30d1\u30c0\u30fc\u30ca\u306e\u9957\u5bb4",
+        "KR": "\uc544\ud30c\ub2e4\ub098\uc758 \uc5f0\ud68c",
+        "PT": "Festa dos Cem Pilares",
+        "RU": "\u041f\u0438\u0440\u0448\u0435\u0441\u0442\u0432\u043e \u0410\u043f\u0430\u0434\u0430\u043d\u044b",
+        "TH": "Feast of Apadana",
+        "TR": "Apadana Ziyafeti",
+        "VI": "B\u1eefa Ti\u1ec7c Apadana"
+    },
     "286623921": {
         "CHS": "\u6b8a\u89e3\u8bf8\u56e0\u63a2\u6848\u96c6",
         "CHT": "\u6b8a\u89e3\u8af8\u56e0\u63a2\u6848\u96c6",
         "DE": "Aufdeckung der Hintergr\u00fcnde",
         "EN": "Investigative Collection",
         "ES": "Canon Shikanoiniano",
         "FR": "Recueil d'enqu\u00eates",
@@ -3395,14 +3531,31 @@
         "KR": "\ub300\uacf5\ud658\ubc95",
         "PT": "Magia Ilus\u00f3ria",
         "RU": "\u041e\u0434\u0437\u043e\u0440\u0430 \u0433\u044d\u043c\u043f\u043e",
         "TH": "Oozora Genpou",
         "TR": "Oozora Genpou",
         "VI": "Oozora Genpou"
     },
+    "2892000521": {
+        "CHS": "\u5929\u56ed\u7684\u7406\u60f3",
+        "CHT": "\u5929\u5712\u7684\u7406\u60f3",
+        "DE": "Tr\u00e4ume von Pairidaeza",
+        "EN": "Pairidaeza's Dreams",
+        "ES": "Canon del para\u00edso",
+        "FR": "Id\u00e9al du jardin c\u00e9leste",
+        "ID": "Pairidaeza's Dreams",
+        "IT": "Sogni del Pairidaeza",
+        "JP": "\u30d1\u30a4\u30ea\u30c0\u30a8\u30fc\u30b6\u306e\u7406\u60f3",
+        "KR": "\ud30c\uc774\ub9ac\ub370\uc790\uc758 \uc774\uc0c1",
+        "PT": "Utopia Celestial",
+        "RU": "\u041c\u0435\u0447\u0442\u044b \u041f\u0430\u0439\u0440\u0438\u0434\u0430\u044d\u0437\u044b",
+        "TH": "Pairidaeza\u2019s Dreams",
+        "TR": "Pairidaeza Hayalleri",
+        "VI": "L\u00fd T\u01b0\u1edfng Pairidaeza"
+    },
     "2904102233": {
         "CHS": "\u5927\u8fa8\u5706\u6210\u4e4b\u5b9e",
         "CHT": "\u5927\u8fa8\u5713\u6210\u4e4b\u5be6",
         "DE": "Frucht der Kulmination der Vernunft",
         "EN": "The Fruit of Reason's Culmination",
         "ES": "Frutos de la culminaci\u00f3n racional",
         "FR": "Fruit d'aboutissement rationnel",
@@ -3650,14 +3803,31 @@
         "KR": "\uc808\uba85\uc758 \uac00\uc18d",
         "PT": "Acelera\u00e7\u00e3o Fatal",
         "RU": "\u0424\u0430\u0442\u0430\u043b\u044c\u043d\u044b\u0439 \u0440\u0430\u0437\u0433\u043e\u043d",
         "TH": "Fatal Acceleration",
         "TR": "\u00d6l\u00fcmc\u00fcl H\u0131zlanma",
         "VI": "Gia T\u1ed1c C\u1ee7a Tuy\u1ec7t M\u1ec7nh"
     },
+    "3110332641": {
+        "CHS": "\u9ad8\u95e8\u7684\u8c12\u793c",
+        "CHT": "\u9ad8\u9580\u7684\u8b01\u79ae",
+        "DE": "Erhabener Gru\u00df",
+        "EN": "Sublime Salutations",
+        "ES": "Modales pudientes",
+        "FR": "Salutation de la grande porte",
+        "ID": "Sublime Salutations",
+        "IT": "Saluti eccelsi",
+        "JP": "\u30a4\u30fc\u30ef\u30fc\u30f3\u306b\u3066\u8b01\u898b",
+        "KR": "\uc774\uc644\uc758 \ubb38",
+        "PT": "Sauda\u00e7\u00f5es Sublimes",
+        "RU": "\u0412\u043e\u0437\u0432\u044b\u0448\u0435\u043d\u043d\u044b\u0435 \u043f\u0440\u0438\u0432\u0435\u0442\u0441\u0442\u0432\u0438\u044f",
+        "TH": "Sublime Salutations",
+        "TR": "Y\u00fccelten \u00d6vg\u00fcler",
+        "VI": "L\u1eddi Ch\u00e0o Cao Qu\u00fd"
+    },
     "3111083697": {
         "CHS": "\u9017\u7559\u91c7\u8840\u8272",
         "CHT": "\u9017\u7559\u63a1\u8840\u8272",
         "DE": "Aderlass",
         "EN": "Lingering Carmine",
         "ES": "Persistencia escarlata",
         "FR": "Rituel du sang",
@@ -4211,14 +4381,31 @@
         "KR": "\uc131\uc778\uc744 \ubc1b\ub4dc\ub294 \ub124 \uac1c\uc758 \ub839",
         "PT": "Refor\u00e7o das Quatro L\u00e2minas",
         "RU": "\u041c\u043e\u043b\u0438\u0442\u0432\u0430 \u0447\u0435\u0442\u044b\u0440\u0451\u043c \u0434\u0443\u0445\u0430\u043c",
         "TH": "Rally of Four Blades",
         "TR": "D\u00f6rt K\u0131l\u0131c\u0131n Birli\u011fi",
         "VI": "T\u1ee9 Linh B\u1ed5ng Th\u00e1nh"
     },
+    "3397892401": {
+        "CHS": "\u4e07\u6237\u95e8\u724c\u901a\u8bc6",
+        "CHT": "\u842c\u6236\u9580\u724c\u901a\u8b58",
+        "DE": "Universelle Erkennung",
+        "EN": "Universal Recognition",
+        "ES": "Conoce a tu vecino",
+        "FR": "Connaissance des lieux",
+        "ID": "Universal Recognition",
+        "IT": "Riconoscimento universale",
+        "JP": "\u4e07\u6238\u9580\u672d\u306b\u901a\u305a",
+        "KR": "\uae38 \ucc3e\uae30 \uc804\ubb38\uac00",
+        "PT": "Reconhecimento Universal",
+        "RU": "\u0417\u043d\u0430\u043d\u0438\u0435 \u0432\u0441\u0435\u0445 \u0430\u0434\u0440\u0435\u0441\u043e\u0432",
+        "TH": "Universal Recognition",
+        "TR": "T\u00fcm D\u00fcnyaya Teslimat",
+        "VI": "T\u01b0\u1eddng T\u1eadn Ng\u00f5 Ng\u00e1ch"
+    },
     "3408467449": {
         "CHS": "\u6674\u971c\u7684\u795d\u5ff5",
         "CHT": "\u6674\u971c\u7684\u795d\u5ff5",
         "DE": "Sonnenfrost-Segen",
         "EN": "Sunfrost Encomium",
         "ES": "Alabanza de la cencellada",
         "FR": "\u00c9loge du givre clair",
@@ -4381,14 +4568,31 @@
         "KR": "\ubed7\uc5b4\ub098\uac00\ub294 \uc6d0\ub8b0",
         "PT": "Trovoada Distante",
         "RU": "\u0414\u0430\u043b\u0451\u043a\u0438\u0435 \u0440\u0430\u0441\u043a\u0430\u0442\u044b",
         "TH": "Distant Crackling",
         "TR": "Uzaklardan \u00c7akan \u015eim\u015fek",
         "VI": "S\u1ea5m Ch\u1edbp Li\u00ean Mi\u00ean"
     },
+    "34942769": {
+        "CHS": "\u5343\u91cc\u4e00\u65e5",
+        "CHT": "\u5343\u91cc\u4e00\u65e5",
+        "DE": "Tausend Meilen jeden Tag",
+        "EN": "A Thousand Miles in a Day",
+        "ES": "Periplo diario",
+        "FR": "Mille lieues par jour",
+        "ID": "A Thousand Miles in a Day",
+        "IT": "Mille miglia al giorno",
+        "JP": "\u4e00\u65e5\u5343\u91cc",
+        "KR": "\uc77c\uc77c\ucc9c\ub9ac",
+        "PT": "Mil Milhas por Dia",
+        "RU": "\u0422\u044b\u0441\u044f\u0447\u0430 \u043a\u0438\u043b\u043e\u043c\u0435\u0442\u0440\u043e\u0432 \u0432 \u0434\u0435\u043d\u044c",
+        "TH": "A Thousand Miles in a Day",
+        "TR": "G\u00fcnde Bin Kilometre",
+        "VI": "M\u1ed9t Ng\u00e0y V\u1ea1n D\u1eb7m"
+    },
     "3498425217": {
         "CHS": "\u914c\u76c8\u5242\u865a",
         "CHT": "\u914c\u76c8\u5291\u865b",
         "DE": "Zuschlag f\u00fcr Defizite",
         "EN": "Discretionary Supplement",
         "ES": "Compensaci\u00f3n de p\u00e9rdidas",
         "FR": "Suppl\u00e9ment discr\u00e9tionnaire",
@@ -4415,14 +4619,31 @@
         "KR": "\uaf43\uc78e\uc5d0\uc11c \uae68\ub2ec\uc740 \uc0ac\uc2e4",
         "PT": "Compreens\u00e3o em Meio as Flores",
         "RU": "\u0412\u043e \u0446\u0432\u0435\u0442\u0435\u043d\u0438\u0438 \u043e\u0441\u043c\u044b\u0441\u043b\u0438\u0432\u0430\u0435\u0442\u0441\u044f \u0438\u0441\u0442\u0438\u043d\u0430",
         "TH": "Comprehension Amidst the Flowers",
         "TR": "\u00c7i\u00e7eklerdeki Anlay\u0131\u015f",
         "VI": "T\u1eeb C\u00e1nh Hoa T\u00ecm Gi\u00e1c Ng\u1ed9"
     },
+    "3502158873": {
+        "CHS": "\u7269\u5668\u6d41\u8f6c",
+        "CHT": "\u7269\u5668\u6d41\u8f49",
+        "DE": "Materialkreislauf",
+        "EN": "Material Circulation",
+        "ES": "Circulaci\u00f3n log\u00edstica",
+        "FR": "Circulation d'objets",
+        "ID": "Material Circulation",
+        "IT": "Circolazione materiale",
+        "JP": "\u5668\u7269\u6d41\u8ee2",
+        "KR": "\ubb3c\ub958 \ud750\ub984",
+        "PT": "Circula\u00e7\u00e3o de Materiais",
+        "RU": "\u041e\u0431\u043e\u0440\u043e\u0442 \u043c\u0430\u0442\u0435\u0440\u0438\u0430\u043b\u043e\u0432",
+        "TH": "Material Circulation",
+        "TR": "Da\u011f\u0131t\u0131m A\u011f\u0131",
+        "VI": "V\u1eadt Ch\u1ea5t L\u01b0u Th\u00f4ng"
+    },
     "3504453161": {
         "CHS": "\u96f6\u5931\u8bef\u5c11\u5973",
         "CHT": "\u96f6\u5931\u8aa4\u5c11\u5973",
         "DE": "Bestnote",
         "EN": "Flawless Alchemistress",
         "ES": "Alquimista infalible",
         "FR": "Z\u00e9ro d\u00e9faut",
@@ -4517,14 +4738,31 @@
         "KR": "\ub354\ube14 \uc2a4\ud0d1",
         "PT": "Duplo-Stop",
         "RU": "\u0421\u043b\u043e\u0436\u043d\u044b\u0439 \u0430\u043a\u043a\u043e\u0440\u0434",
         "TH": "Double-Stop",
         "TR": "\u00c7ift Stop",
         "VI": "Ph\u01b0\u01a1ng Ph\u00e1p Ph\u00e2n Gi\u1ea3i"
     },
+    "3551684865": {
+        "CHS": "\u97e6\u9a6e\u9a8f\u8db3",
+        "CHT": "\u97cb\u99b1\u99ff\u8db3",
+        "DE": "Skanda-Ross",
+        "EN": "Steed of Skanda",
+        "ES": "Corcel de Skanda",
+        "FR": "\u00c9talon de Skanda",
+        "ID": "Steed of Skanda",
+        "IT": "Destriera di Skanda",
+        "JP": "\u97cb\u99c4\u5929\u99ff\u8db3",
+        "KR": "\uc9c8\uc8fc\ud558\ub294 \uc774\ub2e4\ud150",
+        "PT": "Corcel de Skanda",
+        "RU": "\u041b\u043e\u0448\u0430\u0434\u044c \u0421\u043a\u0430\u043d\u0434\u044b",
+        "TH": "Steed of Skanda",
+        "TR": "Skanda'n\u0131n K\u00fcheylan\u0131",
+        "VI": "\u0110\u00f4i Ch\u00e2n Skanda"
+    },
     "3553177833": {
         "CHS": "\u5065\u97e7\u7684\u52b2\u8349",
         "CHT": "\u5065\u97cc\u7684\u52c1\u8349",
         "DE": "Beharrliches Gras",
         "EN": "Green Resilience",
         "ES": "Planta tenaz",
         "FR": "R\u00e9silience verte",
@@ -4570,15 +4808,15 @@
         "RU": "\u0427\u0443\u0436\u0435\u0437\u0435\u043c\u043d\u0430\u044f \u0437\u0432\u0435\u0437\u0434\u0430",
         "TH": "Star of Another World",
         "TR": "Ba\u015fka D\u00fcnyadan Bir Y\u0131ld\u0131z",
         "VI": "Ng\u00f4i Sao D\u1ecb Gi\u1edbi"
     },
     "3582154129": {
         "CHS": "\u5077\u61d2\u7684\u65b0\u65b9\u6cd5",
-        "CHT": "\u5077\u61d2\u7684\u65b0\u65b9\u6cd5",
+        "CHT": "\u5077\u61f6\u7684\u65b0\u65b9\u6cd5",
         "DE": "Profischw\u00e4nzen",
         "EN": "Skiving: New and Improved",
         "ES": "Holgazaner\u00eda innovadora",
         "FR": "Paresse revue et am\u00e9lior\u00e9e",
         "ID": "Skiving: New and Improved",
         "IT": "Pigrizia: nuove tecniche",
         "JP": "\u65b0\u3057\u3044\u30b5\u30dc\u308b\u65b9\u6cd5",
@@ -4923,15 +5161,15 @@
         "IT": "Ti guardo le spalle",
         "JP": "\u652f\u63f4\u306f\u304a\u4efb\u305b\u304f\u3060\u3055\u3044",
         "KR": "\uc9c0\uc6d0\uc740 \uc800\ud55c\ud14c \ub9e1\uae30\uc138\uc694",
         "PT": "Estou na sua Retaguarda",
         "RU": "\u042f \u043f\u0440\u0438\u043a\u0440\u043e\u044e!",
         "TH": "I Got Your Back",
         "TR": "Bana G\u00fcven",
-        "VI": "Chi vi\u1ec7n c\u1ee9 giao cho t\u00f4i"
+        "VI": "Chi Vi\u1ec7n C\u1ee9 Giao Cho T\u00f4i"
     },
     "3753636729": {
         "CHS": "\u9a9e\u6797\u9988\u9057",
         "CHT": "\u9a2b\u6797\u994b\u907a",
         "DE": "Waldgeschenk unterm Mond",
         "EN": "Gift of the Woods",
         "ES": "Obsequio de la naturaleza",
@@ -5197,14 +5435,31 @@
         "KR": "\ub2e4\uc591\ud55c \uc18c\ud488",
         "PT": "Mir\u00edade de Adere\u00e7os",
         "RU": "\u041c\u0438\u0440\u0438\u0430\u0434\u044b \u043c\u0438\u0437\u0430\u043d\u0441\u0446\u0435\u043d",
         "TH": "Myriad Mise-En-Sc\u00e8ne",
         "TR": "Zengin Mizansen",
         "VI": "Ch\u01b0 B\u00e0n Thi\u1ebft M\u1ea1t"
     },
+    "3954516065": {
+        "CHS": "\u516b\u5c16\u88f9\u672f",
+        "CHT": "\u516b\u5c16\u88f9\u8853",
+        "DE": "Perfekt verpackt",
+        "EN": "Perfectly Packaged",
+        "ES": "Embalaje perfecto",
+        "FR": "Emballage parfait",
+        "ID": "Perfectly Packaged",
+        "IT": "Imballaggio perfetto",
+        "JP": "\u516b\u9685\u00b7\u5b8c\u74a7\u68b1\u5305\u8853",
+        "KR": "\uc644\ubcbd \ud3ec\uc7a5\uc220",
+        "PT": "Embalagem Perfeita",
+        "RU": "\u0412\u044b\u0441\u0448\u0435\u0435 \u0438\u0441\u043a\u0443\u0441\u0441\u0442\u0432\u043e \u0443\u043f\u0430\u043a\u043e\u0432\u043a\u0438",
+        "TH": "Perfectly Packaged",
+        "TR": "Kusursuz Kargo Kutusu",
+        "VI": "\u0110\u00f3ng G\u00f3i Ho\u00e0n H\u1ea3o"
+    },
     "3961952345": {
         "CHS": "\u56db\u756a\u00b7\u82b1\u6708\u6b4c\u6d6e\u821f",
         "CHT": "\u56db\u756a\u00b7\u82b1\u6708\u6b4c\u6d6e\u821f",
         "DE": "Yonban \u2013 Aufbruch ins Fr\u00fchjahr",
         "EN": "Yonban: Set Adrift into Spring",
         "ES": "Cuarto acto: Barco a la deriva",
         "FR": "Yonban : D\u00e9rive vers le printemps",
@@ -5656,14 +5911,31 @@
         "KR": "\uc138\uc0c1\uc5d0\ub294 \uc6d0\ucc9c\uc774 \uc788\ub2e4",
         "PT": "Fonte do Mundo",
         "RU": "\u0420\u043e\u0434\u043d\u0438\u043a \u043c\u0438\u0440\u0430",
         "TH": "World Source",
         "TR": "D\u00fcnyan\u0131n Kayna\u011f\u0131",
         "VI": "Su\u1ed1i Ngu\u1ed3n Th\u1ebf Gi\u1edbi"
     },
+    "4262913073": {
+        "CHS": "\u6cd5\u53e4\u89c2\u51a5",
+        "CHT": "\u6cd5\u53e4\u89c0\u51a5",
+        "DE": "Uralte Heilkunst",
+        "EN": "Ancient Art of Perception",
+        "ES": "Contemplaci\u00f3n at\u00e1vica",
+        "FR": "Perception ancienne",
+        "ID": "Ancient Art of Perception",
+        "IT": "Antica arte della percezione",
+        "JP": "\u53e4\u6cd5\u6545\u8996",
+        "KR": "\uc8fd\uc74c \uace0\ucc30",
+        "PT": "Percep\u00e7\u00e3o Ancestral",
+        "RU": "\u0414\u0440\u0435\u0432\u043d\u0435\u0435 \u0438\u0441\u043a\u0443\u0441\u0441\u0442\u0432\u043e \u0432\u043e\u0441\u043f\u0440\u0438\u044f\u0442\u0438\u044f",
+        "TH": "Ancient Art of Perception",
+        "TR": "Kadim Alg\u0131lama Sanat\u0131",
+        "VI": "Ph\u00e1p C\u1ed5 Quan Minh"
+    },
     "4276933609": {
         "CHS": "\u4f34\u541b\u7720\u82b1\u623f",
         "CHT": "\u4f34\u541b\u7720\u82b1\u623f",
         "DE": "Bettung zur ewigen Ruhe",
         "EN": "Garden of Eternal Rest",
         "ES": "Jard\u00edn del reposo eterno",
         "FR": "Jardin du repos \u00e9ternel",
@@ -6149,14 +6421,31 @@
         "KR": "\uce60\uc131\uc758 \uc544\ub984\ub2f5\uace0 \ucc2c\ub780\ud55c \ube5b",
         "PT": "Grandiosas sejam as Sete Estrelas",
         "RU": "\u0413\u0440\u0430\u043d\u0434\u0438\u043e\u0437\u043d\u043e\u0441\u0442\u044c \u0426\u0438\u0441\u0438\u043d",
         "TH": "Grandeur be the Seven Stars",
         "TR": "Yedi Y\u0131ld\u0131z\u0131n \u0130hti\u015fam\u0131",
         "VI": "Th\u1ea5t Tinh L\u01b0u Quang"
     },
+    "63855777": {
+        "CHS": "\u76c8\u865a\u85cf\u8c61",
+        "CHT": "\u76c8\u865b\u85cf\u8c61",
+        "DE": "Verborgene Ebbe und Flut",
+        "EN": "The Hidden Ebb and Flow",
+        "ES": "S\u00edntomas variables",
+        "FR": "Fluctuations d\u00e9routantes",
+        "ID": "The Hidden Ebb and Flow",
+        "IT": "Gli alti e bassi nascosti",
+        "JP": "\u76c8\u865a\u8535\u8c61",
+        "KR": "\uc228\uc740 \ubcd1",
+        "PT": "Sinais Ocultos da Mudan\u00e7a",
+        "RU": "\u0421\u043e\u043a\u0440\u044b\u0442\u044b\u0435 \u0442\u043e\u043a\u0438",
+        "TH": "The Hidden Ebb and Flow",
+        "TR": "Gizli Metcezir",
+        "VI": "Doanh H\u01b0 T\u00e0ng T\u01b0\u1ee3ng"
+    },
     "652576049": {
         "CHS": "\u73ca\u745a\u4e00\u5fc3",
         "CHT": "\u73ca\u745a\u4e00\u5fc3",
         "DE": "Sango Isshin",
         "EN": "Sango Isshin",
         "ES": "Coraz\u00f3n del coral",
         "FR": "Sango Isshin",
@@ -6574,14 +6863,31 @@
         "KR": "\ub098\uc57d\uc744 \ub5a8\uccd0\ub0b4\ub294 \ub9c8\uc74c",
         "PT": "Evitando a Fraqueza",
         "RU": "\u041e\u0442\u043a\u0430\u0437 \u043e\u0442 \u0441\u043b\u0430\u0431\u043e\u0441\u0442\u0438",
         "TH": "To Ward Weakness",
         "TR": "Zay\u0131fl\u0131\u011f\u0131 Koru",
         "VI": "T\u1eeb B\u1ecf Nhu Nh\u01b0\u1ee3c"
     },
+    "858748369": {
+        "CHS": "\u547f\u541f\u81f3\u5fae",
+        "CHT": "\u547f\u541f\u81f3\u5fae",
+        "DE": "Binnen eines Atemzugs",
+        "EN": "Attentive Observation",
+        "ES": "Cuidados intensivos",
+        "FR": "Regard attentif",
+        "ID": "Attentive Observation",
+        "IT": "Osservazione accurata",
+        "JP": "\u81f3\u5fae\u547b\u541f",
+        "KR": "\uace0\ud1b5 \uac10\uc9c0",
+        "PT": "Observa\u00e7\u00e3o Atenta",
+        "RU": "\u041f\u0440\u0438\u0441\u0442\u0430\u043b\u044c\u043d\u043e\u0435 \u043d\u0430\u0431\u043b\u044e\u0434\u0435\u043d\u0438\u0435",
+        "TH": "Attentive Observation",
+        "TR": "Dikkatli G\u00f6zlem",
+        "VI": "Kh\u01b0 Ng\u00e2m Ch\u00ed Vi"
+    },
     "865989105": {
         "CHS": "\u5b9a\u8499",
         "CHT": "\u5b9a\u8499",
         "DE": "Fixierung des Geistes",
         "EN": "Centered Spirit",
         "ES": "Concentraci\u00f3n espiritual",
         "FR": "Esprit centr\u00e9",
@@ -6797,15 +7103,15 @@
         "RU": "\u041e\u0442\u043a\u0430\u0437 \u043e\u0442 \u0441\u0442\u0440\u0430\u0434\u0430\u043d\u0438\u0439",
         "TH": "To Sequester Sorrow",
         "TR": "Kederi G\u00f6m",
         "VI": "T\u1eeb B\u1ecf Kh\u1ed5 \u0110au"
     },
     "973254489": {
         "CHS": "\u6e38\u51fb\u7684\u5fc3\u5f97",
-        "CHT": "\u904a\u64ca\u7684\u5fc3\u5f97",
+        "CHT": "\u6e38\u64ca\u7684\u5fc3\u5f97",
         "DE": "Guerilla-Erfahrung",
         "EN": "Reconnaissance Experience",
         "ES": "Batidor veterano",
         "FR": "Exp\u00e9rience de reconnaissance",
         "ID": "Reconnaissance Experience",
         "IT": "Esperienza ricognitiva",
         "JP": "\u904a\u6483\u306e\u5fc3\u5f97",
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/langs/fight_props.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/langs/fight_props.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9798076923076924%*

 * *Differences: {"'FIGHT_PROP_ATTACK_PERCENT_A'": '{\'FR\': "Pourcentage d\'ATQ"}',*

 * * "'FIGHT_PROP_DEFENSE_PERCENT_A'": "{'FR': 'Pourcentage de DÉF'}",*

 * * "'FIGHT_PROP_ELEMENT_ADD_HURT'": "OrderedDict([('FR', 'Augmentation des DGT élémentaires "*

 * *                                  "infligés'), ('JP', '元素ダメージアップ'), ('CHT', '造成元素傷害提升'), ('ID', "*

 * *                                  "'Meningkatkan Elemental DMG yang diakibatkan'), ('CHS', "*

 * *                                  "'造成元素伤害提升'), ('VI', 'Tăng sát thương nguyên tố gây ra'), (' […]*

```diff
@@ -69,15 +69,15 @@
     },
     "FIGHT_PROP_ATTACK_PERCENT_A": {
         "CHS": "\u653b\u51fb\u529b\u767e\u5206\u6bd4",
         "CHT": "\u653b\u64ca\u529b\u767e\u5206\u6bd4",
         "DE": "ANG-Rate",
         "EN": "ATK Percentage",
         "ES": "Porcentaje de ATQ",
-        "FR": "Pourcentage ATQ",
+        "FR": "Pourcentage d'ATQ",
         "ID": "ATK%",
         "IT": "Percentuale ATT",
         "JP": "\u653b\u6483\u529b\u30d1\u30fc\u30bb\u30f3\u30c6\u30fc\u30b8",
         "KR": "\uacf5\uaca9\ub825 \ubc31\ubd84\uc728",
         "PT": "Porcentagem de ATQ",
         "RU": "\u041f\u0440\u043e\u0446\u0435\u043d\u0442 \u043e\u0442 \u0441\u0438\u043b\u044b \u0430\u0442\u0430\u043a\u0438",
         "TH": "\u0e40\u0e1b\u0e2d\u0e23\u0e4c\u0e40\u0e0b\u0e47\u0e19\u0e15\u0e4c\u0e1e\u0e25\u0e31\u0e07\u0e42\u0e08\u0e21\u0e15\u0e35",
@@ -307,15 +307,15 @@
     },
     "FIGHT_PROP_DEFENSE_PERCENT_A": {
         "CHS": "\u9632\u5fa1\u529b\u767e\u5206\u6bd4",
         "CHT": "\u9632\u79a6\u529b\u767e\u5206\u6bd4",
         "DE": "VTD-Rate",
         "EN": "DEF Percentage",
         "ES": "Porcentaje de DEF",
-        "FR": "Pourcentage D\u00c9F",
+        "FR": "Pourcentage de D\u00c9F",
         "ID": "DEF%",
         "IT": "Percentuale DIF",
         "JP": "\u9632\u5fa1\u529b\u30d1\u30fc\u30bb\u30f3\u30c6\u30fc\u30b8",
         "KR": "\ubc29\uc5b4\ub825 \ubc31\ubd84\uc728",
         "PT": "Porcentagem de DEF",
         "RU": "\u041f\u0440\u043e\u0446\u0435\u043d\u0442 \u043e\u0442 \u0437\u0430\u0449\u0438\u0442\u044b",
         "TH": "\u0e40\u0e1b\u0e2d\u0e23\u0e4c\u0e40\u0e0b\u0e47\u0e19\u0e15\u0e4c\u0e1e\u0e25\u0e31\u0e07\u0e1b\u0e49\u0e2d\u0e07\u0e01\u0e31\u0e19",
@@ -403,14 +403,31 @@
         "KR": "\ubc88\uac1c \uc6d0\uc18c \ub0b4\uc131",
         "PT": "RES Electro",
         "RU": "\u042d\u043b\u0435\u043a\u0442\u0440\u043e \u0441\u043e\u043f\u0440\u043e\u0442\u0438\u0432\u043b\u0435\u043d\u0438\u0435",
         "TH": "\u0e04\u0e27\u0e32\u0e21\u0e15\u0e49\u0e32\u0e19\u0e17\u0e32\u0e19\u0e44\u0e1f\u0e1f\u0e49\u0e32",
         "TR": "Elektrik Direnci",
         "VI": "Kh\u00e1ng Nguy\u00ean T\u1ed1 L\u00f4i"
     },
+    "FIGHT_PROP_ELEMENT_ADD_HURT": {
+        "CHS": "\u9020\u6210\u5143\u7d20\u4f24\u5bb3\u63d0\u5347",
+        "CHT": "\u9020\u6210\u5143\u7d20\u50b7\u5bb3\u63d0\u5347",
+        "DE": "Erh\u00f6ht den verursachten Elementar-SCH.",
+        "EN": "Increases Elemental DMG dealt",
+        "ES": "Aumento del Da\u00f1o Elemental",
+        "FR": "Augmentation des DGT \u00e9l\u00e9mentaires inflig\u00e9s",
+        "ID": "Meningkatkan Elemental DMG yang diakibatkan",
+        "IT": "Aumenta i DAN elementali inflitti",
+        "JP": "\u5143\u7d20\u30c0\u30e1\u30fc\u30b8\u30a2\u30c3\u30d7",
+        "KR": "\uac00\ud558\ub294 \uc6d0\uc18c \ud53c\ud574 \uc99d\uac00",
+        "PT": "Aumenta o Dano Elemental causado",
+        "RU": "\u0423\u0432\u0435\u043b\u0438\u0447\u0438\u0432\u0430\u0435\u0442 \u044d\u043b\u0435\u043c\u0435\u043d\u0442\u0430\u043b\u044c\u043d\u044b\u0439 \u0443\u0440\u043e\u043d",
+        "TH": "\u0e04\u0e27\u0e32\u0e21\u0e40\u0e2a\u0e35\u0e22\u0e2b\u0e32\u0e22\u0e18\u0e32\u0e15\u0e38\u0e08\u0e30\u0e40\u0e1e\u0e34\u0e48\u0e21\u0e02\u0e36\u0e49\u0e19",
+        "TR": "Verilen Element Hasar\u0131n\u0131 art\u0131r\u0131r",
+        "VI": "T\u0103ng s\u00e1t th\u01b0\u01a1ng nguy\u00ean t\u1ed1 g\u00e2y ra"
+    },
     "FIGHT_PROP_ELEMENT_MASTERY": {
         "CHS": "\u5143\u7d20\u7cbe\u901a",
         "CHT": "\u5143\u7d20\u7cbe\u901a",
         "DE": "Elementarkunde",
         "EN": "Elemental Mastery",
         "ES": "Maestr\u00eda Elemental",
         "FR": "Ma\u00eetrise \u00e9l\u00e9mentaire",
@@ -579,15 +596,15 @@
     },
     "FIGHT_PROP_HP_PERCENT_A": {
         "CHS": "\u751f\u547d\u503c\u767e\u5206\u6bd4",
         "CHT": "\u751f\u547d\u503c\u767e\u5206\u6bd4",
         "DE": "LP-Rate",
         "EN": "HP Percentage",
         "ES": "Porcentaje de Vida",
-        "FR": "Pourcentage PV",
+        "FR": "Pourcentage de PV",
         "ID": "HP%",
         "IT": "Percentuale PS",
         "JP": "HP\u30d1\u30fc\u30bb\u30f3\u30c6\u30fc\u30b8",
         "KR": "HP \ubc31\ubd84\uc728",
         "PT": "Porcentagem de Vida",
         "RU": "\u041f\u0440\u043e\u0446\u0435\u043d\u0442 \u043e\u0442 HP",
         "TH": "\u0e40\u0e1b\u0e2d\u0e23\u0e4c\u0e40\u0e0b\u0e47\u0e19\u0e15\u0e4c\u0e1e\u0e25\u0e31\u0e07\u0e0a\u0e35\u0e27\u0e34\u0e15",
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/langs/namecards.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/langs/namecards.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9432914046121592%*

 * *Differences: {"'110943356'": "OrderedDict([('FR', 'Succès - Crépuscule éphémère'), ('JP', 'アチーブメント·木槿の誰そ彼'), "*

 * *                "('CHT', '成就·槿暮'), ('ID', 'Achievement: Senja Fana'), ('CHS', '成就·槿暮'), ('VI', "*

 * *                "'Thành Tựu - Chạng Vạng'), ('ES', 'Logro - Atardecer efímero'), ('TH', "*

 * *                "'ความสำเร็จ - พลบค่ำฉับพลัน'), ('TR', 'Başarım: Gelip Geçici Alacakaranlık'), "*

 * *                "('KR', '업적·밤에 지는 꽃'), ('DE', 'Errungenschaft – Vergänglichkeit'), ('RU', 'Сумерки "*

 * *                "перехода'),  […]*

```diff
@@ -114,14 +114,31 @@
         "KR": "\uc0ac\uc774\ub178\u00b7\uce68\ubb35",
         "PT": "Cyno \u2014 Serenidade",
         "RU": "\u0421\u043f\u043e\u043a\u043e\u0439\u0441\u0442\u0432\u0438\u0435",
         "TH": "Cyno - \u0e40\u0e07\u0e35\u0e22\u0e1a\u0e02\u0e23\u0e36\u0e21",
         "TR": "Cyno: Sessizlik",
         "VI": "Cyno - Y\u00ean L\u1eb7ng"
     },
+    "110943356": {
+        "CHS": "\u6210\u5c31\u00b7\u69ff\u66ae",
+        "CHT": "\u6210\u5c31\u00b7\u69ff\u66ae",
+        "DE": "Errungenschaft \u2013 Verg\u00e4nglichkeit",
+        "EN": "Achievement: Transient Twilight",
+        "ES": "Logro - Atardecer ef\u00edmero",
+        "FR": "Succ\u00e8s - Cr\u00e9puscule \u00e9ph\u00e9m\u00e8re",
+        "ID": "Achievement: Senja Fana",
+        "IT": "Obiettivo: Crepuscolo transiente",
+        "JP": "\u30a2\u30c1\u30fc\u30d6\u30e1\u30f3\u30c8\u00b7\u6728\u69ff\u306e\u8ab0\u305d\u5f7c",
+        "KR": "\uc5c5\uc801\u00b7\ubc24\uc5d0 \uc9c0\ub294 \uaf43",
+        "PT": "Conquista: Entardecer Transit\u00f3rio",
+        "RU": "\u0421\u0443\u043c\u0435\u0440\u043a\u0438 \u043f\u0435\u0440\u0435\u0445\u043e\u0434\u0430",
+        "TH": "\u0e04\u0e27\u0e32\u0e21\u0e2a\u0e33\u0e40\u0e23\u0e47\u0e08 - \u0e1e\u0e25\u0e1a\u0e04\u0e48\u0e33\u0e09\u0e31\u0e1a\u0e1e\u0e25\u0e31\u0e19",
+        "TR": "Ba\u015far\u0131m: Gelip Ge\u00e7ici Alacakaranl\u0131k",
+        "VI": "Th\u00e0nh T\u1ef1u - Ch\u1ea1ng V\u1ea1ng"
+    },
     "1185661092": {
         "CHS": "\u91cd\u4e91\u00b7\u7075\u5203",
         "CHT": "\u91cd\u96f2\u00b7\u9748\u5203",
         "DE": "Chongyun \u2013 Seelenklinge",
         "EN": "Chongyun: Spirit Blade",
         "ES": "Chongyun - Filo espiritual",
         "FR": "Chongyun - Lame de l'esprit",
@@ -556,14 +573,31 @@
         "KR": "\uae30\ud589\u00b7\ucd95\uc6d4",
         "PT": "#Passe de Batalha: {F#Seguidora}{M#Seguidor} da Lua",
         "RU": "\u041b\u0443\u043d\u043d\u0430\u044f \u043e\u0445\u043e\u0442\u0430",
         "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e44\u0e25\u0e48\u0e25\u0e48\u0e32\u0e41\u0e2a\u0e07\u0e08\u0e31\u0e19\u0e17\u0e23\u0e32",
         "TR": "Gezi Notlar\u0131: Ay Pe\u015finde",
         "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - Tr\u1ee5c Nguy\u1ec7t"
     },
+    "1790614036": {
+        "CHS": "\u987b\u5f25\u00b7\u5927\u68a6",
+        "CHT": "\u9808\u5f4c\u00b7\u5927\u5922",
+        "DE": "Sumeru \u2013 Gro\u00dfer Traum",
+        "EN": "Sumeru: The Great Dream",
+        "ES": "Sumeru - Grandes quimeras",
+        "FR": "Sumeru - Grand r\u00eave",
+        "ID": "Sumeru: Mimpi Indah",
+        "IT": "Sumeru: Il Gran Sogno",
+        "JP": "\u30b9\u30e1\u30fc\u30eb\u00b7\u5927\u5922",
+        "KR": "\uc218\uba54\ub974\u00b7\ud070 \uafc8",
+        "PT": "Sumeru: Grandes Sonhos",
+        "RU": "\u0411\u043e\u043b\u044c\u0448\u0430\u044f \u043c\u0435\u0447\u0442\u0430",
+        "TH": "Sumeru - \u0e04\u0e27\u0e32\u0e21\u0e1d\u0e31\u0e19\u0e2d\u0e31\u0e19\u0e22\u0e34\u0e48\u0e07\u0e43\u0e2b\u0e0d\u0e48",
+        "TR": "Sumeru: B\u00fcy\u00fck R\u00fcya",
+        "VI": "Sumeru - Gi\u1ea5c M\u1ed9ng"
+    },
     "179136692": {
         "CHS": "\u96f7\u6cfd\u00b7\u5954\u72fc",
         "CHT": "\u96f7\u6fa4\u00b7\u5954\u72fc",
         "DE": "Razor \u2013 Laufender Wolf",
         "EN": "Razor: Wolvensprint",
         "ES": "Razor - Velocidad de lobo",
         "FR": "Razor - Affaire de loups",
@@ -862,19 +896,36 @@
         "KR": "\uc885\ub824\u00b7\ucc9c\uc131",
         "PT": "Zhongli - Chuva Estelar",
         "RU": "\u041f\u0430\u0434\u0435\u043d\u0438\u0435 \u043a\u043e\u043c\u0435\u0442\u044b",
         "TH": "Zhongli - Planet Befall",
         "TR": "Zhongli: D\u00fc\u015fen Gezegen",
         "VI": "Zhongli - Thi\u00ean Tinh"
     },
+    "2371279924": {
+        "CHS": "\u7eee\u826f\u826f\u00b7\u732b\u7bb1",
+        "CHT": "\u7dba\u826f\u826f\u00b7\u8c93\u7bb1",
+        "DE": "Kirara \u2013 Neko-Kiste",
+        "EN": "Kirara: Neko Box",
+        "ES": "Kirara - Paquete minino",
+        "FR": "Kirara - Neko-colis",
+        "ID": "Kirara: Neko Box",
+        "IT": "Kirara: Nekoscatola",
+        "JP": "\u7dba\u826f\u3005\u00b7\u732b\u7bb1",
+        "KR": "\ud0a4\ub77c\ub77c\u00b7\ub0e5\ub0e5 \uc0c1\uc790",
+        "PT": "Kirara - Caixa para Gatos",
+        "RU": "\u041f\u043e\u0441\u044b\u043b\u043a\u0430 \u043d\u044d\u043a\u043e",
+        "TH": "Kirara - \u0e01\u0e25\u0e48\u0e2d\u0e07\u0e41\u0e21\u0e27",
+        "TR": "Kirara: Neko Kutusu",
+        "VI": "Kirara - B\u01b0u Ki\u1ec7n M\u00e8o"
+    },
     "2373252516": {
         "CHS": "\u574e\u8482\u4e1d\u00b7\u82cd\u9e6d",
         "CHT": "\u574e\u8482\u7d72\u00b7\u84bc\u9dfa",
         "DE": "Candace \u2013 Graureiher",
-        "EN": "Candace: Grey Heron",
+        "EN": "Candace: Gray Heron",
         "ES": "Candace - Garza real",
         "FR": "Candace - H\u00e9ronne cendr\u00e9e",
         "ID": "Candace: Grey Heron",
         "IT": "Candace: Airone grigio",
         "JP": "\u30ad\u30e3\u30f3\u30c7\u30a3\u30b9\u00b7\u84bc\u9dfa",
         "KR": "\uce94\ub514\uc2a4\u00b7\ud478\ub978\ube5b \uc0c8",
         "PT": "Candace \u2014 Gar\u00e7a Cinza",
@@ -998,14 +1049,31 @@
         "KR": "\ud074\ub808\u00b7\ud3ed\ud0c4",
         "PT": "Klee - Explosivo",
         "RU": "\u0411\u043e\u043c\u0431\u043e\u0447\u043a\u0430",
         "TH": "Klee - Explosive",
         "TR": "Klee: Patlay\u0131c\u0131",
         "VI": "Klee - Thu\u1ed1c N\u1ed5"
     },
+    "252168660": {
+        "CHS": "\u7eaa\u884c\u00b7\u79d8\u5178",
+        "CHT": "\u7d00\u884c\u00b7\u79d8\u5178",
+        "DE": "Erlebnispass \u2013 Kodex",
+        "EN": "Travel Notes: Secrets",
+        "ES": "#PB{NON_BREAK_SPACE}-{NON_BREAK_SPACE}As de la invocaci\u00f3n",
+        "FR": "PB - Secret d'invoqueur",
+        "ID": "Catatan Perjalanan: Rahasia Pemanggil",
+        "IT": "Appunti di viaggio: Segreti",
+        "JP": "\u7d00\u884c\u00b7\u79d8\u5178",
+        "KR": "\uae30\ud589\u00b7\ube44\uc804",
+        "PT": "Passe de Batalha: Segredo do Invocador",
+        "RU": "\u0421\u0435\u043a\u0440\u0435\u0442\u044b",
+        "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e04\u0e27\u0e32\u0e21\u0e25\u0e31\u0e1a",
+        "TR": "Gezi Notlar\u0131: S\u0131rlar",
+        "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - Tri\u1ec7u H\u1ed3i"
+    },
     "2541715356": {
         "CHS": "\u963f\u8d1d\u591a\u00b7\u9633\u82b1",
         "CHT": "\u963f\u8c9d\u591a\u00b7\u967d\u82b1",
         "DE": "Albedo \u2013 Sonneneruption",
         "EN": "Albedo: Sun Blossom",
         "ES": "Albedo - Flor solar",
         "FR": "Albedo - Radiance solaire",
@@ -1049,14 +1117,31 @@
         "KR": "\uae30\ud589\u00b7\ud654\uc74c",
         "PT": "Passe de Batalha: Eufonia",
         "RU": "\u0411\u043b\u0430\u0433\u043e\u0437\u0432\u0443\u0447\u0438\u0435",
         "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e2a\u0e31\u0e21\u0e1c\u0e31\u0e2a\u0e04\u0e25\u0e49\u0e2d\u0e07",
         "TR": "Gezi Notlar\u0131: Ritim ve Kafiye",
         "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - H\u00f2a T\u1ea5u"
     },
+    "2684456012": {
+        "CHS": "\u5361\u7ef4\u00b7\u7a79\u5ead",
+        "CHT": "\u5361\u7dad\u00b7\u7a79\u5ead",
+        "DE": "Kaveh \u2013 Firmament",
+        "EN": "Kaveh: Domed Court",
+        "ES": "Kaveh - Alc\u00e1zar abovedado",
+        "FR": "Kaveh - Firmament",
+        "ID": "Kaveh: Domed Court",
+        "IT": "Kaveh: Corte con cupola",
+        "JP": "\u30ab\u30fc\u30f4\u30a7\u00b7\u5929\u7a79\u306e\u5ead",
+        "KR": "\uce74\ubca0\u00b7\ud558\ub298\uc758 \ub3d4",
+        "PT": "Kaveh: Pal\u00e1cio Abobadado",
+        "RU": "\u0421\u0432\u043e\u0434\u0447\u0430\u0442\u044b\u0439 \u0434\u0432\u043e\u0440\u0435\u0446",
+        "TH": "Kaveh - \u0e42\u0e14\u0e21\u0e19\u0e20\u0e32",
+        "TR": "Kaveh: Kubbeli Saray",
+        "VI": "Kaveh - V\u00f2m Tr\u1eddi"
+    },
     "273890284": {
         "CHS": "\u5b89\u67cf\u00b7\u5154\u5154",
         "CHT": "\u5b89\u67cf\u00b7\u5154\u5154",
         "DE": "Amber \u2013 Hoppel",
         "EN": "Amber: Bunny",
         "ES": "Amber - Bar\u00f3n Bunny",
         "FR": "Amber - Baron Lapinou",
@@ -1083,14 +1168,31 @@
         "KR": "\uc57c\ub780\u00b7\uc77c\ucc99",
         "PT": "Yelan: Lan\u00e7amento",
         "RU": "\u0411\u0440\u043e\u0441\u043e\u043a",
         "TH": "Yelan - \u0e40\u0e17\u0e2b\u0e21\u0e14\u0e2b\u0e19\u0e49\u0e32\u0e15\u0e31\u0e01",
         "TR": "Yelan: Zar",
         "VI": "Yelan - \u0110\u1ed5 X\u00fac X\u1eafc"
     },
+    "2816803308": {
+        "CHS": "\u767d\u672f\u00b7\u795b\u98ce",
+        "CHT": "\u767d\u672e\u00b7\u795b\u98a8",
+        "DE": "Baizhu \u2013 Vorbeugung",
+        "EN": "Baizhu: Relief",
+        "ES": "Baizhu - Mitigaci\u00f3n",
+        "FR": "Baizhu - Soulagement",
+        "ID": "Baizhu: Relief",
+        "IT": "Baizhu: Sollievo",
+        "JP": "\u767d\u672e\u00b7\u53bb\u98a8",
+        "KR": "\ubc31\ucd9c\u00b7\uac70\ud48d",
+        "PT": "Baizhu: Al\u00edvio",
+        "RU": "\u041e\u0431\u043b\u0435\u0433\u0447\u0435\u043d\u0438\u0435",
+        "TH": "Baizhu - \u0e02\u0e31\u0e1a\u0e25\u0e21\u0e1b\u0e23\u0e32\u0e13",
+        "TR": "Baizhu: Rahatlama",
+        "VI": "Baizhu - Kh\u01b0 Phong"
+    },
     "2849383404": {
         "CHS": "\u7533\u9e64\u00b7\u6809\u63a0",
         "CHT": "\u7533\u9db4\u00b7\u6adb\u63a0",
         "DE": "Shenhe \u2013 Kamm",
         "EN": "Shenhe: Comb",
         "ES": "Shenhe - Acicalamiento",
         "FR": "Shenhe - Peigne",
@@ -1321,14 +1423,31 @@
         "KR": "\ub370\ud788\uc57c\u00b7\uc815\ud654\uc758 \ubd88\uaf43",
         "PT": "Dehya - Chama Purificadora",
         "RU": "\u041e\u0447\u0438\u0449\u0430\u044e\u0449\u0435\u0435 \u043f\u043b\u0430\u043c\u044f",
         "TH": "Dehya - \u0e40\u0e1e\u0e25\u0e34\u0e07\u0e1c\u0e25\u0e32\u0e0d",
         "TR": "Dehya: Ar\u0131nd\u0131r\u0131c\u0131 Alev",
         "VI": "Dehya - L\u1eeda Thi\u00eang"
     },
+    "3159539884": {
+        "CHS": "\u987b\u5f25\u00b7\u7518\u9732",
+        "CHT": "\u9808\u5f4c\u00b7\u7518\u9732",
+        "DE": "Sumeru \u2013 Amrita",
+        "EN": "Sumeru: Amrita",
+        "ES": "Sumeru - Man\u00e1",
+        "FR": "Sumeru - Amrita",
+        "ID": "Sumeru: Amrita",
+        "IT": "Sumeru: Amrita",
+        "JP": "\u30b9\u30e1\u30fc\u30eb\u00b7\u7518\u9732",
+        "KR": "\uc218\uba54\ub974\u00b7\uac10\ub85c",
+        "PT": "Sumeru\u00b7Amrita",
+        "RU": "\u0410\u043c\u0440\u0438\u0442\u0430",
+        "TH": "Sumeru - \u0e2b\u0e22\u0e32\u0e14\u0e2d\u0e21\u0e24\u0e15",
+        "TR": "Sumeru: Amrita",
+        "VI": "Sumeru - Amrita"
+    },
     "3188840620": {
         "CHS": "\u7eaa\u884c\u00b7\u5929\u547d",
         "CHT": "\u7d00\u884c\u00b7\u5929\u547d",
         "DE": "Erlebnispass \u2013 Himmlischer Wille",
         "EN": "Travel Notes: Divine Will",
         "ES": "PB - Destino",
         "FR": "PB - Destin\u00e9e",
@@ -1678,14 +1797,31 @@
         "KR": "\uc5c5\uc801\u00b7\uc77c\uacf1 \uac1c\uc758 \ube5b",
         "PT": "Conquista: Sete Luzes",
         "RU": "\u0421\u0435\u043c\u044c \u043b\u0443\u0447\u0435\u0439",
         "TH": "\u0e04\u0e27\u0e32\u0e21\u0e2a\u0e33\u0e40\u0e23\u0e47\u0e08 - \u0e41\u0e2a\u0e07\u0e17\u0e31\u0e49\u0e07\u0e40\u0e08\u0e47\u0e14",
         "TR": "Ba\u015far\u0131m: Yedi I\u015f\u0131k",
         "VI": "Th\u00e0nh T\u1ef1u - B\u1ea3y Tia S\u00e1ng"
     },
+    "370573972": {
+        "CHS": "\u6210\u5c31\u00b7\u4e07\u79cd",
+        "CHT": "\u6210\u5c31\u00b7\u842c\u7a2e",
+        "DE": "Errungenschaft \u2013 Unendliche Samen",
+        "EN": "Achievement: Infinitum",
+        "ES": "Logro - Semillas infinitas",
+        "FR": "Succ\u00e8s - Myriade",
+        "ID": "Achievement: Tanpa Batas",
+        "IT": "Obiettivo: Infinitum",
+        "JP": "\u30a2\u30c1\u30fc\u30d6\u30e1\u30f3\u30c8\u00b7\u4e07\u7a2e",
+        "KR": "\uc5c5\uc801\u00b7\ubaa8\ub4e0 \uc528\uc557",
+        "PT": "Conquista: Infinitas Sementes",
+        "RU": "\u0411\u0435\u0441\u043a\u043e\u043d\u0435\u0447\u043d\u043e\u0441\u0442\u044c",
+        "TH": "\u0e04\u0e27\u0e32\u0e21\u0e2a\u0e33\u0e40\u0e23\u0e47\u0e08 - \u0e2a\u0e23\u0e23\u0e1e\u0e2a\u0e34\u0e48\u0e07",
+        "TR": "Ba\u015far\u0131m: Sonsuz",
+        "VI": "Th\u00e0nh T\u1ef1u - V\u1ea1n Ch\u1ee7ng"
+    },
     "3706272004": {
         "CHS": "\u5e86\u5178\u00b7\u9b54\u7403",
         "CHT": "\u6176\u5178\u00b7\u9b54\u7403",
         "DE": "Feierlichkeit \u2013 Bumm-Bumm-Ball",
         "EN": "Celebration: Kaboomball",
         "ES": "Celebraci\u00f3n - Bombabum",
         "FR": "C\u00e9l\u00e9bration - Badaboum",
@@ -2290,14 +2426,31 @@
         "KR": "\uae30\ud589\u00b7\uc2e0\uc7a5(\u795e\u5c07)",
         "PT": "Passe de Batalha: General Divino",
         "RU": "\u0411\u043e\u0436\u0435\u0441\u0442\u0432\u0435\u043d\u043d\u044b\u0439 \u0433\u0435\u043d\u0435\u0440\u0430\u043b",
         "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e41\u0e21\u0e48\u0e17\u0e31\u0e1e\u0e41\u0e2b\u0e48\u0e07\u0e2a\u0e23\u0e27\u0e07\u0e2a\u0e27\u0e23\u0e23\u0e04\u0e4c",
         "TR": "Gezi Notlar\u0131: E\u015fsiz General",
         "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - Th\u1ea7n T\u01b0\u1edbng"
     },
+    "641457676": {
+        "CHS": "\u7eaa\u884c\u00b7\u8363\u5195",
+        "CHT": "\u7d00\u884c\u00b7\u69ae\u5195",
+        "DE": "Erlebnispass \u2013 Blumenkranz",
+        "EN": "Travel Notes: Crown of Glory",
+        "ES": "PB - Corona de la eminencia",
+        "FR": "PB - Lauriers",
+        "ID": "Catatan Perjalanan: Mahkota Kemuliaan",
+        "IT": "Appunti di viaggio: Corona gloriosa",
+        "JP": "\u7d00\u884c\u00b7\u6804\u51a0",
+        "KR": "\uae30\ud589\u00b7\uc601\uad11\uc758 \uad00",
+        "PT": "Passe de Batalha: Coroa Gloriosa",
+        "RU": "\u041a\u043e\u0440\u043e\u043d\u0430 \u0441\u043b\u0430\u0432\u044b",
+        "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e21\u0e07\u0e01\u0e38\u0e0e\u0e40\u0e01\u0e35\u0e22\u0e23\u0e15\u0e34\u0e22\u0e28",
+        "TR": "Gezi Notlar\u0131: \u0130hti\u015fam Tac\u0131",
+        "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - V\u01b0\u01a1ng Mi\u1ec7n"
+    },
     "705455564": {
         "CHS": "\u63d0\u7eb3\u91cc\u00b7\u6c90\u9732",
         "CHT": "\u63d0\u7d0d\u91cc\u00b7\u6c90\u9732",
         "DE": "Tighnari \u2013 Vom Tau gek\u00fcsst",
         "EN": "Tighnari: Dew-Kissed",
         "ES": "Tignari - Roc\u00edo",
         "FR": "Tighnari - Baign\u00e9 de ros\u00e9e",
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/langs/skills.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/langs/skills.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9645752895752897%*

 * *Differences: {"'1011789509'": "OrderedDict([('FR', ''), ('JP', ''), ('CHT', ''), ('ID', ''), ('CHS', "*

 * *                 "'绮良良空中攻击'), ('VI', ''), ('ES', ''), ('TH', ''), ('TR', ''), ('KR', ''), ('DE', "*

 * *                 "''), ('RU', ''), ('IT', ''), ('EN', ''), ('PT', '')])",*

 * * "'1063935965'": "{'ID': 'Normal Attack: Foreign Rockblade'}",*

 * * "'1210107733'": "OrderedDict([('FR', 'Dôme peint'), ('JP', 'ムカルナスの描像'), ('CHT', '繁繪隅穹'), ('ID', "*

 * *                 "'Painted Dome'), ('CHS', '繁绘隅穹'), ('VI', 'Mái Vòm Rực Rỡ'), ('ES', 'B […]*

```diff
@@ -1,8 +1,25 @@
 {
+    "1011789509": {
+        "CHS": "\u7eee\u826f\u826f\u7a7a\u4e2d\u653b\u51fb",
+        "CHT": "",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "1050865533": {
         "CHS": "\u6d1e\u5bdf\u5168\u5c40",
         "CHT": "\u6d1e\u5bdf\u5168\u5c40",
         "DE": "R\u00f6ntgenaugen",
         "EN": "Insight",
         "ES": "Vista de conjunto",
         "FR": "Perception",
@@ -87,15 +104,15 @@
     "1063935965": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5f02\u90a6\u5ca9\u950b",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u7570\u90a6\u5ca9\u92d2",
         "DE": "Standardangriff: Steinerne Klinge aus der Fremde",
         "EN": "Normal Attack: Foreign Rockblade",
         "ES": "Ataque Normal: Espada de piedra extranjera",
         "FR": "Attaque normale : Lame de roche",
-        "ID": "Foreign Rockblade",
+        "ID": "Normal Attack: Foreign Rockblade",
         "IT": "Attacco normale: Lamaroccia straniera",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u7570\u90a6\u306e\u5ca9\u5cf0",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc774\uad6d\uc758 \uc554\ubd09",
         "PT": "Ataque Normal: L\u00e2mina de Rocha Estrangeira",
         "RU": "\u041a\u0430\u043c\u0435\u043d\u043d\u044b\u0439 \u043c\u0435\u0447 \u0438\u043d\u043e\u0437\u0435\u043c\u0446\u0430",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Foreign Rockblade",
         "TR": "Normal Sald\u0131r\u0131: Yabanc\u0131 Ta\u015f K\u0131l\u0131c\u0131",
@@ -471,14 +488,31 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "1210107733": {
+        "CHS": "\u7e41\u7ed8\u9685\u7a79",
+        "CHT": "\u7e41\u7e6a\u9685\u7a79",
+        "DE": "Dimension der \u00e4sthetischen Vermessung",
+        "EN": "Painted Dome",
+        "ES": "B\u00f3veda policromada",
+        "FR": "D\u00f4me peint",
+        "ID": "Painted Dome",
+        "IT": "Volta dipinta",
+        "JP": "\u30e0\u30ab\u30eb\u30ca\u30b9\u306e\u63cf\u50cf",
+        "KR": "\ud558\ub298 \ucc44\uc0c9",
+        "PT": "Pal\u00e1cio Resplandecente",
+        "RU": "\u0420\u0430\u0441\u043f\u0438\u0441\u043d\u043e\u0439 \u043a\u0443\u043f\u043e\u043b",
+        "TH": "Painted Dome",
+        "TR": "Boyal\u0131 Kubbe",
+        "VI": "M\u00e1i V\u00f2m R\u1ef1c R\u1ee1"
+    },
     "1213295293": {
         "CHS": "\u7fbd\u7403\u8282-\u7834\u76fe",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -884,15 +918,15 @@
         "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - V\u0169 \u0110i\u1ec7u Samser"
     },
     "1422444957": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u795e\u5c04\u624b",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u795e\u5c04\u624b",
         "DE": "Standardangriff: Scharfsch\u00fctze",
         "EN": "Normal Attack: Sharpshooter",
-        "ES": "Ataque Normal: Arquero divino",
+        "ES": "Ataque Normal: As de la arquer\u00eda",
         "FR": "Attaque normale : Archerie revisit\u00e9e",
         "ID": "Normal Attack: Sharpshooter",
         "IT": "Attacco normale: Tiratore scelto",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u4e00\u6d41\u5c04\u624b",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc2e0\uad81",
         "PT": "Ataque Normal: Pontaria",
         "RU": "\u041f\u0435\u0440\u0432\u043e\u043a\u043b\u0430\u0441\u0441\u043d\u044b\u0439 \u0441\u0442\u0440\u0435\u043b\u043e\u043a",
@@ -1168,14 +1202,31 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "1538181693": {
+        "CHS": "3.8\u8fc7\u5c71\u8f66-\u8dc3\u8fc1",
+        "CHT": "",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "1543775045": {
         "CHS": "\u6293\u732b\u6254\u9c7c",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -1209,15 +1260,15 @@
     "1555695317": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u6c34\u4e4b\u6d45\u5531",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u6c34\u4e4b\u6dfa\u5531",
         "DE": "Standardangriff: Stille Wasser",
         "EN": "Normal Attack: Whisper of Water",
         "ES": "Ataque Normal: Murmullo del agua",
         "FR": "Attaque normale : Murmure de l'eau",
-        "ID": "Whisper of Water",
+        "ID": "Normal Attack: Whisper of Water",
         "IT": "Attacco normale: Sussurro d'acqua",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u6c34\u306e\u56c1\u304d",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\ubb3c\uc758 \ub178\ub798",
         "PT": "Ataque Normal: Suspiro da \u00c1gua",
         "RU": "\u0428\u0451\u043f\u043e\u0442 \u0432\u043e\u0434\u044b",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Whisper of Water",
         "TR": "Normal Sald\u0131r\u0131: Suyun F\u0131s\u0131lt\u0131s\u0131",
@@ -2324,14 +2375,48 @@
         "KR": "\ube59\ud3ed\uad81",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "2089915453": {
+        "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u7bb1\u7eb8\u5207\u524a\u672f",
+        "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u7bb1\u7d19\u5207\u524a\u8853",
+        "DE": "Standardangriff: Kartonschnitt",
+        "EN": "Normal Attack: Boxcutter",
+        "ES": "Ataque Normal: Kirigami",
+        "FR": "Attaque normale : Ouvre-colis",
+        "ID": "Normal Attack: Boxcutter",
+        "IT": "Attacco normale: Trincetto",
+        "JP": "\u901a\u5e38\u653b\u6483\u00b7\u6bb5\u677f\u7d19\u00b7\u5207\u308a\u88c2\u304d\u8853",
+        "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc885\uc774\uc0c1\uc790 \uc808\ub2e8\uc220",
+        "PT": "Ataque Normal: Estilete",
+        "RU": "\u041d\u0430\u0440\u0435\u0437\u043a\u0430 \u043a\u043e\u0440\u043e\u0431\u043e\u043a",
+        "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Boxcutter",
+        "TR": "Normal Sald\u0131r\u0131: Maket B\u0131\u00e7a\u011f\u0131",
+        "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - C\u00e0o R\u00e1ch H\u1ed9p"
+    },
+    "2101931541": {
+        "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u65cb\u89c4\u8bbe\u77e9",
+        "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u65cb\u898f\u8a2d\u77e9",
+        "DE": "Standardangriff: Drehmomenteinstellung",
+        "EN": "Normal Attack: Schematic Setup",
+        "ES": "Ataque Normal: Boceto esquem\u00e1tico",
+        "FR": "Attaque normale : Configuration sch\u00e9matique",
+        "ID": "Normal Attack: Schematic Setup",
+        "IT": "Attacco normale: Installazione schematica",
+        "JP": "\u901a\u5e38\u653b\u6483\u00b7\u5186\u898f\u5b9a\u5247",
+        "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\ud68c\uc804 \uce21\ub7c9",
+        "PT": "Ataque Normal: Configura\u00e7\u00e3o Esquem\u00e1tica",
+        "RU": "\u0421\u0445\u0435\u043c\u0430\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u043d\u0430\u0441\u0442\u0440\u043e\u0439\u043a\u0430",
+        "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Schematic Setup",
+        "TR": "Normal Sald\u0131r\u0131: \u0130zd\u00fc\u015f\u00fcm D\u00fczlemi",
+        "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - Thi\u1ebft L\u1eadp L\u1ef1c Quay"
+    },
     "2104569853": {
         "CHS": "\u5b89\u67cf\u7a7a\u4e2d\u8fde\u5c04",
         "CHT": "\u5b89\u67cf\u7a7a\u4e2d\u9023\u5c04",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -2365,15 +2450,15 @@
     "2119081949": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5ca9\u96e8",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u5ca9\u96e8",
         "DE": "Standardangriff: Steinhagel",
         "EN": "Normal Attack: Rain of Stone",
         "ES": "Ataque Normal: Lluvia p\u00e9trea",
         "FR": "Attaque normale : Pluie de pierres",
-        "ID": "Rain of Stone",
+        "ID": "Normal Attack: Rain of Stone",
         "IT": "Attacco normale: Pioggia di pietra",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u5ca9\u96e8",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\ubc14\uc704 \ube44",
         "PT": "Ataque Normal: Chuva de Pedras",
         "RU": "\u041a\u0430\u043c\u0435\u043d\u043d\u044b\u0439 \u0434\u043e\u0436\u0434\u044c",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Rain of Stone",
         "TR": "Normal Sald\u0131r\u0131: Ta\u015f Ya\u011fmuru",
@@ -2460,14 +2545,31 @@
         "KR": "\uc131\uc2a4\ub7ec\uc6b4 \uc758\uc2dd\u00b7\ud478\ub978\ube5b \uc0c8\uc758 \ube44\ud638",
         "PT": "Ritual Sagrado: Gar\u00e7a Guardi\u00e3",
         "RU": "\u0421\u0432\u044f\u0449\u0435\u043d\u043d\u044b\u0439 \u043e\u0431\u0440\u044f\u0434: \u041e\u0431\u0438\u0442\u0435\u043b\u044c \u0446\u0430\u043f\u043b\u0438",
         "TH": "Sacred Rite: Heron's Sanctum",
         "TR": "Kutsal Ayin: Bal\u0131k\u00e7\u0131l Kalkan\u0131",
         "VI": "Nghi Th\u1ee9c Th\u1ea7n Th\u00e1nh - V\u1ea1c Tr\u1eddi B\u1ea3o H\u1ed9"
     },
+    "2174036525": {
+        "CHS": "3.8\u8fc7\u5c71\u8f66-\u53f3\u653b\u51fb",
+        "CHT": "",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "2178272253": {
         "CHS": "\u65cb\u4e91\u5f00\u76f8",
         "CHT": "\u65cb\u96f2\u958b\u76f8",
         "DE": "Wolken\u00f6ffnung",
         "EN": "Opening Flourish",
         "ES": "Disipadora de nimbos",
         "FR": "\u00c9panouissement ouvert",
@@ -2501,15 +2603,15 @@
     "2182891949": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5f02\u90a6\u94c1\u98ce",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u7570\u90a6\u9435\u98a8",
         "DE": "Standardangriff: Eiserner Wind aus der Fremde",
         "EN": "Normal Attack: Foreign Ironwind",
         "ES": "Ataque Normal: Viento met\u00e1lico extranjero",
         "FR": "Attaque normale : Vents de la discorde",
-        "ID": "Foreign Ironwind",
+        "ID": "Normal Attack: Foreign Ironwind",
         "IT": "Attacco normale: Ferrovento straniero",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u7570\u90a6\u306e\u9244\u98a8",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc774\uad6d\uc758 \uac15\ucca0\ubc14\ub78c",
         "PT": "Ataque Normal: Vento de Ferro Estrangeiro",
         "RU": "\u0416\u0435\u043b\u0435\u0437\u043d\u044b\u0439 \u0432\u0435\u0442\u0435\u0440 \u0438\u043d\u043e\u0437\u0435\u043c\u0446\u0430",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Foreign Ironwind",
         "TR": "Normal Sald\u0131r\u0131: Yabanc\u0131 Demir F\u0131rt\u0131nas\u0131",
@@ -2902,14 +3004,31 @@
         "KR": "",
         "PT": "",
         "RU": "\u7981\u7528\u5143\u7d20\u6218\u8bb0",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "2409917": {
+        "CHS": "\u592a\u7d20\u8bca\u8981",
+        "CHT": "\u592a\u7d20\u8a3a\u8981",
+        "DE": "Universal-Diagnose",
+        "EN": "Universal Diagnosis",
+        "ES": "Diagn\u00f3stico universal",
+        "FR": "Diagnostic universel",
+        "ID": "Universal Diagnosis",
+        "IT": "Diagnosi universale",
+        "JP": "\u592a\u7d20\u8a3a\u8981",
+        "KR": "\ud0dc\uc18c \uc9c4\ub2e8",
+        "PT": "Diagn\u00f3stico Universal",
+        "RU": "\u0423\u043d\u0438\u0432\u0435\u0440\u0441\u0430\u043b\u044c\u043d\u0430\u044f \u0434\u0438\u0430\u0433\u043d\u043e\u0441\u0442\u0438\u043a\u0430",
+        "TH": "Universal Diagnosis",
+        "TR": "Kapsaml\u0131 Te\u015fhis",
+        "VI": "Ch\u1ea9n \u0110o\u00e1n Ph\u1ed5 Qu\u00e1t"
+    },
     "2422927957": {
         "CHS": "\u5973\u4e3b\u89d2(\u98ce)\u7a7a\u4e2d\u653b\u51fb",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -2973,15 +3092,15 @@
         "TH": "Concealing Beacon",
         "TR": "Gizleyici \u0130\u015faret\u00e7i",
         "VI": "Thi\u1ebft B\u1ecb T\u00e0ng H\u00ecnh"
     },
     "2455313621": {
         "CHS": "\u8bfa\u827e\u5c14\u88ab\u52a8\u5929\u8d4b\uff08\u4e0a\u76fe\uff09",
         "CHT": "\u8afe\u827e\u723e\u88ab\u52d5\u5929\u8ce6\uff08\u4e0a\u76fe\uff09",
-        "DE": "Noelles passive F\u00e4higkeit (oberer Schild)",
+        "DE": "Noelles passive F\u00e4higkeit (Schild erzeugen)",
         "EN": "Noelle's Passive Talent (The Shield)",
         "ES": "Talento pasivo de Noelle (Escudo)",
         "FR": "Aptitude passive de No\u00eblle (bouclier)",
         "ID": "Talenta Pasif Noelle (Perisai)",
         "IT": "Talento passivo di Noelle (scudo)",
         "JP": "\u30ce\u30a8\u30eb\u306e\u30d0\u30b7\u30c3\u30d7\u5929\u8ce6\uff08\u76fe\u3092\u4e0a\u3052\u308b\uff09",
         "KR": "\ub178\uc5d8 \ud328\uc2dc\ube0c \uc2a4\ud0ac(\ubcf4\ud638\ub9c9 on)",
@@ -3130,26 +3249,26 @@
     "2499144501": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u6307\u5c16\u96f7\u66b4",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u6307\u5c16\u96f7\u66b4",
         "DE": "Standardangriff: Elektrisierende Ber\u00fchrung",
         "EN": "Normal Attack: Lightning Touch",
         "ES": "Ataque Normal: Toque de rel\u00e1mpago",
         "FR": "Attaque normale : Touche d'\u00e9clair",
-        "ID": "Lighting Touch",
+        "ID": "Normal Attack: Lightning Touch",
         "IT": "Attacco normale: Tocco di fulmine",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u6307\u5148\u306e\u96f7",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc190\ub05d\uc758 \ub1cc\ud3ed",
         "PT": "Ataque Normal: Toque do Rel\u00e2mpago",
         "RU": "\u041a\u0430\u0441\u0430\u043d\u0438\u0435 \u043c\u043e\u043b\u043d\u0438\u0438",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Lightning Touch",
         "TR": "Normal Sald\u0131r\u0131: Y\u0131ld\u0131r\u0131m Dokunu\u015fu",
         "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng: S\u1ea5m S\u00e9t C\u1ea3m \u1ee8ng"
     },
     "2500225021": {
-        "CHS": "\u6d4b\u8bd5\u89d2\u8272\u7a7a\u4e2d\u653b\u51fb",
+        "CHS": "\u516b\u91cd\u795e\u5b50\u7a7a\u4e2d\u653b\u51fb",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
         "IT": "",
@@ -3242,14 +3361,31 @@
         "KR": "\uc774\ub204\uc790\uce74 \uba4d\uba4d \ubc29\uc6d0\uc9c4",
         "PT": "Defesa Concentrada Inuzaka",
         "RU": "\u0412\u0441\u0435\u0441\u0442\u043e\u0440\u043e\u043d\u043d\u044f\u044f \u0437\u0430\u0449\u0438\u0442\u0430 \u0418\u043d\u0443\u0434\u0437\u0430\u043a\u0438",
         "TH": "Inuzaka All-Round Defense",
         "TR": "Inuzaka Savunma \u00c7emberi",
         "VI": "Tr\u1eadn H\u00ecnh Ph\u00f2ng Th\u1ee7 - Inuzaka"
     },
+    "2543392221": {
+        "CHS": "\u79d8\u6cd5\u00b7\u60ca\u559c\u7279\u6d3e",
+        "CHT": "\u79d8\u6cd5\u00b7\u9a5a\u559c\u7279\u6d3e",
+        "DE": "Geheime Kunst \u2013 Besondere \u00dcberraschung",
+        "EN": "Secret Art: Surprise Dispatch",
+        "ES": "T\u00e9cnica secreta: Entrega sorpresa",
+        "FR": "Art secret : Livraison surprise",
+        "ID": "Secret Art: Surprise Dispatch",
+        "IT": "Arte segreta: Spedizione a sorpresa",
+        "JP": "\u79d8\u6cd5\u00b7\u30b5\u30d7\u30e9\u30a4\u30ba\u7279\u5225\u914d\u9001",
+        "KR": "\ube44\ubc95\u00b7\uae5c\uc9dd \ubc30\ub2ec",
+        "PT": "Arte Secreta: Entrega Urgente",
+        "RU": "\u041d\u0435\u043e\u0436\u0438\u0434\u0430\u043d\u043d\u043e\u0435 \u043e\u0442\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0435",
+        "TH": "Secret Art: Surprise Dispatch",
+        "TR": "Gizli Sanat: S\u00fcrpriz Da\u011f\u0131t\u0131m",
+        "VI": "B\u00ed Ph\u00e1p - Chuy\u1ec3n Ph\u00e1t \u0110\u1eb7c Bi\u1ec7t"
+    },
     "2553270533": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u706b\u6f06\u5236\u5370",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u706b\u6f06\u88fd\u5370",
         "DE": "Standardangriff: Flammendes Siegel",
         "EN": "Normal Attack: Seal of Approval",
         "ES": "Ataque Normal: Sello \u00edgneo",
         "FR": "Attaque normale : Sceau embras\u00e9",
@@ -3446,14 +3582,31 @@
         "KR": "\ud3ec\ud68d!",
         "PT": "Capturar!",
         "RU": "\u041f\u043e\u043f\u0430\u043b\u0441\u044f!",
         "TH": "Capture!",
         "TR": "Yakala!",
         "VI": "B\u1eaft l\u1ea5y!"
     },
+    "2662918965": {
+        "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u91d1\u532e\u9488\u89e3",
+        "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u91d1\u5331\u91dd\u89e3",
+        "DE": "Standardangriff: Klassische Akupunktur",
+        "EN": "Normal Attack: The Classics of Acupuncture",
+        "ES": "Ataque Normal: Acupuntura cl\u00e1sica",
+        "FR": "Attaque normale : Acupuncture dor\u00e9e",
+        "ID": "Normal Attack: The Classics of Acupuncture",
+        "IT": "Attacco normale: Agopuntura classica",
+        "JP": "\u901a\u5e38\u653b\u6483\u00b7\u91d1\u5331\u937c\u89e3",
+        "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uae08\uada4 \uce68\uc220",
+        "PT": "Ataque Normal: Acupuntura Dourada",
+        "RU": "\u041a\u043b\u0430\u0441\u0441\u0438\u043a\u0430 \u0438\u0433\u043b\u043e\u0443\u043a\u0430\u043b\u044b\u0432\u0430\u043d\u0438\u044f",
+        "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: The Classics of Acupuncture",
+        "TR": "Normal Sald\u0131r\u0131: Alt\u0131n Akupunktur \u0130\u011fneleri",
+        "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - Ch\u00e2m C\u1ee9u M\u1ea1 V\u00e0ng"
+    },
     "2669120029": {
         "CHS": "\u5723\u4eea\u00b7\u7070\u9e30\u8852\u6f6e",
         "CHT": "\u8056\u5100\u00b7\u7070\u9d12\u8852\u6f6e",
         "DE": "Heiliger Ritus \u2013 Bachstelzenflut",
         "EN": "Sacred Rite: Wagtail's Tide",
         "ES": "Rito sagrado: Marea de aguzanieves",
         "FR": "Liturgie : Mar\u00e9e de la bergeronnette",
@@ -3742,15 +3895,15 @@
     "2745030989": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5343\u91d1\u63b7",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u5343\u91d1\u64f2",
         "DE": "Standardangriff: Teure Geschosse",
         "EN": "Normal Attack: Sparkling Scatter",
         "ES": "Ataque Normal: Lanzamiento centelleante",
         "FR": "Attaque normale : G\u00e9o-dispersion",
-        "ID": "Sparkling Scatter",
+        "ID": "Normal Attack: Sparkling Scatter",
         "IT": "Attacco normale: Dispersione scintillante",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u5343\u91d1\u64f2",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\ucc9c\uae08\ud22c",
         "PT": "Ataque Normal: Dispers\u00e3o Espumante",
         "RU": "\u0421\u0432\u0435\u0440\u043a\u0430\u044e\u0449\u0438\u0439 \u0434\u043e\u0436\u0434\u044c",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Sparkling Scatter",
         "TR": "Normal Sald\u0131r\u0131: Par\u0131ldayan Par\u00e7ac\u0131klar",
@@ -4364,31 +4517,14 @@
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uace0\uc18d \uc0ac\uaca9",
         "PT": "Ataque Normal: Disparos R\u00e1pidos",
         "RU": "\u0421\u043a\u043e\u0440\u043e\u0441\u0442\u043d\u0430\u044f \u0441\u0442\u0440\u0435\u043b\u044c\u0431\u0430",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Rapid Fire",
         "TR": "Normal Sald\u0131r\u0131: Seri Ok At\u0131\u015f\u0131",
         "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - B\u1eafn Ch\u1edbp Nho\u00e1ng"
     },
-    "299520933": {
-        "CHS": "\u65c5\u884c\u8005\u4e94\u8fde\u51fb(\u6c34)",
-        "CHT": "",
-        "DE": "",
-        "EN": "",
-        "ES": "",
-        "FR": "",
-        "ID": "",
-        "IT": "",
-        "JP": "",
-        "KR": "",
-        "PT": "",
-        "RU": "",
-        "TH": "",
-        "TR": "",
-        "VI": ""
-    },
     "3012298293": {
         "CHS": "\u52e0\u5fc3\u62f3",
         "CHT": "\u52e0\u5fc3\u62f3",
         "DE": "Faust der Br\u00fcderlichkeit",
         "EN": "Heartstopper Strike",
         "ES": "Pu\u00f1etazo cardiaco",
         "FR": "Poing d'arr\u00eat cardiaque",
@@ -4548,15 +4684,15 @@
         "ID": "Rites of Termination",
         "IT": "Sacramento finale",
         "JP": "\u81e8\u7d42\u306e\u8056\u793c",
         "KR": "\uc8fd\uc74c\uc758 \uc131\ub840",
         "PT": "Ritos de Termina\u00e7\u00e3o",
         "RU": "\u041e\u0431\u0440\u044f\u0434 \u043a\u043e\u043d\u0447\u0438\u043d\u044b",
         "TH": "Rites of Termination",
-        "TR": "\u00d6l\u00fcm Ayini",
+        "TR": "Son Ayin",
         "VI": "Th\u00e1nh L\u1ec5 Cu\u1ed1i C\u00f9ng"
     },
     "3085221333": {
         "CHS": "\u59ae\u9732\u5143\u7d20\u6218\u62803",
         "CHT": "",
         "DE": "",
         "EN": "",
@@ -4711,15 +4847,15 @@
     "3128535397": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u897f\u98ce\u5251\u672f",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u897f\u98a8\u528d\u8853",
         "DE": "Standardangriff: Favonius-Schwertkunst",
         "EN": "Normal Attack: Favonius Bladework",
         "ES": "Ataque Normal: T\u00e9cnica de espada Favonius",
         "FR": "Attaque normale : Escrime de Favonius",
-        "ID": "Favonius Bladework",
+        "ID": "Normal Attack: Favonius Bladework",
         "IT": "Attacco normale: Tecnica di Favonius",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u897f\u98a8\u5263\u8853",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\ud398\ubcf4\ub2c8\uc6b0\uc2a4 \uac80\uc220",
         "PT": "Ataque Normal: T\u00e9cnica de Favonius",
         "RU": "\u0424\u0435\u0445\u0442\u043e\u0432\u0430\u043b\u044c\u043d\u044b\u0439 \u0441\u0442\u0438\u043b\u044c \u0424\u0430\u0432\u043e\u043d\u0438\u044f",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Favonius Bladework",
         "TR": "Normal Sald\u0131r\u0131: Favonius K\u0131l\u0131\u00e7 Tekni\u011fi",
@@ -4857,14 +4993,31 @@
         "KR": "\uadfc\uc2ec \uc5c6\ub294 \ubc24",
         "PT": "Noites Solenes",
         "RU": "\u041d\u043e\u0447\u0438 \u043f\u043e\u0447\u0442\u0435\u043d\u043d\u043e\u0433\u043e \u0441\u043e\u0441\u0440\u0435\u0434\u043e\u0442\u043e\u0447\u0435\u043d\u0438\u044f",
         "TH": "Nights of Formal Focus",
         "TR": "Odaklanma Gecesi",
         "VI": "\u0110\u00eam Ngon Gi\u1ea5c"
     },
+    "3206240077": {
+        "CHS": "3.8\u8fc7\u5c71\u8f66-\u5de6\u653b\u51fb",
+        "CHT": "",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "3238405613": {
         "CHS": "\u96f7\u4e3b\u89d2\u5c0f\u6280\u80fd\u767d\u76d2\u6d4b\u8bd51",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -4908,14 +5061,31 @@
         "KR": "\uc808\ubcbd\uc744 \uae4e\ub294 \uae43\ubc1c",
         "PT": "Bandeira Quebra-Rochas",
         "RU": "\u0421\u0442\u044f\u0433 \u0440\u0430\u0437\u0440\u0443\u0448\u0438\u0442\u0435\u043b\u044f \u0441\u043a\u0430\u043b",
         "TH": "Cliffbreaker's Banner",
         "TR": "U\u00e7urum Yaran Sancak",
         "VI": "Ph\u00e1 Ch\u01b0\u1edbng Ki\u1ebfn Tinh Nghi"
     },
+    "3249611093": {
+        "CHS": "\u6108\u6c14\u5168\u5f62\u8bba",
+        "CHT": "\u7652\u6c23\u5168\u5f62\u8ad6",
+        "DE": "Ganzheitliche Heilung",
+        "EN": "Holistic Revivification",
+        "ES": "Sanaci\u00f3n hol\u00edstica",
+        "FR": "Reviviscence holistique",
+        "ID": "Holistic Revivification",
+        "IT": "Rinascita olistica",
+        "JP": "\u7652\u6c17\u5168\u5f62\u8ad6",
+        "KR": "\uce58\uc720 \uc804\ud615\ub860",
+        "PT": "Cura Hol\u00edstica",
+        "RU": "\u0426\u0435\u043b\u043e\u0441\u0442\u043d\u043e\u0435 \u0432\u043e\u0441\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d\u0438\u0435",
+        "TH": "Holistic Revivification",
+        "TR": "B\u00fct\u00fcnc\u00fcl \u0130yile\u015ftirme",
+        "VI": "Tr\u1ecb Li\u1ec7u To\u00e0n Th\u01b0"
+    },
     "3251301293": {
         "CHS": "\u65e9\u67da\u7a7a\u4e2d\u653b\u51fb",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -5000,15 +5170,15 @@
     "3283214237": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5f02\u90a6\u94c1\u98ce",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u7570\u90a6\u9435\u98a8",
         "DE": "Standardangriff: Eiserner Wind aus der Fremde",
         "EN": "Normal Attack: Foreign Ironwind",
         "ES": "Ataque Normal: Viento met\u00e1lico extranjero",
         "FR": "Attaque normale : Vents de la discorde",
-        "ID": "Foreign Ironwind",
+        "ID": "Normal Attack: Foreign Ironwind",
         "IT": "Attacco normale: Ferrovento straniero",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u7570\u90a6\u306e\u9244\u98a8",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc774\uad6d\uc758 \uac15\ucca0\ubc14\ub78c",
         "PT": "Ataque Normal: Vento de Ferro Estrangeiro",
         "RU": "\u0416\u0435\u043b\u0435\u0437\u043d\u044b\u0439 \u0432\u0435\u0442\u0435\u0440 \u0438\u043d\u043e\u0437\u0435\u043c\u0446\u0430",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Foreign Ironwind",
         "TR": "Normal Sald\u0131r\u0131: Yabanc\u0131 Demir F\u0131rt\u0131nas\u0131",
@@ -5044,14 +5214,31 @@
         "KR": "\uc5ed\ub0a0\uc758 \ud654\uc5fc",
         "PT": "Investida Ardente",
         "RU": "\u041e\u0433\u043d\u0435\u043d\u043d\u044b\u0439 \u043d\u0430\u0442\u0438\u0441\u043a",
         "TH": "Searing Onslaught",
         "TR": "Da\u011flayan Taarruz",
         "VI": "L\u01b0\u1ee1i \u0110ao R\u1ef1c L\u1eeda"
     },
+    "331663653": {
+        "CHS": "\u5361\u7ef4\u7a7a\u4e2d\u653b\u51fb",
+        "CHT": "",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "33306749": {
         "CHS": "\u6d41\u6d6a\u8005\u5143\u7d20\u6218\u6280",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -5153,15 +5340,15 @@
     "3392494725": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u94a2\u810a",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u92fc\u810a",
         "DE": "Standardangriff: St\u00e4hlernes Kreuz",
         "EN": "Normal Attack: Steel Fang",
         "ES": "Ataque Normal: Colmillo de acero",
         "FR": "Attaque normale : Croc d'acier",
-        "ID": "Steel Fang",
+        "ID": "Normal Attack: Steel Fang",
         "IT": "Attacco normale: Zanna d'acciaio",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u92fc\u306e\u810a",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uac15\ucca0 \ub9c8\ub8e8",
         "PT": "Ataque Normal: Presa de A\u00e7o",
         "RU": "\u0421\u0442\u0430\u043b\u044c\u043d\u043e\u0439 \u043a\u043b\u044b\u043a",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Steel Fang",
         "TR": "Normal Sald\u0131r\u0131: \u00c7elik Di\u015f",
@@ -5316,14 +5503,31 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "3512914781": {
+        "CHS": "\u545c\u55b5\u753a\u98de\u8db3",
+        "CHT": "\u55da\u55b5\u753a\u98db\u8db3",
+        "DE": "Miauteoritentritt",
+        "EN": "Meow-teor Kick",
+        "ES": "Nekopatada voladora",
+        "FR": "Coup de patte miaou-t\u00e9orite",
+        "ID": "Meow-teor Kick",
+        "IT": "Calcio Miaoteoritico",
+        "JP": "\u306b\u3083\u3093\u306b\u3083\u3093\u753a\u98db\u811a",
+        "KR": "\ub0e5\ub0e5 \uace8\ubaa9 \ub204\ube44\uae30",
+        "PT": "Chute Miauteoro",
+        "RU": "\u041c\u044f\u0443\u0442\u0435\u043e\u0440\u0438\u0442\u043d\u044b\u0439 \u0443\u0434\u0430\u0440",
+        "TH": "Meow-teor Kick",
+        "TR": "Miyav Jitsu",
+        "VI": "M\u00e8o Tung C\u01b0\u1edbc"
+    },
     "3521320029": {
         "CHS": "\u51dd\u6d6a\u4e4b\u5149\u5251",
         "CHT": "\u51dd\u6d6a\u4e4b\u5149\u528d",
         "DE": "Schwert der Brandung",
         "EN": "Glacial Illumination",
         "ES": "Fulgor glacial",
         "FR": "Lame de fond",
@@ -5469,31 +5673,14 @@
         "KR": "\uc6b0\ud654\u00b7\ubc14\ub78c\uc774 \uc804\ud558\ub294 \ub178\ub798",
         "PT": "Pluma Ilustrada: Can\u00e7\u00e3o Graciosa",
         "RU": "\u0425\u0430\u043d\u044d\u0433\u0430: \u041f\u0435\u0441\u043d\u044c \u0432\u0435\u0442\u0440\u0430",
         "TH": "Hanega: Song of the Wind",
         "TR": "Hanega: R\u00fczgar \u015eark\u0131s\u0131",
         "VI": "Hanega - H\u00f9ng Ca Gi\u00f3 Tho\u1ea3ng"
     },
-    "3565118517": {
-        "CHS": "\u65c5\u884c\u8005\u4e94\u8fde\u51fb(\u6c34)",
-        "CHT": "",
-        "DE": "",
-        "EN": "",
-        "ES": "",
-        "FR": "",
-        "ID": "",
-        "IT": "",
-        "JP": "",
-        "KR": "",
-        "PT": "",
-        "RU": "",
-        "TH": "",
-        "TR": "",
-        "VI": ""
-    },
     "3584687669": {
         "CHS": "\u805a\u98ce\u8e74",
         "CHT": "\u805a\u98a8\u8e74",
         "DE": "Tritt des konzentrierten Winds",
         "EN": "Windmuster Kick",
         "ES": "Patada huracanada",
         "FR": "Coup de pied ouragan",
@@ -5756,15 +5943,15 @@
         "IT": "Giuramento di Kurage",
         "JP": "\u6d77\u6708\u306e\u8a93\u3044",
         "KR": "\ud574\ud30c\ub9ac\uc758 \uc11c\uc57d",
         "PT": "Juramento de Kurage",
         "RU": "\u041a\u043b\u044f\u0442\u0432\u0430 \u043a\u0443\u0440\u0430\u0433\u044d",
         "TH": "Kurage's Oath",
         "TR": "Kurage Yemini",
-        "VI": "L\u1eddi Th\u1ec1 \u00c1nh Tr\u0103ng Bi\u1ec3n"
+        "VI": "L\u1eddi Th\u1ec1 Kurage"
     },
     "3699125269": {
         "CHS": "\u8fea\u5e0c\u96c5\u5143\u7d20\u7206\u53d1_QTE",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
@@ -5911,14 +6098,31 @@
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc8c4\uba78\uc758 \ud654\uc0b4",
         "PT": "Ataque Normal: Flechas da Culpa",
         "RU": "\u0421\u0442\u0440\u0435\u043b\u0430 \u0432\u043e\u0437\u043c\u0435\u0437\u0434\u0438\u044f",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Bolts of Downfall",
         "TR": "Normal Sald\u0131r\u0131: D\u00fc\u015fen Y\u0131ld\u0131r\u0131mlar",
         "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - M\u0169i T\u00ean Di\u1ec7t \u00c1c"
     },
+    "3734682949": {
+        "CHS": "\u767d\u672f\u7a7a\u4e2d\u653b\u51fb",
+        "CHT": "",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "3736001053": {
         "CHS": "\u51dd\u5149\u7a7a\u4e2d\u653b\u51fb",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -6088,15 +6292,15 @@
     "379244133": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5f02\u90a6\u5ca9\u950b",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u7570\u90a6\u5ca9\u92d2",
         "DE": "Standardangriff: Steinerne Klinge aus der Fremde",
         "EN": "Normal Attack: Foreign Rockblade",
         "ES": "Ataque Normal: Espada de piedra extranjera",
         "FR": "Attaque normale : Lame de roche",
-        "ID": "Foreign Rockblade",
+        "ID": "Normal Attack: Foreign Rockblade",
         "IT": "Attacco normale: Lamaroccia straniera",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u7570\u90a6\u306e\u5ca9\u5cf0",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc774\uad6d\uc758 \uc554\ubd09",
         "PT": "Ataque Normal: L\u00e2mina de Rocha Estrangeira",
         "RU": "\u041a\u0430\u043c\u0435\u043d\u043d\u044b\u0439 \u043c\u0435\u0447 \u0438\u043d\u043e\u0437\u0435\u043c\u0446\u0430",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Foreign Rockblade",
         "TR": "Normal Sald\u0131r\u0131: Yabanc\u0131 Ta\u015f K\u0131l\u0131c\u0131",
@@ -6105,15 +6309,15 @@
     "3795823997": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u4eea\u5178\u5251\u672f",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u5100\u5178\u528d\u8853",
         "DE": "Standardangriff: Rituelle Schwertkunst",
         "EN": "Normal Attack: Ceremonial Bladework",
         "ES": "Ataque Normal: T\u00e9cnica de espada ceremonial",
         "FR": "Attaque normale : Passe d'armes",
-        "ID": "Ceremonial Bladework",
+        "ID": "Normal Attack: Ceremonial Bladework",
         "IT": "Attacco normale: Tecnica cerimoniale",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u5100\u5178\u306e\u5263\u8853",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc758\uc804 \uac80\uc220",
         "PT": "Ataque Normal: L\u00e2mina Cerimonial",
         "RU": "\u0420\u0438\u0442\u0443\u0430\u043b\u044c\u043d\u043e\u0435 \u0444\u0435\u0445\u0442\u043e\u0432\u0430\u043d\u0438\u0435",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Ceremonial Bladework",
         "TR": "Normal Sald\u0131r\u0131: Merasim K\u0131l\u0131c\u0131 Tekni\u011fi",
@@ -6581,15 +6785,15 @@
     "4043029317": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u795e\u4ee3\u5c04\u672f",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u795e\u4ee3\u5c04\u8853",
         "DE": "Standardangriff: G\u00f6ttliche Schie\u00dfkunst",
         "EN": "Normal Attack: Divine Marksmanship",
         "ES": "Ataque Normal: Punter\u00eda divina",
         "FR": "Attaque normale : Archerie divine",
-        "ID": "Divine Marksmanship",
+        "ID": "Normal Attack: Divine Marksmanship",
         "IT": "Attacco normale: Precisione divina",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u795e\u4ee3\u306e\u5c04\u8853",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc2e0\uc131\ud55c \uc0ac\uaca9\uc220",
         "PT": "Ataque Normal: Tiro com Arco Divino",
         "RU": "\u0411\u043e\u0436\u0435\u0441\u0442\u0432\u0435\u043d\u043d\u0430\u044f \u0442\u043e\u0447\u043d\u043e\u0441\u0442\u044c",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Divine Marksmanship",
         "TR": "Normal Sald\u0131r\u0131: Kutsal Ni\u015fanc\u0131",
@@ -6609,15 +6813,15 @@
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
     "405719917": {
-        "CHS": "\u7a7a\u4e2d\u653b\u51fb",
+        "CHS": "\u73d0\u9732\u73ca\u7a7a\u4e2d\u653b\u51fb",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
         "IT": "",
@@ -7101,14 +7305,31 @@
         "KR": "\uc720\uae08 \uc6b4\uac04\ucd08",
         "PT": "Saxifraga Ryuukin",
         "RU": "\u041a\u0430\u043c\u043d\u0435\u043b\u043e\u043c\u043a\u0430 \u0420\u044e\u043a\u0438\u043d",
         "TH": "Ryuukin Saxifrage",
         "TR": "Ta\u015fk\u0131ran Ryuukin",
         "VI": "C\u1ecf Ryuukin"
     },
+    "4260508917": {
+        "CHS": "\u753b\u5219\u5de7\u65bd",
+        "CHT": "\u756b\u5247\u5de7\u65bd",
+        "DE": "K\u00fcnstlerische Genialit\u00e4t",
+        "EN": "Artistic Ingenuity",
+        "ES": "Genio de la arquitectura",
+        "FR": "Ing\u00e9niosit\u00e9 artistique",
+        "ID": "Artistic Ingenuity",
+        "IT": "Ingegno artistico",
+        "JP": "\u7cbe\u7dfb\u306a\u308b\u7d75\u56f3",
+        "KR": "\uae30\uc608 \ubc1c\ud718",
+        "PT": "Genialidade Art\u00edstica",
+        "RU": "\u0422\u0432\u043e\u0440\u0447\u0435\u0441\u043a\u043e\u0435 \u043c\u0430\u0441\u0442\u0435\u0440\u0441\u0442\u0432\u043e",
+        "TH": "Artistic Ingenuity",
+        "TR": "Sanatsal Marifet",
+        "VI": "Ngh\u1ec7 Thu\u1eadt Tinh T\u1ebf"
+    },
     "4262868373": {
         "CHS": "3.2\u6563\u51752\u9636\u6bb5\u7784\u51c6\u5c04\u51fb",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
@@ -7203,14 +7424,31 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "451737061": {
+        "CHS": "\u5143\u7d20\u6218\u6280\u732b\u732b\u7403\u9000\u51fa",
+        "CHT": "",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "45357229": {
         "CHS": "\u98ce\u8f6e\u4e24\u7acb",
         "CHT": "\u98a8\u8f2a\u5169\u7acb",
         "DE": "Doppeltes Windrad",
         "EN": "Lemniscatic Wind Cycling",
         "ES": "Cicl\u00f3n de viento lemnisc\u00e1tico",
         "FR": "Cycle du vent lemniscatique",
@@ -7863,15 +8101,15 @@
         "ID": "Secret Art: Musou Shinsetsu",
         "IT": "Arte segreta: Musou Shinsetsu",
         "JP": "\u5965\u7fa9\u00b7\u5922\u60f3\u771f\u8aac",
         "KR": "\uc624\uc758\u00b7\ubabd\uc0c1\uc9c4\uc124",
         "PT": "Arte Secreta: Musou Shinsetsu",
         "RU": "\u0422\u0430\u0439\u043d\u043e\u0435 \u0438\u0441\u043a\u0443\u0441\u0441\u0442\u0432\u043e: \u041c\u0443\u0441\u043e \u0441\u0438\u043d\u0441\u044d\u0446\u0443",
         "TH": "Secret Art: Musou Shinsetsu",
-        "TR": "Gizli B\u00fcy\u00fc: Musou Shinsetsu",
+        "TR": "Gizli Sanat: Musou Shinsetsu",
         "VI": "B\u00ed K\u1ef9 - M\u1ed9ng T\u01b0\u1edfng Ch\u00e2n Thuy\u1ebft"
     },
     "737506901": {
         "CHS": "\u62a4\u5fc3\u94e0",
         "CHT": "\u8b77\u5fc3\u93a7",
         "DE": "Brustpanzer",
         "EN": "Breastplate",
@@ -8128,15 +8366,15 @@
     "813430205": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u795e\u91cc\u6d41\u00b7\u503e",
         "CHT": "\u666e\u901a\u653b\u64ca\u00b7\u795e\u91cc\u6d41\u00b7\u50be",
         "DE": "Standardangriff: Kamisato-Stil \u2013 Naname",
         "EN": "Normal Attack: Kamisato Art - Kabuki",
         "ES": "Ataque Normal: Estilo Kamisato - Elegancia",
         "FR": "Attaque normale : \u00c9cole Kamisato - Sveltesse",
-        "ID": "Kamisato Art: Kabuki",
+        "ID": "Normal Attack: Kamisato Art - Kabuki",
         "IT": "Attacco normale: Arte Kamisato - Kabuki",
         "JP": "\u901a\u5e38\u653b\u6483\u00b7\u795e\u91cc\u6d41\u00b7\u50be\u304d",
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uce74\ubbf8\uc0ac\ud1a0\ub958\u00b7\uacbd(\u50be)",
         "PT": "Arte Kamisato: Naname",
         "RU": "\u0418\u0441\u043a\u0443\u0441\u0441\u0442\u0432\u043e \u041a\u0430\u043c\u0438\u0441\u0430\u0442\u043e: \u041d\u0430\u043d\u0430\u043c\u044d",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Kamisato Art - Kabuki",
         "TR": "Normal Sald\u0131r\u0131: Kamisato Sanat\u0131 - Kabuki",
@@ -8326,15 +8564,15 @@
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
     "889413773": {
-        "CHS": "\u6d4b\u8bd5\u89d2\u827250\u7a7a\u4e2d\u653b\u51fb",
+        "CHS": "\u6258\u9a6c\u7a7a\u4e2d\u653b\u51fb",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
         "IT": "",
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets/langs/weapons.json` & `enkanetwork.py-1.4.4/enkanetwork/assets/langs/weapons.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993063063063063%*

 * *Differences: {"'2705029563'": "{'VI': 'Sổ Tay Ma Pháp'}",*

 * * "'3073454867'": "{'PT': 'Água-Marinha de Mahara'}",*

 * * "'316078811'": 'OrderedDict([(\'FR\', "Perceur d\'ibis"), (\'JP\', \'トキの嘴\'), (\'CHT\', '*

 * *                "'䴉穿之喙'), ('ID', 'Ibis Piercer'), ('CHS', '鹮穿之喙'), ('VI', 'Mỏ Cò Xuyên Thấu'), "*

 * *                "('ES', 'Perforaibis'), ('TH', 'Ibis Piercer'), ('TR', 'Telli Turna'), ('KR', '꿰뚫는 "*

 * *                "따오기 부리'), ('DE', 'Durchdringer der Ibisse'), ('RU', 'Клюв ибиса'), ('IT', "*

 * *                '"Becco d\'ibis" […]*

```diff
@@ -1234,15 +1234,15 @@
         "IT": "Grimorio tascabile",
         "JP": "\u30dd\u30b1\u30c3\u30c8\u9b54\u5c0e\u66f8",
         "KR": "\ud3ec\ucf13 \uc8fc\uc220\uc11c",
         "PT": "Grim\u00f3rio de Bolso",
         "RU": "\u041a\u0430\u0440\u043c\u0430\u043d\u043d\u044b\u0439 \u0433\u0440\u0438\u043c\u0443\u0430\u0440",
         "TH": "Pocket Grimoire",
         "TR": "B\u00fcy\u00fc Cep Kitab\u0131",
-        "VI": "S\u1ed1 Tay Ma Ph\u00e1p"
+        "VI": "S\u1ed5 Tay Ma Ph\u00e1p"
     },
     "2719832059": {
         "CHS": "(test)\u7a7f\u6a21\u6d4b\u8bd5",
         "CHT": "",
         "DE": "",
         "EN": "",
         "ES": "",
@@ -1536,15 +1536,15 @@
         "EN": "Makhaira Aquamarine",
         "ES": "M\u00e1jaira Aguamarina",
         "FR": "Aigue-marine de Makhaira",
         "ID": "Makhaira Aquamarine",
         "IT": "Acquamarina di Makhaira",
         "JP": "\u30de\u30ab\u30a4\u30e9\u306e\u6c34\u8272",
         "KR": "\ubb3c\ube5b \ub9c8\uce74\uc774\ub77c",
-        "PT": "\u00c1gua-marinha de Mahara",
+        "PT": "\u00c1gua-Marinha de Mahara",
         "RU": "\u0410\u043a\u0432\u0430\u043c\u0430\u0440\u0438\u043d \u041c\u0430\u0445\u0430\u0439\u0440\u044b",
         "TH": "Makhaira Aquamarine",
         "TR": "Makhaira Deniz Ye\u015fili",
         "VI": "S\u1eafc N\u01b0\u1edbc Makhaira"
     },
     "3090373787": {
         "CHS": "\u6697\u5df7\u7684\u9152\u4e0e\u8bd7",
@@ -1644,14 +1644,31 @@
         "KR": "\uc18c\uc2ec",
         "PT": "Olho da Percep\u00e7\u00e3o",
         "RU": "\u041e\u043a\u043e \u0441\u043e\u0437\u043d\u0430\u043d\u0438\u044f",
         "TH": "Eye of Perception",
         "TR": "Alg\u0131 G\u00f6z\u00fc",
         "VI": "Chi\u00eau T\u00e2m"
     },
+    "316078811": {
+        "CHS": "\u9e6e\u7a7f\u4e4b\u5599",
+        "CHT": "\u4d09\u7a7f\u4e4b\u5599",
+        "DE": "Durchdringer der Ibisse",
+        "EN": "Ibis Piercer",
+        "ES": "Perforaibis",
+        "FR": "Perceur d'ibis",
+        "ID": "Ibis Piercer",
+        "IT": "Becco d'ibis",
+        "JP": "\u30c8\u30ad\u306e\u5634",
+        "KR": "\uaff0\ub6ab\ub294 \ub530\uc624\uae30 \ubd80\ub9ac",
+        "PT": "Bico de \u00cdbis",
+        "RU": "\u041a\u043b\u044e\u0432 \u0438\u0431\u0438\u0441\u0430",
+        "TH": "Ibis Piercer",
+        "TR": "Telli Turna",
+        "VI": "M\u1ecf C\u00f2 Xuy\u00ean Th\u1ea5u"
+    },
     "3169209451": {
         "CHS": "\u5f13\u85cf",
         "CHT": "\u5f13\u85cf",
         "DE": "Rostiger Bogen",
         "EN": "Rust",
         "ES": "Herrumbre",
         "FR": "Arc rouill\u00e9",
@@ -2257,29 +2274,29 @@
         "PT": "T\u00famulo do Lobo",
         "RU": "\u0412\u043e\u043b\u0447\u044c\u044f \u043f\u043e\u0433\u0438\u0431\u0435\u043b\u044c",
         "TH": "Wolf's Gravestone",
         "TR": "Kurdun Mezar Ta\u015f\u0131",
         "VI": "\u0110\u01b0\u1eddng C\u00f9ng C\u1ee7a S\u00f3i"
     },
     "4007372867": {
-        "CHS": "",
-        "CHT": "\u5b9a\u571f\u7389\u572d",
-        "DE": "Urzeitliche Jadeinsignien",
-        "EN": "Primordial Jade Regalia",
-        "ES": "Regalia de Jade Primordial",
-        "FR": "Tablette de jade primordial",
-        "ID": "Primordial Jade Regalia",
-        "IT": "",
-        "JP": "\u571f\u5b9a\u306e\u7389",
-        "KR": "\uc815\ud1a0\uc625\uaddc",
-        "PT": "Presente de Jade Primordial",
-        "RU": "\u0414\u0440\u0435\u0432\u043d\u044f\u044f \u041d\u0435\u0444\u0440\u0438\u0442\u043e\u0432\u0430\u044f \u0420\u0435\u0433\u0430\u043b\u0438\u044f",
-        "TH": "Primordial Jade Regalia",
-        "TR": "",
-        "VI": "Ng\u1ecdc \u0110\u1ecbnh Th\u1ed5"
+        "CHS": "\u78a7\u843d\u4e4b\u73d1",
+        "CHT": "\u78a7\u843d\u4e4b\u74cf",
+        "DE": "Jadesturz-Pracht",
+        "EN": "Jadefall's Splendor",
+        "ES": "Centelleo Jadeca\u00eddo",
+        "FR": "Splendeur de l'azur",
+        "ID": "Jadefall's Splendor",
+        "IT": "Splendore del Giadiluvio",
+        "JP": "\u78a7\u843d\u306e\u74cf",
+        "KR": "\ubcbd\ub77d\uc758 \uc625",
+        "PT": "Esplendor \u00cdndigo",
+        "RU": "\u0412\u0435\u043b\u0438\u043a\u043e\u043b\u0435\u043f\u0438\u0435 \u043b\u0430\u0437\u0443\u0440\u043d\u043e\u0433\u043e \u0441\u0432\u043e\u0434\u0430",
+        "TH": "Jadefall's Splendor",
+        "TR": "Ye\u015fimlerin Ma\u011frur I\u015f\u0131lt\u0131s\u0131",
+        "VI": "Ng\u1ecdc B\u00edch Huy Ho\u00e0ng"
     },
     "4049410651": {
         "CHS": "\u51b3\u6597\u4e4b\u67aa",
         "CHT": "\u6c7a\u9b25\u4e4b\u69cd",
         "DE": "Duelllanze",
         "EN": "Deathmatch",
         "ES": "Lanza del Duelo",
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork/assets.py` & `enkanetwork.py-1.4.4/enkanetwork/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/cache.py` & `enkanetwork.py-1.4.4/enkanetwork/cache.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/client.py` & `enkanetwork.py-1.4.4/enkanetwork/client.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/config.py` & `enkanetwork.py-1.4.4/enkanetwork/config.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/enum.py` & `enkanetwork.py-1.4.4/enkanetwork/enum.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/exception.py` & `enkanetwork.py-1.4.4/enkanetwork/exception.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/http.py` & `enkanetwork.py-1.4.4/enkanetwork/http.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/model/assets.py` & `enkanetwork.py-1.4.4/enkanetwork/model/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/model/base.py` & `enkanetwork.py-1.4.4/enkanetwork/model/base.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/model/build.py` & `enkanetwork.py-1.4.4/enkanetwork/model/build.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/model/character.py` & `enkanetwork.py-1.4.4/enkanetwork/model/character.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/model/equipments.py` & `enkanetwork.py-1.4.4/enkanetwork/model/equipments.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/model/players.py` & `enkanetwork.py-1.4.4/enkanetwork/model/players.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/model/stats.py` & `enkanetwork.py-1.4.4/enkanetwork/model/stats.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/tools.py` & `enkanetwork.py-1.4.4/enkanetwork/tools.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/types/enkanetwork.py` & `enkanetwork.py-1.4.4/enkanetwork/types/enkanetwork.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork/utils.py` & `enkanetwork.py-1.4.4/enkanetwork/utils.py`

 * *Files identical despite different names*

### Comparing `enkanetwork.py-1.4.2/enkanetwork.py.egg-info/PKG-INFO` & `enkanetwork.py-1.4.4/enkanetwork.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: enkanetwork.py
-Version: 1.4.2
+Version: 1.4.4
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/mrwan200/EnkaNetwork.py
 Author: M-307
 Author-email: me@m307.dev
-License: UNKNOWN
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -73,15 +71,15 @@
 
 async def main():
     async with client:
         data = await client.fetch_user(843715177)
         print("=== Player Info ===")
         print(f"Nickname: {data.player.nickname}")
         print(f"Level: {data.player.level}")
-        print(f"Icon: {data.player.icon.url}")
+        print(f"Icon: {data.player.avatar.icon.url}")
         print(f"Signature: {data.player.signature}")
         print(f"Achievement: {data.player.achievement}")
         print(f"Abyss floor: {data.player.abyss_floor} - {data.player.abyss_room}")
         print(f"Cache timeout: {data.ttl}")
 
 asyncio.run(main())
 ```
@@ -435,9 +433,7 @@
 # LICENSE
 
 [MIT License](./LICENSE)
 
 ![Keqing](https://c.tenor.com/MnkpnVCLcb0AAAAC/keqing-dance.gif)
 
 [Picture by KKOMDASTRO](https://twitter.com/KKOMDASTRO)
-
-
```

### Comparing `enkanetwork.py-1.4.2/enkanetwork.py.egg-info/SOURCES.txt` & `enkanetwork.py-1.4.4/enkanetwork.py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,8 +39,9 @@
 enkanetwork/model/equipments.py
 enkanetwork/model/hoyos.py
 enkanetwork/model/players.py
 enkanetwork/model/profile.py
 enkanetwork/model/stats.py
 enkanetwork/model/utils.py
 enkanetwork/types/__init__.py
-enkanetwork/types/enkanetwork.py
+enkanetwork/types/enkanetwork.py
+test/test.test.py
```

### Comparing `enkanetwork.py-1.4.2/setup.py` & `enkanetwork.py-1.4.4/setup.py`

 * *Files identical despite different names*

