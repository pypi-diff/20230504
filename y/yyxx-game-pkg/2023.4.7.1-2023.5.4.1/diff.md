# Comparing `tmp/yyxx_game_pkg-2023.4.7.1.tar.gz` & `tmp/yyxx_game_pkg-2023.5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg-2023.4.7.1.tar", max compression
+gzip compressed data, was "yyxx_game_pkg-2023.5.4.1.tar", max compression
```

## Comparing `yyxx_game_pkg-2023.4.7.1.tar` & `yyxx_game_pkg-2023.5.4.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     3888 2023-04-07 09:03:02.119412 yyxx_game_pkg-2023.4.7.1/README.md
--rw-r--r--   0        0        0     1122 2023-04-07 09:03:12.419337 yyxx_game_pkg-2023.4.7.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/__init__.py
--rw-r--r--   0        0        0       83 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/dbops/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/dbops/mysql_op.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      676 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      522 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/helpers/test_mysql_helper.py
--rw-r--r--   0        0        0      455 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      481 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0       83 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1295 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5597 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      979 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/mongo_op.py
--rw-r--r--   0        0        0     3955 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2099 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     1266 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2667 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-04-07 09:03:02.123412 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0     3467 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1530 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0      378 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/common/log.py
--rw-r--r--   0        0        0       69 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4418 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      693 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4286 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0      961 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0       83 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5035 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     2845 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3016 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     5255 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     6161 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     3101 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0       69 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     2858 2023-04-07 09:03:02.191409 yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.4.7.1/PKG-INFO
+-rw-r--r--   0        0        0     3888 2023-05-04 04:10:07.938087 yyxx_game_pkg-2023.5.4.1/README.md
+-rw-r--r--   0        0        0     1170 2023-05-04 04:10:20.550173 yyxx_game_pkg-2023.5.4.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1295 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     5597 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0      979 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mongo_op.py
+-rw-r--r--   0        0        0     3955 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2408 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     1266 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2850 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-05-04 04:10:08.018087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-05-04 04:10:08.018087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2326 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0     3467 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     2154 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      667 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      987 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2206 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0     1183 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0       83 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     5652 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     2845 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     6099 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     6161 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     3091 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0       69 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     2858 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     5505 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.5.4.1/PKG-INFO
```

### Comparing `yyxx_game_pkg-2023.4.7.1/README.md` & `yyxx_game_pkg-2023.5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/pyproject.toml` & `yyxx_game_pkg-2023.5.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 equires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yyxx-game-pkg"
-version = "v2023.04.07.001"
+version = "v2023.05.04.001"
 description = "yyxx game custom module"
 authors = [ "yyxx-game",]
 license = "MIT"
 homepage = "https://github.com/yyxxgame/yyxxgame-pkg"
 repository = "https://github.com/yyxxgame/yyxxgame-pkg"
 readme = "README.md"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
@@ -34,7 +34,8 @@
 opentelemetry-instrumentation-fastapi = "0.37b.0"
 pika = "^1.3.1"
 pymysql = "^1.0.2"
 dbutils = "^3.0.2"
 opentelemetry-instrumentation-celery = "0.37b0"
 ujson = "^5.7.0"
 pandas = "^1.5.3"
+opentelemetry-instrumentation-django = "0.37b0"
```

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/dbops/mysql_op.py` & `yyxx_game_pkg-2023.5.4.1/tests/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/__init__.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg-2023.5.4.1/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/helpers/test_mysql_helper.py` & `yyxx_game_pkg-2023.5.4.1/tests/helpers/test_mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/submit/test_submit.py` & `yyxx_game_pkg-2023.5.4.1/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/test_logger.py` & `yyxx_game_pkg-2023.5.4.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/test_xtrace.py` & `yyxx_game_pkg-2023.5.4.1/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/tests/xcelery/task_register.py` & `yyxx_game_pkg-2023.5.4.1/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/ch_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/das_api.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/mongo_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mongo_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/mysql_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,55 +2,60 @@
 """
 @File: mysql_helper.py
 @Author: ltw
 @Time: 2023/3/22
 """
 import pymysql
 from dbutils.pooled_db import PooledDB
-from yyxx_game_pkg.utils.decorator import except_monitor, log_execute_time_monitor, singleton_unique
+from yyxx_game_pkg.utils.decorator import except_monitor, log_execute_time_monitor, singleton_unique_obj_args
 from yyxx_game_pkg.logger.log import root_log
 
 
 # #################### 模块对外接口 ####################
 def get_dbpool(config: dict):
     class Config(MysqlConfig):
         HOST = config["host"]
         PORT = config["port"]
         USER = config["user"]
         PASSWD = config["password"]
         DB = config["db"]
-        USE_UNICODE = config.get("use_unicode", False)
+        USE_UNICODE = config.get("use_unicode", True)
         CHARSET = config.get("charset", "utf8")
+        MAX_CACHED = config.get("maxcached", 0)
+        MAX_CONNECTIONS = config.get("maxconnections", 0)
 
     return MysqlDbPool(Config())
 
 
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
+            self.HOST, self.PORT, self.DB, self.USE_UNICODE, self.CHARSET, self.MAX_CACHED, self.MAX_CONNECTIONS
         )
 
 
-@singleton_unique
+@singleton_unique_obj_args
 class MysqlDbPool(object):
 
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
```

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 @File: redis_helper
 @Author: ltw
 @Time: 2023/3/9
 """
 import redis
-from yyxx_game_pkg.utils.decorator import singleton_unique
+from yyxx_game_pkg.utils.decorator import singleton_unique_obj_args
 
 
 def get_redis(config: dict):
     """
     缓存redis
     :return:
     """
@@ -35,16 +35,21 @@
 
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
```

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/logger/log.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/common.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/instance.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/decorator.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xListStr.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xdataframe.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdataframe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @File: xdataframe
 @Author: ltw
 @Time: 2022/8/4
 """
