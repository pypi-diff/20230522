# Comparing `tmp/starrail-toolkit-0.5.8.tar.gz` & `tmp/starrail-toolkit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.5.8.tar", last modified: Thu May 18 17:24:08 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.6.0.tar", last modified: Mon May 22 18:25:03 2023, max compression
```

## Comparing `starrail-toolkit-0.5.8.tar` & `starrail-toolkit-0.6.0.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.630131 starrail-toolkit-0.5.8/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     5497 2023-05-18 17:24:08.630006 starrail-toolkit-0.5.8/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     4990 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-18 17:24:08.630169 starrail-toolkit-0.5.8/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.624603 starrail-toolkit-0.5.8/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.625084 starrail-toolkit-0.5.8/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3000 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      988 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.626150 starrail-toolkit-0.5.8/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1103 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5092 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4547 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.626385 starrail-toolkit-0.5.8/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6046 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.626983 starrail-toolkit-0.5.8/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      978 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/common/config.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.627624 starrail-toolkit-0.5.8/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    13661 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4267 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.628033 starrail-toolkit-0.5.8/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.628458 starrail-toolkit-0.5.8/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1832 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/utils/accounts.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      937 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.629146 starrail-toolkit-0.5.8/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     3291 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     7271 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.629842 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     5497 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1530 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.701978 starrail-toolkit-0.6.0/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.0/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5798 2023-05-22 18:25:03.701849 starrail-toolkit-0.6.0/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5291 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-22 18:25:03.702013 starrail-toolkit-0.6.0/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.0/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.695617 starrail-toolkit-0.6.0/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.696058 starrail-toolkit-0.6.0/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3642 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.697224 starrail-toolkit-0.6.0/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1134 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5092 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4547 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.697445 starrail-toolkit-0.6.0/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6480 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.698090 starrail-toolkit-0.6.0/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1802 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/common/config.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      282 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.698845 starrail-toolkit-0.6.0/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    13545 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/unlock_fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.699260 starrail-toolkit-0.6.0/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.699578 starrail-toolkit-0.6.0/starrail/unlock/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/unlock/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/unlock/fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/unlock/service.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.700163 starrail-toolkit-0.6.0/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1832 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/accounts.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.701001 starrail-toolkit-0.6.0/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4292 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     9255 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      504 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/misc.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.701670 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5798 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1669 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.5.8/LICENSE` & `starrail-toolkit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/PKG-INFO` & `starrail-toolkit-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,46 @@
-Metadata-Version: 2.1
-Name: starrail-toolkit
-Version: 0.5.8
-Summary: Honkai Star Rail Toolkit
-Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
-Author: LittleNyima
-Author-email: littlenyima@163.com
-License: GPLv3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
+
+<b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
+
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.5.8    |    0.5.8     |   0.5.8   |   0.5.4    |
+|   0.6.0    |    0.6.0     |   0.6.0   |   0.6.0    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
-- [ ] 支持更多的可设置选项
+- [x] 支持更多的可设置选项
 - [ ] 支持国际服
+- [x] 支持解锁120帧
 - [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
-- [ ] 美化抽卡导出页面
+- [ ] 美化程序界面
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i8l5L0v48e5i)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/iwDYF0x00q0f)，两种途径的内容相同，可以自行选择下载方式。
 
 ***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
 
