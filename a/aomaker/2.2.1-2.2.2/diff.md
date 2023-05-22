# Comparing `tmp/aomaker-2.2.1.tar.gz` & `tmp/aomaker-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aomaker-2.2.1.tar", last modified: Wed Apr 12 10:31:21 2023, max compression
+gzip compressed data, was "aomaker-2.2.2.tar", last modified: Mon May 22 08:31:47 2023, max compression
```

## Comparing `aomaker-2.2.1.tar` & `aomaker-2.2.2.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.934692 aomaker-2.2.1/
--rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.2.1/LICENSE
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       37 2022-11-30 11:05:04.000000 aomaker-2.2.1/MANIFEST.in
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-04-12 10:31:21.934559 aomaker-2.2.1/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.2.1/README.md
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.929968 aomaker-2.2.1/aomaker/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-04-12 10:31:01.000000 aomaker-2.2.1/aomaker/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9285 2023-04-12 10:30:39.000000 aomaker-2.2.1/aomaker/_aomaker.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.2.1/aomaker/_constants.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/_log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.2.1/aomaker/aomaker.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.931193 aomaker-2.2.1/aomaker/base/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/base/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.2.1/aomaker/base/base_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/base/base_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     6167 2023-04-10 07:53:59.000000 aomaker-2.2.1/aomaker/cache.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9697 2023-03-23 05:48:22.000000 aomaker-2.2.1/aomaker/cli.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.931890 aomaker-2.2.1/aomaker/database/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/database/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.2.1/aomaker/database/base_db.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/database/mysql.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/database/sqlite.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1394 2022-12-05 05:36:42.000000 aomaker-2.2.1/aomaker/exceptions.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.932012 aomaker-2.2.1/aomaker/extension/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/extension/__init__.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.932297 aomaker-2.2.1/aomaker/extension/har_parse/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.2.1/aomaker/extension/har_parse/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/extension/har_parse/har_parse.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.932812 aomaker-2.2.1/aomaker/extension/recording/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.2.1/aomaker/extension/recording/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/extension/recording/addons.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/extension/recording/recording.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/field.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3000 2023-03-23 05:16:42.000000 aomaker-2.2.1/aomaker/fixture.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.2.1/aomaker/hook_manager.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.933369 aomaker-2.2.1/aomaker/html/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.2.1/aomaker/html/heading.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.2.1/aomaker/html/report.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2022-12-22 09:57:22.000000 aomaker-2.2.1/aomaker/html/template.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.2.1/aomaker/log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/make.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/make_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/make_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2118 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/models.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      450 2023-03-16 15:19:31.000000 aomaker-2.2.1/aomaker/param_types.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      691 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/path.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3002 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8814 2023-04-10 03:38:53.000000 aomaker-2.2.1/aomaker/runner.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8576 2023-04-10 14:08:17.000000 aomaker-2.2.1/aomaker/scaffold.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.933719 aomaker-2.2.1/aomaker/send_msg/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/send_msg/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/send_msg/wechat.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/swagger2yaml.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/template.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.934183 aomaker-2.2.1/aomaker/utils/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/utils/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9343 2023-02-01 03:18:54.000000 aomaker-2.2.1/aomaker/utils/gen_allure_report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.2.1/aomaker/utils/utils.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/yaml2case.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.930641 aomaker-2.2.1/aomaker.egg-info/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1329 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/SOURCES.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/dependency_links.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/entry_points.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/requires.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/top_level.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-04-12 10:31:21.934736 aomaker-2.2.1/setup.cfg
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-04-12 10:31:01.000000 aomaker-2.2.1/setup.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.763894 aomaker-2.2.2/
+-rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.2.2/LICENSE
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       43 2023-05-20 11:36:28.000000 aomaker-2.2.2/MANIFEST.in
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-05-22 08:31:47.763769 aomaker-2.2.2/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.2.2/README.md
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.758753 aomaker-2.2.2/aomaker/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-05-20 11:24:05.000000 aomaker-2.2.2/aomaker/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9285 2023-04-12 10:30:39.000000 aomaker-2.2.2/aomaker/_aomaker.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.2.2/aomaker/_constants.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/_log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1245 2023-05-20 14:38:18.000000 aomaker-2.2.2/aomaker/_printer.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.2.2/aomaker/aomaker.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.760035 aomaker-2.2.2/aomaker/base/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/base/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.2.2/aomaker/base/base_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/base/base_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6167 2023-04-10 07:53:59.000000 aomaker-2.2.2/aomaker/cache.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9697 2023-03-23 05:48:22.000000 aomaker-2.2.2/aomaker/cli.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.760939 aomaker-2.2.2/aomaker/database/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/database/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.2.2/aomaker/database/base_db.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/database/mysql.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/database/sqlite.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1394 2022-12-05 05:36:42.000000 aomaker-2.2.2/aomaker/exceptions.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.761179 aomaker-2.2.2/aomaker/extension/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/extension/__init__.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.761632 aomaker-2.2.2/aomaker/extension/har_parse/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.2.2/aomaker/extension/har_parse/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/extension/har_parse/har_parse.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.762146 aomaker-2.2.2/aomaker/extension/recording/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.2.2/aomaker/extension/recording/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/extension/recording/addons.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/extension/recording/recording.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/field.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2813 2023-05-20 14:38:18.000000 aomaker-2.2.2/aomaker/fixture.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.2.2/aomaker/hook_manager.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.762751 aomaker-2.2.2/aomaker/html/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.2.2/aomaker/html/heading.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.2.2/aomaker/html/report.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2023-05-20 11:43:25.000000 aomaker-2.2.2/aomaker/html/template.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.2.2/aomaker/log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/make.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/make_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/make_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2118 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/models.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      450 2023-03-16 15:19:31.000000 aomaker-2.2.2/aomaker/param_types.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      691 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/path.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2890 2023-05-20 14:38:18.000000 aomaker-2.2.2/aomaker/report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8531 2023-05-22 07:24:31.000000 aomaker-2.2.2/aomaker/runner.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8576 2023-04-10 14:08:17.000000 aomaker-2.2.2/aomaker/scaffold.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.763143 aomaker-2.2.2/aomaker/send_msg/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/send_msg/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/send_msg/wechat.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/swagger2yaml.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/template.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.763477 aomaker-2.2.2/aomaker/utils/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/utils/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9385 2023-05-22 08:31:42.000000 aomaker-2.2.2/aomaker/utils/gen_allure_report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.2.2/aomaker/utils/utils.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/yaml2case.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.759503 aomaker-2.2.2/aomaker.egg-info/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1349 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/entry_points.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/requires.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/top_level.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-05-22 08:31:47.763935 aomaker-2.2.2/setup.cfg
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-05-20 11:27:03.000000 aomaker-2.2.2/setup.py
```

### Comparing `aomaker-2.2.1/LICENSE` & `aomaker-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/PKG-INFO` & `aomaker-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.2.1
+Version: 2.2.2
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.2.1/README.md` & `aomaker-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/__init__.py` & `aomaker-2.2.2/aomaker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from emoji import emojize
 
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 __description__ = "Quickly Arrange,Quickly Test!"
 __image__ = emojize(fr"""
               :----.                                                             ::::
              .------            .:::::::::::::::::::::::::::::::::::::::::::::. :---:  ::::::::::::::::::::::::::
             .---::--:                                                           ----
             ----  :--:          ..::::.      :.:..::::  .::::     ..:::. .:::  :---: ...:.    .::::.     .:.:..::
            :---    :::        .---------:   :-----------------   :----------:  ----.:---:   :---::---:   -------:
```

### Comparing `aomaker-2.2.1/aomaker/_aomaker.py` & `aomaker-2.2.2/aomaker/_aomaker.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/_constants.py` & `aomaker-2.2.2/aomaker/_constants.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/_log.py` & `aomaker-2.2.2/aomaker/_log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/base/base_api.py` & `aomaker-2.2.2/aomaker/base/base_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/base/base_testcase.py` & `aomaker-2.2.2/aomaker/base/base_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/cache.py` & `aomaker-2.2.2/aomaker/cache.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/cli.py` & `aomaker-2.2.2/aomaker/cli.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/database/base_db.py` & `aomaker-2.2.2/aomaker/database/base_db.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/database/mysql.py` & `aomaker-2.2.2/aomaker/database/mysql.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/database/sqlite.py` & `aomaker-2.2.2/aomaker/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/exceptions.py` & `aomaker-2.2.2/aomaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/extension/har_parse/__init__.py` & `aomaker-2.2.2/aomaker/extension/har_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/extension/har_parse/har_parse.py` & `aomaker-2.2.2/aomaker/extension/har_parse/har_parse.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/extension/recording/__init__.py` & `aomaker-2.2.2/aomaker/extension/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/extension/recording/recording.py` & `aomaker-2.2.2/aomaker/extension/recording/recording.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/field.py` & `aomaker-2.2.2/aomaker/field.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/fixture.py` & `aomaker-2.2.2/aomaker/fixture.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # --coding:utf-8--
 import os
 from abc import ABCMeta, abstractmethod
 
 import yaml
 
+from aomaker._printer import printer
 from aomaker.path import CONF_DIR
 from aomaker.cache import cache, config
-from aomaker.log import logger
 from aomaker.exceptions import FileNotFound, ConfKeyError
 from aomaker._constants import Conf
 
 
 class ReadConfig:
     def __init__(self, conf_name=Conf.CONF_NAME):
         self.conf_path = os.path.join(CONF_DIR, conf_name)
@@ -82,20 +82,19 @@
         if self.login_obj:
             resp = self.login_obj.login()
             headers = self.login_obj.make_headers(resp)
         cache.set('headers', headers)
 
 
 class TearDownSession:
+    @printer("clean_env")
     def clear_env(self):
-        logger.info('******************************测试结束，开始清理环境******************************')
         cache.clear()
         cache.close()
         config.close()
-        logger.info('******************************清理环境完成******************************')
 
 
 if __name__ == '__main__':
     # print(ReadConfig().conf)
     print(EnvVars().current_env)
     print(EnvVars().current_env_conf)
     # save_env_vars_to_db()
```

### Comparing `aomaker-2.2.1/aomaker/hook_manager.py` & `aomaker-2.2.2/aomaker/hook_manager.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/html/heading.html` & `aomaker-2.2.2/aomaker/html/heading.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/html/report.html` & `aomaker-2.2.2/aomaker/html/report.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/html/template.html` & `aomaker-2.2.2/aomaker/html/template.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/log.py` & `aomaker-2.2.2/aomaker/log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/make.py` & `aomaker-2.2.2/aomaker/make.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/make_api.py` & `aomaker-2.2.2/aomaker/make_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/make_testcase.py` & `aomaker-2.2.2/aomaker/make_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/models.py` & `aomaker-2.2.2/aomaker/models.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/path.py` & `aomaker-2.2.2/aomaker/path.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/report.py` & `aomaker-2.2.2/aomaker/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # --coding:utf-8--
 import os
 
 from jinja2 import Template
 
 from aomaker.utils.gen_allure_report import CaseSummary, CaseDetail
 from aomaker.path import AOMAKER_HTML
+from aomaker._printer import printer
 
 base_dir = os.path.dirname(__file__)
 base_html_path = os.path.join(base_dir, "html")
 
 
 class HtmlMaker:
     def __init__(self, report_target_path=AOMAKER_HTML):
@@ -50,16 +51,16 @@
         # 2.全部内容渲染到目标报告：aoreporter.html
         with open(self.report_target_path, "w", encoding='utf-8') as f:
             temp = Template(template_str)
             temp_str = temp.render(html_rendered_dict)
             f.write(temp_str)
 
 
+@printer("gen_rep")
 def gen_reports():
-    print("-----------测试结束, AoMaker开始收集报告-----------")
     case_summary = CaseSummary()
     case_detail = CaseDetail()
     summary = {
         "total": case_summary.total_count,
         "passed_count": case_summary.passed_count,
         "failed_count": case_summary.failed_count,
         "error_count": case_summary.broken_count,
@@ -71,8 +72,7 @@
         "duration": case_summary.duration,
         "start_time": case_summary.start_time,
         "end_time": case_summary.stop_time,
         "case_list": case_detail.case_detail_info()
     }
     html_maker = HtmlMaker()
     html_maker.render_template_html(summary)
-    print(f"-----------AoMaker已完成测试报告!报告路径：{AOMAKER_HTML}-----------")
```

### Comparing `aomaker-2.2.1/aomaker/runner.py` & `aomaker-2.2.2/aomaker/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 import shutil
 from multiprocessing import Pool
 from functools import singledispatchmethod
 from concurrent.futures import ThreadPoolExecutor, wait, ALL_COMPLETED
 
 import pytest
-from emoji import emojize
 
+from aomaker._printer import printer
 from aomaker.cache import config
 from aomaker.fixture import SetUpSession, TearDownSession, BaseLogin
 from aomaker.log import logger, aomaker_logger
 from aomaker._constants import Allure
 from aomaker.exceptions import LoginError
 from aomaker.path import REPORT_DIR, PYTEST_INI_DIR
 from aomaker.report import gen_reports
@@ -23,37 +23,36 @@
     "ProcessesRunner": "mp",
     "ThreadsRunner": "mt"
 }
 
 
 def fixture_session(func):
     """全局夹具装饰器"""
-
     def wrapper(*args, **kwargs):
         # Login登录类对象
         login = kwargs.get('login')
-        # 前置
-        logger.info(emojize(
-            '******************************:puzzle_piece: 开始初始化环境 :puzzle_piece:******************************'))
-        method_of_class_name = func.__qualname__.split('.')[0]
-        config.set("run_mode", RUN_MODE[method_of_class_name])
-        SetUpSession(login).set_session_vars()
-        shutil.rmtree(allure_json_dir, ignore_errors=True)
-        if _cli_hook.custom_kwargs:
-            _cli_hook.run()
-        _session_hook.run()
-        logger.info(emojize(
-            '*****************:beer_mug: 环境初始化完成，所有全局配置已加载到config表 :beer_mug:*****************'))
+        _init(func, login)
         r = func(*args, **kwargs)
         TearDownSession().clear_env()
         return r
 
     return wrapper
 
 
+@printer("init_env")
+def _init(func, login):
+    method_of_class_name = func.__qualname__.split('.')[0]
+    config.set("run_mode", RUN_MODE[method_of_class_name])
+    SetUpSession(login).set_session_vars()
+    shutil.rmtree(allure_json_dir, ignore_errors=True)
+    if _cli_hook.custom_kwargs:
+        _cli_hook.run()
+    _session_hook.run()
+
+
 class Runner:
     def __init__(self, is_processes=False):
         self.pytest_args = ["-s",
                             f"--alluredir={allure_json_dir}",
                             "--show-capture=no",  # 控制台不显示pytest的捕获日志
                             "--log-format=%(asctime)s %(message)s",
                             "--log-date-format=%Y-%m-%d %H:%M:%S"
```

### Comparing `aomaker-2.2.1/aomaker/scaffold.py` & `aomaker-2.2.2/aomaker/scaffold.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/send_msg/wechat.py` & `aomaker-2.2.2/aomaker/send_msg/wechat.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/swagger2yaml.py` & `aomaker-2.2.2/aomaker/swagger2yaml.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/template.py` & `aomaker-2.2.2/aomaker/template.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/utils/gen_allure_report.py` & `aomaker-2.2.2/aomaker/utils/gen_allure_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # --coding:utf-8--
+import configparser
 import json
 import os
 import time
 from typing import List, Dict
 
-from aomaker.path import REPORT_DIR, BASEDIR
+from aomaker.path import REPORT_DIR, PYTEST_INI_DIR
+from aomaker.utils.utils import HandleIni
 
 ALLURE_HTML_PATH = os.path.join(REPORT_DIR, "html")
 ALLURE_JSON_PATH = os.path.join(REPORT_DIR, "json")
 WIDGETS_PATH = os.path.join(ALLURE_HTML_PATH, "widgets")
 SUMMARY_JSON_PATH = os.path.join(WIDGETS_PATH, "summary.json")
-PYTEST_MARKS = ["dependency", "skip", "skipif", "xfail", "usefixtures", "filterwarnings", "flaky"]
 
 
 def gen_allure_summary() -> dict:
     """ 收集allure总览信息 """
     with open(SUMMARY_JSON_PATH, 'r', encoding='utf-8') as fp:
         allure_summary = json.load(fp)
     return allure_summary
@@ -24,48 +25,48 @@
     """解析allure json"""
     # 1.find all result.json file
     results = {}
     result_jsons = parse_allure_res_json()
     n = 0
     all_results_json = []
     status_list = []
+    marks_group = _get_marks_group_from_pytest_ini()
     for result_json in result_jsons:
         with open(result_json, encoding="utf-8") as load_f:
             load_dict = json.load(load_f)
             keys = load_dict.keys()
             # 判断是否有labels
             if "labels" in keys and "status" in keys:
                 result = {
                     "name": load_dict["name"],
                     "full_name": load_dict["fullName"],
                     "labels": load_dict["labels"],
-                    "case_id": load_dict['testCaseId']
+                    "case_id": load_dict['testCaseId'],
+                    "parameters": load_dict.get("parameters")
                 }
                 status = load_dict["status"]
                 start_time = load_dict["start"]
                 status_dict = {"name": load_dict["name"], "status": status, "full_name": load_dict["fullName"],
                                "start_time": start_time}
                 if result in all_results_json:
-
+                    # 处理重试机制
                     index = all_results_json.index(result)
                     elem = status_list[index]
                     # 处理重试机制时，状态变更的情况，用最后一次状态
                     if start_time > elem["start_time"]:
                         elem["status"] = status
                 else:
-                    # 处理重试机制
                     all_results_json.append(result)
                     status_list.append(status_dict)
     for load_dict, status_dict in zip(all_results_json, status_list):
         status = status_dict["status"]
         tags = [label.get("value") for label in _handle_labels(load_dict['labels'])]
-        product_name = _handle_tags(tags, sep=sep)
-        if results.get(product_name) is None:
-            results[product_name] = {"passed": 0, "failed": 0, "skipped": 0, "broken": 0}
-        results[product_name][status] += 1
+        product_name = _handle_tags(tags, marks_group, sep=sep)
+        if product_name is not None:
+            results[product_name][status] += 1
     results = _count_passed_rate(results)
     return results
 
 
 def parse_allure_res_json():
     res = []
     for root, directory, files in os.walk(ALLURE_JSON_PATH):
@@ -73,38 +74,35 @@
             name, suf = os.path.splitext(filename)
             if suf == ".json":
                 res.append(os.path.join(root, filename))
     result_jsons = [data for data in res if "result.json" in data]
     return result_jsons
 
 
+def _get_marks_group_from_pytest_ini() -> str:
+    pytest_config_parser = HandleIni(PYTEST_INI_DIR)
+    try:
+        marks_group = pytest_config_parser.get("pytest", "marks_group")
+    except (configparser.NoSectionError, configparser.NoOptionError):
+        marks_group = ""
+    return marks_group
+
+
 def _handle_labels(labels: list):
     for label in labels:
         if label.get('name') == "tag":
             yield label
 
 
-def _handle_tags(tags: list, sep=None):
+def _handle_tags(tags: list, marks_group, sep=None):
     """将标记按照指定分隔符分割,默认按空格"""
     for tag in tags:
-        if sep is None:
-            split_tag = tag.split()
-            return split_tag
-        if __check_pytest_marks(tag) is False:
-            continue
-        split_tag = tag.split(sep)
-        if len(split_tag) > 0:
-            return split_tag[0]
-
-
-def __check_pytest_marks(tag: str):
-    for m in PYTEST_MARKS:
-        if m in tag:
-            return False
-    return True
+        prefix_tag = tag.split(sep)[0]
+        if prefix_tag in marks_group:
+            return prefix_tag
 
 
 def _count_passed_rate(results: dict) -> dict:
     new_results = results
     for product, result in results.items():
         passed_count = result["passed"]
         failed_count = result["failed"]
```

### Comparing `aomaker-2.2.1/aomaker/utils/utils.py` & `aomaker-2.2.2/aomaker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker/yaml2case.py` & `aomaker-2.2.2/aomaker/yaml2case.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.1/aomaker.egg-info/PKG-INFO` & `aomaker-2.2.2/aomaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.2.1
+Version: 2.2.2
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.2.1/aomaker.egg-info/SOURCES.txt` & `aomaker-2.2.2/aomaker.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.py
 aomaker/__init__.py
 aomaker/_aomaker.py
 aomaker/_constants.py
 aomaker/_log.py
+aomaker/_printer.py
 aomaker/aomaker.py
 aomaker/cache.py
 aomaker/cli.py
 aomaker/exceptions.py
 aomaker/field.py
 aomaker/fixture.py
 aomaker/hook_manager.py
```

### Comparing `aomaker-2.2.1/setup.py` & `aomaker-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # --coding:utf-8--
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="aomaker",
-    version="2.2.1",
+    version="2.2.2",
     author="ancientone",
     author_email="listeningsss@163.com",
     description="An api testing framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ae86sen/aomaker",
     packages=setuptools.find_packages(),
```