+import functools
 import json
 from bisect import bisect_left
 import pandas as pd
 import numpy as np
 
 
 def empty_df(columns=None):
@@ -79,53 +80,65 @@
             _bins.insert(0, 0)
         return _bins
 
     bins = prefix_bins(bins)
     return _df[key].apply(cut_bins, bins=bins)
 
 
-def cal_round_rate(data, precision=2, suffix="%"):
+def cal_round_rate(data, precision=2, suffix="%", invalid_value="-"):
     """
     :param data:
     :param precision:
     :param suffix:
+    :param invalid_value:
     :return:
     """
     if isinstance(data, pd.DataFrame):
         return data.apply(cal_round_rate, args=(precision, suffix), axis=0)
     if isinstance(data, pd.Series):
-        return data.round(precision).apply(
-            lambda d: "-" if (d == np.inf or np.isnan(d)) else f"{d}{suffix}"
-        )
+        if str(invalid_value).isdigit():
+            data = data.fillna(invalid_value)
+        if precision == 0:
+            data = data.astype(int)
+        else:
+            data = data.astype(float).round(precision)
+        return data.apply(lambda d: invalid_value if (d == np.inf or np.isnan(d)) else f"{d}{suffix}")
     if isinstance(data, (int, float)):
-        return str(round(data, 2)) + suffix
-    return "-"
+        if np.isnan(data) or data == np.inf:
+            return invalid_value
+        if precision == 0:
+            return str(int(data)) + suffix
+        return str(round(data, precision)) + suffix
+    return invalid_value
 
 
 def func_cal_round_rate(func, **kw):
     """
     用于快速构造用agg或apply传递的cal_round_rate函数
     :param func:
     :param kw:
     :return:
     """
 
+    @functools.wraps(func)
     def wrapper(data, *args, **kwargs):
         if isinstance(func, str):
             data = getattr(data, func)()
         else:
             data = func(data)
         return cal_round_rate(data, **kw)
 
     return wrapper
 
 
 def dict_to_json(data):
     """用于es对象转json,并且正常显示中文"""
     if not data:
+        if not isinstance(data, (str, bytes)):
+            data = str(data)
         return data
     if isinstance(data, float) and pd.isna(data):
         return ""
     return json.dumps(data, ensure_ascii=False)
 
 
 def df_json_normalize(_df, columns, prefixes=None, sep=".", column_prefix=False):