-![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+![gui preview gacha](https://s1.ax1x.com/2023/05/23/p9o7y3d.png)
+
+![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 python3 -m pip install starrail-toolkit --force-reinstall --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
@@ -79,27 +70,29 @@
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
 # 非 Windows 平台
-hksr --api https://api-takumi.mihoyo.com/xxx
+hksr gacha --api https://api-takumi.mihoyo.com/xxx
 # Windows 平台无需 --api 参数
-hksr
+hksr gacha
 ```
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
 - `--request-interval`：（可选）请求间隔。两次请求之间的最小间隔，默认为 `0.1`。若某些情况下因请求过于频繁导致 IP 被 ban，可以适度把这个值调大一点。
 
+**如果想要进一步了解命令行使用方法，请参考[命令行使用指南](docs/cli-guidance.md)。**
+
 本项目目前正处于快速迭代阶段，使用方式可能会发生改变，请及时更新程序，更新时请留意本部分关于使用方式的说明。
 
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
```

### Comparing `starrail-toolkit-0.5.8/README.md` & `starrail-toolkit-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,61 @@
+Metadata-Version: 2.1
+Name: starrail-toolkit
+Version: 0.6.0
+Summary: Honkai Star Rail Toolkit
+Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
+Author: LittleNyima
+Author-email: littlenyima@163.com
+License: GPLv3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
+
+<b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
+
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.5.8    |    0.5.8     |   0.5.8   |   0.5.4    |
+|   0.6.0    |    0.6.0     |   0.6.0   |   0.6.0    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
-- [ ] 支持更多的可设置选项
+- [x] 支持更多的可设置选项
 - [ ] 支持国际服
+- [x] 支持解锁120帧
 - [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
-- [ ] 美化抽卡导出页面
+- [ ] 美化程序界面
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i8l5L0v48e5i)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/iwDYF0x00q0f)，两种途径的内容相同，可以自行选择下载方式。
 
 ***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
 
-![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+![gui preview gacha](https://s1.ax1x.com/2023/05/23/p9o7y3d.png)
+
+![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 python3 -m pip install starrail-toolkit --force-reinstall --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
@@ -64,27 +85,29 @@
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
 # 非 Windows 平台
-hksr --api https://api-takumi.mihoyo.com/xxx
+hksr gacha --api https://api-takumi.mihoyo.com/xxx
 # Windows 平台无需 --api 参数
-hksr
+hksr gacha
 ```
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
 - `--request-interval`：（可选）请求间隔。两次请求之间的最小间隔，默认为 `0.1`。若某些情况下因请求过于频繁导致 IP 被 ban，可以适度把这个值调大一点。
 
+**如果想要进一步了解命令行使用方法，请参考[命令行使用指南](docs/cli-guidance.md)。**
+
 本项目目前正处于快速迭代阶段，使用方式可能会发生改变，请及时更新程序，更新时请留意本部分关于使用方式的说明。
 
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
```

### Comparing `starrail-toolkit-0.5.8/setup.py` & `starrail-toolkit-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/__init__.py` & `starrail-toolkit-0.6.0/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/config.py` & `starrail-toolkit-0.6.0/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/entry/cli.py` & `starrail-toolkit-0.6.0/starrail/entry/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 import argparse
 import traceback
 
 from starrail import __version__, digital_version
 from starrail.config import configuration as cfg
 from starrail.entry.setup import setup
 from starrail.gacha.service import export_gacha_from_api
+from starrail.unlock.service import unlock_fps
 from starrail.utils import babelfish, loggings
 from starrail.utils.auto_update import check_update
 
 logger = loggings.get_logger(__file__)
 
 
-def parse_args():
+def get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         prog='hksr',
         description='Honkai: Star Rail Toolkit',
     )
     parser.add_argument(
-        '--api', type=str,
-        help='URL of the gacha api, please refer to README.md for details.',
-    )
-    parser.add_argument(
-        '--export', nargs='+', type=str, default=['all'],
-        choices=['all', 'csv', 'html', 'json', 'md', 'xlsx'],
-        help='Types of expected export formats.',
-    )
-    parser.add_argument(
         '--locale', type=str, default='zhs',
         choices=['en', 'zhs'],
         help=(
             'Language of gacha report. Abbreviations: `en` for English, '
             '`zhs` for simplified Chinese'
         ),
     )
     parser.add_argument(
         '--log-level', type=str, default='DEBUG',
         choices=['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG'],
         help='Controlling the level of logging output.',
     )
-    parser.add_argument(
+
+    subparsers = parser.add_subparsers(dest='command')
+
+    gacha = subparsers.add_parser('gacha')
+    gacha.add_argument(
+        '--api', type=str,
+        help='URL of the gacha api, please refer to README.md for details.',
+    )
+    gacha.add_argument(
+        '--export', nargs='+', type=str, default=['all'],
+        choices=['all', 'csv', 'html', 'json', 'md', 'xlsx'],
+        help='Types of expected export formats.',
+    )
+    gacha.add_argument(
         '--request-interval', type=float, default=0.1,
         help='Minimum interval (seconds) between two requests.',
     )
 
-    return parser.parse_args()
+    unlock = subparsers.add_parser('unlock')
+    unlock.add_argument(
+        '--fps', type=int,
+        help='Target FPS of the game',
+    )
+    unlock.add_argument(
+        '--reset', action='store_true',
+        help='Reset FPS to the initial value',
+    )
+
+    return parser
 
 
 def cli_check_update():
     if cfg.check_update:
         try:
             latest = check_update()
             logger.info('Check Update:')
@@ -59,33 +74,40 @@
                 logger.info(
                     f'If you use cli, please update with pip: `f{cmd}`',
                 )
                 logger.info('If you use GUI, please download executables:')
                 for name, url in latest.dist.items():
                     logger.info(f' * {babelfish.translate(name)}: {url}')
             else:
-                logger.info('No update is required.')
+                logger.info('Your program is the latest version.')
         except Exception:
             logger.warning(
                 'Check update failed. '
                 'Please check your network connection.',
             )
 
 
 def cli_entry():
-    args = parse_args()
+    parser = get_parser()
+    args = parser.parse_args()
     setup(log_level=args.log_level, locale=args.locale)
     logger.info(args)
     logger.info(cfg)
     cli_check_update()
-    export_gacha_from_api(
-        api_url=args.api,
-        export=args.export,
-        request_interval=args.request_interval,
-    )
+
+    if args.command == 'gacha':
+        export_gacha_from_api(
+            api_url=args.api,
+            export=args.export,
+            request_interval=args.request_interval,
+        )
+    elif args.command == 'unlock':
+        unlock_fps(fps=args.fps, reset=args.reset)
+    else:
+        parser.print_help()
 
 
 if __name__ == '__main__':
     try:
         cli_entry()
     except Exception:
         traceback.print_exc()
```

### Comparing `starrail-toolkit-0.5.8/starrail/entry/gui.py` & `starrail-toolkit-0.6.0/starrail/entry/gui.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 logger = loggings.get_logger(__file__)
 
 try:
     from PySide6.QtCore import Qt
     from PySide6.QtWidgets import QApplication
 
     from starrail.gui.application import StarRailToolkit
+    from starrail.gui.common.config import qcfg
 except ImportError as e:
     logger.critical(
         'Graphic mode is defaultly not enabled. If you want to run the GUI, '
         'please download the executables or launch from the source code. '
         'See: https://github.com/LittleNyima/honkai-starrail-toolkit for '
         'further information.',
     )
     raise e
 
 
 def gui_entry():
-    setup(log_level=cfg.log_level, locale=cfg.locale)
+    setup(log_level=cfg.log_level, locale=qcfg.locale.value.value.name())
 
     AA = Qt.ApplicationAttribute
     app = QApplication(sys.argv)
     app.setAttribute(AA.AA_DontCreateNativeWidgetSiblings)
 
     window = StarRailToolkit()
     window.show()
```

### Comparing `starrail-toolkit-0.5.8/starrail/entry/setup.py` & `starrail-toolkit-0.6.0/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gacha/autodet.py` & `starrail-toolkit-0.6.0/starrail/gacha/autodet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 import configparser
-import functools
-import importlib
 import os
 import platform
 import re
 from urllib.parse import parse_qsl, urlparse
 
 from starrail.utils import loggings
+from starrail.utils.misc import lazy_import
 
 logger = loggings.get_logger(__file__)
 
 
 reg_key_prefix = 'SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\Uninstall\\'
 reg_key_cn = reg_key_prefix + '崩坏：星穹铁道'
 # reg_key_os = reg_key_prefix + 'Star Rail'
 api_pattern = re.compile(r'https://.+/api/getGachaLog.+game_biz=hkrpg.+')
 
 
-@functools.lru_cache()
-def lazyload(module_name):
-    return importlib.import_module(module_name)
-
-
 def detect_game_install_path():
     logger.info('Detecting game install path')
-    winreg = lazyload('winreg')
+    winreg = lazy_import('winreg')
     with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, reg_key_cn) as rk:
         install_path = winreg.QueryValueEx(rk, 'InstallPath')[0]
     config_path = os.path.join(install_path, 'config.ini')
     parser = configparser.ConfigParser()
     parser.read(config_path)
     game_install_path = parser.get('launcher', 'game_install_path')
     if not os.path.exists(game_install_path):
```

### Comparing `starrail-toolkit-0.5.8/starrail/gacha/database.py` & `starrail-toolkit-0.6.0/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gacha/fetch.py` & `starrail-toolkit-0.6.0/starrail/gacha/fetch.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 import requests
 
 from starrail.utils import loggings
 
 logger = loggings.get_logger(__file__)
 
 
-def fetch_json(url):  # no typing annotations to pass mypy check
+def fetch_json(url, timeout=None):  # no typing annotations to pass mypy check
     """
     Fetches JSON content from a URL and returns it as a dictionary.
 
     Args:
         url: A string representing the URL to fetch the JSON content from.
 
     Returns:
         A dictionary representing the JSON content fetched from the URL.
     """
 
     try:
-        r = requests.get(url)
+        r = requests.get(url, timeout=timeout)
         if 200 <= r.status_code < 300:
             content = r.content.decode('utf-8', errors='ignore')
             payload = json.loads(content)
             logger.debug(json.dumps(payload, ensure_ascii=False, indent=2))
             return payload, r.status_code
     except Exception:
         traceback.print_exc()
```

### Comparing `starrail-toolkit-0.5.8/starrail/gacha/fileio.py` & `starrail-toolkit-0.6.0/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gacha/parse.py` & `starrail-toolkit-0.6.0/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gacha/service.py` & `starrail-toolkit-0.6.0/starrail/gacha/service.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gacha/url.py` & `starrail-toolkit-0.6.0/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gui/application.py` & `starrail-toolkit-0.6.0/starrail/gui/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from starrail.gui.common.config import qcfg
 from starrail.gui.common.icon import Icon
 from starrail.gui.common.stylesheet import StyleSheet
 from starrail.gui.common.utils import checkUpdate
 from starrail.gui.interfaces.gacha_sync import GachaSyncInterface
 from starrail.gui.interfaces.home import HomeInterface
 from starrail.gui.interfaces.setting import SettingInterface
+from starrail.gui.interfaces.unlock_fps import UnlockFpsInterface
 from starrail.gui.interfaces.users import UsersInterface
 from starrail.gui.widgets.title_bar import CustomTitleBar
 from starrail.utils import babelfish
 
 
 class StackedWidget(QFrame):
 
@@ -58,24 +59,29 @@
         self.hBoxLayout = QHBoxLayout(self)
         self.widgetLayout = QHBoxLayout()
 
         self.stackWidget = StackedWidget(self)
         self.navigationInterface = NavigationInterface(self, True, True)
 
         self.homeInterface = HomeInterface(self)
-        self.usersInterface = UsersInterface(
-            babelfish.ui_users(),
-            babelfish.ui_users_desc(),
-            self,
-        )
         self.gachaSyncInterface = GachaSyncInterface(
             babelfish.ui_gacha_sync(),
             babelfish.ui_gacha_sync_desc(),
             self,
         )
+        self.unlockFpsInterface = UnlockFpsInterface(
+            babelfish.ui_unlock_fps(),
+            babelfish.ui_unlock_fps_desc(),
+            self,
+        )
+        self.usersInterface = UsersInterface(
+            babelfish.ui_users(),
+            babelfish.ui_users_desc(),
+            self,
+        )
         self.settingInterface = SettingInterface(self)
 
         self.initLayout()
         self.initNavigation()
         self.initWindow()
 
     def initLayout(self):
@@ -109,14 +115,22 @@
             'gachaSyncInterface',
             qfluentwidgets.FluentIcon.SYNC,
             babelfish.ui_gacha_sync(),
             NavigationItemPosition.TOP,
         )
 
         self.addSubInterface(
+            self.unlockFpsInterface,
+            'unlockFpsInterface',
+            Icon.UNLOCK,
+            'unlock fps',
+            NavigationItemPosition.TOP,
+        )
+
+        self.addSubInterface(
             self.usersInterface,
             'usersInterface',
             Icon.USER,
             babelfish.ui_users(),
             NavigationItemPosition.BOTTOM,
         )
```

### Comparing `starrail-toolkit-0.5.8/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.6.0/starrail/gui/common/stylesheet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gui/common/utils.py` & `starrail-toolkit-0.6.0/starrail/gui/common/utils.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.6.0/starrail/gui/interfaces/gacha_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
 class GachaSyncInterface(BaseInterface):
 
     def __init__(self, title, subtitle, parent):
         super().__init__(title, subtitle, parent)
 
         # Buttons
-        self.buttonLayout = QtWidgets.QHBoxLayout()
+        self.buttonsCard = None
         self.syncButton = qfw.PrimaryPushButton(
             text=babelfish.ui_sync(),
             parent=self,
             icon=qfw.FluentIcon.SYNC,
         )
         self.syncButton.clicked.connect(self.onSyncButtonClicked)
         self.saveButton = qfw.PrimaryPushButton(
@@ -245,27 +245,25 @@
         if self.uid:
             self.updateTableDisplay()
             self.saveButton.setEnabled(True)
 
         self.__initWidget()
 
     def __initWidget(self):
-        self.buttonLayout.setSpacing(0)
-        self.buttonLayout.setContentsMargins(0, 0, 0, 0)
-        self.buttonLayout.setAlignment(AF.AlignLeft)
-        self.buttonLayout.addWidget(self.syncButton)
-        self.buttonLayout.addSpacing(10)
-        self.buttonLayout.addWidget(self.saveButton)
+        self.buttonsCard = self.addCard(babelfish.ui_operation_zone())
+        self.buttonsCard.addWidget(self.syncButton)
+        self.buttonsCard.addSpacing(10)
+        self.buttonsCard.addWidget(self.saveButton)
+        self.buttonsCard.addStretch(1)
 
         self.tableLayout.addWidget(self.stellarTable)
         self.tableLayout.addWidget(self.departureTable)
         self.tableLayout.addWidget(self.characterTable)
         self.tableLayout.addWidget(self.lightConeTable)
 
-        self.vBoxLayout.addLayout(self.buttonLayout)
         self.vBoxLayout.addLayout(self.tableLayout)
 
     def resizeEvent(self, e):
         if self.syncToolTip:
             self.syncToolTip.move(self.syncToolTip.getSuitablePos())
         return super().resizeEvent(e)
```

### Comparing `starrail-toolkit-0.5.8/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.6.0/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.6.0/starrail/gui/interfaces/setting.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,33 +10,54 @@
 from starrail.utils import babelfish
 
 
 class SettingInterface(qfw.ScrollArea):
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
+        self.initialParent = parent
         self.scrollWidget = QWidget()
         self.expandLayout = qfw.ExpandLayout(self.scrollWidget)
 
         self.settingLabel = QLabel(babelfish.ui_settings(), self)
 
         self.personalGroup = qfw.SettingCardGroup(
-            babelfish.ui_personalization(), self.scrollWidget,
+            title=babelfish.ui_personalization(),
+            parent=self.scrollWidget,
         )
         self.themeModeCard = qfw.OptionsSettingCard(
-            qcfg.themeMode,
-            FluentIcon.BRUSH,
-            babelfish.ui_theme_mode(),
-            babelfish.ui_theme_mode_settings_desc(),
-            [
+            configItem=qcfg.themeMode,
+            icon=FluentIcon.BRUSH,
+            title=babelfish.ui_theme_mode(),
+            content=babelfish.ui_theme_mode_settings_desc(),
+            texts=[
                 babelfish.ui_theme_mode_light(),
                 babelfish.ui_theme_mode_dark(),
-                babelfish.ui_theme_mode_auto(),
+                babelfish.ui_auto(),
             ],
-            self.personalGroup,
+            parent=self.personalGroup,
+        )
+        self.localeCard = qfw.OptionsSettingCard(
+            configItem=qcfg.locale,
+            icon=qfw.FluentIcon.LANGUAGE,
+            title=babelfish.ui_locale(),
+            content=babelfish.ui_locale_setting_desc(),
+            texts=[
+                babelfish.ui_auto(),
+                babelfish.ui_zhs(),
+                babelfish.ui_en(),
+            ],
+            parent=self.personalGroup,
+        )
+        self.checkUpdateCard = qfw.SwitchSettingCard(
+            icon=qfw.FluentIcon.UPDATE,
+            title=babelfish.ui_check_update_at_start(),
+            content=babelfish.ui_check_update_at_start_desc(),
+            configItem=qcfg.check_update,
+            parent=self.personalGroup,
         )
 
         self.aboutGroup = qfw.SettingCardGroup(
             babelfish.ui_about(), self.scrollWidget,
         )
         self.getStartCard = qfw.HyperlinkCard(
             babelfish.constants.DOCS_URL,
@@ -98,24 +119,38 @@
         self.settingLabel.setObjectName('settingLabel')
         StyleSheet.SETTING_INTERFACE.apply(self)
 
     def __initLayout(self):
         self.settingLabel.move(36, 30)
 
         self.personalGroup.addSettingCard(self.themeModeCard)
+        self.personalGroup.addSettingCard(self.localeCard)
+        self.personalGroup.addSettingCard(self.checkUpdateCard)
 
         self.aboutGroup.addSettingCard(self.getStartCard)
         self.aboutGroup.addSettingCard(self.troubleshootingCard)
         self.aboutGroup.addSettingCard(self.openSourceCard)
         self.aboutGroup.addSettingCard(self.feedbackCard)
         self.aboutGroup.addSettingCard(self.aboutCard)
 
         self.expandLayout.setSpacing(28)
         self.expandLayout.setContentsMargins(36, 10, 36, 0)
         self.expandLayout.addWidget(self.personalGroup)
         self.expandLayout.addWidget(self.aboutGroup)
 
+    def __showRestartToolTip(self):
+        qfw.InfoBar.success(
+            title=babelfish.ui_setting_restart_title(),
+            content=babelfish.ui_setting_restart_content(),
+            orient=Qt.Orientation.Horizontal,
+            isClosable=True,
+            duration=2000,
+            position=qfw.InfoBarPosition.TOP_RIGHT,
+            parent=self,
+        )
+
     def __connectSignalToSlot(self):
-        qfw.qconfig.themeChanged.connect(qfw.setTheme)
+        qcfg.themeChanged.connect(qfw.setTheme)
+        qcfg.appRestartSig.connect(self.__showRestartToolTip)
 
     def checkUpdateAction(self):
-        checkUpdate(parent=self.parent(), show_success=True)
+        checkUpdate(parent=self.initialParent, show_success=True)
```

### Comparing `starrail-toolkit-0.5.8/starrail/gui/widgets/dialog.py` & `starrail-toolkit-0.6.0/starrail/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gui/widgets/link_card.py` & `starrail-toolkit-0.6.0/starrail/gui/widgets/link_card.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.6.0/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/utils/accounts.py` & `starrail-toolkit-0.6.0/starrail/utils/accounts.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/utils/auto_update.py` & `starrail-toolkit-0.6.0/starrail/utils/auto_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     'changelog': 'desc'
 }
 """
 
 
 def get_distribution(cdn_type):
     distribution = fr'{cdn_templ[cdn_type]}releases/dist.json'
-    return fetch_json(distribution)
+    return fetch_json(distribution, timeout=5)
 
 
 def check_update():
-    for cdn_type in ['github', 'gitee']:
+    for cdn_type in ['gitee', 'github']:
         payload, _ = get_distribution(cdn_type)
         if payload is not None:
             return easydict.EasyDict(payload)
     return None
```

### Comparing `starrail-toolkit-0.5.8/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.6.0/starrail/utils/babelfish/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,68 +7,89 @@
 gacha_report = dictionary.gacha_report
 gacha_title = dictionary.gacha_title
 history_of_5_stars = dictionary.history_of_5_stars
 html_thead = dictionary.html_thead
 markdown_thead = dictionary.markdown_thead
 ui_about = dictionary.ui_about
 ui_about_this = dictionary.ui_about_this
+ui_auto = dictionary.ui_auto
 ui_cancel_update = dictionary.ui_cancel_update
 ui_check_update = dictionary.ui_check_update
+ui_check_update_at_start = dictionary.ui_check_update_at_start
+ui_check_update_at_start_desc = dictionary.ui_check_update_at_start_desc
 ui_check_update_fail = dictionary.ui_check_update_fail
 ui_check_update_success = dictionary.ui_check_update_success
 ui_copyright = dictionary.ui_copyright
+ui_curr_fps = dictionary.ui_curr_fps
 ui_current_version = dictionary.ui_current_version
 ui_deduce_uid_fail = dictionary.ui_deduce_uid_fail
 ui_downloading_gacha = dictionary.ui_downloading_gacha
+ui_en = dictionary.ui_en
 ui_extract_api_fail = dictionary.ui_extract_api_fail
 ui_extract_api_fail_with_msg = dictionary.ui_extract_api_fail_with_msg
 ui_extracting_api_url = dictionary.ui_extracting_api_url
 ui_fine = dictionary.ui_fine
 ui_fine1 = dictionary.ui_fine1
 ui_fine2 = dictionary.ui_fine2
+ui_fps_is_already = dictionary.ui_fps_is_already
+ui_fps_is_set_to = dictionary.ui_fps_is_set_to
 ui_gacha_basic_prob = dictionary.ui_gacha_basic_prob
 ui_gacha_count = dictionary.ui_gacha_count
 ui_gacha_since_last = dictionary.ui_gacha_since_last
 ui_gacha_sync = dictionary.ui_gacha_sync
 ui_gacha_sync_desc = dictionary.ui_gacha_sync_desc
 ui_gacha_true_prob = dictionary.ui_gacha_true_prob
 ui_gacha_type = dictionary.ui_gacha_type
 ui_get_started = dictionary.ui_get_started
 ui_get_started_desc = dictionary.ui_get_started_desc
 ui_github_repo = dictionary.ui_github_repo
 ui_github_repo_desc = dictionary.ui_github_repo_desc
 ui_is_latest_version = dictionary.ui_is_latest_version
+ui_locale = dictionary.ui_locale
+ui_locale_setting_desc = dictionary.ui_locale_setting_desc
 ui_no_data = dictionary.ui_no_data
 ui_not_good = dictionary.ui_not_good
 ui_ooops = dictionary.ui_ooops
 ui_open_docs = dictionary.ui_open_docs
 ui_open_issues = dictionary.ui_open_issues
 ui_open_repo = dictionary.ui_open_repo
 ui_open_troubleshooting = dictionary.ui_open_troubleshooting
+ui_operation_zone = dictionary.ui_operation_zone
 ui_personalization = dictionary.ui_personalization
+ui_reset_fps = dictionary.ui_reset_fps
+ui_reset_panel = dictionary.ui_reset_panel
 ui_save_data = dictionary.ui_save_data
 ui_save_success = dictionary.ui_save_success
 ui_save_success_msg = dictionary.ui_save_success_msg
 ui_send_feedback = dictionary.ui_send_feedback
 ui_send_feedback_desc = dictionary.ui_send_feedback_desc
+ui_set_fps_fail_with_msg = dictionary.ui_set_fps_fail_with_msg
+ui_setting_failure = dictionary.ui_setting_failure
+ui_setting_panel = dictionary.ui_setting_panel
+ui_setting_restart_content = dictionary.ui_setting_restart_content
+ui_setting_restart_title = dictionary.ui_setting_restart_title
+ui_setting_success = dictionary.ui_setting_success
 ui_settings = dictionary.ui_settings
+ui_status_panel = dictionary.ui_status_panel
 ui_sync = dictionary.ui_sync
 ui_sync_gacha_fail = dictionary.ui_sync_gacha_fail
 ui_sync_gacha_initial = dictionary.ui_sync_gacha_initial
 ui_sync_gacha_success = dictionary.ui_sync_gacha_success
 ui_synchronizing_gacha = dictionary.ui_synchronizing_gacha
 ui_theme_mode = dictionary.ui_theme_mode
-ui_theme_mode_auto = dictionary.ui_theme_mode_auto
 ui_theme_mode_dark = dictionary.ui_theme_mode_dark
 ui_theme_mode_light = dictionary.ui_theme_mode_light
 ui_theme_mode_settings_desc = dictionary.ui_theme_mode_settings_desc
 ui_title = dictionary.ui_title
 ui_traceback = dictionary.ui_traceback
 ui_troubleshooting = dictionary.ui_troubleshooting
 ui_troubleshooting_desc = dictionary.ui_troubleshooting_desc
+ui_unlock_fps = dictionary.ui_unlock_fps
+ui_unlock_fps_desc = dictionary.ui_unlock_fps_desc
 ui_update_available = dictionary.ui_update_available
 ui_update_desc = dictionary.ui_update_desc
 ui_users = dictionary.ui_users
 ui_users_desc = dictionary.ui_users_desc
 ui_welcome = dictionary.ui_welcome
+ui_zhs = dictionary.ui_zhs
 
 __all__ = ['constants', 'translate']
```

### Comparing `starrail-toolkit-0.5.8/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.6.0/starrail/utils/babelfish/dictionary.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,40 +41,57 @@
     zhs=(
         '| 星级 | 数量 | 基础概率 | 综合概率 | 距上次 |\n'
         '| ---- | ---- | ------ | ------- | ---- |\n'
     ),
 )
 ui_about = _MS(en='About', zhs='关于')
 ui_about_this = _MS(en='About This Application', zhs='关于本软件')
+ui_auto = _MS(en='Auto', zhs='跟随系统设置')
 ui_cancel_update = _MS(en='Cancel Update', zhs='暂不更新')
 ui_check_update = _MS(en='Check Update', zhs='检查更新')
+ui_check_update_at_start = _MS(
+    en='Check Update at Application Start',
+    zhs='启动时自动检查更新',
+)
+ui_check_update_at_start_desc = _MS(
+    en='It\'s strongly recommended to turn this on to get the latest feature',
+    zhs='强烈建议打开检查更新，本app版本快速迭代中，会加入更多功能。',
+)
 ui_check_update_fail = _MS(
     en='Check update failed. Please check your network connection.',
     zhs='检查更新失败，请检查你的网络连接并重试。（不重试也行，但是你可能没联网）',
 )
 ui_check_update_success = _MS(
     en='Check update finished',
     zhs='检查更新完成',
 )
 ui_copyright = _MS(
     en='Copyright © {} LittleNyima.',
     zhs='版权所有 © {} LittleNyima。',
 )
+ui_curr_fps = _MS(
+    en='Current FPS in Game Settings: {}.',
+    zhs='当前游戏设定帧率：{}。',
+)
 ui_current_version = _MS(
     en='Current version: {}.',
     zhs='当前版本：{}。',
 )
 ui_deduce_uid_fail = _MS(
     en='Fail to deduce uid. There may be no record. Please check.',
     zhs='检测 UID 失败，账号可能没有抽卡记录，请重试。',
 )
 ui_downloading_gacha = _MS(
     en='Downloading page {page} of type {name}',
     zhs='正在导出{name}的第{page}页',
 )
+ui_en = _MS(
+    en='English',
+    zhs='英语',
+)
 ui_extract_api_fail = _MS(
     en='Extracting API URL failed. Please retry after exiting the game.',
     zhs='提取 API URL 失败，请关闭游戏或重新查询抽卡信息后重试。',
 )
 ui_extract_api_fail_with_msg = _MS(
     en='Extracting API URL failed. Failed with: {}',
     zhs='提取 API URL 失败，遇到的问题：{}',
@@ -82,14 +99,22 @@
 ui_extracting_api_url = _MS(
     en='Extracting API URL',
     zhs='正在提取 API URL',
 )
 ui_fine = _MS(en='Fine', zhs='好')
 ui_fine1 = _MS(en='Fine', zhs='好的')
 ui_fine2 = _MS(en='Fine', zhs='好吧')
+ui_fps_is_already = _MS(
+    en='FPS is already {}~',
+    zhs='帧率已经是{}啦～',
+)
+ui_fps_is_set_to = _MS(
+    en='FPS is successfully set to {}.',
+    zhs='帧率已成功设置为{}。',
+)
 ui_gacha_basic_prob = _MS(en='Basic Prob.', zhs='基础概率')
 ui_gacha_count = _MS(en='Count', zhs='数量')
 ui_gacha_since_last = _MS(en='Since Last', zhs='距上次')
 ui_gacha_sync = _MS(en='Sync Gacha Data', zhs='抽卡数据同步')
 ui_gacha_sync_desc = _MS(
     en=(
         'First query warp record in the game, then close the game and click '
@@ -109,31 +134,55 @@
     en='This project is open-resource, licenced under GPLv3. View code here.',
     zhs='本项目代码开源，以 GPLv3 分发。点此查看源代码。',
 )
 ui_is_latest_version = _MS(
     en='Your application is the latest version.',
     zhs='已经是最新版本啦',
 )
+ui_locale = _MS(en='Display Language', zhs='显示语言')
+ui_locale_setting_desc = _MS(en='Changing the display language', zhs='改变显示语言')
 ui_no_data = _MS(en='No Data', zhs='暂无数据')
 ui_not_good = _MS(en='No', zhs='不好')
 ui_ooops = _MS(en='OOOPS!', zhs='出错了！')
 ui_open_docs = _MS(en='Open Documentations', zhs='打开帮助页面')
 ui_open_issues = _MS(en='Open Issue Page', zhs='打开反馈页面')
 ui_open_repo = _MS(en='Open GitHub Repo', zhs='打开代码仓库')
 ui_open_troubleshooting = _MS(en='Open Troubleshooting', zhs='打开常见问题')
+ui_operation_zone = _MS(en='Operations', zhs='操作区')
 ui_personalization = _MS(en='Personalization', zhs='个性化')
+ui_reset_fps = _MS(
+    en='Reset FPS',
+    zhs='重置帧率',
+)
+ui_reset_panel = _MS(en='Reset Panel', zhs='重置面板')
 ui_save_data = _MS(en='Save As', zhs='保存数据')
 ui_save_success = _MS(en='Data Save Success', zhs='保存成功')
 ui_save_success_msg = _MS(en='Data is saved to {}', zhs='数据已保存到{}')
 ui_send_feedback = _MS(en='Send Feedback', zhs='提交反馈')
 ui_send_feedback_desc = _MS(
     en='Feedback is welcome if you encounter problems or have suggestions.',
     zhs='如果你遇到问题，或对本项目有更多建议，欢迎提交反馈。',
 )
+ui_set_fps_fail_with_msg = _MS(
+    en='Setting FPS failed. Failed with: {}',
+    zhs='设置帧率失败，遇到的问题：{}',
+)
+ui_setting_failure = _MS(
+    en='Error',
+    zhs='设置失败',
+)
+ui_setting_panel = _MS(en='Setting Panel', zhs='设置面板')
+ui_setting_restart_content = _MS(
+    en='Please restart to apply changes.',
+    zhs='请重启以应用新设置。',
+)
+ui_setting_restart_title = _MS(en='Success', zhs='设置成功')
+ui_setting_success = _MS(en='Success', zhs='设置成功')
 ui_settings = _MS(en='Settings', zhs='设置')
+ui_status_panel = _MS(en='Status Panel', zhs='状态面板')
 ui_sync = _MS(en='Sync Data', zhs='同步数据')
 ui_sync_gacha_fail = _MS(
     en='Synchronization Failed',
     zhs='同步失败',
 )
 ui_sync_gacha_initial = _MS(
     en='Initializing...',
@@ -144,28 +193,38 @@
     zhs='同步成功',
 )
 ui_synchronizing_gacha = _MS(
     en='Synchronizing...',
     zhs='正在同步抽卡数据',
 )
 ui_theme_mode = _MS(en='Theme Mode', zhs='应用主题')
-ui_theme_mode_auto = _MS(en='Auto', zhs='跟随系统设置')
 ui_theme_mode_dark = _MS(en='Dark', zhs='深色')
 ui_theme_mode_light = _MS(en='Light', zhs='浅色')
 ui_theme_mode_settings_desc = _MS(
     en='Changing the appearance of application',
     zhs='改变应用外观',
 )
 ui_title = _MS(en='Honkai: Star Rail Toolkit', zhs='崩坏：星穹铁道工具箱')
 ui_traceback = _MS(en='Traceback', zhs='报错信息')
 ui_troubleshooting = _MS(en='TroubleShooting', zhs='常见问题')
 ui_troubleshooting_desc = _MS(
     en='Click here to view FAQ.',
     zhs='点此查看常见问题解答。',
 )
+ui_unlock_fps = _MS(
+    en='Unlock FPS Settings',
+    zhs='解锁帧率',
+)
+ui_unlock_fps_desc = _MS(
+    en=(
+        'First set the frame rate in the game at least once, and then use the '
+        'functions of this interface.'
+    ),
+    zhs='首先至少在游戏中设置一次帧率，再使用本页面中的功能。',
+)
 ui_update_available = _MS(
     en='New Version is Available',
     zhs='检查到新版本',
 )
 ui_update_desc = _MS(
     en=(
         'New Version of Honkai: Star Rail Toolkit is available. '
@@ -180,9 +239,13 @@
 )
 ui_users = _MS(en='Users', zhs='用户管理')
 ui_users_desc = _MS(en='Multi-user management', zhs='如果有多个账号可以用这个切换')
 ui_welcome = _MS(
     en='Welcome to HKSR Toolkit!',
     zhs='欢迎登车！',
 )
+ui_zhs = _MS(
+    en='Simplified Chinese',
+    zhs='简体中文',
+)
 
 # === END OF PRE-DEFINED VOCABULARIES ===
```

### Comparing `starrail-toolkit-0.5.8/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.6.0/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail/utils/loggings.py` & `starrail-toolkit-0.6.0/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.8/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.6.0/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.8
+Version: 0.6.0
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,42 +14,48 @@
 License-File: LICENSE
 
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
+
+<b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
+
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.5.8    |    0.5.8     |   0.5.8   |   0.5.4    |
+|   0.6.0    |    0.6.0     |   0.6.0   |   0.6.0    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
-- [ ] 支持更多的可设置选项
+- [x] 支持更多的可设置选项
 - [ ] 支持国际服
+- [x] 支持解锁120帧
 - [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
-- [ ] 美化抽卡导出页面
+- [ ] 美化程序界面
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i8l5L0v48e5i)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/iwDYF0x00q0f)，两种途径的内容相同，可以自行选择下载方式。
 
 ***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
 
-![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+![gui preview gacha](https://s1.ax1x.com/2023/05/23/p9o7y3d.png)
+
+![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 python3 -m pip install starrail-toolkit --force-reinstall --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
@@ -79,27 +85,29 @@
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
 # 非 Windows 平台
-hksr --api https://api-takumi.mihoyo.com/xxx
+hksr gacha --api https://api-takumi.mihoyo.com/xxx
 # Windows 平台无需 --api 参数
-hksr
+hksr gacha
 ```
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
 - `--request-interval`：（可选）请求间隔。两次请求之间的最小间隔，默认为 `0.1`。若某些情况下因请求过于频繁导致 IP 被 ban，可以适度把这个值调大一点。
 
+**如果想要进一步了解命令行使用方法，请参考[命令行使用指南](docs/cli-guidance.md)。**
+
 本项目目前正处于快速迭代阶段，使用方式可能会发生改变，请及时更新程序，更新时请留意本部分关于使用方式的说明。
 
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
```

### Comparing `starrail-toolkit-0.5.8/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.6.0/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,23 +25,28 @@
 starrail/gui/common/stylesheet.py
 starrail/gui/common/utils.py
 starrail/gui/interfaces/__init__.py
 starrail/gui/interfaces/base.py
 starrail/gui/interfaces/gacha_sync.py
 starrail/gui/interfaces/home.py
 starrail/gui/interfaces/setting.py
+starrail/gui/interfaces/unlock_fps.py
 starrail/gui/interfaces/users.py
 starrail/gui/widgets/__init__.py
 starrail/gui/widgets/dialog.py
 starrail/gui/widgets/link_card.py
 starrail/gui/widgets/title_bar.py
+starrail/unlock/__init__.py
+starrail/unlock/fps.py
+starrail/unlock/service.py
 starrail/utils/__init__.py
 starrail/utils/accounts.py
 starrail/utils/auto_update.py
 starrail/utils/loggings.py
+starrail/utils/misc.py
 starrail/utils/babelfish/__init__.py
 starrail/utils/babelfish/constants.py
 starrail/utils/babelfish/dictionary.py
 starrail/utils/babelfish/locale.py
 starrail/utils/babelfish/multilingual.py
 starrail/utils/babelfish/translate.py
 starrail_toolkit.egg-info/PKG-INFO
```

