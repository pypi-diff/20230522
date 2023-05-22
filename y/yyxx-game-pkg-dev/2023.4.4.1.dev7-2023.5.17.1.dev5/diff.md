# Comparing `tmp/yyxx_game_pkg_dev-2023.4.4.1.dev7.tar.gz` & `tmp/yyxx_game_pkg_dev-2023.5.17.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg_dev-2023.4.4.1.dev7.tar", max compression
+gzip compressed data, was "yyxx_game_pkg_dev-2023.5.17.1.dev5.tar", max compression
```

## Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7.tar` & `yyxx_game_pkg_dev-2023.5.17.1.dev5.tar`

### file list

```diff
@@ -1,86 +1,114 @@
--rw-r--r--   0        0        0     3888 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/README.md
--rw-r--r--   0        0        0     1130 2023-04-06 09:31:49.181752 yyxx_game_pkg_dev-2023.4.4.1.dev7/pyproject.toml
--rw-r--r--   0        0        0       68 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      676 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/helpers/__init__.py
--rw-r--r--   0        0        0      439 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      468 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0       83 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1295 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5597 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      979 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/mongo_op.py
--rw-r--r--   0        0        0     4086 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2099 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     1266 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2667 2023-04-06 09:31:37.425043 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-04-06 09:31:37.429044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0     3467 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1530 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0      378 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/common/log.py
--rw-r--r--   0        0        0       69 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4418 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      693 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4286 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0      961 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0       83 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5035 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     2845 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3016 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     5255 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     6161 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     3101 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0       69 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     2858 2023-04-06 09:31:37.501044 yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     5451 1970-01-01 00:00:00.000000 yyxx_game_pkg_dev-2023.4.4.1.dev7/PKG-INFO
+-rw-r--r--   0        0        0     4895 2023-05-22 01:43:16.075163 yyxx_game_pkg_dev-2023.5.17.1.dev5/README.md
+-rw-r--r--   0        0        0     1799 2023-05-22 01:43:31.907184 yyxx_game_pkg_dev-2023.5.17.1.dev5/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/__init__.py
+-rw-r--r--   0        0        0     5089 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/Operator.py
+-rw-r--r--   0        0        0     1505 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/OperatorServer.py
+-rw-r--r--   0        0        0     2572 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/RechargeConfig.py
+-rw-r--r--   0        0        0     2600 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/TableFieldConf.py
+-rw-r--r--   0        0        0      125 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/__init__.py
+-rw-r--r--   0        0        0     4379 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/check_token.py
+-rw-r--r--   0        0        0     5887 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/map_core.py
+-rw-r--r--   0        0        0     2957 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/recharge.py
+-rw-r--r--   0        0        0     6895 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/conf/__init__.py
+-rw-r--r--   0        0        0     2054 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/conf/global_settings.py
+-rw-r--r--   0        0        0      129 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/aes.py
+-rw-r--r--   0        0        0     1114 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/basic.py
+-rw-r--r--   0        0        0     1312 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/make_sign.py
+-rw-r--r--   0        0        0     2653 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/rsa.py
+-rw-r--r--   0        0        0       83 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1295 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     5597 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0      979 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/mongo_op.py
+-rw-r--r--   0        0        0     3955 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2512 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     2959 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/op_helper.py
+-rw-r--r--   0        0        0     1266 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2966 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2326 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0     3467 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     2154 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      667 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      987 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2206 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0     1183 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0      427 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/cookiecutter.json
+-rw-r--r--   0        0        0     3410 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
+-rw-r--r--   0        0        0      624 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
+-rw-r--r--   0        0        0     4208 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
+-rw-r--r--   0        0        0       83 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     5652 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     3136 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/error_code.py
+-rw-r--r--   0        0        0     2845 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     8255 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     6238 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     3091 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0      574 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xstring.py
+-rw-r--r--   0        0        0       69 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     2858 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 yyxx_game_pkg_dev-2023.5.17.1.dev5/PKG-INFO
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/README.md` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -62,14 +62,47 @@
 3.配置虚拟环境并激活
 ```shell
 - poetry env use python3
 - poetry env list
 - poetry shell
 ```
 
