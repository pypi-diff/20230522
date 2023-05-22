# Comparing `tmp/fez-language-1.3.4.tar.gz` & `tmp/fez-language-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fez-language-1.3.4.tar", last modified: Thu Oct 13 08:55:40 2022, max compression
+gzip compressed data, was "fez-language-1.4.0.tar", last modified: Mon May 22 09:41:39 2023, max compression
```

## Comparing `fez-language-1.3.4.tar` & `fez-language-1.4.0.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.435002 fez-language-1.3.4/
--rw-r--r--   0 simon      (501) staff       (20)      129 2021-06-11 13:22:17.000000 fez-language-1.3.4/.readthedocs.yaml
--rw-r--r--   0 simon      (501) staff       (20)      340 2021-10-28 11:02:46.000000 fez-language-1.3.4/AUTHORS.txt
--rw-r--r--   0 simon      (501) staff       (20)     1094 2021-10-28 11:03:18.000000 fez-language-1.3.4/CONTRIBUTORS.txt
--rw-r--r--   0 simon      (501) staff       (20)     1520 2021-10-28 11:12:50.000000 fez-language-1.3.4/LICENSE
--rw-r--r--   0 simon      (501) staff       (20)     2160 2021-06-11 11:47:21.000000 fez-language-1.3.4/Makefile
--rw-r--r--   0 simon      (501) staff       (20)     3208 2022-10-13 08:55:40.434760 fez-language-1.3.4/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     2639 2022-10-13 08:33:23.000000 fez-language-1.3.4/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.411928 fez-language-1.3.4/bin/
--rwxr-xr-x   0 simon      (501) staff       (20)     1659 2022-10-13 08:33:23.000000 fez-language-1.3.4/bin/fez2fea
--rwxr-xr-x   0 simon      (501) staff       (20)     1265 2021-06-11 13:35:56.000000 fez-language-1.3.4/bin/mergefez
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.414579 fez-language-1.3.4/docs/
--rw-r--r--   0 simon      (501) staff       (20)      634 2021-06-11 11:41:40.000000 fez-language-1.3.4/docs/Makefile
--rw-r--r--   0 simon      (501) staff       (20)     1976 2021-10-23 21:07:43.000000 fez-language-1.3.4/docs/conf.py
--rw-r--r--   0 simon      (501) staff       (20)    38622 2021-06-11 11:44:43.000000 fez-language-1.3.4/docs/fez.png
--rw-r--r--   0 simon      (501) staff       (20)    12096 2022-10-13 08:33:23.000000 fez-language-1.3.4/docs/getting-started.rst
--rw-r--r--   0 simon      (501) staff       (20)     1016 2021-10-23 20:51:48.000000 fez-language-1.3.4/docs/index.rst
--rw-r--r--   0 simon      (501) staff       (20)      727 2021-10-23 12:11:20.000000 fez-language-1.3.4/docs/optionalverbs.rst
--rw-r--r--   0 simon      (501) staff       (20)    11781 2021-10-22 13:02:47.000000 fez-language-1.3.4/docs/plugins.rst
--rw-r--r--   0 simon      (501) staff       (20)      149 2021-06-11 13:11:18.000000 fez-language-1.3.4/docs/rtd-requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5570 2022-10-13 08:33:23.000000 fez-language-1.3.4/docs/syntax.rst
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.417337 fez-language-1.3.4/fez-samples/
--rw-r--r--   0 simon      (501) staff       (20)      446 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/anchors.fez
--rw-r--r--   0 simon      (501) staff       (20)       42 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/binned.fez
--rw-r--r--   0 simon      (501) staff       (20)      110 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/chain.fez
--rw-r--r--   0 simon      (501) staff       (20)      117 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/collision.fea
--rw-r--r--   0 simon      (501) staff       (20)      192 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/kerntodistance.fea
--rw-r--r--   0 simon      (501) staff       (20)      121 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/languages.fez
--rw-r--r--   0 simon      (501) staff       (20)       77 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/matras.fez
--rw-r--r--   0 simon      (501) staff       (20)      366 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/new-bariye.fez
--rw-r--r--   0 simon      (501) staff       (20)      483 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/noto-urdu.fea
--rw-r--r--   0 simon      (501) staff       (20)    11929 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/qalmi.fez
--rw-r--r--   0 simon      (501) staff       (20)     1771 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/test-fred.fez
--rw-r--r--   0 simon      (501) staff       (20)       39 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/test-include.fez
--rw-r--r--   0 simon      (501) staff       (20)      172 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/test-lang.fez
--rw-r--r--   0 simon      (501) staff       (20)      932 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/test.fez
--rw-r--r--   0 simon      (501) staff       (20)      348 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/variables.fez
--rw-r--r--   0 simon      (501) staff       (20)      425 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/yb-dropdots.fez
--rw-r--r--   0 simon      (501) staff       (20)      180 2021-06-11 10:24:20.000000 fez-language-1.3.4/fez-samples/yb-overhangfix.fez
--rw-r--r--   0 simon      (501) staff       (20)    38622 2021-06-11 11:39:01.000000 fez-language-1.3.4/fez.png
--rw-r--r--   0 simon      (501) staff       (20)    35173 2021-06-11 11:37:41.000000 fez-language-1.3.4/fez.svg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.408479 fez-language-1.3.4/lib/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.422690 fez-language-1.3.4/lib/fez/
--rw-r--r--   0 simon      (501) staff       (20)     8012 2022-01-30 22:23:15.000000 fez-language-1.3.4/lib/fez/Anchors.py
--rw-r--r--   0 simon      (501) staff       (20)     1116 2021-06-11 10:24:20.000000 fez-language-1.3.4/lib/fez/Arabic.py
--rw-r--r--   0 simon      (501) staff       (20)     2911 2021-06-11 10:24:20.000000 fez-language-1.3.4/lib/fez/AvoidCollision.py
--rw-r--r--   0 simon      (501) staff       (20)    18335 2022-10-13 08:33:23.000000 fez-language-1.3.4/lib/fez/BariYe.py
--rw-r--r--   0 simon      (501) staff       (20)     2462 2021-10-28 14:11:24.000000 fez-language-1.3.4/lib/fez/Chain.py
--rw-r--r--   0 simon      (501) staff       (20)    12302 2021-11-24 11:25:40.000000 fez-language-1.3.4/lib/fez/ClassDefinition.py
--rw-r--r--   0 simon      (501) staff       (20)     1805 2022-06-23 09:06:13.000000 fez-language-1.3.4/lib/fez/Conditional.py
--rw-r--r--   0 simon      (501) staff       (20)      654 2021-10-11 11:57:25.000000 fez-language-1.3.4/lib/fez/CopyAnchors.py
--rw-r--r--   0 simon      (501) staff       (20)      981 2021-06-11 10:24:20.000000 fez-language-1.3.4/lib/fez/Debug.py
--rw-r--r--   0 simon      (501) staff       (20)      782 2021-06-11 10:24:20.000000 fez-language-1.3.4/lib/fez/Delete.py
--rw-r--r--   0 simon      (501) staff       (20)     2204 2022-10-13 08:33:23.000000 fez-language-1.3.4/lib/fez/Feature.py
--rw-r--r--   0 simon      (501) staff       (20)     3861 2021-06-17 14:24:16.000000 fez-language-1.3.4/lib/fez/FontEngineering.py
--rw-r--r--   0 simon      (501) staff       (20)     1051 2021-11-24 12:44:21.000000 fez-language-1.3.4/lib/fez/ForLoop.py
--rw-r--r--   0 simon      (501) staff       (20)     3196 2021-06-17 14:19:46.000000 fez-language-1.3.4/lib/fez/IMatra.py
--rw-r--r--   0 simon      (501) staff       (20)     3906 2021-06-11 10:24:20.000000 fez-language-1.3.4/lib/fez/IfCollides.py
--rw-r--r--   0 simon      (501) staff       (20)     1262 2021-11-24 12:35:15.000000 fez-language-1.3.4/lib/fez/Include.py
--rw-r--r--   0 simon      (501) staff       (20)     2495 2021-06-11 10:24:20.000000 fez-language-1.3.4/lib/fez/KernToDistance.py
--rw-r--r--   0 simon      (501) staff       (20)     2682 2022-10-13 08:54:56.000000 fez-language-1.3.4/lib/fez/Kerning.py
--rw-r--r--   0 simon      (501) staff       (20)     1268 2021-06-11 10:24:20.000000 fez-language-1.3.4/lib/fez/LigatureFinder.py
--rw-r--r--   0 simon      (501) staff       (20)     1541 2021-11-24 12:35:18.000000 fez-language-1.3.4/lib/fez/LoadPlugin.py
--rw-r--r--   0 simon      (501) staff       (20)     2073 2021-06-17 14:39:56.000000 fez-language-1.3.4/lib/fez/MedialRa.py
--rw-r--r--   0 simon      (501) staff       (20)     4057 2021-11-24 11:10:55.000000 fez-language-1.3.4/lib/fez/Position.py
--rw-r--r--   0 simon      (501) staff       (20)     5403 2022-10-13 08:33:23.000000 fez-language-1.3.4/lib/fez/Routine.py
--rw-r--r--   0 simon      (501) staff       (20)     3849 2021-11-24 11:57:41.000000 fez-language-1.3.4/lib/fez/Substitute.py
--rw-r--r--   0 simon      (501) staff       (20)     1607 2021-11-24 12:38:01.000000 fez-language-1.3.4/lib/fez/Swap.py
--rw-r--r--   0 simon      (501) staff       (20)     1783 2022-10-13 08:33:23.000000 fez-language-1.3.4/lib/fez/Variables.py
--rw-r--r--   0 simon      (501) staff       (20)    22172 2022-10-13 08:32:50.000000 fez-language-1.3.4/lib/fez/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      423 2021-06-11 10:24:20.000000 fez-language-1.3.4/lib/fez/util.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.423473 fez-language-1.3.4/lib/fez_language.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     3208 2022-10-13 08:55:40.000000 fez-language-1.3.4/lib/fez_language.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     2427 2022-10-13 08:55:40.000000 fez-language-1.3.4/lib/fez_language.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2022-10-13 08:55:40.000000 fez-language-1.3.4/lib/fez_language.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2022-10-13 08:55:40.000000 fez-language-1.3.4/lib/fez_language.egg-info/not-zip-safe
--rw-r--r--   0 simon      (501) staff       (20)      102 2022-10-13 08:55:40.000000 fez-language-1.3.4/lib/fez_language.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        4 2022-10-13 08:55:40.000000 fez-language-1.3.4/lib/fez_language.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)      102 2021-12-02 09:15:32.000000 fez-language-1.3.4/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)       38 2022-10-13 08:55:40.435099 fez-language-1.3.4/setup.cfg
--rw-r--r--   0 simon      (501) staff       (20)     1251 2022-10-13 08:55:37.000000 fez-language-1.3.4/setup.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.424960 fez-language-1.3.4/tests/
--rw-r--r--   0 simon      (501) staff       (20)      156 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.433140 fez-language-1.3.4/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)     1008 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
--rw-r--r--   0 simon      (501) staff       (20)     1380 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
--rw-r--r--   0 simon      (501) staff       (20)     1084 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/341421e629668b1a1242245d39238ca48432d35d.ttf
--rw-r--r--   0 simon      (501) staff       (20)     3300 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
--rw-r--r--   0 simon      (501) staff       (20)     1204 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
--rw-r--r--   0 simon      (501) staff       (20)    22980 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
--rw-r--r--   0 simon      (501) staff       (20)   554616 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/Amiri-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)   496504 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/LibertinusSans-Regular.otf
--rw-r--r--   0 simon      (501) staff       (20)     6353 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/Noto Sans Sharada GSUB.txt
--rw-r--r--   0 simon      (501) staff       (20)   515100 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/Roboto-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     5555 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/SimpleTwoAxis.glyphs
--rw-r--r--   0 simon      (501) staff       (20)     2720 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/a014549f766436cf55b2ceb40e462038938ee899.ttf
--rw-r--r--   0 simon      (501) staff       (20)     1840 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/acbe26ce904463c690fb67f70679447059d13ee4.otf
--rw-r--r--   0 simon      (501) staff       (20)     6332 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
--rw-r--r--   0 simon      (501) staff       (20)    41830 2021-06-11 10:24:20.000000 fez-language-1.3.4/tests/data/notdef.ttx
--rw-r--r--   0 simon      (501) staff       (20)      982 2021-06-11 10:24:31.000000 fez-language-1.3.4/tests/test_classdefs.py
--rw-r--r--   0 simon      (501) staff       (20)     1288 2021-11-24 12:38:23.000000 fez-language-1.3.4/tests/test_fez.py
--rw-r--r--   0 simon      (501) staff       (20)     1321 2021-10-19 12:52:46.000000 fez-language-1.3.4/tests/test_fez_anchors.py
--rw-r--r--   0 simon      (501) staff       (20)     7121 2021-11-24 13:01:59.000000 fez-language-1.3.4/tests/test_fez_parser.py
--rw-r--r--   0 simon      (501) staff       (20)     1133 2021-10-19 12:52:22.000000 fez-language-1.3.4/tests/test_languages.py
--rw-r--r--   0 simon      (501) staff       (20)     1395 2021-11-24 12:06:44.000000 fez-language-1.3.4/tests/test_variable.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-10-13 08:55:40.434463 fez-language-1.3.4/vim/
--rw-r--r--   0 simon      (501) staff       (20)     1728 2021-06-11 10:24:20.000000 fez-language-1.3.4/vim/fee.vim
--rw-r--r--   0 simon      (501) staff       (20)     3307 2021-11-24 13:25:19.000000 fez-language-1.3.4/vim/fez.iro
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.825661 fez-language-1.4.0/
+-rw-r--r--   0 simon      (501) staff       (20)      129 2021-06-11 13:22:17.000000 fez-language-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 simon      (501) staff       (20)      313 2023-02-03 11:08:13.000000 fez-language-1.4.0/AUTHORS.txt
+-rw-r--r--   0 simon      (501) staff       (20)     1094 2021-10-28 11:03:18.000000 fez-language-1.4.0/CONTRIBUTORS.txt
+-rw-r--r--   0 simon      (501) staff       (20)     1517 2023-02-03 11:08:13.000000 fez-language-1.4.0/LICENSE
+-rw-r--r--   0 simon      (501) staff       (20)     2160 2021-06-11 11:47:21.000000 fez-language-1.4.0/Makefile
+-rw-r--r--   0 simon      (501) staff       (20)     3188 2023-05-22 09:41:39.825506 fez-language-1.4.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     2639 2022-10-13 08:33:23.000000 fez-language-1.4.0/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.801755 fez-language-1.4.0/bin/
+-rwxr-xr-x   0 simon      (501) staff       (20)     1659 2022-10-13 08:33:23.000000 fez-language-1.4.0/bin/fez2fea
+-rwxr-xr-x   0 simon      (501) staff       (20)     1265 2021-06-11 13:35:56.000000 fez-language-1.4.0/bin/mergefez
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.804159 fez-language-1.4.0/docs/
+-rw-r--r--   0 simon      (501) staff       (20)      634 2021-06-11 11:41:40.000000 fez-language-1.4.0/docs/Makefile
+-rw-r--r--   0 simon      (501) staff       (20)     1976 2021-10-23 21:07:43.000000 fez-language-1.4.0/docs/conf.py
+-rw-r--r--   0 simon      (501) staff       (20)    38622 2021-06-11 11:44:43.000000 fez-language-1.4.0/docs/fez.png
+-rw-r--r--   0 simon      (501) staff       (20)    12096 2022-10-13 08:33:23.000000 fez-language-1.4.0/docs/getting-started.rst
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2021-10-23 20:51:48.000000 fez-language-1.4.0/docs/index.rst
+-rw-r--r--   0 simon      (501) staff       (20)      757 2023-05-22 09:03:37.000000 fez-language-1.4.0/docs/optionalverbs.rst
+-rw-r--r--   0 simon      (501) staff       (20)    11781 2021-10-22 13:02:47.000000 fez-language-1.4.0/docs/plugins.rst
+-rw-r--r--   0 simon      (501) staff       (20)      149 2021-06-11 13:11:18.000000 fez-language-1.4.0/docs/rtd-requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5570 2022-10-13 08:33:23.000000 fez-language-1.4.0/docs/syntax.rst
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.807115 fez-language-1.4.0/fez-samples/
+-rw-r--r--   0 simon      (501) staff       (20)      446 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/anchors.fez
+-rw-r--r--   0 simon      (501) staff       (20)       42 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/binned.fez
+-rw-r--r--   0 simon      (501) staff       (20)      110 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/chain.fez
+-rw-r--r--   0 simon      (501) staff       (20)      117 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/collision.fea
+-rw-r--r--   0 simon      (501) staff       (20)      192 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/kerntodistance.fea
+-rw-r--r--   0 simon      (501) staff       (20)      121 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/languages.fez
+-rw-r--r--   0 simon      (501) staff       (20)       77 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/matras.fez
+-rw-r--r--   0 simon      (501) staff       (20)      366 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/new-bariye.fez
+-rw-r--r--   0 simon      (501) staff       (20)      483 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/noto-urdu.fea
+-rw-r--r--   0 simon      (501) staff       (20)    11929 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/qalmi.fez
+-rw-r--r--   0 simon      (501) staff       (20)     1771 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/test-fred.fez
+-rw-r--r--   0 simon      (501) staff       (20)       39 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/test-include.fez
+-rw-r--r--   0 simon      (501) staff       (20)      172 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/test-lang.fez
+-rw-r--r--   0 simon      (501) staff       (20)      932 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/test.fez
+-rw-r--r--   0 simon      (501) staff       (20)      348 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/variables.fez
+-rw-r--r--   0 simon      (501) staff       (20)      425 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/yb-dropdots.fez
+-rw-r--r--   0 simon      (501) staff       (20)      180 2021-06-11 10:24:20.000000 fez-language-1.4.0/fez-samples/yb-overhangfix.fez
+-rw-r--r--   0 simon      (501) staff       (20)    38622 2021-06-11 11:39:01.000000 fez-language-1.4.0/fez.png
+-rw-r--r--   0 simon      (501) staff       (20)    35173 2021-06-11 11:37:41.000000 fez-language-1.4.0/fez.svg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.798967 fez-language-1.4.0/lib/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.812982 fez-language-1.4.0/lib/fez/
+-rw-r--r--   0 simon      (501) staff       (20)     8265 2023-02-03 11:08:13.000000 fez-language-1.4.0/lib/fez/Anchors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1116 2021-06-11 10:24:20.000000 fez-language-1.4.0/lib/fez/Arabic.py
+-rw-r--r--   0 simon      (501) staff       (20)     2911 2021-06-11 10:24:20.000000 fez-language-1.4.0/lib/fez/AvoidCollision.py
+-rw-r--r--   0 simon      (501) staff       (20)    18335 2022-10-13 08:33:23.000000 fez-language-1.4.0/lib/fez/BariYe.py
+-rw-r--r--   0 simon      (501) staff       (20)     2462 2021-10-28 14:11:24.000000 fez-language-1.4.0/lib/fez/Chain.py
+-rw-r--r--   0 simon      (501) staff       (20)    12263 2023-02-03 11:08:13.000000 fez-language-1.4.0/lib/fez/ClassDefinition.py
+-rw-r--r--   0 simon      (501) staff       (20)     1805 2022-06-23 09:06:13.000000 fez-language-1.4.0/lib/fez/Conditional.py
+-rw-r--r--   0 simon      (501) staff       (20)      654 2021-10-11 11:57:25.000000 fez-language-1.4.0/lib/fez/CopyAnchors.py
+-rw-r--r--   0 simon      (501) staff       (20)      981 2021-06-11 10:24:20.000000 fez-language-1.4.0/lib/fez/Debug.py
+-rw-r--r--   0 simon      (501) staff       (20)      782 2021-06-11 10:24:20.000000 fez-language-1.4.0/lib/fez/Delete.py
+-rw-r--r--   0 simon      (501) staff       (20)     2204 2022-10-13 08:33:23.000000 fez-language-1.4.0/lib/fez/Feature.py
+-rw-r--r--   0 simon      (501) staff       (20)     3861 2021-06-17 14:24:16.000000 fez-language-1.4.0/lib/fez/FontEngineering.py
+-rw-r--r--   0 simon      (501) staff       (20)     1051 2021-11-24 12:44:21.000000 fez-language-1.4.0/lib/fez/ForLoop.py
+-rw-r--r--   0 simon      (501) staff       (20)     6221 2023-05-22 09:38:20.000000 fez-language-1.4.0/lib/fez/Fractions.py
+-rw-r--r--   0 simon      (501) staff       (20)     3196 2021-06-17 14:19:46.000000 fez-language-1.4.0/lib/fez/IMatra.py
+-rw-r--r--   0 simon      (501) staff       (20)     3906 2021-06-11 10:24:20.000000 fez-language-1.4.0/lib/fez/IfCollides.py
+-rw-r--r--   0 simon      (501) staff       (20)     1262 2021-11-24 12:35:15.000000 fez-language-1.4.0/lib/fez/Include.py
+-rw-r--r--   0 simon      (501) staff       (20)     2495 2021-06-11 10:24:20.000000 fez-language-1.4.0/lib/fez/KernToDistance.py
+-rw-r--r--   0 simon      (501) staff       (20)     2682 2023-02-03 11:08:13.000000 fez-language-1.4.0/lib/fez/Kerning.py
+-rw-r--r--   0 simon      (501) staff       (20)     1268 2021-06-11 10:24:20.000000 fez-language-1.4.0/lib/fez/LigatureFinder.py
+-rw-r--r--   0 simon      (501) staff       (20)     1541 2021-11-24 12:35:18.000000 fez-language-1.4.0/lib/fez/LoadPlugin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2073 2021-06-17 14:39:56.000000 fez-language-1.4.0/lib/fez/MedialRa.py
+-rw-r--r--   0 simon      (501) staff       (20)     4057 2021-11-24 11:10:55.000000 fez-language-1.4.0/lib/fez/Position.py
+-rw-r--r--   0 simon      (501) staff       (20)     5403 2022-10-13 08:33:23.000000 fez-language-1.4.0/lib/fez/Routine.py
+-rw-r--r--   0 simon      (501) staff       (20)     3849 2021-11-24 11:57:41.000000 fez-language-1.4.0/lib/fez/Substitute.py
+-rw-r--r--   0 simon      (501) staff       (20)     1607 2021-11-24 12:38:01.000000 fez-language-1.4.0/lib/fez/Swap.py
+-rw-r--r--   0 simon      (501) staff       (20)     1783 2022-10-13 08:33:23.000000 fez-language-1.4.0/lib/fez/Variables.py
+-rw-r--r--   0 simon      (501) staff       (20)    22212 2023-02-03 11:08:13.000000 fez-language-1.4.0/lib/fez/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      423 2021-06-11 10:24:20.000000 fez-language-1.4.0/lib/fez/util.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.813835 fez-language-1.4.0/lib/fez_language.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     3188 2023-05-22 09:41:39.000000 fez-language-1.4.0/lib/fez_language.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     2448 2023-05-22 09:41:39.000000 fez-language-1.4.0/lib/fez_language.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-22 09:41:39.000000 fez-language-1.4.0/lib/fez_language.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-22 09:41:39.000000 fez-language-1.4.0/lib/fez_language.egg-info/not-zip-safe
+-rw-r--r--   0 simon      (501) staff       (20)      102 2023-05-22 09:41:39.000000 fez-language-1.4.0/lib/fez_language.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        4 2023-05-22 09:41:39.000000 fez-language-1.4.0/lib/fez_language.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)      102 2021-12-02 09:15:32.000000 fez-language-1.4.0/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-22 09:41:39.825705 fez-language-1.4.0/setup.cfg
+-rw-r--r--   0 simon      (501) staff       (20)     1251 2023-05-22 09:41:24.000000 fez-language-1.4.0/setup.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.815302 fez-language-1.4.0/tests/
+-rw-r--r--   0 simon      (501) staff       (20)      156 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.824520 fez-language-1.4.0/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     1084 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/341421e629668b1a1242245d39238ca48432d35d.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     3300 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     1204 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
+-rw-r--r--   0 simon      (501) staff       (20)    22980 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
+-rw-r--r--   0 simon      (501) staff       (20)   554616 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/Amiri-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)   496504 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/LibertinusSans-Regular.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/Noto Sans Sharada GSUB.txt
+-rw-r--r--   0 simon      (501) staff       (20)   515100 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/Roboto-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     5555 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/SimpleTwoAxis.glyphs
+-rw-r--r--   0 simon      (501) staff       (20)     2720 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/a014549f766436cf55b2ceb40e462038938ee899.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     1840 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/acbe26ce904463c690fb67f70679447059d13ee4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6332 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
+-rw-r--r--   0 simon      (501) staff       (20)    41830 2021-06-11 10:24:20.000000 fez-language-1.4.0/tests/data/notdef.ttx
+-rw-r--r--   0 simon      (501) staff       (20)      982 2021-06-11 10:24:31.000000 fez-language-1.4.0/tests/test_classdefs.py
+-rw-r--r--   0 simon      (501) staff       (20)     1288 2021-11-24 12:38:23.000000 fez-language-1.4.0/tests/test_fez.py
+-rw-r--r--   0 simon      (501) staff       (20)     1326 2023-02-03 11:08:13.000000 fez-language-1.4.0/tests/test_fez_anchors.py
+-rw-r--r--   0 simon      (501) staff       (20)     7361 2023-02-03 11:08:13.000000 fez-language-1.4.0/tests/test_fez_parser.py
+-rw-r--r--   0 simon      (501) staff       (20)     1133 2021-10-19 12:52:22.000000 fez-language-1.4.0/tests/test_languages.py
+-rw-r--r--   0 simon      (501) staff       (20)     1395 2021-11-24 12:06:44.000000 fez-language-1.4.0/tests/test_variable.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-22 09:41:39.825250 fez-language-1.4.0/vim/
+-rw-r--r--   0 simon      (501) staff       (20)     1728 2021-06-11 10:24:20.000000 fez-language-1.4.0/vim/fee.vim
+-rw-r--r--   0 simon      (501) staff       (20)     3307 2021-11-24 13:25:19.000000 fez-language-1.4.0/vim/fez.iro
```

### Comparing `fez-language-1.3.4/CONTRIBUTORS.txt` & `fez-language-1.4.0/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/LICENSE` & `fez-language-1.4.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020, Simon Cozens
+Copyright (c) 2020 Google LLC
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `fez-language-1.3.4/Makefile` & `fez-language-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/PKG-INFO` & `fez-language-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fez-language
-Version: 1.3.4
+Version: 1.4.0
 Summary: The FEZ language: Font Engineering made eaZy
 Home-page: https://github.com/simoncozens/fez
 Author: Simon Cozens
 Author-email: simon@simon-cozens.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -101,9 +100,7 @@
 
 ## Contributors
 
 See the [CONTRIBUTORS.txt](CONTRIBUTORS.txt) file for the full list of contributors. Major contributions are described below:
 
 * FEZ was originally written by Simon Cozens
 * Fred Brennan contributed a new parser and documentation updates
-
-
```

