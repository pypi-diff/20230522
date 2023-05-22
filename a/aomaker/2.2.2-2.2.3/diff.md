# Comparing `tmp/aomaker-2.2.2.tar.gz` & `tmp/aomaker-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aomaker-2.2.2.tar", last modified: Mon May 22 08:31:47 2023, max compression
+gzip compressed data, was "aomaker-2.2.3.tar", last modified: Mon May 22 08:33:31 2023, max compression
```

## Comparing `aomaker-2.2.2.tar` & `aomaker-2.2.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.763894 aomaker-2.2.2/
--rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.2.2/LICENSE
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       43 2023-05-20 11:36:28.000000 aomaker-2.2.2/MANIFEST.in
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-05-22 08:31:47.763769 aomaker-2.2.2/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.2.2/README.md
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.758753 aomaker-2.2.2/aomaker/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-05-20 11:24:05.000000 aomaker-2.2.2/aomaker/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9285 2023-04-12 10:30:39.000000 aomaker-2.2.2/aomaker/_aomaker.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.2.2/aomaker/_constants.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/_log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1245 2023-05-20 14:38:18.000000 aomaker-2.2.2/aomaker/_printer.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.2.2/aomaker/aomaker.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.760035 aomaker-2.2.2/aomaker/base/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/base/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.2.2/aomaker/base/base_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/base/base_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     6167 2023-04-10 07:53:59.000000 aomaker-2.2.2/aomaker/cache.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9697 2023-03-23 05:48:22.000000 aomaker-2.2.2/aomaker/cli.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.760939 aomaker-2.2.2/aomaker/database/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/database/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.2.2/aomaker/database/base_db.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/database/mysql.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/database/sqlite.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1394 2022-12-05 05:36:42.000000 aomaker-2.2.2/aomaker/exceptions.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.761179 aomaker-2.2.2/aomaker/extension/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/extension/__init__.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.761632 aomaker-2.2.2/aomaker/extension/har_parse/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.2.2/aomaker/extension/har_parse/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/extension/har_parse/har_parse.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.762146 aomaker-2.2.2/aomaker/extension/recording/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.2.2/aomaker/extension/recording/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/extension/recording/addons.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/extension/recording/recording.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/field.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2813 2023-05-20 14:38:18.000000 aomaker-2.2.2/aomaker/fixture.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.2.2/aomaker/hook_manager.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.762751 aomaker-2.2.2/aomaker/html/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.2.2/aomaker/html/heading.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.2.2/aomaker/html/report.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2023-05-20 11:43:25.000000 aomaker-2.2.2/aomaker/html/template.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.2.2/aomaker/log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/make.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/make_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/make_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2118 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/models.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      450 2023-03-16 15:19:31.000000 aomaker-2.2.2/aomaker/param_types.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      691 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/path.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2890 2023-05-20 14:38:18.000000 aomaker-2.2.2/aomaker/report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8531 2023-05-22 07:24:31.000000 aomaker-2.2.2/aomaker/runner.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8576 2023-04-10 14:08:17.000000 aomaker-2.2.2/aomaker/scaffold.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.763143 aomaker-2.2.2/aomaker/send_msg/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/send_msg/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/send_msg/wechat.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/swagger2yaml.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/template.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.763477 aomaker-2.2.2/aomaker/utils/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/utils/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9385 2023-05-22 08:31:42.000000 aomaker-2.2.2/aomaker/utils/gen_allure_report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.2.2/aomaker/utils/utils.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.2.2/aomaker/yaml2case.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:31:47.759503 aomaker-2.2.2/aomaker.egg-info/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1349 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/SOURCES.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/dependency_links.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/entry_points.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/requires.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-05-22 08:31:47.000000 aomaker-2.2.2/aomaker.egg-info/top_level.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-05-22 08:31:47.763935 aomaker-2.2.2/setup.cfg
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-05-20 11:27:03.000000 aomaker-2.2.2/setup.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.350748 aomaker-2.2.3/
+-rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.2.3/LICENSE
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       43 2023-05-20 11:36:28.000000 aomaker-2.2.3/MANIFEST.in
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-05-22 08:33:31.350611 aomaker-2.2.3/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.2.3/README.md
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.346271 aomaker-2.2.3/aomaker/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-05-22 08:33:28.000000 aomaker-2.2.3/aomaker/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9285 2023-04-12 10:30:39.000000 aomaker-2.2.3/aomaker/_aomaker.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.2.3/aomaker/_constants.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/_log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1245 2023-05-20 14:38:18.000000 aomaker-2.2.3/aomaker/_printer.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.2.3/aomaker/aomaker.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.347385 aomaker-2.2.3/aomaker/base/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/base/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.2.3/aomaker/base/base_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/base/base_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6167 2023-04-10 07:53:59.000000 aomaker-2.2.3/aomaker/cache.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9697 2023-03-23 05:48:22.000000 aomaker-2.2.3/aomaker/cli.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.348086 aomaker-2.2.3/aomaker/database/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/database/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.2.3/aomaker/database/base_db.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/database/mysql.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/database/sqlite.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1394 2022-12-05 05:36:42.000000 aomaker-2.2.3/aomaker/exceptions.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.348195 aomaker-2.2.3/aomaker/extension/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/extension/__init__.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.348467 aomaker-2.2.3/aomaker/extension/har_parse/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.2.3/aomaker/extension/har_parse/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/extension/har_parse/har_parse.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.348914 aomaker-2.2.3/aomaker/extension/recording/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.2.3/aomaker/extension/recording/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/extension/recording/addons.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/extension/recording/recording.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/field.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2813 2023-05-20 14:38:18.000000 aomaker-2.2.3/aomaker/fixture.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.2.3/aomaker/hook_manager.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.349487 aomaker-2.2.3/aomaker/html/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.2.3/aomaker/html/heading.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.2.3/aomaker/html/report.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2023-05-20 11:43:25.000000 aomaker-2.2.3/aomaker/html/template.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.2.3/aomaker/log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/make.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/make_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/make_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2118 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/models.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      450 2023-03-16 15:19:31.000000 aomaker-2.2.3/aomaker/param_types.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      691 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/path.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2890 2023-05-20 14:38:18.000000 aomaker-2.2.3/aomaker/report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8531 2023-05-22 07:24:31.000000 aomaker-2.2.3/aomaker/runner.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8576 2023-04-10 14:08:17.000000 aomaker-2.2.3/aomaker/scaffold.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.349832 aomaker-2.2.3/aomaker/send_msg/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/send_msg/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/send_msg/wechat.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/swagger2yaml.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/template.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.350260 aomaker-2.2.3/aomaker/utils/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/utils/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9529 2023-05-22 08:33:10.000000 aomaker-2.2.3/aomaker/utils/gen_allure_report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.2.3/aomaker/utils/utils.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.2.3/aomaker/yaml2case.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-05-22 08:33:31.346924 aomaker-2.2.3/aomaker.egg-info/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-05-22 08:33:31.000000 aomaker-2.2.3/aomaker.egg-info/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1349 2023-05-22 08:33:31.000000 aomaker-2.2.3/aomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-05-22 08:33:31.000000 aomaker-2.2.3/aomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-05-22 08:33:31.000000 aomaker-2.2.3/aomaker.egg-info/entry_points.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-05-22 08:33:31.000000 aomaker-2.2.3/aomaker.egg-info/requires.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-05-22 08:33:31.000000 aomaker-2.2.3/aomaker.egg-info/top_level.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-05-22 08:33:31.350800 aomaker-2.2.3/setup.cfg
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-05-22 08:33:28.000000 aomaker-2.2.3/setup.py
```

### Comparing `aomaker-2.2.2/LICENSE` & `aomaker-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/PKG-INFO` & `aomaker-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.2.2
+Version: 2.2.3
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.2.2/README.md` & `aomaker-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/__init__.py` & `aomaker-2.2.3/aomaker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from emoji import emojize
 