+4.添加包
+
+关于`poetry`的使用，参考文档：[http://yydocs.yyxxgame.com/web/#/183/1758](http://yydocs.yyxxgame.com/web/#/183/1758)
+
+```shell
+- poetry add numpy  # 基本使用
+- poetry add numpy --optional  # 添加额外包（针对项目单独使用的包）
+```
+> 如果使用`--optional`，需要手动修改`pyproject.toml`文件
+>   - 1.在`[tool.poetry.extras]`增加相应`extra`分组和包
+>   - 2.命令行`poetry lock`更新`poetry.lock`文件
+>   - 3.命令行`poetry install -E center_api`安装`optional`中的包
+
+```toml
+# example
+[tool.poetry.extras]
+center_api = ["flask", "numpy"]
+stat = ["pandas", "numpy"]
+```
+
+5.安装依赖
+```shell
+# 开发 yyxxgame-pkg 安装依赖
+# 安装基础依赖，以及额外center_api依赖
+- poetry install -E stat
+- poetry install -E stat -E center_api  # 安装多个额外依赖
+- poetry install --extras "stat center_api"
+
+# 项目中使用 yyxxgame-pkg 安装依赖
+- poetry add yyxx-game-pkg[stat]
+- pip install yyxx-game-pkg[stat]
+```
+
 ### 文件目录说明
 ```
 yyxxgame-pkg 
 ├── README.md
 ├── gen_version.py
 ├── images
 │   └── logo.png
```

#### html2text {}

```diff
@@ -11,28 +11,42 @@
 (#æ¨¡åä»ç») - [xtrace](#xtrace) - [stat](#stat) - [ä»£ç ç¤ºä¾]
 (#ä»£ç ç¤ºä¾) - [çæ¬æ§å¶](#çæ¬æ§å¶) ### ä¸ææå ######
 ç¯å¢éç½® 1.ç¯å¢å®è£python3.11ä»¥ä¸çæ¬ ###### å®è£æ­¥éª¤
 1.Cloneä»£ç  ```shell git clone https://github.com/yyxxgame/yyxxgame-pkg.git
 ``` 2.å®è£poetry ```shell - curl -sSL https://install.python-poetry.org |
 python3 - export PATH="/root/.local/bin:$PATH" ```
 3.éç½®èæç¯å¢å¹¶æ¿æ´» ```shell - poetry env use python3 - poetry env
-list - poetry shell ``` ### æä»¶ç®å½è¯´æ ``` yyxxgame-pkg âââ
-README.md âââ gen_version.py âââ images âÂ Â  âââ logo.png
-âââ poetry.lock âââ pyproject.toml âââ tests âÂ Â 
-âââ __init__.py âÂ Â  âââ dispatch âÂ Â  âââ submit
-âÂ Â  âââ test_ip2region.py âÂ Â  âââ test_logger.py âÂ Â 
-âââ test_xtrace.py âÂ Â  âââ utils âÂ Â  âââ xcelery
-âââ yyxx_game_pkg âââ __init__.py âââ helpers âââ
-ip2region âââ logger âââ stat âââ utils âââ xtrace ```
-### é¨ç½² ###### develop æäº¤æ³¨éä¸­æ·»å `
-[BUILD]`å³é®å­å¹¶æ¨éä¼è§¦ågithub actionsçdevçæ¬æå»ºå¹¶åå¸å°
-[yyxx-game-pkg-dev](https://pypi.org/project/yyxx-game-pkg-dev/) ###### release
-æ°å»º`tag`å¹¶æ¨éä¼è§¦ågithub actionsçæ­£å¼çæ¬æå»ºå¹¶åå¸å°
-[yyxx-game-pkg](https://pypi.org/project/yyxx-game-pkg/) ### æ¨¡åä»ç»
-yyxxgame-pkgåå«ä»¥ä¸æ¨¡åï¼ ###### xtrace `xtrace`
+list - poetry shell ``` 4.æ·»å å å³äº`poetry`çä½¿ç¨ï¼åèææ¡£ï¼
+[http://yydocs.yyxxgame.com/web/#/183/1758](http://yydocs.yyxxgame.com/web/#/
+183/1758) ```shell - poetry add numpy # åºæ¬ä½¿ç¨ - poetry add numpy --
+optional # æ·»å é¢å¤åï¼éå¯¹é¡¹ç®åç¬ä½¿ç¨çåï¼ ``` >
+å¦æä½¿ç¨`--optional`ï¼éè¦æå¨ä¿®æ¹`pyproject.toml`æä»¶ > - 1.å¨`
+[tool.poetry.extras]`å¢å ç¸åº`extra`åç»åå > - 2.å½ä»¤è¡`poetry
+lock`æ´æ°`poetry.lock`æä»¶ > - 3.å½ä»¤è¡`poetry install -
+E center_api`å®è£`optional`ä¸­çå ```toml # example [tool.poetry.extras]
+center_api = ["flask", "numpy"] stat = ["pandas", "numpy"] ``` 5.å®è£ä¾èµ
+```shell # å¼å yyxxgame-pkg å®è£ä¾èµ #
+å®è£åºç¡ä¾èµï¼ä»¥åé¢å¤center_apiä¾èµ - poetry install -E stat -
+poetry install -E stat -E center_api # å®è£å¤ä¸ªé¢å¤ä¾èµ - poetry
+install --extras "stat center_api" # é¡¹ç®ä¸­ä½¿ç¨ yyxxgame-pkg å®è£ä¾èµ
+- poetry add yyxx-game-pkg[stat] - pip install yyxx-game-pkg[stat] ``` ###
+æä»¶ç®å½è¯´æ ``` yyxxgame-pkg âââ README.md âââ
+gen_version.py âââ images âÂ Â  âââ logo.png âââ
+poetry.lock âââ pyproject.toml âââ tests âÂ Â  âââ
+__init__.py âÂ Â  âââ dispatch âÂ Â  âââ submit âÂ Â 
+âââ test_ip2region.py âÂ Â  âââ test_logger.py âÂ Â  âââ
+test_xtrace.py âÂ Â  âââ utils âÂ Â  âââ xcelery âââ
+yyxx_game_pkg âââ __init__.py âââ helpers âââ ip2region
+âââ logger âââ stat âââ utils âââ xtrace ``` ### é¨ç½²
+###### develop æäº¤æ³¨éä¸­æ·»å `[BUILD]`å³é®å­å¹¶æ¨éä¼è§¦ågithub
+actionsçdevçæ¬æå»ºå¹¶åå¸å°[yyxx-game-pkg-dev](https://pypi.org/
+project/yyxx-game-pkg-dev/) ###### release æ°å»º`tag`å¹¶æ¨éä¼è§¦ågithub
+actionsçæ­£å¼çæ¬æå»ºå¹¶åå¸å°[yyxx-game-pkg](https://pypi.org/
+project/yyxx-game-pkg/) ### æ¨¡åä»ç» yyxxgame-pkgåå«ä»¥ä¸æ¨¡åï¼
+###### xtrace `xtrace`
 æ¨¡åå°è£äºé¾è·¯è¿½è¸ªçå¸®å©ç±»ï¼å¯ä»¥å¸®å©å¼åäººåå¿«éå°å®ç°é¾è·¯è¿½è¸ªåè½ã
 ###### stat
 `stat`æ¨¡ååå«yyxxgameåé¨ç»è®¡ä¸å¡çåºå±æ¡æ¶ï¼ç®ååå«`dispatch`ã`submit`ã`xceleryå ä¸ªæ¨¡å`
 ### ä»£ç ç¤ºä¾ åè[test](https://github.com/yyxxgame/yyxxgame-pkg/tree/
 master/tests) ä¸­çè°ç¨ä¾å­ ### çæ¬æ§å¶
 è¯¥é¡¹ç®ä½¿ç¨Gitè¿è¡çæ¬ç®¡çãæ¨å¯ä»¥å¨repositoryåçå½åå¯ç¨çæ¬ã
 [your-project-path]:yyxxgame/yyxxgame-pkg [contributors-shield]: https://
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/rules/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # @Author   : KaiShin
 # @Time     : 2023/3/14
 
 import os
 import importlib
 from os.path import dirname