### Comparing `fez-language-1.3.4/README.md` & `fez-language-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/bin/fez2fea` & `fez-language-1.4.0/bin/fez2fea`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/bin/mergefez` & `fez-language-1.4.0/bin/mergefez`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/docs/Makefile` & `fez-language-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/docs/conf.py` & `fez-language-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/docs/fez.png` & `fez-language-1.4.0/docs/fez.png`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/docs/getting-started.rst` & `fez-language-1.4.0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/docs/index.rst` & `fez-language-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/docs/optionalverbs.rst` & `fez-language-1.4.0/docs/optionalverbs.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 As well as being useful *per se* for font engineers, inspecting the source code
 to these plugins is also a good way to learn how to write your own plugins and
 add verbs to the language.
 
 .. automodule:: fez.Arabic
 .. automodule:: fez.BariYe
 .. automodule:: fez.FontEngineering
+.. automodule:: fez.Fractions
 .. automodule:: fez.IMatra
 .. automodule:: fez.KernToDistance
 .. automodule:: fez.LigatureFinder
 .. automodule:: fez.MedialRa
 .. automodule:: fez.Swap
```

### Comparing `fez-language-1.3.4/docs/plugins.rst` & `fez-language-1.4.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/docs/syntax.rst` & `fez-language-1.4.0/docs/syntax.rst`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/fez-samples/qalmi.fez` & `fez-language-1.4.0/fez-samples/qalmi.fez`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/fez-samples/test-fred.fez` & `fez-language-1.4.0/fez-samples/test-fred.fez`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/fez-samples/test.fez` & `fez-language-1.4.0/fez-samples/test.fez`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/fez.png` & `fez-language-1.4.0/fez.png`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/fez.svg` & `fez-language-1.4.0/fez.svg`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Anchors.py` & `fez-language-1.4.0/lib/fez/Anchors.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 
       Feature mark { Attach &top &_top bases; };
 
 The ``Attach`` verb takes three parameters: a base anchor name, a mark anchor
 name, and a class filter, which is either ``marks``, ``bases``, ``cursive``
 or a glyph selector.
 
