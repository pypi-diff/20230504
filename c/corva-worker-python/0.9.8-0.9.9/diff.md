# Comparing `tmp/corva-worker-python-0.9.8.tar.gz` & `tmp/corva-worker-python-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corva-worker-python-0.9.8.tar", last modified: Mon Jul 19 18:09:47 2021, max compression
+gzip compressed data, was "corva-worker-python-0.9.9.tar", last modified: Wed Aug  4 19:55:51 2021, max compression
```

## Comparing `corva-worker-python-0.9.8.tar` & `corva-worker-python-0.9.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.360446 corva-worker-python-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2021-07-19 18:09:47.360446 corva-worker-python-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.352446 corva-worker-python-0.9.8/corva_worker_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2021-07-19 18:09:47.000000 corva-worker-python-0.9.8/corva_worker_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2021-07-19 18:09:47.000000 corva-worker-python-0.9.8/corva_worker_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-19 18:09:47.000000 corva-worker-python-0.9.8/corva_worker_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-07-19 18:09:47.000000 corva-worker-python-0.9.8/corva_worker_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-07-19 18:09:47.000000 corva-worker-python-0.9.8/corva_worker_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-07-19 18:09:47.360446 corva-worker-python-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      873 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.352446 corva-worker-python-0.9.8/testcase/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.352446 corva-worker-python-0.9.8/testcase/app/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/app/app_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/app/app_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/app/disable_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/app/drilling_efficiency_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     5408 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/app/surface_mse_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/run_lambda_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/run_local_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.352446 corva-worker-python-0.9.8/testcase/state_testing_app/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/state_testing_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/state_testing_app/app_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/state_testing_app/app_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)     6836 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/state_testing_app/state_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/state_testing_app/state_testing_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6411 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/test_activity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/test_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/test_lambda_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/test_rollbar_payload_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/test_state_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5245 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    33449 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/test_wellbore.py
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/testcase/test_wits.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.352446 corva-worker-python-0.9.8/worker/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.352446 corva-worker-python-0.9.8/worker/app/
--rw-r--r--   0 runner    (1001) docker     (121)    10695 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.356446 corva-worker-python-0.9.8/worker/app/modules/
--rw-r--r--   0 runner    (1001) docker     (121)     7459 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/app/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/app/modules/activity_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/app/modules/connection_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/app/modules/depth_activity_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/app/modules/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/app/modules/time_activity_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/app/modules/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.356446 corva-worker-python-0.9.8/worker/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.356446 corva-worker-python-0.9.8/worker/data/activity/
--rw-r--r--   0 runner    (1001) docker     (121)     5240 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/activity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8717 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/activity/activity_grouping.py
--rw-r--r--   0 runner    (1001) docker     (121)     2977 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/alert.py
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/math.py
--rw-r--r--   0 runner    (1001) docker     (121)    11792 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/task_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/two_way_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/unit_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11294 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/data/wits.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.356446 corva-worker-python-0.9.8/worker/event/
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3253 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/event/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/event/scheduled.py
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/event/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.356446 corva-worker-python-0.9.8/worker/framework/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/framework/timeout_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.356446 corva-worker-python-0.9.8/worker/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/mixins/rollbar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.356446 corva-worker-python-0.9.8/worker/state/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/state/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.356446 corva-worker-python-0.9.8/worker/state/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/state/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/state/handlers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/state/handlers/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     4244 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/state/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.360446 corva-worker-python-0.9.8/worker/test/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6772 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/test/lambda_function_test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.360446 corva-worker-python-0.9.8/worker/test/local_testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/test/local_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11951 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/test/local_testing/to_local_transfer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.360446 corva-worker-python-0.9.8/worker/wellbore/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14486 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/measured_depth_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:47.360446 corva-worker-python-0.9.8/worker/wellbore/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/ann.py
--rw-r--r--   0 runner    (1001) docker     (121)     3645 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/annulus.py
--rw-r--r--   0 runner    (1001) docker     (121)     6578 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/drillstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    14766 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/drillstring_components.py
--rw-r--r--   0 runner    (1001) docker     (121)     3191 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/element.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     9621 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/hole.py
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/hole_section.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/model/riser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/sections_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    11394 2021-07-19 18:09:45.000000 corva-worker-python-0.9.8/worker/wellbore/wellbore.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.172582 corva-worker-python-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2021-08-04 19:55:51.172582 corva-worker-python-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.164582 corva-worker-python-0.9.9/corva_worker_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2021-08-04 19:55:50.000000 corva-worker-python-0.9.9/corva_worker_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2021-08-04 19:55:51.000000 corva-worker-python-0.9.9/corva_worker_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-04 19:55:50.000000 corva-worker-python-0.9.9/corva_worker_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-08-04 19:55:50.000000 corva-worker-python-0.9.9/corva_worker_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-08-04 19:55:50.000000 corva-worker-python-0.9.9/corva_worker_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-08-04 19:55:51.172582 corva-worker-python-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      873 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.164582 corva-worker-python-0.9.9/testcase/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.164582 corva-worker-python-0.9.9/testcase/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/app/app_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/app/app_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/app/disable_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/app/drilling_efficiency_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5408 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/app/surface_mse_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/run_lambda_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/run_local_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.164582 corva-worker-python-0.9.9/testcase/state_testing_app/
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/state_testing_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/state_testing_app/app_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/state_testing_app/app_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6836 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/state_testing_app/state_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/state_testing_app/state_testing_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6411 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/test_activity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/test_lambda_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/test_rollbar_payload_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      857 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/test_state_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5245 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33449 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/test_wellbore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/testcase/test_wits.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.164582 corva-worker-python-0.9.9/worker/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.164582 corva-worker-python-0.9.9/worker/app/
+-rw-r--r--   0 runner    (1001) docker     (121)    10844 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.164582 corva-worker-python-0.9.9/worker/app/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)     7459 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/app/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5837 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/app/modules/activity_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/app/modules/connection_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/app/modules/depth_activity_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/app/modules/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/app/modules/time_activity_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/app/modules/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/data/activity/
+-rw-r--r--   0 runner    (1001) docker     (121)     5240 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/activity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8717 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/activity/activity_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2977 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/alert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2951 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/math.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11890 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3058 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3211 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/task_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/two_way_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/unit_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11294 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/data/wits.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/event/
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3253 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/event/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2356 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/event/scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/event/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/framework/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/framework/timeout_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3089 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/mixins/rollbar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/state/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/state/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/state/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/state/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4509 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/state/handlers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2949 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/state/handlers/redis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4244 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/state/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6772 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/test/lambda_function_test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/test/local_testing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/test/local_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11951 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/test/local_testing/to_local_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.168582 corva-worker-python-0.9.9/worker/wellbore/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14486 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/measured_depth_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:51.172582 corva-worker-python-0.9.9/worker/wellbore/model/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/ann.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3645 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/annulus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6578 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/drillstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14766 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/drillstring_components.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3191 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/element.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9621 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/hole.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1761 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/hole_section.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/model/riser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/sections_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11394 2021-08-04 19:55:45.000000 corva-worker-python-0.9.9/worker/wellbore/wellbore.py
```

### Comparing `corva-worker-python-0.9.8/PKG-INFO` & `corva-worker-python-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: corva-worker-python
-Version: 0.9.8
+Version: 0.9.9
 Summary: SDK for interacting with Corva
 Home-page: https://github.com/corva-ai/corva-worker-python
 Author: Jordan Ambra <jordan.ambra@corva.ai>, Mohammadreza Kamyab <m.kamyab@corva.ai>
 Author-email: UNKNOWN
 License: The Unlicense
 Description: UNKNOWN
 Keywords: corva,worker