-from yyxx_game_pkg.stat.dispatch.common.log import local_log
+from yyxx_game_pkg.stat.log import local_log
 
 
 def rules_auto_import():
     pkg_dir = dirname(__file__)
     files = os.listdir(pkg_dir)
     for idx, filepath in enumerate(files):
         if filepath.startswith("__init__"):
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/submit/test_submit.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/test_logger.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/test_xtrace.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/tests/xcelery/task_register.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/ch_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/das_api.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/mongo_op.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/mongo_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,65 +18,56 @@
         """
         执行sql返回处理结果
         :param sql:
         :param conn:
         :param params:
         :return:
         """
-        # todo with statement ltw
-        # with connection:
-        #     with connection.cursor() as cursor:
-        #         # Read a single record
-        #         sql = f"""
-        #             SELECT id, create_time, name
-        #             FROM svr_server
-        #             WHERE is_pull = 1
-        #             AND id = {sid}
-        #             ORDER BY game_addr
-        #         """
-        #         cursor.execute(sql)
-        #         cursor.fetchall()
-        cursor = conn.cursor()
-        if params is None:
-            cursor.execute(sql)
-        else:
-            cursor.execute(sql, params)
-        return conn.submit()
+        sql = self.check_sql(sql)
+        with conn:
+            with conn.cursor() as cursor:
+                if params is None:
+                    cursor.execute(sql)
+                else:
+                    cursor.execute(sql, params)
+                conn.commit()
 
     def get_one(self, sql, conn, params=None):
         """
         查询一条数据, 返回元组结构
         :param sql:
         :param conn:
         :param params:
         :return:
         """
