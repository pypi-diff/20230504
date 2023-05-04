# Comparing `tmp/cylc-flow-8.1.3.tar.gz` & `tmp/cylc-flow-8.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc-flow-8.1.3.tar", last modified: Fri Apr 28 11:30:58 2023, max compression
+gzip compressed data, was "cylc-flow-8.1.4.tar", last modified: Thu May  4 12:38:02 2023, max compression
```

## Comparing `cylc-flow-8.1.3.tar` & `cylc-flow-8.1.4.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.411959 cylc-flow-8.1.3/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.423959 cylc-flow-8.1.3/cylc/flow/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/async_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/broadcast_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/broadcast_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/c3mro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.423959 cylc-flow-8.1.3/cylc/flow/cfgspec/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cfgspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cfgspec/glbl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    71511 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cfgspec/globalcfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    83023 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cfgspec/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/command_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    97151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/context_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.423959 cylc-flow-8.1.3/cylc/flow/cycling/
--rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34957 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cylc_subproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22194 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/data_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    89336 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/data_store_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/dbstatecheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.423959 cylc-flow-8.1.3/cylc/flow/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     7934 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/cylc
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/cylc-completion.bash
--rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/job.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc-mode.el
--rw-r--r--   0 runner    (1001) docker     (123)    25186 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.lang
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.vim
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/api-keys
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.411959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.415959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/forecast
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/inheritance-tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/map-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/map-template/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.415959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/message-trigger-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/retries-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/retries-tutorial/.validate
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.415959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/runtime
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/
--rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/flow_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    35572 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/graphnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/host_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/hostuserutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/id.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/id_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/id_match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/install_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/install_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/install_plugins/log_vc_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.415959 cylc-flow-8.1.3/cylc/flow/jinja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/jinja/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/jinja/filters/duration_as.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/jinja/filters/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/jinja/filters/strftime.py
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/background.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/loadleveler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/moab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/slurm_packjob.py
--rw-r--r--   0 runner    (1001) docker     (123)    33912 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/listify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/log_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/loggingutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/main_loop/
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/auto_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/log_data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/log_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/log_main_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/log_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/reset_bad_hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/network/
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/authorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    74542 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/ssh_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    28587 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/option_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/param_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.435959 cylc-flow-8.1.3/cylc/flow/parsec/
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/OrderedDict.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/empysupport.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/fileparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/include.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/jinja2support.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/pathutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    25192 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/prerequisite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/print_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    39289 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/rundb.py
--rw-r--r--   0 runner    (1001) docker     (123)    80364 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scheduler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc/flow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15346 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/broadcast.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19658 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/cat_log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5028 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/check_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2617 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/completion_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6429 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8931 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/cycle_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/cylc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6042 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8083 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/ext_trigger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/function_run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2514 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/get_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1871 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/get_workflow_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2311 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/get_workflow_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4378 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10639 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/install.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/jobs_kill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/jobs_poll.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/jobs_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2483 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/kill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24919 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/lint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6228 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6419 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/pause.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3955 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/play.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/psutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/reinstall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3711 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/release.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3254 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/reload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/remote_init.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1533 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/remote_tidy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13206 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/report_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/scan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3504 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/set_outputs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/set_verbosity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12679 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/show.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8360 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/stop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/subscribe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5272 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/tui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6321 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/validate_install_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/validate_reinstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10001 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/subprocctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    23404 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/subprocpool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_action_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    63362 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_events_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55110 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_job_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80010 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    18451 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc/flow/task_queues/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_queues/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_remote_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    25327 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_remote_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_state_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/taskdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/templatevars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc/flow/tui/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/unicode_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/wallclock.py
--rw-r--r--   0 runner    (1001) docker     (123)    33592 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/workflow_db_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/workflow_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    69723 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/workflow_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/workflow_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtrigger_mgr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc/flow/xtriggers/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/wall_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/xrandom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc_flow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-28 11:30:58.443959 cylc-flow-8.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.202397 cylc-flow-8.1.4/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.222397 cylc-flow-8.1.4/cylc/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/async_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/broadcast_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/broadcast_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/c3mro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.222397 cylc-flow-8.1.4/cylc/flow/cfgspec/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cfgspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cfgspec/glbl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71511 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cfgspec/globalcfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83023 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cfgspec/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/command_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/context_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.222397 cylc-flow-8.1.4/cylc/flow/cycling/
+-rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34957 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cylc_subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22194 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/data_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89336 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/data_store_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/dbstatecheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7934 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/cylc
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/cylc-completion.bash
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/job.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc-mode.el
+-rw-r--r--   0 runner    (1001) docker     (123)    25186 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.lang
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.vim
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/api-keys
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/forecast
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/inheritance-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/map-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/map-template/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/message-trigger-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/retries-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/retries-tutorial/.validate
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/runtime
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/flow_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35572 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/graphnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/host_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/hostuserutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/id_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/id_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/install_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/install_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/install_plugins/log_vc_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/jinja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/jinja/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/jinja/filters/duration_as.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/jinja/filters/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/jinja/filters/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.238397 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/loadleveler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/slurm_packjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33912 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/listify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/log_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/loggingutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.238397 cylc-flow-8.1.4/cylc/flow/main_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/auto_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/log_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/log_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/log_main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/log_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/reset_bad_hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.242397 cylc-flow-8.1.4/cylc/flow/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74542 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/ssh_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28587 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/option_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/param_expand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.242397 cylc-flow-8.1.4/cylc/flow/parsec/
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/OrderedDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/empysupport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/fileparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/jinja2support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/pathutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25192 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/prerequisite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/print_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39289 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80364 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scheduler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.250397 cylc-flow-8.1.4/cylc/flow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15346 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/broadcast.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20637 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/cat_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5028 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/check_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2617 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/completion_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6429 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8931 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/cycle_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/cylc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6042 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8083 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/ext_trigger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/function_run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2514 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/get_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1871 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/get_workflow_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2311 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/get_workflow_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4378 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10639 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/jobs_kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/jobs_poll.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/jobs_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2483 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24919 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/lint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6228 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6419 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/pause.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3955 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/play.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/reinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3711 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/release.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3254 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/reload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/remote_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1533 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/remote_tidy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13206 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/report_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3504 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/set_outputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/set_verbosity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12679 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/show.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8360 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/stop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/subscribe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5272 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/tui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6321 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/validate_install_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/validate_reinstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10001 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/subprocctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23404 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/subprocpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_action_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63362 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_events_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55110 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_job_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80010 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18451 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.250397 cylc-flow-8.1.4/cylc/flow/task_queues/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_queues/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_remote_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25375 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_remote_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_state_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/taskdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/templatevars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/cylc/flow/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/unicode_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/wallclock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33592 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/workflow_db_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/workflow_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69723 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/workflow_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/workflow_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtrigger_mgr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/cylc/flow/xtriggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/wall_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/xrandom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/cylc_flow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/setup.py
```

### Comparing `cylc-flow-8.1.3/COPYING` & `cylc-flow-8.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/PKG-INFO` & `cylc-flow-8.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.1.3
+Version: 8.1.4
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
```

### Comparing `cylc-flow-8.1.3/README.md` & `cylc-flow-8.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/__init__.py` & `cylc-flow-8.1.4/cylc/flow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # running pre-5.0 cylc via the posix nohup command; is it still the
     # case in post-5.0 daemon-mode cylc?)
     os.environ['PYTHONUNBUFFERED'] = 'true'
 
 
 environ_init()
 