+It also optionally takes a mark class name:
+
+      Feature mark { Attach &top &_top @topmarks bases; };
+
 The verb acts by collecting all the glyphs which have anchors defined, and
 filtering them according to their class definition in the ``GDEF`` table.
 In this case, we have asked for ``bases``, so glyph ``A`` will be selected.
 Then it looks for anchor definitions containing the mark anchor name
 (here ``_top``), which will select ``acutecomb``, and writes an attachment
 rule to tie them together. As shown in the example, this
 is the most efficient way of expressing a mark-to-base feature.
@@ -72,15 +76,16 @@
 action: glyphselector anchors
 anchors: anchor+
 anchor: BARENAME "<" valuerecord_number valuerecord_number ">"
 """
 
 Attach_GRAMMAR = """
 ?start: action
-action: "&" BARENAME "&" BARENAME (ATTACHTYPE | glyphselector) maybe_languages
+action: "&" BARENAME "&" BARENAME maybe_classname (ATTACHTYPE | glyphselector) maybe_languages
+maybe_classname: classname?
 maybe_languages: languages?
 ATTACHTYPE: "marks" | "bases" | "cursive"
 """
 
 LoadAnchors_GRAMMAR = """
 ?start: action
 action:
@@ -145,15 +150,15 @@
                     self.parser.fontfeatures.anchors[glyphname][a.name] = (x,y)
                 this_anchor = self.parser.fontfeatures.anchors[glyphname][a.name]
                 this_anchor[0].add_value(m.location, a.x)
                 this_anchor[1].add_value(m.location, a.y)
 
 class Attach(FEZVerb):
     def action(self, args):