-        cursor = conn.cursor()
         sql = self.check_sql(sql)
-        if params is None:
-            cursor.execute(sql)
-        else:
-            cursor.execute(sql, params)
-        return cursor.fetchone()
+        with conn:
+            with conn.cursor() as cursor:
+                if params is None:
+                    cursor.execute(sql)
+                else:
+                    cursor.execute(sql, params)
+                return cursor.fetchone()
 
     def get_all(self, sql, conn, params=None):
         """
         查询多条数据，返回list(元组) 结构
         :param sql:
         :param conn:
         :param params:
         :return:
         """
-        cursor = conn.cursor()
         sql = self.check_sql(sql)
-        if params is None:
-            cursor.execute(sql)
-        else:
-            cursor.execute(sql, params)
-        return cursor.fetchall()
+        with conn:
+            with conn.cursor() as cursor:
+                if params is None:
+                    cursor.execute(sql)
+                else:
+                    cursor.execute(sql, params)
+                return cursor.fetchall()
 
     def get_one_df(self, *args, **kwargs):
         """
         获取单次数据
         :param args:
         :param kwargs:
         :return:
@@ -94,54 +85,54 @@
     def insert(self, conn, save_table, results):
         """
         :param conn:
         :param save_table:
         :param results:
         :return:
         """
-        cursor = conn.cursor()
-
         def get_field_str(_data):
             """
             根据数据长度生成{data_value}
             :param _data:
             :return:
             """
             _size = len(_data[0])
             _list = []
             for _ in range(_size):
                 _list.append("%s")
             _str = ",".join(_list)
             return _str
 
-        def get_table_desc(_table_name, _data_list):
+        def get_table_desc(_table_name, _data_list, _cs):
             """
             :param _table_name:
             :param _data_list:
             :return:
             """
             sql = f"describe {_table_name}"
-            cursor.execute(sql)
-            _desc = cursor.fetchall()
+            _cs.execute(sql)
+            _desc = _cs.fetchall()
             _column = []
             for _data in _desc:
                 if _data[0] in ("id", "create_time"):  # 自增id和默认插入时间过滤
                     continue
                 _column.append(_data[0])
             _size = len(_data_list[0])
             table_column = _column[:_size]
             return ",".join(table_column)
 
         insert_sql_template = (
             "INSERT INTO {save_table} ({column_value}) VALUES({data_value})"
         )
         results = xListStr.split_list(results)
-        for result in results:
-            if not result:
-                continue
-            field_str = get_field_str(result)
-            column_value = get_table_desc(save_table, result)
-            insert_sql = insert_sql_template.format(
-                save_table=save_table, column_value=column_value, data_value=field_str
-            )
-            cursor.executemany(insert_sql, result)
-            conn.commit()
+        with conn:
+            with conn.cursor() as cursor:
+                for result in results:
+                    if not result:
+                        continue
+                    field_str = get_field_str(result)
+                    column_value = get_table_desc(save_table, result, cursor)
+                    insert_sql = insert_sql_template.format(
+                        save_table=save_table, column_value=column_value, data_value=field_str
+                    )
+                    cursor.executemany(insert_sql, result)
+                    conn.commit()
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/mysql_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,55 +2,53 @@
 """
 @File: mysql_helper.py
 @Author: ltw
 @Time: 2023/3/22
 """
 import pymysql
 from dbutils.pooled_db import PooledDB
-from yyxx_game_pkg.utils.decorator import except_monitor, log_execute_time_monitor, singleton_unique
+from yyxx_game_pkg.utils.decorator import (
+    except_monitor,
+    log_execute_time_monitor,
+    singleton_unique_obj_args,
+)
 from yyxx_game_pkg.logger.log import root_log
 
 
-# #################### 模块对外接口 ####################
-def get_dbpool(config: dict):
-    class Config(MysqlConfig):
-        HOST = config["host"]
-        PORT = config["port"]
-        USER = config["user"]
-        PASSWD = config["password"]
-        DB = config["db"]
-        USE_UNICODE = config.get("use_unicode", False)
-        CHARSET = config.get("charset", "utf8")
-
-    return MysqlDbPool(Config())
-
-
 # ####################################################
 class MysqlConfig:
     HOST = None
     PORT = None
     USER = None
     PASSWD = None
     DB = None
     USE_UNICODE = None
     CHARSET = None
+    MAX_CACHED = None
+    MAX_CONNECTIONS = None
 
     def __str__(self):
-        return "host:{},port:{},db:{},use_unicode:{},charset:{}".format(
-            self.HOST, self.PORT, self.DB, self.USE_UNICODE, self.CHARSET
+        return "host:{},port:{},db:{},use_unicode:{},charset:{},max_cache:{},max_connections:{}".format(
+            self.HOST,
+            self.PORT,
+            self.DB,
+            self.USE_UNICODE,
+            self.CHARSET,
+            self.MAX_CACHED,
+            self.MAX_CONNECTIONS,
         )
 
 
-@singleton_unique
+@singleton_unique_obj_args
 class MysqlDbPool(object):
-
     def __init__(self, config: MysqlConfig):
         self.DB_POOL = PooledDB(
             creator=pymysql,
-            maxcached=10,
+            maxcached=config.MAX_CACHED,
+            maxconnections=config.MAX_CONNECTIONS,
             host=config.HOST,
             port=config.PORT,
             user=config.USER,
             passwd=config.PASSWD,
             db=config.DB,
             use_unicode=config.USE_UNICODE,
             charset=config.CHARSET,
@@ -65,7 +63,23 @@
     def close_connection(self):
         """
         关闭线程池,线程池最少占用1连接,100个进程跑1000个相同IP库的服时,最多会生成10W连接，所以需要关闭线程池，释放全部连接。
         优化点：以后可以相同IP的服务器共用1个线程池（现阶段sql查game库没有指定库名,改动地方多,搁置）
         :return:
         """
         self.DB_POOL.close()
+
+
+# #################### 模块对外接口 ####################
+def get_dbpool(config: dict) -> MysqlDbPool:
+    class Config(MysqlConfig):
+        HOST = config["host"]
+        PORT = config["port"]
+        USER = config["user"]
+        PASSWD = config["password"]
+        DB = config["db"]
+        USE_UNICODE = config.get("use_unicode", True)
+        CHARSET = config.get("charset", "utf8")
+        MAX_CACHED = config.get("maxcached", 0)
+        MAX_CONNECTIONS = config.get("maxconnections", 0)
+
+    return MysqlDbPool(Config())
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,43 @@
 # -*- coding: utf-8 -*-
 """
 @File: redis_helper
 @Author: ltw
 @Time: 2023/3/9
 """
 import redis
-from yyxx_game_pkg.utils.decorator import singleton_unique
-
-
-def get_redis(config: dict):
-    """
-    缓存redis
-    :return:
-    """
-
-    class Config(RedisConfig):
-        """
-        redis config
-        """
-
-        HOST = config["host"]
-        PORT = config["port"]
-        DB = config["db"]
-        PASSWORD = config["password"]
-        OVERDUE_SECOND = config.get("overdue_second", 86400)
-
-    return RedisHelper(Config())
+from yyxx_game_pkg.logger.log import root_log
+from yyxx_game_pkg.utils.decorator import singleton_unique_obj_args
 
 
 class RedisConfig:
     """
     redis config
     """
 
     HOST = None
     PORT = None
     DB = None
     PASSWORD = None
     OVERDUE_SECOND = 86400
 
+    def __str__(self):
+        return "host:{}, port:{}, db:{}, OVERDUE_SECOND:{}".format(
+            self.HOST, self.PORT, self.DB, self.OVERDUE_SECOND
+        )
+
 
-@singleton_unique
+@singleton_unique_obj_args
 class RedisHelper:
     def __init__(self, config: RedisConfig):
         connection_pool = redis.ConnectionPool(
             host=config.HOST, port=config.PORT, db=config.DB, password=config.PASSWORD
         )
         self.__r = redis.Redis(connection_pool=connection_pool)
+        root_log(f"<RedisHelper> init, info:{config}")
 
     @property
     def redis_cli(self):
         return self.__r
 
     def get_data(self, key):
         return self.__r.get(key)
@@ -114,7 +101,27 @@
         分片获取元素
         :param key:
         :param start:
         :param end:
         :return:
         """
         return self.__r.lrange(key, start, end)