-__version__ = '8.1.3'
+__version__ = '8.1.4'
 
 
 def iter_entry_points(entry_point_name):
     """Iterate over Cylc entry points."""
     import pkg_resources
     yield from (
         entry_point
```

### Comparing `cylc-flow-8.1.3/cylc/flow/async_util.py` & `cylc-flow-8.1.4/cylc/flow/async_util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/broadcast_mgr.py` & `cylc-flow-8.1.4/cylc/flow/broadcast_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/broadcast_report.py` & `cylc-flow-8.1.4/cylc/flow/broadcast_report.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/c3mro.py` & `cylc-flow-8.1.4/cylc/flow/c3mro.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cfgspec/__init__.py` & `cylc-flow-8.1.4/cylc/flow/cfgspec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cfgspec/glbl_cfg.py` & `cylc-flow-8.1.4/cylc/flow/cfgspec/glbl_cfg.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cfgspec/globalcfg.py` & `cylc-flow-8.1.4/cylc/flow/cfgspec/globalcfg.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cfgspec/workflow.py` & `cylc-flow-8.1.4/cylc/flow/cfgspec/workflow.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/command_polling.py` & `cylc-flow-8.1.4/cylc/flow/command_polling.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/config.py` & `cylc-flow-8.1.4/cylc/flow/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/context_node.py` & `cylc-flow-8.1.4/cylc/flow/context_node.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cycling/__init__.py` & `cylc-flow-8.1.4/cylc/flow/cycling/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cycling/integer.py` & `cylc-flow-8.1.4/cylc/flow/cycling/integer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cycling/iso8601.py` & `cylc-flow-8.1.4/cylc/flow/cycling/iso8601.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cycling/loader.py` & `cylc-flow-8.1.4/cylc/flow/cycling/loader.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cycling/util.py` & `cylc-flow-8.1.4/cylc/flow/cycling/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/cylc_subproc.py` & `cylc-flow-8.1.4/cylc/flow/cylc_subproc.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/daemonize.py` & `cylc-flow-8.1.4/cylc/flow/daemonize.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/data_messages_pb2.py` & `cylc-flow-8.1.4/cylc/flow/data_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/data_store_mgr.py` & `cylc-flow-8.1.4/cylc/flow/data_store_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/dbstatecheck.py` & `cylc-flow-8.1.4/cylc/flow/dbstatecheck.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/cylc` & `cylc-flow-8.1.4/cylc/flow/etc/cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/cylc-completion.bash` & `cylc-flow-8.1.4/cylc/flow/etc/cylc-completion.bash`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/job.sh` & `cylc-flow-8.1.4/cylc/flow/etc/job.sh`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc-mode.el` & `cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc-mode.el`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.lang` & `cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.lang`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.vim` & `cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.vim`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.xml` & `cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.xml`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/.validate` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/forecast` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/util.py` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/map-template/map-template.html` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/map-template/map-template.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/retries-tutorial/.validate` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/retries-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/.validate` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/runtime` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/runtime`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/rainfall.csv` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv` & `cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/exceptions.py` & `cylc-flow-8.1.4/cylc/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/flags.py` & `cylc-flow-8.1.4/cylc/flow/flags.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/flow_mgr.py` & `cylc-flow-8.1.4/cylc/flow/flow_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/graph_parser.py` & `cylc-flow-8.1.4/cylc/flow/graph_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/graphnode.py` & `cylc-flow-8.1.4/cylc/flow/graphnode.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/host_select.py` & `cylc-flow-8.1.4/cylc/flow/host_select.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/hostuserutil.py` & `cylc-flow-8.1.4/cylc/flow/hostuserutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/id.py` & `cylc-flow-8.1.4/cylc/flow/id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/id_cli.py` & `cylc-flow-8.1.4/cylc/flow/id_cli.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/id_match.py` & `cylc-flow-8.1.4/cylc/flow/id_match.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/install_plugins/__init__.py` & `cylc-flow-8.1.4/cylc/flow/install_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/install_plugins/log_vc_info.py` & `cylc-flow-8.1.4/cylc/flow/install_plugins/log_vc_info.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/jinja/filters/duration_as.py` & `cylc-flow-8.1.4/cylc/flow/jinja/filters/duration_as.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/jinja/filters/pad.py` & `cylc-flow-8.1.4/cylc/flow/jinja/filters/pad.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/jinja/filters/strftime.py` & `cylc-flow-8.1.4/cylc/flow/jinja/filters/strftime.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_file.py` & `cylc-flow-8.1.4/cylc/flow/job_file.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/__init__.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/at.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/at.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/background.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/background.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/documentation.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/documentation.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/loadleveler.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/loadleveler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/lsf.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/lsf.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/moab.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/moab.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/pbs.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/pbs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/pbs_multi_cluster.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/pbs_multi_cluster.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/sge.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/sge.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/slurm.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/slurm.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/slurm_packjob.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/slurm_packjob.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/job_runner_mgr.py` & `cylc-flow-8.1.4/cylc/flow/job_runner_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/listify.py` & `cylc-flow-8.1.4/cylc/flow/listify.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/log_diagnosis.py` & `cylc-flow-8.1.4/cylc/flow/log_diagnosis.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/loggingutil.py` & `cylc-flow-8.1.4/cylc/flow/loggingutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/main_loop/__init__.py` & `cylc-flow-8.1.4/cylc/flow/main_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/main_loop/auto_restart.py` & `cylc-flow-8.1.4/cylc/flow/main_loop/auto_restart.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/main_loop/health_check.py` & `cylc-flow-8.1.4/cylc/flow/main_loop/health_check.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/main_loop/log_data_store.py` & `cylc-flow-8.1.4/cylc/flow/main_loop/log_data_store.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/main_loop/log_db.py` & `cylc-flow-8.1.4/cylc/flow/main_loop/log_db.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/main_loop/log_main_loop.py` & `cylc-flow-8.1.4/cylc/flow/main_loop/log_main_loop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/main_loop/log_memory.py` & `cylc-flow-8.1.4/cylc/flow/main_loop/log_memory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/main_loop/reset_bad_hosts.py` & `cylc-flow-8.1.4/cylc/flow/main_loop/reset_bad_hosts.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/__init__.py` & `cylc-flow-8.1.4/cylc/flow/network/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/authentication.py` & `cylc-flow-8.1.4/cylc/flow/network/authentication.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/authorisation.py` & `cylc-flow-8.1.4/cylc/flow/network/authorisation.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/client.py` & `cylc-flow-8.1.4/cylc/flow/network/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/client_factory.py` & `cylc-flow-8.1.4/cylc/flow/network/client_factory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/graphql.py` & `cylc-flow-8.1.4/cylc/flow/network/graphql.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/multi.py` & `cylc-flow-8.1.4/cylc/flow/network/multi.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/publisher.py` & `cylc-flow-8.1.4/cylc/flow/network/publisher.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/replier.py` & `cylc-flow-8.1.4/cylc/flow/network/replier.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/resolvers.py` & `cylc-flow-8.1.4/cylc/flow/network/resolvers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/scan.py` & `cylc-flow-8.1.4/cylc/flow/network/scan.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/schema.py` & `cylc-flow-8.1.4/cylc/flow/network/schema.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/server.py` & `cylc-flow-8.1.4/cylc/flow/network/server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/ssh_client.py` & `cylc-flow-8.1.4/cylc/flow/network/ssh_client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/network/subscriber.py` & `cylc-flow-8.1.4/cylc/flow/network/subscriber.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/option_parsers.py` & `cylc-flow-8.1.4/cylc/flow/option_parsers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/param_expand.py` & `cylc-flow-8.1.4/cylc/flow/param_expand.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/OrderedDict.py` & `cylc-flow-8.1.4/cylc/flow/parsec/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/__init__.py` & `cylc-flow-8.1.4/cylc/flow/parsec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/config.py` & `cylc-flow-8.1.4/cylc/flow/parsec/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/empysupport.py` & `cylc-flow-8.1.4/cylc/flow/parsec/empysupport.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/exceptions.py` & `cylc-flow-8.1.4/cylc/flow/parsec/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/fileparse.py` & `cylc-flow-8.1.4/cylc/flow/parsec/fileparse.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/include.py` & `cylc-flow-8.1.4/cylc/flow/parsec/include.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/jinja2support.py` & `cylc-flow-8.1.4/cylc/flow/parsec/jinja2support.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/upgrade.py` & `cylc-flow-8.1.4/cylc/flow/parsec/upgrade.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/util.py` & `cylc-flow-8.1.4/cylc/flow/parsec/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/parsec/validate.py` & `cylc-flow-8.1.4/cylc/flow/parsec/validate.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/pathutil.py` & `cylc-flow-8.1.4/cylc/flow/pathutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/platforms.py` & `cylc-flow-8.1.4/cylc/flow/platforms.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/prerequisite.py` & `cylc-flow-8.1.4/cylc/flow/prerequisite.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/print_tree.py` & `cylc-flow-8.1.4/cylc/flow/print_tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/profiler.py` & `cylc-flow-8.1.4/cylc/flow/profiler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/remote.py` & `cylc-flow-8.1.4/cylc/flow/remote.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/resources.py` & `cylc-flow-8.1.4/cylc/flow/resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/rundb.py` & `cylc-flow-8.1.4/cylc/flow/rundb.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scheduler.py` & `cylc-flow-8.1.4/cylc/flow/scheduler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scheduler_cli.py` & `cylc-flow-8.1.4/cylc/flow/scheduler_cli.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/__init__.py` & `cylc-flow-8.1.4/cylc/flow/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/broadcast.py` & `cylc-flow-8.1.4/cylc/flow/scripts/broadcast.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/cat_log.py` & `cylc-flow-8.1.4/cylc/flow/scripts/cat_log.py`

 * *Files 3% similar despite different names*

```diff
@@ -257,26 +257,26 @@
 
     """
     # The log file path may contain '$USER' to be evaluated on the job host.
     if mode == 'print':
         # Print location even if the workflow does not exist yet.
         print(logpath)
         return 0
-    if not os.path.exists(logpath) and batchview_cmd is None:
-        # Note: batchview_cmd may not need to have access to logpath, so don't
-        # test for existence of path if it is set.
-        sys.stderr.write('file not found: %s\n' % logpath)
-        return 1
     if mode == 'print-dir':
         print(os.path.dirname(logpath))
         return 0
     if mode == 'list-dir':
         for entry in sorted(os.listdir(os.path.dirname(logpath))):
             print(entry)
         return 0
+    if not os.path.exists(logpath) and batchview_cmd is None:
+        # Note: batchview_cmd may not need to have access to logpath, so don't
+        # test for existence of path if it is set.
+        sys.stderr.write('file not found: %s\n' % logpath)
+        return 1
     if prepend_path:
         from cylc.flow.hostuserutil import get_host
         print(f'# {get_host()}:{logpath}')
     if mode == 'cat':
         # print file contents to stdout.
         if batchview_cmd is not None:
             cmd = shlex.split(batchview_cmd)
@@ -360,34 +360,43 @@
         default=False,
     )
 
     return parser
 
 
 def get_task_job_attrs(workflow_id, point, task, submit_num):
-    """Return job (platform, job_runner_name, live_job_id).
+    """Retrieve job info from the database.
+
+    * live_job_id is the job ID if job is running, else None.
+    * submit_failed is True if the the submission failed.
 
-    live_job_id is the job ID if job is running, else None.
+    Returns:
+        tuple - (platform, job_runner_name, live_job_id, submit_failed)
 
     """
     with CylcWorkflowDAO(
         get_workflow_run_pub_db_path(workflow_id), is_public=True
     ) as dao:
         task_job_data = dao.select_task_job(point, task, submit_num)
     if task_job_data is None:
-        return (None, None, None)
+        return (None, None, None, None)
     job_runner_name = task_job_data["job_runner_name"]
     job_id = task_job_data["job_id"]
     if (not job_runner_name or not job_id
             or not task_job_data["time_run"]
             or task_job_data["time_run_exit"]):
         live_job_id = None
     else:
         live_job_id = job_id
-    return (task_job_data["platform_name"], job_runner_name, live_job_id)
+    return (
+        task_job_data["platform_name"],
+        job_runner_name,
+        live_job_id,
+        bool(task_job_data['submit_status']),
+    )
 
 
 @cli_function(get_option_parser)
 def main(
     parser: COP,
     options: 'Values',
     *ids,
@@ -508,15 +517,15 @@
         if options.filename is None:
             options.filename = JOB_LOG_OUT
         else:
             # Convert short filename args to long (e.g. 'o' to 'job.out').
             with suppress(KeyError):
                 options.filename = JOB_LOG_OPTS[options.filename]
                 # KeyError: Is already long form (standard log, or custom).
-        platform_name, job_runner_name, live_job_id = get_task_job_attrs(
+        platform_name, _, live_job_id, submit_failed = get_task_job_attrs(
             workflow_id, point, task, submit_num)
         platform = get_platform(platform_name)
         batchview_cmd = None
         if live_job_id is not None:
             # Job is currently running. Get special job runner log view
             # command (e.g. qcat) if one exists, and the log is out or err.
             conf_key = None
@@ -534,19 +543,32 @@
                 batchview_cmd_tmpl = None
                 with suppress(KeyError):
                     batchview_cmd_tmpl = platform[conf_key]
                 if batchview_cmd_tmpl is not None:
                     batchview_cmd = batchview_cmd_tmpl % {
                         "job_id": str(live_job_id)}
 
+        local_log_dir = get_workflow_run_job_dir(
+            workflow_id, point, task, submit_num
+        )
+
         log_is_remote = (is_remote_platform(platform)
                          and (options.filename != JOB_LOG_ACTIVITY))
         log_is_retrieved = (platform['retrieve job logs']
                             and live_job_id is None)
-        if log_is_remote and (not log_is_retrieved or options.force_remote):
+        if (
+            # only go remote for log files we can't get locally
+            log_is_remote
+            # don't look for remote log files for submit-failed tasks
+            # (there might not be any at all)
+            and not submit_failed
+            # don't go remote if the log should be retrieved (unless
+            # --force-remote is specified)
+            and (not log_is_retrieved or options.force_remote)
+        ):
             logpath = os.path.normpath(get_remote_workflow_run_job_dir(
                 workflow_id, point, task, submit_num,
                 options.filename))
             tail_tmpl = platform["tail command template"]
             # Reinvoke the cat-log command on the remote account.
             cmd = ['cat-log', *verbosity_to_opts(cylc.flow.flags.verbosity)]
             for item in [logpath, mode, tail_tmpl]:
@@ -564,19 +586,28 @@
                 remote_cylc_cmd(
                     cmd,
                     platform,
                     capture_process=False,
                     manage=(mode == 'tail'),
                     text=False
                 )
+            if (
+                mode == 'list-dir'
+                and os.path.exists(
+                    os.path.join(
+                        local_log_dir,
+                        'job-activity.log'
+                    )
+                )
+            ):
+                # add the local-only job-activity.log file to the remote-list
+                print('job-activity.log')
         else:
             # Local task job or local job log.
-            logpath = os.path.normpath(get_workflow_run_job_dir(
-                workflow_id, point, task, submit_num,
-                options.filename))
+            logpath = os.path.join(local_log_dir, options.filename)
             tail_tmpl = os.path.expandvars(platform["tail command template"])
             out = view_log(
                 logpath,
                 mode,
                 tail_tmpl,
                 batchview_cmd,
                 color=color,
```

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/check_versions.py` & `cylc-flow-8.1.4/cylc/flow/scripts/check_versions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/clean.py` & `cylc-flow-8.1.4/cylc/flow/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/client.py` & `cylc-flow-8.1.4/cylc/flow/scripts/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/common.py` & `cylc-flow-8.1.4/cylc/flow/scripts/common.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/completion_server.py` & `cylc-flow-8.1.4/cylc/flow/scripts/completion_server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/config.py` & `cylc-flow-8.1.4/cylc/flow/scripts/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/cycle_point.py` & `cylc-flow-8.1.4/cylc/flow/scripts/cycle_point.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/cylc.py` & `cylc-flow-8.1.4/cylc/flow/scripts/cylc.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/diff.py` & `cylc-flow-8.1.4/cylc/flow/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/dump.py` & `cylc-flow-8.1.4/cylc/flow/scripts/dump.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/ext_trigger.py` & `cylc-flow-8.1.4/cylc/flow/scripts/ext_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/function_run.py` & `cylc-flow-8.1.4/cylc/flow/scripts/function_run.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/get_resources.py` & `cylc-flow-8.1.4/cylc/flow/scripts/get_resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/get_workflow_contact.py` & `cylc-flow-8.1.4/cylc/flow/scripts/get_workflow_contact.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/get_workflow_version.py` & `cylc-flow-8.1.4/cylc/flow/scripts/get_workflow_version.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/graph.py` & `cylc-flow-8.1.4/cylc/flow/scripts/graph.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/hold.py` & `cylc-flow-8.1.4/cylc/flow/scripts/hold.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/install.py` & `cylc-flow-8.1.4/cylc/flow/scripts/install.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/jobs_kill.py` & `cylc-flow-8.1.4/cylc/flow/scripts/jobs_kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/jobs_poll.py` & `cylc-flow-8.1.4/cylc/flow/scripts/jobs_poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/jobs_submit.py` & `cylc-flow-8.1.4/cylc/flow/scripts/jobs_submit.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/kill.py` & `cylc-flow-8.1.4/cylc/flow/scripts/kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/lint.py` & `cylc-flow-8.1.4/cylc/flow/scripts/lint.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/list.py` & `cylc-flow-8.1.4/cylc/flow/scripts/list.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/message.py` & `cylc-flow-8.1.4/cylc/flow/scripts/message.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/pause.py` & `cylc-flow-8.1.4/cylc/flow/scripts/pause.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/ping.py` & `cylc-flow-8.1.4/cylc/flow/scripts/ping.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/play.py` & `cylc-flow-8.1.4/cylc/flow/scripts/play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/poll.py` & `cylc-flow-8.1.4/cylc/flow/scripts/poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/psutil.py` & `cylc-flow-8.1.4/cylc/flow/scripts/psutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/reinstall.py` & `cylc-flow-8.1.4/cylc/flow/scripts/reinstall.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/release.py` & `cylc-flow-8.1.4/cylc/flow/scripts/release.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/reload.py` & `cylc-flow-8.1.4/cylc/flow/scripts/reload.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/remote_init.py` & `cylc-flow-8.1.4/cylc/flow/scripts/remote_init.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/remote_tidy.py` & `cylc-flow-8.1.4/cylc/flow/scripts/remote_tidy.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/remove.py` & `cylc-flow-8.1.4/cylc/flow/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/report_timings.py` & `cylc-flow-8.1.4/cylc/flow/scripts/report_timings.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/scan.py` & `cylc-flow-8.1.4/cylc/flow/scripts/scan.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/set_outputs.py` & `cylc-flow-8.1.4/cylc/flow/scripts/set_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/set_verbosity.py` & `cylc-flow-8.1.4/cylc/flow/scripts/set_verbosity.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/show.py` & `cylc-flow-8.1.4/cylc/flow/scripts/show.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/stop.py` & `cylc-flow-8.1.4/cylc/flow/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/subscribe.py` & `cylc-flow-8.1.4/cylc/flow/scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/trigger.py` & `cylc-flow-8.1.4/cylc/flow/scripts/trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/tui.py` & `cylc-flow-8.1.4/cylc/flow/scripts/tui.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/validate.py` & `cylc-flow-8.1.4/cylc/flow/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/validate_install_play.py` & `cylc-flow-8.1.4/cylc/flow/scripts/validate_install_play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/validate_reinstall.py` & `cylc-flow-8.1.4/cylc/flow/scripts/validate_reinstall.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/view.py` & `cylc-flow-8.1.4/cylc/flow/scripts/view.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/scripts/workflow_state.py` & `cylc-flow-8.1.4/cylc/flow/scripts/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/subprocctx.py` & `cylc-flow-8.1.4/cylc/flow/subprocctx.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/subprocpool.py` & `cylc-flow-8.1.4/cylc/flow/subprocpool.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_action_timer.py` & `cylc-flow-8.1.4/cylc/flow/task_action_timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_events_mgr.py` & `cylc-flow-8.1.4/cylc/flow/task_events_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_id.py` & `cylc-flow-8.1.4/cylc/flow/task_id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_job_logs.py` & `cylc-flow-8.1.4/cylc/flow/task_job_logs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_job_mgr.py` & `cylc-flow-8.1.4/cylc/flow/task_job_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_message.py` & `cylc-flow-8.1.4/cylc/flow/task_message.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_outputs.py` & `cylc-flow-8.1.4/cylc/flow/task_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_pool.py` & `cylc-flow-8.1.4/cylc/flow/task_pool.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_proxy.py` & `cylc-flow-8.1.4/cylc/flow/task_proxy.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_queues/__init__.py` & `cylc-flow-8.1.4/cylc/flow/task_queues/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_queues/independent.py` & `cylc-flow-8.1.4/cylc/flow/task_queues/independent.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_remote_cmd.py` & `cylc-flow-8.1.4/cylc/flow/task_remote_cmd.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_remote_mgr.py` & `cylc-flow-8.1.4/cylc/flow/task_remote_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,17 @@
                 $(command) format, or an environment variable holding
                 a hostname.
 
         Returns 'localhost' if evaluated name is equivalent
         (e.g. localhost4.localdomain4).
         """
         host = self._subshell_eval(host_str, HOST_REC_COMMAND)
-        return host if is_remote_host(host) else 'localhost'
+        if host is not None and not is_remote_host(host):
+            return 'localhost'
+        return host
 
     def eval_platform(self, platform_str: str) -> Optional[str]:
         """Evaluate a platform from a possible subshell string.
 
         Args:
             platform_str: An explicit platform name, a command in $(command)
                 format, or an environment variable holding a platform name.
```

### Comparing `cylc-flow-8.1.3/cylc/flow/task_state.py` & `cylc-flow-8.1.4/cylc/flow/task_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_state_prop.py` & `cylc-flow-8.1.4/cylc/flow/task_state_prop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/task_trigger.py` & `cylc-flow-8.1.4/cylc/flow/task_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/taskdef.py` & `cylc-flow-8.1.4/cylc/flow/taskdef.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/templatevars.py` & `cylc-flow-8.1.4/cylc/flow/templatevars.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/terminal.py` & `cylc-flow-8.1.4/cylc/flow/terminal.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/time_parser.py` & `cylc-flow-8.1.4/cylc/flow/time_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/timer.py` & `cylc-flow-8.1.4/cylc/flow/timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/tui/__init__.py` & `cylc-flow-8.1.4/cylc/flow/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/tui/app.py` & `cylc-flow-8.1.4/cylc/flow/tui/app.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/tui/data.py` & `cylc-flow-8.1.4/cylc/flow/tui/data.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/tui/overlay.py` & `cylc-flow-8.1.4/cylc/flow/tui/overlay.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/tui/tree.py` & `cylc-flow-8.1.4/cylc/flow/tui/tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/tui/util.py` & `cylc-flow-8.1.4/cylc/flow/tui/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/unicode_rules.py` & `cylc-flow-8.1.4/cylc/flow/unicode_rules.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/util.py` & `cylc-flow-8.1.4/cylc/flow/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/wallclock.py` & `cylc-flow-8.1.4/cylc/flow/wallclock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/workflow_db_mgr.py` & `cylc-flow-8.1.4/cylc/flow/workflow_db_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/workflow_events.py` & `cylc-flow-8.1.4/cylc/flow/workflow_events.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/workflow_files.py` & `cylc-flow-8.1.4/cylc/flow/workflow_files.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/workflow_status.py` & `cylc-flow-8.1.4/cylc/flow/workflow_status.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/xtrigger_mgr.py` & `cylc-flow-8.1.4/cylc/flow/xtrigger_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/xtriggers/__init__.py` & `cylc-flow-8.1.4/cylc/flow/xtriggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/xtriggers/echo.py` & `cylc-flow-8.1.4/cylc/flow/xtriggers/echo.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/xtriggers/wall_clock.py` & `cylc-flow-8.1.4/cylc/flow/xtriggers/wall_clock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/xtriggers/workflow_state.py` & `cylc-flow-8.1.4/cylc/flow/xtriggers/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc/flow/xtriggers/xrandom.py` & `cylc-flow-8.1.4/cylc/flow/xtriggers/xrandom.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc_flow.egg-info/PKG-INFO` & `cylc-flow-8.1.4/cylc_flow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.1.3
+Version: 8.1.4
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
```

### Comparing `cylc-flow-8.1.3/cylc_flow.egg-info/SOURCES.txt` & `cylc-flow-8.1.4/cylc_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc_flow.egg-info/entry_points.txt` & `cylc-flow-8.1.4/cylc_flow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/cylc_flow.egg-info/requires.txt` & `cylc-flow-8.1.4/cylc_flow.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/setup.cfg` & `cylc-flow-8.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.3/setup.py` & `cylc-flow-8.1.4/setup.py`

 * *Files identical despite different names*