-        (aFrom, aTo, attachtype, languages) = args
+        (aFrom, aTo, markClass, attachtype, languages) = args
 
         bases = {}
         marks = {}
         catcache = {}
         if isinstance(attachtype, GlyphSelector):
             glyph_filter = attachtype.resolve(self.parser.fontfeatures, self.parser.font)
         else:
@@ -191,20 +196,23 @@
                     k: v
                     for k, v in marks.items()
                     if _category(k) == "mark"
                 }
         return [
             fontFeatures.Routine(
                 rules=[
-                    fontFeatures.Attachment(aFrom, aTo, bases, marks, font=self.parser.font)
+                    fontFeatures.Attachment(aFrom, aTo, markClass, bases, marks, font=self.parser.font)
                 ],
                 languages = languages
             )
         ]
 
+    def maybe_classname(self, args):
+        return args[0] if len(args) else ''
+
     def languages(self, args):
         rv = []
         while args:
             rv.append(tuple(map((lambda x: "%-4s" % x),args[0:2])))
             args = args[2:]
         return rv
```

### Comparing `fez-language-1.3.4/lib/fez/Arabic.py` & `fez-language-1.4.0/lib/fez/Arabic.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/AvoidCollision.py` & `fez-language-1.4.0/lib/fez/AvoidCollision.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/BariYe.py` & `fez-language-1.4.0/lib/fez/BariYe.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Chain.py` & `fez-language-1.4.0/lib/fez/Chain.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/ClassDefinition.py` & `fez-language-1.4.0/lib/fez/ClassDefinition.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,20 +178,20 @@
 primary: primary_action | ("(" primary_action ")")
 conjunction: primary CONJUNCTOR primary
 
 """
 
 DefineClass_GRAMMAR = """
 ?start: action