+
+
+def get_redis(config: dict) -> RedisHelper:
+    """
+    缓存redis
+    :return:
+    """
+
+    class Config(RedisConfig):
+        """
+        redis config
+        """
+
+        HOST = config["host"]
+        PORT = config["port"]
+        DB = config["db"]
+        PASSWORD = config["password"]
+        OVERDUE_SECOND = config.get("overdue_second", 86400)
+
+    return RedisHelper(Config())
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/logger/log.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/common/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # @Author   : KaiShin
 # @Time     : 2023/3/14
 import functools
 
 from fastapi.exceptions import HTTPException
 
-from yyxx_game_pkg.stat.dispatch.common.log import local_log
+from yyxx_game_pkg.stat.log import local_log
 from yyxx_game_pkg.xtrace.helper import get_current_trace_id, add_span_events
 
 
 def split_list(target_list, list_per_len):
     """
     把target_list分割成若干个小list（连续切割）
     :param target_list: [1,2,3]
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Author   : KaiShin
 # @Time     : 2023/3/9
 import traceback
 
 from yyxx_game_pkg.stat.dispatch.common.common import fastapi_except_monitor
-from yyxx_game_pkg.stat.dispatch.common.log import local_log
+from yyxx_game_pkg.stat.log import local_log
 from yyxx_game_pkg.stat.dispatch.core.manager import RuleManager
 from yyxx_game_pkg.stat.dispatch.core.structs import ProtoSchedule
 from yyxx_game_pkg.stat.dispatch.core.workflows import WorkFlowMethods
 
 
 # region logic入口
 from yyxx_game_pkg.xtrace.helper import get_current_trace_id
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Author   : KaiShin
 # @Time     : 2023/3/13
 import os
 import importlib
 from os.path import dirname
-from yyxx_game_pkg.stat.dispatch.common.log import local_log
+from yyxx_game_pkg.stat.log import local_log
 
 
 def rules_auto_import():
     pkg_dir = dirname(__file__)
     files = os.listdir(pkg_dir)
     for idx, filepath in enumerate(files):
         if filepath.startswith("__init__"):
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # @Author   : KaiShin
 # @Time     : 2023/3/14
-from yyxx_game_pkg.stat.dispatch.common.log import local_log
+from yyxx_game_pkg.stat.log import local_log
 from yyxx_game_pkg.stat.dispatch.core.manager import rule_register
 from yyxx_game_pkg.stat.dispatch.core.workflows import WorkFlowMethods
 from yyxx_game_pkg.stat.dispatch.logic.task_logic import parse_task
 from yyxx_game_pkg.stat.dispatch.rules.rule_base import RuleBase
 
 
 @rule_register(inst_name_list=["work_flow_instance"])
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
         conf_jaeger = _app.conf.get("JAEGER")
         if conf_jaeger:
             from opentelemetry.instrumentation.celery import CeleryInstrumentor
             from opentelemetry.instrumentation.requests import RequestsInstrumentor
             from yyxx_game_pkg.xtrace.helper import register_to_jaeger
 
+            if celery_name:
+                conf_jaeger["service_name"] += f"-{celery_name}"
+
             register_to_jaeger(**conf_jaeger)
             CeleryInstrumentor().instrument()
             RequestsInstrumentor().instrument()
             root_log(f"<CeleryInstance> tracer on, jaeger:{conf_jaeger}")
 
         log_str = (
             f"<CeleryInstance> get_celery_instance, app_name:{celery_name}, config:{_app.conf}, publish_flag:"
@@ -51,14 +54,15 @@
     @staticmethod
     def get_current_task_id():
         """
         当前task id [如果有]
         :return:
         """
         from celery import current_task
+
         try:
             return current_task.request.id
         except:
             return -1
 
     # endregion
 
@@ -71,14 +75,15 @@
         -c 配置文件
         :return:
         """
         parser = argparse.ArgumentParser(allow_abbrev=False)
         parser.add_argument("-n", "--name")
         args = parser.parse_known_args()
         return args[0]
