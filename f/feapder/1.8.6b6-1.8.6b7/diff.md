# Comparing `tmp/feapder-1.8.6b6.tar.gz` & `tmp/feapder-1.8.6b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feapder-1.8.6b6.tar", last modified: Wed Mar 29 13:32:12 2023, max compression
+gzip compressed data, was "feapder-1.8.6b7.tar", last modified: Mon May 22 04:00:03 2023, max compression
```

## Comparing `feapder-1.8.6b6.tar` & `feapder-1.8.6b7.tar`

### file list

```diff
@@ -1,219 +1,220 @@
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.554470 feapder-1.8.6b6/
--rw-r--r--   0 liubo      (501) staff       (20)     1102 2021-08-04 13:29:34.000000 feapder-1.8.6b6/LICENSE
--rw-r--r--   0 liubo      (501) staff       (20)      231 2021-08-12 03:51:27.000000 feapder-1.8.6b6/MANIFEST.in
--rw-r--r--   0 liubo      (501) staff       (20)     4568 2023-03-29 13:32:12.554036 feapder-1.8.6b6/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     4144 2023-03-28 02:44:40.000000 feapder-1.8.6b6/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.327801 feapder-1.8.6b6/feapder/
--rw-r--r--   0 liubo      (501) staff       (20)       11 2023-03-29 13:31:20.000000 feapder-1.8.6b6/feapder/VERSION
--rw-r--r--   0 liubo      (501) staff       (20)      815 2022-12-05 01:53:26.000000 feapder-1.8.6b6/feapder/__init__.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.336098 feapder-1.8.6b6/feapder/buffer/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.8.6b6/feapder/buffer/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)    14141 2022-11-18 03:50:33.000000 feapder-1.8.6b6/feapder/buffer/item_buffer.py
--rw-r--r--   0 liubo      (501) staff       (20)     5356 2022-11-29 02:59:23.000000 feapder-1.8.6b6/feapder/buffer/request_buffer.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.345322 feapder-1.8.6b6/feapder/commands/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.6b6/feapder/commands/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     3824 2023-03-13 06:31:28.000000 feapder-1.8.6b6/feapder/commands/cmdline.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.365090 feapder-1.8.6b6/feapder/commands/create/
--rw-r--r--   0 liubo      (501) staff       (20)      543 2021-09-02 10:23:23.000000 feapder-1.8.6b6/feapder/commands/create/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      975 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/commands/create/create_cookies.py
--rw-r--r--   0 liubo      (501) staff       (20)      670 2021-02-08 06:31:07.000000 feapder-1.8.6b6/feapder/commands/create/create_init.py
--rw-r--r--   0 liubo      (501) staff       (20)     6004 2022-09-07 03:39:37.000000 feapder-1.8.6b6/feapder/commands/create/create_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     1366 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/commands/create/create_json.py
--rw-r--r--   0 liubo      (501) staff       (20)     1106 2021-09-02 10:23:23.000000 feapder-1.8.6b6/feapder/commands/create/create_params.py
--rw-r--r--   0 liubo      (501) staff       (20)     1360 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/commands/create/create_project.py
--rw-r--r--   0 liubo      (501) staff       (20)      693 2021-08-04 13:29:34.000000 feapder-1.8.6b6/feapder/commands/create/create_setting.py
--rw-r--r--   0 liubo      (501) staff       (20)     3648 2022-09-07 03:39:37.000000 feapder-1.8.6b6/feapder/commands/create/create_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     4288 2022-10-18 13:06:20.000000 feapder-1.8.6b6/feapder/commands/create/create_table.py
--rw-r--r--   0 liubo      (501) staff       (20)     3984 2022-10-21 10:06:04.000000 feapder-1.8.6b6/feapder/commands/create_builder.py
--rw-r--r--   0 liubo      (501) staff       (20)     1354 2022-11-18 05:01:30.000000 feapder-1.8.6b6/feapder/commands/retry.py
--rw-r--r--   0 liubo      (501) staff       (20)     5514 2022-10-21 10:06:04.000000 feapder-1.8.6b6/feapder/commands/shell.py
--rw-r--r--   0 liubo      (501) staff       (20)     2572 2022-11-23 05:48:49.000000 feapder-1.8.6b6/feapder/commands/zip.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.378370 feapder-1.8.6b6/feapder/core/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.8.6b6/feapder/core/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     6240 2022-12-01 11:29:17.000000 feapder-1.8.6b6/feapder/core/base_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)     3256 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/core/collector.py
--rw-r--r--   0 liubo      (501) staff       (20)     2808 2022-11-18 04:36:04.000000 feapder-1.8.6b6/feapder/core/handle_failed_items.py
--rw-r--r--   0 liubo      (501) staff       (20)     1733 2022-11-18 04:36:47.000000 feapder-1.8.6b6/feapder/core/handle_failed_requests.py
--rw-r--r--   0 liubo      (501) staff       (20)    32694 2023-03-29 13:25:50.000000 feapder-1.8.6b6/feapder/core/parser_control.py
--rw-r--r--   0 liubo      (501) staff       (20)    21656 2023-03-07 03:52:29.000000 feapder-1.8.6b6/feapder/core/scheduler.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.387687 feapder-1.8.6b6/feapder/core/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)      417 2022-07-25 12:58:57.000000 feapder-1.8.6b6/feapder/core/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     4368 2023-03-07 03:52:29.000000 feapder-1.8.6b6/feapder/core/spiders/air_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    49433 2023-03-07 03:52:29.000000 feapder-1.8.6b6/feapder/core/spiders/batch_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    13420 2023-03-07 03:52:29.000000 feapder-1.8.6b6/feapder/core/spiders/spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    27875 2023-03-17 09:21:13.000000 feapder-1.8.6b6/feapder/core/spiders/task_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.394868 feapder-1.8.6b6/feapder/db/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-12-21 10:30:46.000000 feapder-1.8.6b6/feapder/db/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1117 2022-11-29 03:06:04.000000 feapder-1.8.6b6/feapder/db/memorydb.py
--rw-r--r--   0 liubo      (501) staff       (20)    13606 2021-12-04 11:42:58.000000 feapder-1.8.6b6/feapder/db/mongodb.py
--rw-r--r--   0 liubo      (501) staff       (20)    10799 2023-03-17 09:18:25.000000 feapder-1.8.6b6/feapder/db/mysqldb.py
--rw-r--r--   0 liubo      (501) staff       (20)    29292 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/db/redisdb.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.403400 feapder-1.8.6b6/feapder/dedup/
--rw-r--r--   0 liubo      (501) staff       (20)     6616 2022-09-25 13:50:01.000000 feapder-1.8.6b6/feapder/dedup/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      901 2022-09-25 13:50:01.000000 feapder-1.8.6b6/feapder/dedup/basefilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     4131 2022-11-15 02:02:15.000000 feapder-1.8.6b6/feapder/dedup/bitarray.py
--rw-r--r--   0 liubo      (501) staff       (20)    12518 2022-09-25 13:50:01.000000 feapder-1.8.6b6/feapder/dedup/bloomfilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     2309 2022-12-19 02:45:20.000000 feapder-1.8.6b6/feapder/dedup/expirefilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     1854 2023-01-03 05:05:31.000000 feapder-1.8.6b6/feapder/dedup/litefilter.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.416807 feapder-1.8.6b6/feapder/network/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.6b6/feapder/network/__init__.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.423055 feapder-1.8.6b6/feapder/network/downloader/
--rw-r--r--   0 liubo      (501) staff       (20)      179 2022-09-25 13:50:01.000000 feapder-1.8.6b6/feapder/network/downloader/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     3217 2022-11-02 03:08:06.000000 feapder-1.8.6b6/feapder/network/downloader/_playwright.py
--rw-r--r--   0 liubo      (501) staff       (20)     1440 2022-09-09 06:16:43.000000 feapder-1.8.6b6/feapder/network/downloader/_requests.py
--rw-r--r--   0 liubo      (501) staff       (20)     3093 2022-11-02 03:08:41.000000 feapder-1.8.6b6/feapder/network/downloader/_selenium.py
--rw-r--r--   0 liubo      (501) staff       (20)      694 2022-09-07 03:39:37.000000 feapder-1.8.6b6/feapder/network/downloader/base.py
--rw-r--r--   0 liubo      (501) staff       (20)     4341 2022-11-18 02:40:30.000000 feapder-1.8.6b6/feapder/network/item.py
--rw-r--r--   0 liubo      (501) staff       (20)    23025 2022-10-21 09:57:37.000000 feapder-1.8.6b6/feapder/network/proxy_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)    17351 2022-11-17 11:54:34.000000 feapder-1.8.6b6/feapder/network/request.py
--rw-r--r--   0 liubo      (501) staff       (20)    12743 2023-03-21 10:12:57.000000 feapder-1.8.6b6/feapder/network/response.py
--rw-r--r--   0 liubo      (501) staff       (20)     5661 2022-11-02 07:43:23.000000 feapder-1.8.6b6/feapder/network/selector.py
--rw-r--r--   0 liubo      (501) staff       (20)    42550 2021-08-12 03:51:27.000000 feapder-1.8.6b6/feapder/network/user_agent.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.429021 feapder-1.8.6b6/feapder/network/user_pool/
--rw-r--r--   0 liubo      (501) staff       (20)      329 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/network/user_pool/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     6397 2022-11-25 01:54:53.000000 feapder-1.8.6b6/feapder/network/user_pool/base_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)    10762 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/network/user_pool/gold_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     5372 2022-09-25 13:50:01.000000 feapder-1.8.6b6/feapder/network/user_pool/guest_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     8648 2023-03-17 09:07:47.000000 feapder-1.8.6b6/feapder/network/user_pool/normal_user_pool.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.437306 feapder-1.8.6b6/feapder/pipelines/
--rw-r--r--   0 liubo      (501) staff       (20)     1382 2021-09-23 09:22:51.000000 feapder-1.8.6b6/feapder/pipelines/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1392 2022-09-25 13:50:01.000000 feapder-1.8.6b6/feapder/pipelines/console_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2405 2021-09-23 09:22:51.000000 feapder-1.8.6b6/feapder/pipelines/mongo_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2088 2021-04-08 03:41:12.000000 feapder-1.8.6b6/feapder/pipelines/mysql_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)      363 2022-10-24 13:37:46.000000 feapder-1.8.6b6/feapder/requirements.txt
--rw-r--r--   0 liubo      (501) staff       (20)    10750 2022-12-05 01:53:03.000000 feapder-1.8.6b6/feapder/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.444342 feapder-1.8.6b6/feapder/templates/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.6b6/feapder/templates/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)      592 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/templates/air_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)     2083 2022-09-07 03:39:38.000000 feapder-1.8.6b6/feapder/templates/batch_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)      353 2021-12-22 05:53:07.000000 feapder-1.8.6b6/feapder/templates/item_template.tmpl
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.448703 feapder-1.8.6b6/feapder/templates/project_template/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.6b6/feapder/templates/project_template/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)     1574 2021-08-04 13:29:34.000000 feapder-1.8.6b6/feapder/templates/project_template/CHECK_DATA.md
--rw-r--r--   0 liubo      (501) staff       (20)       81 2021-08-04 13:29:34.000000 feapder-1.8.6b6/feapder/templates/project_template/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.449634 feapder-1.8.6b6/feapder/templates/project_template/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.6b6/feapder/templates/project_template/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     2089 2021-09-02 10:23:23.000000 feapder-1.8.6b6/feapder/templates/project_template/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     8745 2022-12-05 01:53:03.000000 feapder-1.8.6b6/feapder/templates/project_template/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.450855 feapder-1.8.6b6/feapder/templates/project_template/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.6b6/feapder/templates/project_template/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      808 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/templates/spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.8.6b6/feapder/templates/task_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)      365 2022-09-19 07:00:37.000000 feapder-1.8.6b6/feapder/templates/update_item_template.tmpl
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.459029 feapder-1.8.6b6/feapder/utils/
--rw-r--r--   0 liubo      (501) staff       (20)      135 2021-08-04 13:29:34.000000 feapder-1.8.6b6/feapder/utils/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1959 2021-02-07 13:26:42.000000 feapder-1.8.6b6/feapder/utils/custom_argparse.py
--rw-r--r--   0 liubo      (501) staff       (20)     2537 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/utils/email_sender.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.462131 feapder-1.8.6b6/feapder/utils/js/
--rw-r--r--   0 liubo      (501) staff       (20)     6344 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/utils/js/intercept.js
--rw-r--r--   0 liubo      (501) staff       (20)   166307 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/utils/js/stealth.min.js
--rw-r--r--   0 liubo      (501) staff       (20)     8097 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/utils/log.py
--rw-r--r--   0 liubo      (501) staff       (20)    16467 2023-03-17 03:23:27.000000 feapder-1.8.6b6/feapder/utils/metrics.py
--rw-r--r--   0 liubo      (501) staff       (20)     2123 2021-08-12 03:51:27.000000 feapder-1.8.6b6/feapder/utils/perfect_dict.py
--rw-r--r--   0 liubo      (501) staff       (20)     3670 2022-06-10 02:51:23.000000 feapder-1.8.6b6/feapder/utils/redis_lock.py
--rw-r--r--   0 liubo      (501) staff       (20)    73692 2022-11-22 08:59:30.000000 feapder-1.8.6b6/feapder/utils/tools.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.472156 feapder-1.8.6b6/feapder/utils/webdriver/
--rw-r--r--   0 liubo      (501) staff       (20)      380 2022-10-17 08:53:37.000000 feapder-1.8.6b6/feapder/utils/webdriver/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     9330 2022-10-19 03:56:09.000000 feapder-1.8.6b6/feapder/utils/webdriver/playwright_driver.py
--rw-r--r--   0 liubo      (501) staff       (20)    12628 2022-11-04 06:05:47.000000 feapder-1.8.6b6/feapder/utils/webdriver/selenium_driver.py
--rw-r--r--   0 liubo      (501) staff       (20)     2574 2022-10-13 12:10:47.000000 feapder-1.8.6b6/feapder/utils/webdriver/webdirver.py
--rw-r--r--   0 liubo      (501) staff       (20)     3282 2022-11-02 03:08:54.000000 feapder-1.8.6b6/feapder/utils/webdriver/webdriver_pool.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.333340 feapder-1.8.6b6/feapder.egg-info/
--rw-r--r--   0 liubo      (501) staff       (20)     4568 2023-03-29 13:32:12.000000 feapder-1.8.6b6/feapder.egg-info/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     5729 2023-03-29 13:32:12.000000 feapder-1.8.6b6/feapder.egg-info/SOURCES.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2023-03-29 13:32:12.000000 feapder-1.8.6b6/feapder.egg-info/dependency_links.txt
--rw-r--r--   0 liubo      (501) staff       (20)       61 2023-03-29 13:32:12.000000 feapder-1.8.6b6/feapder.egg-info/entry_points.txt
--rw-r--r--   0 liubo      (501) staff       (20)      371 2023-03-29 13:32:12.000000 feapder-1.8.6b6/feapder.egg-info/requires.txt
--rw-r--r--   0 liubo      (501) staff       (20)        8 2023-03-29 13:32:12.000000 feapder-1.8.6b6/feapder.egg-info/top_level.txt
--rw-r--r--   0 liubo      (501) staff       (20)       38 2023-03-29 13:32:12.554618 feapder-1.8.6b6/setup.cfg
--rw-r--r--   0 liubo      (501) staff       (20)     2030 2022-10-24 13:39:07.000000 feapder-1.8.6b6/setup.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.506299 feapder-1.8.6b6/tests/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.511737 feapder-1.8.6b6/tests/air-spider/
--rw-r--r--   0 liubo      (501) staff       (20)     1218 2022-11-29 03:10:00.000000 feapder-1.8.6b6/tests/air-spider/test_air_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     1075 2022-10-25 08:06:13.000000 feapder-1.8.6b6/tests/air-spider/test_air_spider_filter.py
--rw-r--r--   0 liubo      (501) staff       (20)     1094 2022-12-19 02:05:14.000000 feapder-1.8.6b6/tests/air-spider/test_air_spider_item.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.514399 feapder-1.8.6b6/tests/batch-spider/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.522189 feapder-1.8.6b6/tests/batch-spider/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2021-09-03 07:47:43.000000 feapder-1.8.6b6/tests/batch-spider/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      586 2021-09-12 14:22:50.000000 feapder-1.8.6b6/tests/batch-spider/items/spider_data_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     2020 2022-10-24 09:10:44.000000 feapder-1.8.6b6/tests/batch-spider/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2227 2021-09-02 10:23:23.000000 feapder-1.8.6b6/tests/batch-spider/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.524518 feapder-1.8.6b6/tests/batch-spider/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       31 2021-02-08 08:09:47.000000 feapder-1.8.6b6/tests/batch-spider/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1513 2021-10-09 11:17:03.000000 feapder-1.8.6b6/tests/batch-spider/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      851 2021-02-08 08:29:51.000000 feapder-1.8.6b6/tests/batch-spider/table.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.517421 feapder-1.8.6b6/tests/batch-spider-integration/
--rw-r--r--   0 liubo      (501) staff       (20)      746 2021-03-03 03:39:52.000000 feapder-1.8.6b6/tests/batch-spider-integration/batch_spider_integration_task.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.518160 feapder-1.8.6b6/tests/batch-spider-integration/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.8.6b6/tests/batch-spider-integration/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1686 2021-12-30 08:52:14.000000 feapder-1.8.6b6/tests/batch-spider-integration/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.8.6b6/tests/batch-spider-integration/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.520501 feapder-1.8.6b6/tests/batch-spider-integration/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.8.6b6/tests/batch-spider-integration/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      581 2021-03-18 02:19:03.000000 feapder-1.8.6b6/tests/batch-spider-integration/spiders/sina_news_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)      584 2021-03-18 02:19:03.000000 feapder-1.8.6b6/tests/batch-spider-integration/spiders/tencent_news_parser.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.525230 feapder-1.8.6b6/tests/db/
--rw-r--r--   0 liubo      (501) staff       (20)      373 2021-03-06 15:13:19.000000 feapder-1.8.6b6/tests/db/test_redis.py
--rw-r--r--   0 liubo      (501) staff       (20)     2087 2021-03-18 02:19:03.000000 feapder-1.8.6b6/tests/jd_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     1011 2021-12-01 05:56:45.000000 feapder-1.8.6b6/tests/mongo_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.527333 feapder-1.8.6b6/tests/spider/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.537896 feapder-1.8.6b6/tests/spider/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2022-01-27 08:13:00.000000 feapder-1.8.6b6/tests/spider/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      358 2021-12-22 05:05:06.000000 feapder-1.8.6b6/tests/spider/items/spider_data_item.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.538922 feapder-1.8.6b6/tests/spider/log/
--rw-r--r--   0 liubo      (501) staff       (20)     1719 2021-08-11 01:59:56.000000 feapder-1.8.6b6/tests/spider/log/haha.log
--rw-r--r--   0 liubo      (501) staff       (20)      296 2022-08-31 02:19:25.000000 feapder-1.8.6b6/tests/spider/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2676 2022-10-25 08:22:58.000000 feapder-1.8.6b6/tests/spider/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.541533 feapder-1.8.6b6/tests/spider/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       42 2021-02-21 15:44:20.000000 feapder-1.8.6b6/tests/spider/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      985 2022-10-25 08:22:40.000000 feapder-1.8.6b6/tests/spider/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      612 2021-08-04 13:29:34.000000 feapder-1.8.6b6/tests/spider/spiders/test_spider2.py
--rw-r--r--   0 liubo      (501) staff       (20)      320 2021-02-08 08:40:34.000000 feapder-1.8.6b6/tests/spider/table.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.528843 feapder-1.8.6b6/tests/spider-integration/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.529804 feapder-1.8.6b6/tests/spider-integration/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.8.6b6/tests/spider-integration/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      517 2021-12-30 08:51:43.000000 feapder-1.8.6b6/tests/spider-integration/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.8.6b6/tests/spider-integration/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.533539 feapder-1.8.6b6/tests/spider-integration/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.8.6b6/tests/spider-integration/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      470 2023-03-29 13:31:04.000000 feapder-1.8.6b6/tests/spider-integration/spiders/sina_news_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)      456 2021-09-24 05:52:08.000000 feapder-1.8.6b6/tests/spider-integration/spiders/tencent_news_parser.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.542463 feapder-1.8.6b6/tests/task-spider/
--rw-r--r--   0 liubo      (501) staff       (20)     2133 2023-03-17 09:29:04.000000 feapder-1.8.6b6/tests/task-spider/test_task_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.546563 feapder-1.8.6b6/tests/test-pipeline/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.548090 feapder-1.8.6b6/tests/test-pipeline/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2021-03-18 02:19:03.000000 feapder-1.8.6b6/tests/test-pipeline/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      586 2021-03-18 02:19:03.000000 feapder-1.8.6b6/tests/test-pipeline/items/spider_data_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     1250 2022-09-07 03:39:38.000000 feapder-1.8.6b6/tests/test-pipeline/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     1416 2021-04-08 03:41:12.000000 feapder-1.8.6b6/tests/test-pipeline/pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2021-09-02 10:23:23.000000 feapder-1.8.6b6/tests/test-pipeline/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.549986 feapder-1.8.6b6/tests/test-pipeline/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       31 2021-03-30 02:34:20.000000 feapder-1.8.6b6/tests/test-pipeline/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1514 2021-03-18 02:19:03.000000 feapder-1.8.6b6/tests/test-pipeline/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      851 2021-03-18 02:19:03.000000 feapder-1.8.6b6/tests/test-pipeline/table.sql
--rw-r--r--   0 liubo      (501) staff       (20)      281 2022-11-22 03:30:44.000000 feapder-1.8.6b6/tests/test.py
--rw-r--r--   0 liubo      (501) staff       (20)     3140 2022-12-19 02:27:37.000000 feapder-1.8.6b6/tests/test_dedup.py
--rw-r--r--   0 liubo      (501) staff       (20)      469 2021-09-02 10:22:59.000000 feapder-1.8.6b6/tests/test_lock.py
--rw-r--r--   0 liubo      (501) staff       (20)      189 2022-03-26 15:56:04.000000 feapder-1.8.6b6/tests/test_log.py
--rw-r--r--   0 liubo      (501) staff       (20)      506 2022-10-21 09:39:04.000000 feapder-1.8.6b6/tests/test_metrics.py
--rw-r--r--   0 liubo      (501) staff       (20)     4678 2021-12-01 05:56:51.000000 feapder-1.8.6b6/tests/test_mongodb.py
--rw-r--r--   0 liubo      (501) staff       (20)      232 2021-10-14 08:25:11.000000 feapder-1.8.6b6/tests/test_mysqldb.py
--rw-r--r--   0 liubo      (501) staff       (20)     1086 2022-10-31 02:55:57.000000 feapder-1.8.6b6/tests/test_playwright.py
--rw-r--r--   0 liubo      (501) staff       (20)     3477 2022-11-14 06:18:23.000000 feapder-1.8.6b6/tests/test_playwright2.py
--rw-r--r--   0 liubo      (501) staff       (20)     1177 2021-04-08 03:41:12.000000 feapder-1.8.6b6/tests/test_proxies_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)      660 2022-10-28 07:20:27.000000 feapder-1.8.6b6/tests/test_rander.py
--rw-r--r--   0 liubo      (501) staff       (20)      769 2021-07-08 11:51:50.000000 feapder-1.8.6b6/tests/test_rander2.py
--rw-r--r--   0 liubo      (501) staff       (20)      519 2022-09-14 07:25:07.000000 feapder-1.8.6b6/tests/test_rander3.py
--rw-r--r--   0 liubo      (501) staff       (20)     1983 2022-09-07 09:10:17.000000 feapder-1.8.6b6/tests/test_rander_xhr.py
--rw-r--r--   0 liubo      (501) staff       (20)      148 2021-08-12 03:51:27.000000 feapder-1.8.6b6/tests/test_redisdb.py
--rw-r--r--   0 liubo      (501) staff       (20)     1634 2022-09-25 13:50:01.000000 feapder-1.8.6b6/tests/test_request.py
--rw-r--r--   0 liubo      (501) staff       (20)      637 2021-04-08 03:41:12.000000 feapder-1.8.6b6/tests/test_spider_params.py
--rw-r--r--   0 liubo      (501) staff       (20)      593 2022-07-25 12:58:57.000000 feapder-1.8.6b6/tests/test_task.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.550978 feapder-1.8.6b6/tests/test_template/
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.8.6b6/tests/test_template/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      429 2022-05-17 07:19:13.000000 feapder-1.8.6b6/tests/test_tools.py
--rw-r--r--   0 liubo      (501) staff       (20)     1011 2022-09-07 09:10:23.000000 feapder-1.8.6b6/tests/test_webdriver.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-03-29 13:32:12.553175 feapder-1.8.6b6/tests/user_pool/
--rw-r--r--   0 liubo      (501) staff       (20)     2423 2022-06-10 02:51:23.000000 feapder-1.8.6b6/tests/user_pool/test_gold_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     2121 2022-06-10 02:51:23.000000 feapder-1.8.6b6/tests/user_pool/test_guest_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     1427 2022-06-10 02:51:23.000000 feapder-1.8.6b6/tests/user_pool/test_normal_user_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.578266 feapder-1.8.6b7/
+-rw-r--r--   0 liubo      (501) staff       (20)     1102 2021-08-04 13:29:34.000000 feapder-1.8.6b7/LICENSE
+-rw-r--r--   0 liubo      (501) staff       (20)      231 2021-08-12 03:51:27.000000 feapder-1.8.6b7/MANIFEST.in
+-rw-r--r--   0 liubo      (501) staff       (20)     4568 2023-05-22 04:00:03.577899 feapder-1.8.6b7/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     4144 2023-03-30 02:09:37.000000 feapder-1.8.6b7/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.378508 feapder-1.8.6b7/feapder/
+-rw-r--r--   0 liubo      (501) staff       (20)       11 2023-05-22 03:59:20.000000 feapder-1.8.6b7/feapder/VERSION
+-rw-r--r--   0 liubo      (501) staff       (20)      815 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/__init__.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.383382 feapder-1.8.6b7/feapder/buffer/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.8.6b7/feapder/buffer/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)    14141 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/buffer/item_buffer.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5356 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/buffer/request_buffer.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.386927 feapder-1.8.6b7/feapder/commands/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.6b7/feapder/commands/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3824 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/commands/cmdline.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.394696 feapder-1.8.6b7/feapder/commands/create/
+-rw-r--r--   0 liubo      (501) staff       (20)      543 2021-09-02 10:23:23.000000 feapder-1.8.6b7/feapder/commands/create/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      975 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/commands/create/create_cookies.py
+-rw-r--r--   0 liubo      (501) staff       (20)      670 2021-02-08 06:31:07.000000 feapder-1.8.6b7/feapder/commands/create/create_init.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6004 2022-09-07 03:39:37.000000 feapder-1.8.6b7/feapder/commands/create/create_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1366 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/commands/create/create_json.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1106 2021-09-02 10:23:23.000000 feapder-1.8.6b7/feapder/commands/create/create_params.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1360 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/commands/create/create_project.py
+-rw-r--r--   0 liubo      (501) staff       (20)      693 2021-08-04 13:29:34.000000 feapder-1.8.6b7/feapder/commands/create/create_setting.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3648 2022-09-07 03:39:37.000000 feapder-1.8.6b7/feapder/commands/create/create_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4288 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/commands/create/create_table.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3984 2022-10-21 10:06:04.000000 feapder-1.8.6b7/feapder/commands/create_builder.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1354 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/commands/retry.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5514 2022-10-21 10:06:04.000000 feapder-1.8.6b7/feapder/commands/shell.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2572 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/commands/zip.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.399515 feapder-1.8.6b7/feapder/core/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.8.6b7/feapder/core/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6240 2022-12-01 11:29:17.000000 feapder-1.8.6b7/feapder/core/base_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3256 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/core/collector.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2808 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/core/handle_failed_items.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1733 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/core/handle_failed_requests.py
+-rw-r--r--   0 liubo      (501) staff       (20)    32694 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/core/parser_control.py
+-rw-r--r--   0 liubo      (501) staff       (20)    21656 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/core/scheduler.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.403798 feapder-1.8.6b7/feapder/core/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)      417 2022-07-25 12:58:57.000000 feapder-1.8.6b7/feapder/core/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4368 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/core/spiders/air_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    49433 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/core/spiders/batch_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    13420 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/core/spiders/spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    27875 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/core/spiders/task_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.407432 feapder-1.8.6b7/feapder/db/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-12-21 10:30:46.000000 feapder-1.8.6b7/feapder/db/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1117 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/db/memorydb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    13606 2021-12-04 11:42:58.000000 feapder-1.8.6b7/feapder/db/mongodb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10799 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/db/mysqldb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    29379 2023-05-22 03:57:39.000000 feapder-1.8.6b7/feapder/db/redisdb.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.411532 feapder-1.8.6b7/feapder/dedup/
+-rw-r--r--   0 liubo      (501) staff       (20)     6616 2022-09-25 13:50:01.000000 feapder-1.8.6b7/feapder/dedup/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      901 2022-09-25 13:50:01.000000 feapder-1.8.6b7/feapder/dedup/basefilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4131 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/dedup/bitarray.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12518 2022-09-25 13:50:01.000000 feapder-1.8.6b7/feapder/dedup/bloomfilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2309 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/dedup/expirefilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1854 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/dedup/litefilter.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.419527 feapder-1.8.6b7/feapder/network/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.6b7/feapder/network/__init__.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.450431 feapder-1.8.6b7/feapder/network/downloader/
+-rw-r--r--   0 liubo      (501) staff       (20)      179 2022-09-25 13:50:01.000000 feapder-1.8.6b7/feapder/network/downloader/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3217 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/downloader/_playwright.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1440 2022-09-09 06:16:43.000000 feapder-1.8.6b7/feapder/network/downloader/_requests.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3093 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/downloader/_selenium.py
+-rw-r--r--   0 liubo      (501) staff       (20)      694 2022-09-07 03:39:37.000000 feapder-1.8.6b7/feapder/network/downloader/base.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4341 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/item.py
+-rw-r--r--   0 liubo      (501) staff       (20)    23025 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/proxy_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)    17351 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/request.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12743 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/response.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5661 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/selector.py
+-rw-r--r--   0 liubo      (501) staff       (20)    42550 2023-04-11 08:22:57.000000 feapder-1.8.6b7/feapder/network/user_agent.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.459597 feapder-1.8.6b7/feapder/network/user_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)      329 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/network/user_pool/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6397 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/user_pool/base_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10762 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/network/user_pool/gold_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5372 2022-09-25 13:50:01.000000 feapder-1.8.6b7/feapder/network/user_pool/guest_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8648 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/network/user_pool/normal_user_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.470777 feapder-1.8.6b7/feapder/pipelines/
+-rw-r--r--   0 liubo      (501) staff       (20)     1382 2021-09-23 09:22:51.000000 feapder-1.8.6b7/feapder/pipelines/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1392 2022-09-25 13:50:01.000000 feapder-1.8.6b7/feapder/pipelines/console_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2405 2021-09-23 09:22:51.000000 feapder-1.8.6b7/feapder/pipelines/mongo_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2088 2021-04-08 03:41:12.000000 feapder-1.8.6b7/feapder/pipelines/mysql_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)      363 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/requirements.txt
+-rw-r--r--   0 liubo      (501) staff       (20)    10826 2023-05-22 03:58:15.000000 feapder-1.8.6b7/feapder/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.483927 feapder-1.8.6b7/feapder/templates/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.6b7/feapder/templates/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)      592 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/templates/air_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)     2083 2022-09-07 03:39:38.000000 feapder-1.8.6b7/feapder/templates/batch_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)      353 2021-12-22 05:53:07.000000 feapder-1.8.6b7/feapder/templates/item_template.tmpl
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.493509 feapder-1.8.6b7/feapder/templates/project_template/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.6b7/feapder/templates/project_template/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)     1574 2021-08-04 13:29:34.000000 feapder-1.8.6b7/feapder/templates/project_template/CHECK_DATA.md
+-rw-r--r--   0 liubo      (501) staff       (20)       81 2021-08-04 13:29:34.000000 feapder-1.8.6b7/feapder/templates/project_template/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.494624 feapder-1.8.6b7/feapder/templates/project_template/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.6b7/feapder/templates/project_template/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2089 2021-09-02 10:23:23.000000 feapder-1.8.6b7/feapder/templates/project_template/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8825 2023-05-22 03:59:20.000000 feapder-1.8.6b7/feapder/templates/project_template/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.495507 feapder-1.8.6b7/feapder/templates/project_template/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.6b7/feapder/templates/project_template/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      808 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/templates/spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.8.6b7/feapder/templates/task_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)      365 2022-09-19 07:00:37.000000 feapder-1.8.6b7/feapder/templates/update_item_template.tmpl
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.505297 feapder-1.8.6b7/feapder/utils/
+-rw-r--r--   0 liubo      (501) staff       (20)      135 2021-08-04 13:29:34.000000 feapder-1.8.6b7/feapder/utils/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1959 2021-02-07 13:26:42.000000 feapder-1.8.6b7/feapder/utils/custom_argparse.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2537 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/utils/email_sender.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.508031 feapder-1.8.6b7/feapder/utils/js/
+-rw-r--r--   0 liubo      (501) staff       (20)     6344 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/utils/js/intercept.js
+-rw-r--r--   0 liubo      (501) staff       (20)   166307 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/utils/js/stealth.min.js
+-rw-r--r--   0 liubo      (501) staff       (20)     8097 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/utils/log.py
+-rw-r--r--   0 liubo      (501) staff       (20)    16820 2023-04-28 09:52:17.000000 feapder-1.8.6b7/feapder/utils/metrics.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2123 2021-08-12 03:51:27.000000 feapder-1.8.6b7/feapder/utils/perfect_dict.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3670 2022-06-10 02:51:23.000000 feapder-1.8.6b7/feapder/utils/redis_lock.py
+-rw-r--r--   0 liubo      (501) staff       (20)    73692 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/utils/tools.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.516792 feapder-1.8.6b7/feapder/utils/webdriver/
+-rw-r--r--   0 liubo      (501) staff       (20)      380 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/utils/webdriver/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     9330 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/utils/webdriver/playwright_driver.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12628 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/utils/webdriver/selenium_driver.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2574 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/utils/webdriver/webdirver.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3282 2023-03-30 02:09:37.000000 feapder-1.8.6b7/feapder/utils/webdriver/webdriver_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.381182 feapder-1.8.6b7/feapder.egg-info/
+-rw-r--r--   0 liubo      (501) staff       (20)     4568 2023-05-22 04:00:03.000000 feapder-1.8.6b7/feapder.egg-info/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     5768 2023-05-22 04:00:03.000000 feapder-1.8.6b7/feapder.egg-info/SOURCES.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2023-05-22 04:00:03.000000 feapder-1.8.6b7/feapder.egg-info/dependency_links.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       61 2023-05-22 04:00:03.000000 feapder-1.8.6b7/feapder.egg-info/entry_points.txt
+-rw-r--r--   0 liubo      (501) staff       (20)      371 2023-05-22 04:00:03.000000 feapder-1.8.6b7/feapder.egg-info/requires.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        8 2023-05-22 04:00:03.000000 feapder-1.8.6b7/feapder.egg-info/top_level.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       38 2023-05-22 04:00:03.578376 feapder-1.8.6b7/setup.cfg
+-rw-r--r--   0 liubo      (501) staff       (20)     2030 2023-04-11 08:22:57.000000 feapder-1.8.6b7/setup.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.537935 feapder-1.8.6b7/tests/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.541024 feapder-1.8.6b7/tests/air-spider/
+-rw-r--r--   0 liubo      (501) staff       (20)     1218 2022-11-29 03:10:00.000000 feapder-1.8.6b7/tests/air-spider/test_air_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1075 2023-03-30 02:09:37.000000 feapder-1.8.6b7/tests/air-spider/test_air_spider_filter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1094 2023-03-30 02:09:37.000000 feapder-1.8.6b7/tests/air-spider/test_air_spider_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)      638 2023-04-28 09:18:56.000000 feapder-1.8.6b7/tests/air-spider/test_render_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.543723 feapder-1.8.6b7/tests/batch-spider/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.551741 feapder-1.8.6b7/tests/batch-spider/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2021-09-03 07:47:43.000000 feapder-1.8.6b7/tests/batch-spider/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      586 2021-09-12 14:22:50.000000 feapder-1.8.6b7/tests/batch-spider/items/spider_data_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2020 2022-10-24 09:10:44.000000 feapder-1.8.6b7/tests/batch-spider/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2227 2021-09-02 10:23:23.000000 feapder-1.8.6b7/tests/batch-spider/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.553382 feapder-1.8.6b7/tests/batch-spider/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       31 2021-02-08 08:09:47.000000 feapder-1.8.6b7/tests/batch-spider/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1513 2021-10-09 11:17:03.000000 feapder-1.8.6b7/tests/batch-spider/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      851 2021-02-08 08:29:51.000000 feapder-1.8.6b7/tests/batch-spider/table.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.546577 feapder-1.8.6b7/tests/batch-spider-integration/
+-rw-r--r--   0 liubo      (501) staff       (20)      746 2021-03-03 03:39:52.000000 feapder-1.8.6b7/tests/batch-spider-integration/batch_spider_integration_task.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.547601 feapder-1.8.6b7/tests/batch-spider-integration/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.8.6b7/tests/batch-spider-integration/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1686 2021-12-30 08:52:14.000000 feapder-1.8.6b7/tests/batch-spider-integration/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.8.6b7/tests/batch-spider-integration/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.549617 feapder-1.8.6b7/tests/batch-spider-integration/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.8.6b7/tests/batch-spider-integration/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      581 2021-03-18 02:19:03.000000 feapder-1.8.6b7/tests/batch-spider-integration/spiders/sina_news_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)      584 2021-03-18 02:19:03.000000 feapder-1.8.6b7/tests/batch-spider-integration/spiders/tencent_news_parser.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.554115 feapder-1.8.6b7/tests/db/
+-rw-r--r--   0 liubo      (501) staff       (20)      373 2021-03-06 15:13:19.000000 feapder-1.8.6b7/tests/db/test_redis.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2087 2021-03-18 02:19:03.000000 feapder-1.8.6b7/tests/jd_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1011 2021-12-01 05:56:45.000000 feapder-1.8.6b7/tests/mongo_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.556328 feapder-1.8.6b7/tests/spider/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.562682 feapder-1.8.6b7/tests/spider/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2022-01-27 08:13:00.000000 feapder-1.8.6b7/tests/spider/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      358 2021-12-22 05:05:06.000000 feapder-1.8.6b7/tests/spider/items/spider_data_item.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.563606 feapder-1.8.6b7/tests/spider/log/
+-rw-r--r--   0 liubo      (501) staff       (20)     1719 2021-08-11 01:59:56.000000 feapder-1.8.6b7/tests/spider/log/haha.log
+-rw-r--r--   0 liubo      (501) staff       (20)      296 2022-08-31 02:19:25.000000 feapder-1.8.6b7/tests/spider/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2676 2023-03-30 02:09:37.000000 feapder-1.8.6b7/tests/spider/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.566478 feapder-1.8.6b7/tests/spider/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       42 2021-02-21 15:44:20.000000 feapder-1.8.6b7/tests/spider/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      985 2022-10-25 08:22:40.000000 feapder-1.8.6b7/tests/spider/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      612 2021-08-04 13:29:34.000000 feapder-1.8.6b7/tests/spider/spiders/test_spider2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      320 2021-02-08 08:40:34.000000 feapder-1.8.6b7/tests/spider/table.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.557861 feapder-1.8.6b7/tests/spider-integration/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.558632 feapder-1.8.6b7/tests/spider-integration/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.8.6b7/tests/spider-integration/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      517 2021-12-30 08:51:43.000000 feapder-1.8.6b7/tests/spider-integration/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.8.6b7/tests/spider-integration/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.560809 feapder-1.8.6b7/tests/spider-integration/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.8.6b7/tests/spider-integration/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      470 2023-03-29 13:31:04.000000 feapder-1.8.6b7/tests/spider-integration/spiders/sina_news_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)      456 2021-09-24 05:52:08.000000 feapder-1.8.6b7/tests/spider-integration/spiders/tencent_news_parser.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.567407 feapder-1.8.6b7/tests/task-spider/
+-rw-r--r--   0 liubo      (501) staff       (20)     2133 2023-03-30 02:09:37.000000 feapder-1.8.6b7/tests/task-spider/test_task_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.571161 feapder-1.8.6b7/tests/test-pipeline/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.573151 feapder-1.8.6b7/tests/test-pipeline/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2021-03-18 02:19:03.000000 feapder-1.8.6b7/tests/test-pipeline/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      586 2021-03-18 02:19:03.000000 feapder-1.8.6b7/tests/test-pipeline/items/spider_data_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1250 2022-09-07 03:39:38.000000 feapder-1.8.6b7/tests/test-pipeline/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1416 2021-04-08 03:41:12.000000 feapder-1.8.6b7/tests/test-pipeline/pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2021-09-02 10:23:23.000000 feapder-1.8.6b7/tests/test-pipeline/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.574483 feapder-1.8.6b7/tests/test-pipeline/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       31 2021-03-30 02:34:20.000000 feapder-1.8.6b7/tests/test-pipeline/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1514 2021-03-18 02:19:03.000000 feapder-1.8.6b7/tests/test-pipeline/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      851 2021-03-18 02:19:03.000000 feapder-1.8.6b7/tests/test-pipeline/table.sql
+-rw-r--r--   0 liubo      (501) staff       (20)      281 2022-11-22 03:30:44.000000 feapder-1.8.6b7/tests/test.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3140 2023-03-30 02:09:37.000000 feapder-1.8.6b7/tests/test_dedup.py
+-rw-r--r--   0 liubo      (501) staff       (20)      469 2021-09-02 10:22:59.000000 feapder-1.8.6b7/tests/test_lock.py
+-rw-r--r--   0 liubo      (501) staff       (20)      189 2022-03-26 15:56:04.000000 feapder-1.8.6b7/tests/test_log.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1229 2023-05-22 03:51:23.000000 feapder-1.8.6b7/tests/test_metrics.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4678 2021-12-01 05:56:51.000000 feapder-1.8.6b7/tests/test_mongodb.py
+-rw-r--r--   0 liubo      (501) staff       (20)      232 2021-10-14 08:25:11.000000 feapder-1.8.6b7/tests/test_mysqldb.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1086 2023-03-30 02:09:37.000000 feapder-1.8.6b7/tests/test_playwright.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3477 2023-03-30 02:09:37.000000 feapder-1.8.6b7/tests/test_playwright2.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1177 2021-04-08 03:41:12.000000 feapder-1.8.6b7/tests/test_proxies_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)      660 2022-10-28 07:20:27.000000 feapder-1.8.6b7/tests/test_rander.py
+-rw-r--r--   0 liubo      (501) staff       (20)      769 2021-07-08 11:51:50.000000 feapder-1.8.6b7/tests/test_rander2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      519 2022-09-14 07:25:07.000000 feapder-1.8.6b7/tests/test_rander3.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1983 2022-09-07 09:10:17.000000 feapder-1.8.6b7/tests/test_rander_xhr.py
+-rw-r--r--   0 liubo      (501) staff       (20)      148 2021-08-12 03:51:27.000000 feapder-1.8.6b7/tests/test_redisdb.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1634 2022-09-25 13:50:01.000000 feapder-1.8.6b7/tests/test_request.py
+-rw-r--r--   0 liubo      (501) staff       (20)      637 2021-04-08 03:41:12.000000 feapder-1.8.6b7/tests/test_spider_params.py
+-rw-r--r--   0 liubo      (501) staff       (20)      593 2022-07-25 12:58:57.000000 feapder-1.8.6b7/tests/test_task.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.575089 feapder-1.8.6b7/tests/test_template/
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.8.6b7/tests/test_template/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      429 2022-05-17 07:19:13.000000 feapder-1.8.6b7/tests/test_tools.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1011 2022-09-07 09:10:23.000000 feapder-1.8.6b7/tests/test_webdriver.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-05-22 04:00:03.577173 feapder-1.8.6b7/tests/user_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)     2423 2022-06-10 02:51:23.000000 feapder-1.8.6b7/tests/user_pool/test_gold_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2121 2022-06-10 02:51:23.000000 feapder-1.8.6b7/tests/user_pool/test_guest_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1427 2022-06-10 02:51:23.000000 feapder-1.8.6b7/tests/user_pool/test_normal_user_pool.py
```

### Comparing `feapder-1.8.6b6/LICENSE` & `feapder-1.8.6b7/LICENSE`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/PKG-INFO` & `feapder-1.8.6b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feapder
-Version: 1.8.6b6
+Version: 1.8.6b7
 Summary: feapder是一款支持分布式、批次采集、任务防丢、报警丰富的python爬虫框架
 Home-page: https://github.com/Boris-code/feapder.git
 Author: Boris
 Author-email: feapder@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `feapder-1.8.6b6/README.md` & `feapder-1.8.6b7/README.md`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/__init__.py` & `feapder-1.8.6b7/feapder/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/buffer/item_buffer.py` & `feapder-1.8.6b7/feapder/buffer/item_buffer.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/buffer/request_buffer.py` & `feapder-1.8.6b7/feapder/buffer/request_buffer.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/cmdline.py` & `feapder-1.8.6b7/feapder/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/__init__.py` & `feapder-1.8.6b7/feapder/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_cookies.py` & `feapder-1.8.6b7/feapder/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_init.py` & `feapder-1.8.6b7/feapder/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_item.py` & `feapder-1.8.6b7/feapder/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_json.py` & `feapder-1.8.6b7/feapder/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_params.py` & `feapder-1.8.6b7/feapder/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_project.py` & `feapder-1.8.6b7/feapder/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_setting.py` & `feapder-1.8.6b7/feapder/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_spider.py` & `feapder-1.8.6b7/feapder/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create/create_table.py` & `feapder-1.8.6b7/feapder/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/create_builder.py` & `feapder-1.8.6b7/feapder/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/retry.py` & `feapder-1.8.6b7/feapder/commands/retry.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/shell.py` & `feapder-1.8.6b7/feapder/commands/shell.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/commands/zip.py` & `feapder-1.8.6b7/feapder/commands/zip.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/base_parser.py` & `feapder-1.8.6b7/feapder/core/base_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/collector.py` & `feapder-1.8.6b7/feapder/core/collector.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/handle_failed_items.py` & `feapder-1.8.6b7/feapder/core/handle_failed_items.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/handle_failed_requests.py` & `feapder-1.8.6b7/feapder/core/handle_failed_requests.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/parser_control.py` & `feapder-1.8.6b7/feapder/core/parser_control.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/scheduler.py` & `feapder-1.8.6b7/feapder/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/spiders/air_spider.py` & `feapder-1.8.6b7/feapder/core/spiders/air_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/spiders/batch_spider.py` & `feapder-1.8.6b7/feapder/core/spiders/batch_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/spiders/spider.py` & `feapder-1.8.6b7/feapder/core/spiders/spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/core/spiders/task_spider.py` & `feapder-1.8.6b7/feapder/core/spiders/task_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/db/memorydb.py` & `feapder-1.8.6b7/feapder/db/memorydb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/db/mongodb.py` & `feapder-1.8.6b7/feapder/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/db/mysqldb.py` & `feapder-1.8.6b7/feapder/db/mysqldb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/db/redisdb.py` & `feapder-1.8.6b7/feapder/db/redisdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,16 @@
             ip_ports = setting.REDISDB_IP_PORTS
         if db is None:
             db = setting.REDISDB_DB
         if user_pass is None:
             user_pass = setting.REDISDB_USER_PASS
         if service_name is None:
             service_name = setting.REDISDB_SERVICE_NAME
+        if kwargs is None:
+            kwargs = setting.REDISDB_KWARGS
 
         self._is_redis_cluster = False
 
         self.__redis = None
         self._url = url
         self._ip_ports = ip_ports
         self._db = db
@@ -176,15 +178,15 @@
                         decode_responses=self._decode_responses,
                         max_connections=self._max_connections,
                         **self._kwargs,
                     )
                     self._is_redis_cluster = False
             else:
                 self._redis = redis.StrictRedis.from_url(
-                    self._url, decode_responses=self._decode_responses
+                    self._url, decode_responses=self._decode_responses, **self._kwargs
                 )
                 self._is_redis_cluster = False
 
         except Exception as e:
             raise e
 
         # 不要写成self._redis.ping() 否则循环调用了
```