-__version__ = "2.2.2"
+__version__ = "2.2.3"
 __description__ = "Quickly Arrange,Quickly Test!"
 __image__ = emojize(fr"""
               :----.                                                             ::::
              .------            .:::::::::::::::::::::::::::::::::::::::::::::. :---:  ::::::::::::::::::::::::::
             .---::--:                                                           ----
             ----  :--:          ..::::.      :.:..::::  .::::     ..:::. .:::  :---: ...:.    .::::.     .:.:..::
            :---    :::        .---------:   :-----------------   :----------:  ----.:---:   :---::---:   -------:
```

### Comparing `aomaker-2.2.2/aomaker/_aomaker.py` & `aomaker-2.2.3/aomaker/_aomaker.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/_constants.py` & `aomaker-2.2.3/aomaker/_constants.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/_log.py` & `aomaker-2.2.3/aomaker/_log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/_printer.py` & `aomaker-2.2.3/aomaker/_printer.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/base/base_api.py` & `aomaker-2.2.3/aomaker/base/base_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/base/base_testcase.py` & `aomaker-2.2.3/aomaker/base/base_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/cache.py` & `aomaker-2.2.3/aomaker/cache.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/cli.py` & `aomaker-2.2.3/aomaker/cli.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/database/base_db.py` & `aomaker-2.2.3/aomaker/database/base_db.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/database/mysql.py` & `aomaker-2.2.3/aomaker/database/mysql.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/database/sqlite.py` & `aomaker-2.2.3/aomaker/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/exceptions.py` & `aomaker-2.2.3/aomaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/extension/har_parse/__init__.py` & `aomaker-2.2.3/aomaker/extension/har_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/extension/har_parse/har_parse.py` & `aomaker-2.2.3/aomaker/extension/har_parse/har_parse.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/extension/recording/__init__.py` & `aomaker-2.2.3/aomaker/extension/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/extension/recording/recording.py` & `aomaker-2.2.3/aomaker/extension/recording/recording.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/field.py` & `aomaker-2.2.3/aomaker/field.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/fixture.py` & `aomaker-2.2.3/aomaker/fixture.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/hook_manager.py` & `aomaker-2.2.3/aomaker/hook_manager.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/html/heading.html` & `aomaker-2.2.3/aomaker/html/heading.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/html/report.html` & `aomaker-2.2.3/aomaker/html/report.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/html/template.html` & `aomaker-2.2.3/aomaker/html/template.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/log.py` & `aomaker-2.2.3/aomaker/log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/make.py` & `aomaker-2.2.3/aomaker/make.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/make_api.py` & `aomaker-2.2.3/aomaker/make_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/make_testcase.py` & `aomaker-2.2.3/aomaker/make_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/models.py` & `aomaker-2.2.3/aomaker/models.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/path.py` & `aomaker-2.2.3/aomaker/path.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/report.py` & `aomaker-2.2.3/aomaker/report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/runner.py` & `aomaker-2.2.3/aomaker/runner.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/scaffold.py` & `aomaker-2.2.3/aomaker/scaffold.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/send_msg/wechat.py` & `aomaker-2.2.3/aomaker/send_msg/wechat.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/swagger2yaml.py` & `aomaker-2.2.3/aomaker/swagger2yaml.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/template.py` & `aomaker-2.2.3/aomaker/template.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/utils/gen_allure_report.py` & `aomaker-2.2.3/aomaker/utils/gen_allure_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
                     all_results_json.append(result)
                     status_list.append(status_dict)
     for load_dict, status_dict in zip(all_results_json, status_list):
         status = status_dict["status"]
         tags = [label.get("value") for label in _handle_labels(load_dict['labels'])]
         product_name = _handle_tags(tags, marks_group, sep=sep)
         if product_name is not None:
+            if results.get(product_name) is None:
+                results[product_name] = {"passed": 0, "failed": 0, "skipped": 0, "broken": 0}
             results[product_name][status] += 1
     results = _count_passed_rate(results)
     return results
 
 
 def parse_allure_res_json():
     res = []
```

### Comparing `aomaker-2.2.2/aomaker/utils/utils.py` & `aomaker-2.2.3/aomaker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker/yaml2case.py` & `aomaker-2.2.3/aomaker/yaml2case.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/aomaker.egg-info/PKG-INFO` & `aomaker-2.2.3/aomaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.2.2
+Version: 2.2.3
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.2.2/aomaker.egg-info/SOURCES.txt` & `aomaker-2.2.3/aomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.2/setup.py` & `aomaker-2.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # --coding:utf-8--
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="aomaker",
-    version="2.2.2",
+    version="2.2.3",
     author="ancientone",
     author_email="listeningsss@163.com",
     description="An api testing framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ae86sen/aomaker",
     packages=setuptools.find_packages(),
```