+
     # endregion
 
 
 # region celery实例化
 """
 app.conf.get('worker_max_tasks_per_child', 0)
 """
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 # -*- coding: utf-8 -*-
 """
 @File: decorator
 @Author: ltw
 @Time: 2022/8/4
 """
+import functools
+import pickle
+import random
 import time
 import traceback
-import random
-import pickle
-import functools
 from concurrent import futures
+
 from yyxx_game_pkg.logger.log import root_log
+from yyxx_game_pkg.xtrace.helper import get_current_trace_id
 
 
 def fix_str(obj, max_len=5000):
     """
-    切割过长str, 避免打印过多无用信息 
+    切割过长str, 避免打印过多无用信息
     """
     msg = str(obj)
-    return msg[0: min(len(msg), max_len)]
+    return msg[0 : min(len(msg), max_len)]
 
 
 def log_execute_time_monitor(exec_lmt_time=20):
     """
     超时函数监控
     :param exec_lmt_time:秒
     :return:
     """
 
     def decorator(func):
+        @functools.wraps(func)
         def inner(*args, **kwargs):
-
             begin_dt = time.time()
             res = func(*args, **kwargs)
             end_dt = time.time()
             offset = end_dt - begin_dt
             if offset >= exec_lmt_time:
                 ex_info = None
                 if kwargs.get("connection") is not None:
                     ex_info = kwargs.get("connection")._con._kwargs.get("host")
                 _args = []
                 for _arg in args:
                     _args.append(fix_str(_arg, 100))
                 for k, _v in kwargs.items():
                     kwargs[k] = fix_str(_v, 100)