### Comparing `feapder-1.8.6b6/feapder/dedup/__init__.py` & `feapder-1.8.6b7/feapder/dedup/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/dedup/basefilter.py` & `feapder-1.8.6b7/feapder/dedup/basefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/dedup/bitarray.py` & `feapder-1.8.6b7/feapder/dedup/bitarray.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/dedup/bloomfilter.py` & `feapder-1.8.6b7/feapder/dedup/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/dedup/expirefilter.py` & `feapder-1.8.6b7/feapder/dedup/expirefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/dedup/litefilter.py` & `feapder-1.8.6b7/feapder/dedup/litefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/downloader/_playwright.py` & `feapder-1.8.6b7/feapder/network/downloader/_playwright.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/downloader/_requests.py` & `feapder-1.8.6b7/feapder/network/downloader/_requests.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/downloader/_selenium.py` & `feapder-1.8.6b7/feapder/network/downloader/_selenium.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/downloader/base.py` & `feapder-1.8.6b7/feapder/network/downloader/base.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/item.py` & `feapder-1.8.6b7/feapder/network/item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/proxy_pool.py` & `feapder-1.8.6b7/feapder/network/proxy_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/request.py` & `feapder-1.8.6b7/feapder/network/request.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/response.py` & `feapder-1.8.6b7/feapder/network/response.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/selector.py` & `feapder-1.8.6b7/feapder/network/selector.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/user_agent.py` & `feapder-1.8.6b7/feapder/network/user_agent.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/user_pool/base_user_pool.py` & `feapder-1.8.6b7/feapder/network/user_pool/base_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/user_pool/gold_user_pool.py` & `feapder-1.8.6b7/feapder/network/user_pool/gold_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/user_pool/guest_user_pool.py` & `feapder-1.8.6b7/feapder/network/user_pool/guest_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/network/user_pool/normal_user_pool.py` & `feapder-1.8.6b7/feapder/network/user_pool/normal_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/pipelines/__init__.py` & `feapder-1.8.6b7/feapder/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/pipelines/console_pipeline.py` & `feapder-1.8.6b7/feapder/pipelines/console_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/pipelines/mongo_pipeline.py` & `feapder-1.8.6b7/feapder/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/pipelines/mysql_pipeline.py` & `feapder-1.8.6b7/feapder/pipelines/mysql_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/setting.py` & `feapder-1.8.6b7/feapder/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 MONGO_USER_PASS = os.getenv("MONGO_USER_PASS")
 
 # REDIS
 # ip:port 多个可写为列表或者逗号隔开 如 ip1:port1,ip2:port2 或 ["ip1:port1", "ip2:port2"]
 REDISDB_IP_PORTS = os.getenv("REDISDB_IP_PORTS")
 REDISDB_USER_PASS = os.getenv("REDISDB_USER_PASS")
 REDISDB_DB = int(os.getenv("REDISDB_DB", 0))