-action: CLASSNAME "=" primary
+action: classname "=" primary
 """
 
 DefineClassBinned_GRAMMAR = """
 ?start: action
-action: CLASSNAME "[" METRIC "," NUMBER "]" "=" primary
+action: classname "[" METRIC "," NUMBER "]" "=" primary
 """
 
 PARSEOPTS = dict(use_helpers=True)
 VERBS = ["DefineClass", "DefineClassBinned"]
 
 class DefineClass(FEZVerb):
     def _add_glyphs_to_named_class(self, glyphs, classname):
@@ -252,15 +252,14 @@
             return [g for g in l if r(self._get_metrics(g), g)]
 
         return {"conjunction": {"&":"and","|":"or","-":"subtract"}[conjunctor], "left": l, "right": r}
 
     def action(self, args):
         parser = self.parser
         classname, glyphs = args
-        classname = classname[1:] # -@
 
         self._add_glyphs_to_named_class(glyphs, classname)
 
         return args[0]
 
     @classmethod
     def resolve_definition(self, parser, primary):
```

### Comparing `fez-language-1.3.4/lib/fez/Conditional.py` & `fez-language-1.4.0/lib/fez/Conditional.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/CopyAnchors.py` & `fez-language-1.4.0/lib/fez/CopyAnchors.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Debug.py` & `fez-language-1.4.0/lib/fez/Debug.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Delete.py` & `fez-language-1.4.0/lib/fez/Delete.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Feature.py` & `fez-language-1.4.0/lib/fez/Feature.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/FontEngineering.py` & `fez-language-1.4.0/lib/fez/FontEngineering.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/ForLoop.py` & `fez-language-1.4.0/lib/fez/ForLoop.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/IMatra.py` & `fez-language-1.4.0/lib/fez/IMatra.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/IfCollides.py` & `fez-language-1.4.0/lib/fez/IfCollides.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Include.py` & `fez-language-1.4.0/lib/fez/Include.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/KernToDistance.py` & `fez-language-1.4.0/lib/fez/KernToDistance.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Kerning.py` & `fez-language-1.4.0/lib/fez/Kerning.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/LigatureFinder.py` & `fez-language-1.4.0/lib/fez/LigatureFinder.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/LoadPlugin.py` & `fez-language-1.4.0/lib/fez/LoadPlugin.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/MedialRa.py` & `fez-language-1.4.0/lib/fez/MedialRa.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Position.py` & `fez-language-1.4.0/lib/fez/Position.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Routine.py` & `fez-language-1.4.0/lib/fez/Routine.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Substitute.py` & `fez-language-1.4.0/lib/fez/Substitute.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Swap.py` & `fez-language-1.4.0/lib/fez/Swap.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/Variables.py` & `fez-language-1.4.0/lib/fez/Variables.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/lib/fez/__init__.py` & `fez-language-1.4.0/lib/fez/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,27 +247,30 @@
 
     VERB: /[A-Z]/ (LETTER | DIGIT | "_")+
     ARG: (/[^\\s;]+/)
 
     STARTGLYPHNAME: LETTER | DIGIT | "_"
     MIDGLYPHNAME: STARTGLYPHNAME | "." | "-"
     BARENAME: STARTGLYPHNAME MIDGLYPHNAME*
-    inlineclass: "[" (WS* (CLASSNAME | BARENAME | REGEX | UNICODEGLYPH))* "]"
-    CLASSNAME: "@" STARTGLYPHNAME+
+    inlineclass: "[" (WS* (_glyphselector_inner))* "]"
+    CLASSNAME: STARTGLYPHNAME+
+    _CLASS_SIGIL: "@"
+    classname: _CLASS_SIGIL CLASSNAME
 
     ANYTHING: /[^\\s]/
     REGEX: "/" ANYTHING* "/"
 
     HEXDIGIT: /[0-9A-Fa-f]/
     UNICODEGLYPH: "U+" HEXDIGIT~1..6
     unicoderange: UNICODEGLYPH "=>" UNICODEGLYPH
 
     SUFFIXTYPE: ("." | "~")
     glyphsuffix: SUFFIXTYPE STARTGLYPHNAME+
-    glyphselector: (unicoderange | UNICODEGLYPH | REGEX | CLASSNAME | inlineclass | singleglyph) glyphsuffix*
+    _glyphselector_inner: (unicoderange | UNICODEGLYPH | REGEX | classname | inlineclass | singleglyph)
+    glyphselector: _glyphselector_inner glyphsuffix*
     singleglyph: BARENAME | glyph_variable
     glyph_variable: VARIABLE
 
     valuerecord: valuerecord_number | fez_value_record | fea_value_record
     valuerecord_number: variable_scalar | basic_valuerecord_number
     basic_valuerecord_number: integer_container
     fez_value_record: "<" ( FEZ_VALUE_VERB "=" valuerecord_number )+ ">"
@@ -530,14 +533,17 @@
 
     def VARIABLE(self, tok):
         return lark.Token("VARIABLE", tok[1:])
 
     def singleglyph(self, args):
         return args[0]
 
+    def classname(self, args):
+        return args[0]
+
     def integer_constant(self, args):
         return int(args[0])
 
     def constant_glyphvalue(self, args):
         (metric, glyph) = args
         return self._get_metrics(glyph.value, metric.value)
 
@@ -564,24 +570,22 @@
             return args[0]
         return ScalarOrVariable(args[0], self.parser)
 
     def glyph_variable(self, args):
         return ScalarOrVariable(args[0], self.parser)
 
     def unicoderange(self, args):
-        return lark.Token("UNICODERANGE", range(_UNICODEGLYPH(args[0].value), _UNICODEGLYPH(args[1].value)+1), args[0].pos_in_stream)
+        return lark.Token("UNICODERANGE", range(_UNICODEGLYPH(args[0].value), _UNICODEGLYPH(args[1].value)+1))
 
     def inlineclass(self, args):
         return lark.Token("INLINECLASS", [self._glyphselector(t) for t in args if t.type != "WS"])
 
     def _glyphselector(self, token):
         if isinstance(token, ScalarOrVariable):
             return {"variable": token}
-        if token.type == "CLASSNAME":
-            val = token.value[1:]
         elif token.type == "REGEX":
             val = token.value[1:-1]
         elif token.type == "UNICODEGLYPH":
             val = _UNICODEGLYPH(token.value)
         else:
             val = token.value
```

### Comparing `fez-language-1.3.4/lib/fez_language.egg-info/PKG-INFO` & `fez-language-1.4.0/lib/fez_language.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fez-language
-Version: 1.3.4
+Version: 1.4.0
 Summary: The FEZ language: Font Engineering made eaZy
 Home-page: https://github.com/simoncozens/fez
 Author: Simon Cozens
 Author-email: simon@simon-cozens.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -101,9 +100,7 @@
 
 ## Contributors
 
 See the [CONTRIBUTORS.txt](CONTRIBUTORS.txt) file for the full list of contributors. Major contributions are described below:
 
 * FEZ was originally written by Simon Cozens
 * Fred Brennan contributed a new parser and documentation updates
-
-
```

### Comparing `fez-language-1.3.4/lib/fez_language.egg-info/SOURCES.txt` & `fez-language-1.4.0/lib/fez_language.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 lib/fez/Conditional.py
 lib/fez/CopyAnchors.py
 lib/fez/Debug.py
 lib/fez/Delete.py
 lib/fez/Feature.py
 lib/fez/FontEngineering.py
 lib/fez/ForLoop.py
+lib/fez/Fractions.py
 lib/fez/IMatra.py
 lib/fez/IfCollides.py
 lib/fez/Include.py
 lib/fez/KernToDistance.py
 lib/fez/Kerning.py
 lib/fez/LigatureFinder.py
 lib/fez/LoadPlugin.py
```

### Comparing `fez-language-1.3.4/setup.py` & `fez-language-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'author': 'Simon Cozens',
     'author_email': 'simon@simon-cozens.org',
     'url': 'https://github.com/simoncozens/fez',
     'description': 'The FEZ language: Font Engineering made eaZy',
     'long_description': open('README.md', 'r').read(),
     'long_description_content_type': 'text/markdown',
     'license': 'MIT',
-    'version': '1.3.4',
+    'version': '1.4.0',
     'install_requires': install_requires,
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta"
```

### Comparing `fez-language-1.3.4/tests/data/1735326da89f0818cd8c51a0600e9789812c0f94.ttf` & `fez-language-1.4.0/tests/data/1735326da89f0818cd8c51a0600e9789812c0f94.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf` & `fez-language-1.4.0/tests/data/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/341421e629668b1a1242245d39238ca48432d35d.ttf` & `fez-language-1.4.0/tests/data/341421e629668b1a1242245d39238ca48432d35d.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/55c88ebbe938680b08f92c3de20713183e0c7481.ttf` & `fez-language-1.4.0/tests/data/55c88ebbe938680b08f92c3de20713183e0c7481.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf` & `fez-language-1.4.0/tests/data/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf` & `fez-language-1.4.0/tests/data/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/Amiri-Regular.ttf` & `fez-language-1.4.0/tests/data/Amiri-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/LibertinusSans-Regular.otf` & `fez-language-1.4.0/tests/data/LibertinusSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/Noto Sans Sharada GSUB.txt` & `fez-language-1.4.0/tests/data/Noto Sans Sharada GSUB.txt`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/Roboto-Regular.ttf` & `fez-language-1.4.0/tests/data/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/SimpleTwoAxis.glyphs` & `fez-language-1.4.0/tests/data/SimpleTwoAxis.glyphs`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/a014549f766436cf55b2ceb40e462038938ee899.ttf` & `fez-language-1.4.0/tests/data/a014549f766436cf55b2ceb40e462038938ee899.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/acbe26ce904463c690fb67f70679447059d13ee4.otf` & `fez-language-1.4.0/tests/data/acbe26ce904463c690fb67f70679447059d13ee4.otf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/df768b9c257e0c9c35786c47cae15c46571d56be.ttf` & `fez-language-1.4.0/tests/data/df768b9c257e0c9c35786c47cae15c46571d56be.ttf`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/data/notdef.ttx` & `fez-language-1.4.0/tests/data/notdef.ttx`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/test_classdefs.py` & `fez-language-1.4.0/tests/test_classdefs.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/test_fez.py` & `fez-language-1.4.0/tests/test_fez.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/test_fez_anchors.py` & `fez-language-1.4.0/tests/test_fez_anchors.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       Anchors B
         top <611 1612>
       ;
 
       Anchors acutecomb _top <-570 1290>;
       Anchors tildecomb _top <-542 1256>;
 
-      Feature mark { Attach &top &_top bases; };
+      Feature mark { Attach &top &_top @top bases; };
 """
         )
 
         self.assertEqual(p.fontfeatures.anchors["A"]["top"], (679, 1600))
         self.assertSufficientlyEqual(
             p.fontfeatures.asFea(),
             """    markClass acutecomb <anchor -570 1290> @top;
```

### Comparing `fez-language-1.3.4/tests/test_fez_parser.py` & `fez-language-1.4.0/tests/test_fez_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,34 +55,34 @@
 #############
 # ClassName #
 #############
 
 class ClassNameModule:
     GRAMMAR = """
     ?start: action
-    action: CLASSNAME
+    action: classname
     """
 
     VERBS = ["ClassName"]
 
     PARSEOPTS = dict(use_helpers=True)
 
     class ClassName(FEZVerb):
         def action(self, args):
             return args
 
 def test_classname(parser):
     parser.register_plugin(ClassNameModule, "ClassName")
 
     def test_classname_string(test_bn):
-        s = "ClassName %s;" % test_bn
+        s = "ClassName @%s;" % test_bn
         a = parser.parseString(s)
         assert a == [Token('CLASSNAME', test_bn)]
 
-    test_classname_string("@foo")
+    test_classname_string("foo")
 
 ###############
 # InlineClass #
 ###############
 
 class InlineClassModule:
     GRAMMAR = """
@@ -255,7 +255,15 @@
 def test_for_loop(parser):
     s = "Feature rlig { For $g in /^[a-z]$/ { If width[$g] >= width[w] { Substitute $g -> $g.sc; }; }; };"
     parser.parseString(s)
     assert alltrim(parser.fontfeatures.asFea()) == alltrim(
         "lookup Routine_1 { ; sub m by m.sc; sub w by w.sc; } Routine_1; feature rlig { lookup Routine_1; } rlig;"
     )
 
+# issue 14
+
+def test_issue14(parser):
+    s = "DefineClass @consonants = [U+20=>U+21 U+30=>U+31];"
+    parser.parseString(s)
+    assert alltrim(parser.fontfeatures.asFea()) == alltrim(
+        "@consonants = [space exclam zero one];"
+    )
```

### Comparing `fez-language-1.3.4/tests/test_languages.py` & `fez-language-1.4.0/tests/test_languages.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/tests/test_variable.py` & `fez-language-1.4.0/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/vim/fee.vim` & `fez-language-1.4.0/vim/fee.vim`

 * *Files identical despite different names*

### Comparing `fez-language-1.3.4/vim/fez.iro` & `fez-language-1.4.0/vim/fez.iro`

 * *Files identical despite different names*