+                trace_id = get_current_trace_id()
                 root_log(
-                    f"<log_execute_time_monitor>func <<{func.__name__}>> deal over time "
+                    f"<log_execute_time_monitor> trace_id: {trace_id} "
+                    f"func <<{func.__name__}>> deal over time "
                     f"begin_at: {begin_dt} end_at: {end_dt}, sec: {offset}"
                     f"ex_info{ex_info}, params: {str(args)}, {str(kwargs)}"
                 )
             return res
 
         return inner
 
@@ -70,16 +74,17 @@
             res = func(*args, **kwargs)
         except Exception as e:
             _args = []
             for _arg in args:
                 _args.append(fix_str(_arg, 100))
             for k, _v in kwargs.items():
                 kwargs[k] = fix_str(_v, 100)
+            trace_id = get_current_trace_id()
             root_log(
-                f"<except_monitor> "
+                f"<except_monitor> trace_id: {trace_id} "
                 f"func:{func.__module__}.{func.__name__}, args:{str(_args)}, kwargs:{str(kwargs)}, "
                 f"exc: {traceback.format_exc()} {e}"
             )
         return res
 
     return inner
 
@@ -114,27 +119,40 @@
             instances[cls] = cls(*args, **kw)
         return instances[cls]
 
     return get_instance
 
 
 def singleton_unique(cls):