+# 连接redis时携带的其他参数，如ssl=True
+REDISDB_KWARGS = dict()
 # 适用于redis哨兵模式
 REDISDB_SERVICE_NAME = os.getenv("REDISDB_SERVICE_NAME")
 
 # 数据入库的pipeline，可自定义，默认MysqlPipeline
 ITEM_PIPELINES = [
     "feapder.pipelines.mysql_pipeline.MysqlPipeline",
     # "feapder.pipelines.mongo_pipeline.MongoPipeline",
```

### Comparing `feapder-1.8.6b6/feapder/templates/.DS_Store` & `feapder-1.8.6b7/feapder/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/templates/air_spider_template.tmpl` & `feapder-1.8.6b7/feapder/templates/air_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/templates/batch_spider_template.tmpl` & `feapder-1.8.6b7/feapder/templates/batch_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/templates/project_template/.DS_Store` & `feapder-1.8.6b7/feapder/templates/project_template/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/templates/project_template/CHECK_DATA.md` & `feapder-1.8.6b7/feapder/templates/project_template/CHECK_DATA.md`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/templates/project_template/main.py` & `feapder-1.8.6b7/feapder/templates/project_template/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/templates/project_template/setting.py` & `feapder-1.8.6b7/feapder/templates/project_template/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # MONGO_USER_PASS = ""
 #
 # # REDIS
 # # ip:port 多个可写为列表或者逗号隔开 如 ip1:port1,ip2:port2 或 ["ip1:port1", "ip2:port2"]
 # REDISDB_IP_PORTS = "localhost:6379"
 # REDISDB_USER_PASS = ""
 # REDISDB_DB = 0
+# # 连接redis时携带的其他参数，如ssl=True
+# REDISDB_KWARGS = dict()
 # # 适用于redis哨兵模式
 # REDISDB_SERVICE_NAME = ""
 #
 # # 数据入库的pipeline，可自定义，默认MysqlPipeline
 # ITEM_PIPELINES = [
 #     "feapder.pipelines.mysql_pipeline.MysqlPipeline",
 #     # "feapder.pipelines.mongo_pipeline.MongoPipeline",
```

### Comparing `feapder-1.8.6b6/feapder/templates/spider_template.tmpl` & `feapder-1.8.6b7/feapder/templates/spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/templates/task_spider_template.tmpl` & `feapder-1.8.6b7/feapder/templates/task_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/custom_argparse.py` & `feapder-1.8.6b7/feapder/utils/custom_argparse.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/email_sender.py` & `feapder-1.8.6b7/feapder/utils/email_sender.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/js/intercept.js` & `feapder-1.8.6b7/feapder/utils/js/intercept.js`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/js/stealth.min.js` & `feapder-1.8.6b7/feapder/utils/js/stealth.min.js`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/log.py` & `feapder-1.8.6b7/feapder/utils/log.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/metrics.py` & `feapder-1.8.6b7/feapder/utils/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,27 @@
 
     def define_tagkv(self, tagk, tagvs):
         self.tagkv[tagk] = set(tagvs)
 
     def _point_tagset(self, p):
         return f"{p['measurement']}-{sorted(p['tags'].items())}-{p['time']}"
 
+    def _make_time_to_ns(self, _time):
+        """
+        将时间转换为 ns 级别的时间戳，补足长度 19 位
+        Args:
+            _time:
+
+        Returns:
+
+        """
+        time_len = len(str(_time))
+        random_str = "".join(random.sample(string.digits, 19 - time_len))
+        return int(str(_time) + random_str)
+
     def _accumulate_points(self, points):
         """
         对于处于同一个 key 的点做聚合
 
           - 对于 counter 类型，同一个 key 的值(_count)可以累加
           - 对于 store 类型，不做任何操作，influxdb 会自行覆盖
           - 对于 timer 类型，通过添加一个 _seq 值来区分每个不同的点
@@ -98,26 +111,26 @@
                 if self.max_timer_seq and timer_seqs[tagset] > self.max_timer_seq:
                     continue
                 # 掷一把骰子，如果足够幸运才打点
                 if self.ratio < 1.0 and random.random() > self.ratio:
                     continue
                 # 增加 _seq tag，以便区分不同的点
                 point["tags"]["_seq"] = timer_seqs[tagset]
+                point["time"] = self._make_time_to_ns(point["time"])
                 timer_seqs[tagset] += 1
                 new_points.append(point)
             else:
                 if self.ratio < 1.0 and random.random() > self.ratio:
                     continue
+                point["time"] = self._make_time_to_ns(point["time"])
                 new_points.append(point)
 
         for point in counters.values():
             # 修改下counter类型的点的时间戳，补足19位, 伪装成纳秒级时间戳，防止influxdb对同一秒内的数据进行覆盖
-            time_len = len(str(point["time"]))
-            random_str = "".join(random.sample(string.digits, 19 - time_len))
-            point["time"] = int(str(point["time"]) + random_str)
+            point["time"] = self._make_time_to_ns(point["time"])
             new_points.append(point)
 
             # 把拟合后的 counter 值添加进来
             new_points.append(point)
         return new_points
 
     def _get_ready_emit(self, force=False):
```

### Comparing `feapder-1.8.6b6/feapder/utils/perfect_dict.py` & `feapder-1.8.6b7/feapder/utils/perfect_dict.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/redis_lock.py` & `feapder-1.8.6b7/feapder/utils/redis_lock.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/tools.py` & `feapder-1.8.6b7/feapder/utils/tools.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/webdriver/playwright_driver.py` & `feapder-1.8.6b7/feapder/utils/webdriver/playwright_driver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/webdriver/selenium_driver.py` & `feapder-1.8.6b7/feapder/utils/webdriver/selenium_driver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/webdriver/webdirver.py` & `feapder-1.8.6b7/feapder/utils/webdriver/webdirver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder/utils/webdriver/webdriver_pool.py` & `feapder-1.8.6b7/feapder/utils/webdriver/webdriver_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/feapder.egg-info/PKG-INFO` & `feapder-1.8.6b7/feapder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feapder
-Version: 1.8.6b6
+Version: 1.8.6b7
 Summary: feapder是一款支持分布式、批次采集、任务防丢、报警丰富的python爬虫框架
 Home-page: https://github.com/Boris-code/feapder.git
 Author: Boris
 Author-email: feapder@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `feapder-1.8.6b6/feapder.egg-info/SOURCES.txt` & `feapder-1.8.6b7/feapder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 tests/test_spider_params.py
 tests/test_task.py
 tests/test_tools.py
 tests/test_webdriver.py
 tests/air-spider/test_air_spider.py
 tests/air-spider/test_air_spider_filter.py
 tests/air-spider/test_air_spider_item.py
+tests/air-spider/test_render_spider.py
 tests/batch-spider/main.py
 tests/batch-spider/setting.py
 tests/batch-spider/table.sql
 tests/batch-spider-integration/batch_spider_integration_task.sql
 tests/batch-spider-integration/main.py
 tests/batch-spider-integration/setting.py
 tests/batch-spider-integration/items/__init__.py
```

### Comparing `feapder-1.8.6b6/setup.py` & `feapder-1.8.6b7/setup.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/air-spider/test_air_spider.py` & `feapder-1.8.6b7/tests/air-spider/test_air_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/air-spider/test_air_spider_filter.py` & `feapder-1.8.6b7/tests/air-spider/test_air_spider_filter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/air-spider/test_air_spider_item.py` & `feapder-1.8.6b7/tests/air-spider/test_air_spider_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider/items/spider_data_item.py` & `feapder-1.8.6b7/tests/batch-spider/items/spider_data_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider/main.py` & `feapder-1.8.6b7/tests/batch-spider/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider/setting.py` & `feapder-1.8.6b7/tests/batch-spider/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider/spiders/test_spider.py` & `feapder-1.8.6b7/tests/batch-spider/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider/table.sql` & `feapder-1.8.6b7/tests/batch-spider/table.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider-integration/batch_spider_integration_task.sql` & `feapder-1.8.6b7/tests/batch-spider-integration/batch_spider_integration_task.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider-integration/main.py` & `feapder-1.8.6b7/tests/batch-spider-integration/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider-integration/setting.py` & `feapder-1.8.6b7/tests/batch-spider-integration/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider-integration/spiders/sina_news_parser.py` & `feapder-1.8.6b7/tests/batch-spider-integration/spiders/sina_news_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/batch-spider-integration/spiders/tencent_news_parser.py` & `feapder-1.8.6b7/tests/batch-spider-integration/spiders/tencent_news_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/jd_spider.py` & `feapder-1.8.6b7/tests/jd_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/mongo_spider.py` & `feapder-1.8.6b7/tests/mongo_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/spider/log/haha.log` & `feapder-1.8.6b7/tests/spider/log/haha.log`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/spider/setting.py` & `feapder-1.8.6b7/tests/spider/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/spider/spiders/test_spider.py` & `feapder-1.8.6b7/tests/spider/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/spider/spiders/test_spider2.py` & `feapder-1.8.6b7/tests/spider/spiders/test_spider2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/spider-integration/main.py` & `feapder-1.8.6b7/tests/spider-integration/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/spider-integration/setting.py` & `feapder-1.8.6b7/tests/spider-integration/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/task-spider/test_task_spider.py` & `feapder-1.8.6b7/tests/task-spider/test_task_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test-pipeline/items/spider_data_item.py` & `feapder-1.8.6b7/tests/test-pipeline/items/spider_data_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test-pipeline/main.py` & `feapder-1.8.6b7/tests/test-pipeline/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test-pipeline/pipeline.py` & `feapder-1.8.6b7/tests/test-pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test-pipeline/setting.py` & `feapder-1.8.6b7/tests/test-pipeline/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test-pipeline/spiders/test_spider.py` & `feapder-1.8.6b7/tests/test-pipeline/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test-pipeline/table.sql` & `feapder-1.8.6b7/tests/test-pipeline/table.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_dedup.py` & `feapder-1.8.6b7/tests/test_dedup.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_mongodb.py` & `feapder-1.8.6b7/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_playwright.py` & `feapder-1.8.6b7/tests/test_playwright.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_playwright2.py` & `feapder-1.8.6b7/tests/test_playwright2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_proxies_pool.py` & `feapder-1.8.6b7/tests/test_proxies_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_rander.py` & `feapder-1.8.6b7/tests/test_rander.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_rander2.py` & `feapder-1.8.6b7/tests/test_rander2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_rander3.py` & `feapder-1.8.6b7/tests/test_rander3.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_rander_xhr.py` & `feapder-1.8.6b7/tests/test_rander_xhr.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_request.py` & `feapder-1.8.6b7/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_spider_params.py` & `feapder-1.8.6b7/tests/test_spider_params.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_task.py` & `feapder-1.8.6b7/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_template/test_spider.py` & `feapder-1.8.6b7/tests/test_template/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/test_webdriver.py` & `feapder-1.8.6b7/tests/test_webdriver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/user_pool/test_gold_user_pool.py` & `feapder-1.8.6b7/tests/user_pool/test_gold_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/user_pool/test_guest_user_pool.py` & `feapder-1.8.6b7/tests/user_pool/test_guest_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.6b6/tests/user_pool/test_normal_user_pool.py` & `feapder-1.8.6b7/tests/user_pool/test_normal_user_pool.py`

 * *Files identical despite different names*