@@ -133,15 +146,17 @@
     df: 原df数据
     record_paths: 需要解析的列名list
     record_prefixes: 需要填充前缀list
     sep: 填充前缀的分隔符
     column_prefix: 使用字段名作为前缀
     """
     for idx, record_column in enumerate(columns):
-        tmp_df = pd.DataFrame(_df[record_column].tolist())
+        if record_column not in _df.columns:
+            continue
+        tmp_df = pd.DataFrame(_df[record_column].apply(fill_dict).tolist())
         record_prefix = None
         if column_prefix:
             record_prefix = record_column
         elif prefixes is not None:
             record_prefix = prefixes[idx]
         if record_prefix:
             tmp_df.columns = [f"{record_prefix}{sep}{col}" for col in tmp_df.columns]
@@ -193,7 +208,17 @@
         if rm_columns:
             _df = _df.drop(rm_columns)
     else:
         rm_columns = [column for column in columns if column in _df.columns]
         if rm_columns:
             _df = _df.drop(columns=rm_columns)
     return _df
+
+
+def fill_dict(data):
+    """填充{}到nan"""
+    return {} if not isinstance(data, dict) and pd.isna(data) else data
+
+
+def fill_list(data):
+    """填充[]到nan"""
+    return [] if not isinstance(data, list) and pd.isna(data) else data
```

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdate.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xhttp.py`

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

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.4.7.1/PKG-INFO` & `yyxx_game_pkg-2023.5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yyxx-game-pkg
-Version: 2023.4.7.1
+Version: 2023.5.4.1
 Summary: yyxx game custom module
 Home-page: https://github.com/yyxxgame/yyxxgame-pkg
 License: MIT
 Author: yyxx-game
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Requires-Dist: celery (>=5.2.7,<6.0.0)
 Requires-Dist: dbutils (>=3.0.2,<4.0.0)
 Requires-Dist: fastapi (>=0.94.0,<0.95.0)
 Requires-Dist: line-profiler (>=4.0.3,<5.0.0)
 Requires-Dist: opentelemetry-api (>=1.16.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-jaeger (>=1.16.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-celery (==0.37b0)
+Requires-Dist: opentelemetry-instrumentation-django (==0.37b0)
 Requires-Dist: opentelemetry-instrumentation-fastapi (==0.37b.0)
 Requires-Dist: opentelemetry-instrumentation-requests (>=0.37b0,<0.38)
 Requires-Dist: opentelemetry-sdk (>=1.16.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: pymysql (>=1.0.2,<2.0.0)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.4.7.1 Summary: yyxx
+Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.5.4.1 Summary: yyxx
 game custom module Home-page: https://github.com/yyxxgame/yyxxgame-pkg License:
 MIT Author: yyxx-game Requires-Python: >=3.8,<4 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
 Requires-Dist: celery (>=5.2.7,<6.0.0) Requires-Dist: dbutils (>=3.0.2,<4.0.0)
 Requires-Dist: fastapi (>=0.94.0,<0.95.0) Requires-Dist: line-profiler
 (>=4.0.3,<5.0.0) Requires-Dist: opentelemetry-api (>=1.16.0,<2.0.0) Requires-
 Dist: opentelemetry-exporter-jaeger (>=1.16.0,<2.0.0) Requires-Dist:
 opentelemetry-instrumentation-celery (==0.37b0) Requires-Dist: opentelemetry-
-instrumentation-fastapi (==0.37b.0) Requires-Dist: opentelemetry-
-instrumentation-requests (>=0.37b0,<0.38) Requires-Dist: opentelemetry-sdk
-(>=1.16.0,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: pika
-(>=1.3.1,<2.0.0) Requires-Dist: pymysql (>=1.0.2,<2.0.0) Requires-Dist: redis
-(>=4.5.1,<5.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: toml
-(>=0.10.2,<0.11.0) Requires-Dist: ujson (>=5.7.0,<6.0.0) Requires-Dist: uvicorn
-(>=0.21.0,<0.22.0) Project-URL: Repository, https://github.com/yyxxgame/
-yyxxgame-pkg Description-Content-Type: text/markdown # YYXXGAME-PKG `yyxx-game-
-pkg` æ¯ä¸ä¸ªä¸é¨ä¸ºåæ¸¸å¬å¸åå°å¼åç Python åé¨æ¥å£éåã
-[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![MIT License][license-shield]][license-url]
+instrumentation-django (==0.37b0) Requires-Dist: opentelemetry-instrumentation-
+fastapi (==0.37b.0) Requires-Dist: opentelemetry-instrumentation-requests
+(>=0.37b0,<0.38) Requires-Dist: opentelemetry-sdk (>=1.16.0,<2.0.0) Requires-
+Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: pika (>=1.3.1,<2.0.0) Requires-
+Dist: pymysql (>=1.0.2,<2.0.0) Requires-Dist: redis (>=4.5.1,<5.0.0) Requires-
+Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: ujson (>=5.7.0,<6.0.0) Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
+Project-URL: Repository, https://github.com/yyxxgame/yyxxgame-pkg Description-
+Content-Type: text/markdown # YYXXGAME-PKG `yyxx-game-pkg`
+æ¯ä¸ä¸ªä¸é¨ä¸ºåæ¸¸å¬å¸åå°å¼åç Python åé¨æ¥å£éåã  [!
+[Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
+[forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
+[issues-url] [![MIT License][license-shield]][license-url]
                                 [åæ¸¸ä¿¡æ¯]
                             **** åæ¸¸ä¿¡æ¯ ****
 ## ç®å½ - [ä¸ææå](#ä¸ææå) - [ç¯å¢éç½®](#ç¯å¢éç½®) -
 [å®è£æ­¥éª¤](#å®è£æ­¥éª¤) - [æä»¶ç®å½è¯´æ](#æä»¶ç®å½è¯´æ) -
 [é¨ç½²](#é¨ç½²) - [develop](#develop) - [release](#release) - [æ¨¡åä»ç»]
 (#æ¨¡åä»ç») - [xtrace](#xtrace) - [stat](#stat) - [ä»£ç ç¤ºä¾]
 (#ä»£ç ç¤ºä¾) - [çæ¬æ§å¶](#çæ¬æ§å¶) ### ä¸ææå ######
```