-
     instances = {}
 
     @functools.wraps(cls)
     def get_instance(*args, **kw):
         unique_key = f"{cls}_{args}_{kw}"
         if unique_key not in instances:
             instances[unique_key] = cls(*args, **kw)
         return instances[unique_key]
 
     return get_instance
 
 
+def singleton_unique_obj_args(cls):
+    # object 需重写 __str__
+    instances = {}
+
+    @functools.wraps(cls)
+    def get_instance(*args, **kw):
+        unique_key = f"{cls}_{list(map(str, args))}_{kw}"
+        if unique_key not in instances:
+            instances[unique_key] = cls(*args, **kw)
+        return instances[unique_key]
+
+    return get_instance
+
+
 def timeout_run(timeout=2, default=None):
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kw):
             try:
                 executor = futures.ThreadPoolExecutor(1)
                 future = executor.submit(func, *args, **kw)
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xListStr.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     :param split_size:
     :return:
     """
     if not isinstance(pending_lst, (list, tuple)):
         return pending_lst
     if not isinstance(pending_lst[0], (list, tuple)):
         pending_lst = [pending_lst]
+    if split_size == -1:
+        return pending_lst
     base_num = split_size
     result = pending_lst[0]
     size = len(result) / base_num
     if len(result) % base_num != 0:
         size += 1
     data_list = []
     for index in range(int(size)):
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xdate.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,14 +113,17 @@
     :param end: 0: 00:00:00 / 1: 23:59:59
     :return:
     """
     if end:
         return date2dt_day_end(date) + datetime.timedelta(days=delta)
     return date2dt_day(date) + datetime.timedelta(days=delta)
 
+def add_days(date, delta, end=0):
+    return delta_dt_day(date, delta, end)
+
 
 def date2stamp(dt_date):
     """
     datetime转时间戳
     """
     return time.mktime(dt_date.timetuple())
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xhttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,22 +71,22 @@
         elif isinstance(_v, dict):
             params_list.append((k, json.dumps(_v)))
         else:
             params_list.append((k, _v))
     return urllib.parse.urlencode(params_list)
 
 
-def http_push_server(url, data):
+def http_push_server(url, data, server_api_key):
     """
     单服推送
     :param url:
     :param data:
+    :param server_api_key:
     :return:
     """
-    server_api_key = current_app.conf.SERVER_API_KEY
     if not url:
         local_log(f"Error http_push_server url: {url}  data: {json.dumps(data)}")
         return None
 
     _t = int(time.time())
     values = {"time": _t, "params": json.dumps(data)}
     keys = values.keys()
```

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.4.4.1.dev7/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/xtrace/helper.py`

 * *Files identical despite different names*