```

### Comparing `corva-worker-python-0.9.8/README.md` & `corva-worker-python-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/corva_worker_python.egg-info/PKG-INFO` & `corva-worker-python-0.9.9/corva_worker_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: corva-worker-python
-Version: 0.9.8
+Version: 0.9.9
 Summary: SDK for interacting with Corva
 Home-page: https://github.com/corva-ai/corva-worker-python
 Author: Jordan Ambra <jordan.ambra@corva.ai>, Mohammadreza Kamyab <m.kamyab@corva.ai>
 Author-email: UNKNOWN
 License: The Unlicense
 Description: UNKNOWN
 Keywords: corva,worker
```

### Comparing `corva-worker-python-0.9.8/corva_worker_python.egg-info/SOURCES.txt` & `corva-worker-python-0.9.9/corva_worker_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/setup.py` & `corva-worker-python-0.9.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'Topic :: Software Development :: Libraries',
 ]
 
 setup(
     name='corva-worker-python',
     author='Jordan Ambra <jordan.ambra@corva.ai>, Mohammadreza Kamyab <m.kamyab@corva.ai>',
     url='https://github.com/corva-ai/corva-worker-python',
-    version='0.9.8',
+    version='0.9.9',
     classifiers=classifiers,
     description='SDK for interacting with Corva',
     keywords='corva, worker',
     packages=find_packages(exclude=["test"]),
     install_requires=["numpy", "redis", "requests", "cached-property"],
     include_package_data=True,
     license='The Unlicense',
```

### Comparing `corva-worker-python-0.9.8/testcase/app/surface_mse_module.py` & `corva-worker-python-0.9.9/testcase/app/surface_mse_module.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/run_lambda_app.py` & `corva-worker-python-0.9.9/testcase/run_lambda_app.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/run_local_testing.py` & `corva-worker-python-0.9.9/testcase/run_local_testing.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/state_testing_app/app_constants.py` & `corva-worker-python-0.9.9/testcase/state_testing_app/app_constants.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/state_testing_app/app_lambda.py` & `corva-worker-python-0.9.9/testcase/state_testing_app/app_lambda.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/state_testing_app/state_modules.py` & `corva-worker-python-0.9.9/testcase/state_testing_app/state_modules.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/test_activity.py` & `corva-worker-python-0.9.9/testcase/test_activity.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/test_events.py` & `corva-worker-python-0.9.9/testcase/test_events.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/test_lambda_app.py` & `corva-worker-python-0.9.9/testcase/test_lambda_app.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/test_rollbar_payload_handler.py` & `corva-worker-python-0.9.9/testcase/test_rollbar_payload_handler.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/test_state_mixin.py` & `corva-worker-python-0.9.9/testcase/test_state_mixin.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/test_utils.py` & `corva-worker-python-0.9.9/testcase/test_utils.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/test_wellbore.py` & `corva-worker-python-0.9.9/testcase/test_wellbore.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/testcase/test_wits.py` & `corva-worker-python-0.9.9/testcase/test_wits.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/app/__init__.py` & `corva-worker-python-0.9.9/worker/app/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,17 @@
         end_timestamp = event[-1].start_time
 
         # the event is converted from scheduler to wits stream
         scheduler_event = gather_data_for_period(
             asset_id=asset_id,
             start=start_timestamp - max_lookback_seconds,
             end=end_timestamp,
-            limit=constants.get('global.query-limit'))
+            limit=constants.get('global.query-limit'),
+            fields=constants.get('global.wits_query_fields', None)
+        )
 
         return scheduler_event
 
     def load_wits_stream_event(self, asset_id: int, event: StreamEvent, max_lookback_seconds: int) -> List[dict]:
         """
         To load a wits stream event and get more data if necessary
         :param asset_id: The asset to load
@@ -198,15 +200,16 @@
             # Subtract one from the timestamp so that we don't reselect the final data item that was sent in the event
             end_timestamp = first_timestamp - 1
 
             previous_events = gather_data_for_period(
                 asset_id=asset_id,
                 start=first_timestamp - max_lookback_seconds,
                 end=end_timestamp,
-                limit=constants.get('global.query-limit')
+                limit=constants.get('global.query-limit'),
+                fields=constants.get('global.wits_query_fields', None)
             )
 
             records = previous_events + records
 
         return records
 
     @staticmethod
```

### Comparing `corva-worker-python-0.9.8/worker/app/modules/__init__.py` & `corva-worker-python-0.9.9/worker/app/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/app/modules/activity_module.py` & `corva-worker-python-0.9.9/worker/app/modules/activity_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,23 +75,23 @@
         if not data:
             return []
 
         first_wits = data[0]
         drillstring_id = first_wits.get('metadata', {}).get('drillstring', None)
         casing_id = first_wits.get('metadata', {}).get('casing', None)
 
-        if not drillstring_id and not casing_id:
-            return []
-
         if drillstring_id:
             active_string_type = 'drillstring'
             active_string_id = drillstring_id
         elif casing_id:
             active_string_type = 'casing'
             active_string_id = casing_id
+        else:
+            active_string_type = None
+            active_string_id = None
 
         if previous_string == active_string_id:
             return []
 
         asset_id = self.global_state['asset_id']
         main_structure = self.build_empty_output(first_wits)
```

### Comparing `corva-worker-python-0.9.8/worker/app/modules/connection_module.py` & `corva-worker-python-0.9.9/worker/app/modules/connection_module.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/app/modules/depth_activity_module.py` & `corva-worker-python-0.9.9/worker/app/modules/depth_activity_module.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/app/modules/scheduler.py` & `corva-worker-python-0.9.9/worker/app/modules/scheduler.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/app/modules/time_activity_module.py` & `corva-worker-python-0.9.9/worker/app/modules/time_activity_module.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/app/modules/trigger.py` & `corva-worker-python-0.9.9/worker/app/modules/trigger.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/activity/__init__.py` & `corva-worker-python-0.9.9/worker/data/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/activity/activity_grouping.py` & `corva-worker-python-0.9.9/worker/data/activity/activity_grouping.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/alert.py` & `corva-worker-python-0.9.9/worker/data/alert.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/api.py` & `corva-worker-python-0.9.9/worker/data/api.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/enums.py` & `corva-worker-python-0.9.9/worker/data/enums.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/json_encoder.py` & `corva-worker-python-0.9.9/worker/data/json_encoder.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/math.py` & `corva-worker-python-0.9.9/worker/data/math.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/operations.py` & `corva-worker-python-0.9.9/worker/data/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,37 @@
 from worker.data import math
 from worker.data.api import API
 from worker.data.enums import EventTypes, Environment
 from worker.data.wits import WITS
 from worker.exceptions import NotFound
 
 
-def gather_data_for_period(asset_id: int, start: int, end: int, limit: int = 1800, collection: str = "wits") -> list:
+def gather_data_for_period(
+        asset_id: int, start: int, end: int, limit: int = 1800,
+        collection: str = "wits", fields: str = None
+) -> list:
     """
     Get the wits data from API for an asset over an interval
     :param asset_id: asset id
     :param start: start timestamp
     :param end: end timestamp
     :param limit: count of the data
     :param collection: any collection
+    :param fields: fields to be filtered
     :return: a list of wits data
     """
     if start >= end:
         return []
 
     query = '{timestamp#gte#%s}AND{timestamp#lte#%s}' % (start, end)
     worker = API()
+
     wits_dataset = worker.get(
-        path="/v1/data/corva", collection=collection, asset_id=asset_id, sort="{timestamp: 1}", limit=limit, query=query
-    ).data
+        path="/v1/data/corva", collection=collection, asset_id=asset_id, sort="{timestamp: 1}", limit=limit,
+        query=query, fields=fields).data
 
     if not wits_dataset:
         return []
 
     return wits_dataset
```

### Comparing `corva-worker-python-0.9.8/worker/data/serialization.py` & `corva-worker-python-0.9.9/worker/data/serialization.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/task_handler.py` & `corva-worker-python-0.9.9/worker/data/task_handler.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/two_way_dict.py` & `corva-worker-python-0.9.9/worker/data/two_way_dict.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/data/wits.py` & `corva-worker-python-0.9.9/worker/data/wits.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/event/__init__.py` & `corva-worker-python-0.9.9/worker/event/__init__.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/event/event_handler.py` & `corva-worker-python-0.9.9/worker/event/event_handler.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/event/scheduled.py` & `corva-worker-python-0.9.9/worker/event/scheduled.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/event/stream.py` & `corva-worker-python-0.9.9/worker/event/stream.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/framework/constants.py` & `corva-worker-python-0.9.9/worker/framework/constants.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/framework/timeout_handler.py` & `corva-worker-python-0.9.9/worker/framework/timeout_handler.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/mixins/logging.py` & `corva-worker-python-0.9.9/worker/mixins/logging.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/mixins/rollbar.py` & `corva-worker-python-0.9.9/worker/mixins/rollbar.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/state/handlers/__init__.py` & `corva-worker-python-0.9.9/worker/state/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/state/handlers/mongo.py` & `corva-worker-python-0.9.9/worker/state/handlers/mongo.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/state/handlers/redis.py` & `corva-worker-python-0.9.9/worker/state/handlers/redis.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/state/mixins.py` & `corva-worker-python-0.9.9/worker/state/mixins.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/state/state.py` & `corva-worker-python-0.9.9/worker/state/state.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/test/lambda_function_test_run.py` & `corva-worker-python-0.9.9/worker/test/lambda_function_test_run.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/test/local_testing/to_local_transfer.py` & `corva-worker-python-0.9.9/worker/test/local_testing/to_local_transfer.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/test/utils.py` & `corva-worker-python-0.9.9/worker/test/utils.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/factory.py` & `corva-worker-python-0.9.9/worker/wellbore/factory.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/ann.py` & `corva-worker-python-0.9.9/worker/wellbore/model/ann.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/annulus.py` & `corva-worker-python-0.9.9/worker/wellbore/model/annulus.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/drillstring.py` & `corva-worker-python-0.9.9/worker/wellbore/model/drillstring.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/drillstring_components.py` & `corva-worker-python-0.9.9/worker/wellbore/model/drillstring_components.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/element.py` & `corva-worker-python-0.9.9/worker/wellbore/model/element.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/enums.py` & `corva-worker-python-0.9.9/worker/wellbore/model/enums.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/hole.py` & `corva-worker-python-0.9.9/worker/wellbore/model/hole.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/hole_section.py` & `corva-worker-python-0.9.9/worker/wellbore/model/hole_section.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/model/riser.py` & `corva-worker-python-0.9.9/worker/wellbore/model/riser.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/sections_mixin.py` & `corva-worker-python-0.9.9/worker/wellbore/sections_mixin.py`

 * *Files identical despite different names*

### Comparing `corva-worker-python-0.9.8/worker/wellbore/wellbore.py` & `corva-worker-python-0.9.9/worker/wellbore/wellbore.py`

 * *Files identical despite different names*

