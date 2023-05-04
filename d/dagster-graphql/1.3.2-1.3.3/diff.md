# Comparing `tmp/dagster-graphql-1.3.2.tar.gz` & `tmp/dagster-graphql-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.2.tar", last modified: Thu Apr 27 19:31:28 2023, max compression
+gzip compressed data, was "dagster-graphql-1.3.3.tar", last modified: Thu May  4 17:50:47 2023, max compression
```

## Comparing `dagster-graphql-1.3.2.tar` & `dagster-graphql-1.3.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.799791 dagster-graphql-1.3.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-27 19:31:28.799791 dagster-graphql-1.3.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.471790 dagster-graphql-1.3.2/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.475790 dagster-graphql-1.3.2/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21649 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.551791 dagster-graphql-1.3.2/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18443 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.559791 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11579 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8796 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4457 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7454 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12620 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15183 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8258 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10803 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3175 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8080 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.711791 dagster-graphql-1.3.2/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40629 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    15150 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18079 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16323 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10989 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    23351 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.715791 dagster-graphql-1.3.2/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20899 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    16816 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.727791 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11072 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39816 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1262 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.791791 dagster-graphql-1.3.2/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    25590 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    36271 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4051 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.795791 dagster-graphql-1.3.2/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8314 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7971 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29755 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.795791 dagster-graphql-1.3.2/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6376 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.471790 dagster-graphql-1.3.2/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4150 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-27 19:31:28.799791 dagster-graphql-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1455 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.723851 dagster-graphql-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-04 17:50:47.723851 dagster-graphql-1.3.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.663851 dagster-graphql-1.3.3/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.667851 dagster-graphql-1.3.3/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21544 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.679851 dagster-graphql-1.3.3/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.683851 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11506 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4653 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4404 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12609 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15110 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10796 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8081 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.703851 dagster-graphql-1.3.3/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40446 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16333 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16323 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    25158 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.707851 dagster-graphql-1.3.3/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17489 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.715851 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39461 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.719851 dagster-graphql-1.3.3/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    25580 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    36191 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4113 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.723851 dagster-graphql-1.3.3/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8309 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7986 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.723851 dagster-graphql-1.3.3/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6376 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.663851 dagster-graphql-1.3.3/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-04 17:50:47.727851 dagster-graphql-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/setup.py
```

### Comparing `dagster-graphql-1.3.2/LICENSE` & `dagster-graphql-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/PKG-INFO` & `dagster-graphql-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.2
+Version: 1.3.3
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/__init__.py` & `dagster-graphql-1.3.3/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/cli.py` & `dagster-graphql-1.3.3/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/client/client.py` & `dagster-graphql-1.3.3/dagster_graphql/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     RELOAD_REPOSITORY_LOCATION_MUTATION,
     SHUTDOWN_REPOSITORY_LOCATION_MUTATION,
     TERMINATE_RUN_JOB_MUTATION,
 )
 from .utils import (
     DagsterGraphQLClientError,
     InvalidOutputErrorInfo,
-    PipelineInfo,
+    JobInfo,
     ReloadRepositoryLocationInfo,
     ReloadRepositoryLocationStatus,
     ShutdownRepositoryLocationInfo,
     ShutdownRepositoryLocationStatus,
 )
 
 
@@ -98,23 +98,21 @@
             return self._client.execute(gql(query), variable_values=variables)
         except Exception as exc:  # catch generic Exception from the gql client
             raise DagsterGraphQLClientError(
                 f"Exception occured during execution of query \n{query}\n with variables"
                 f" \n{variables}\n"
             ) from exc
 
-    def _get_repo_locations_and_names_with_pipeline(self, pipeline_name: str) -> List[PipelineInfo]:
+    def _get_repo_locations_and_names_with_pipeline(self, job_name: str) -> List[JobInfo]:
         res_data = self._execute(CLIENT_GET_REPO_LOCATIONS_NAMES_AND_PIPELINES_QUERY)
         query_res = res_data["repositoriesOrError"]
         repo_connection_status = query_res["__typename"]
         if repo_connection_status == "RepositoryConnection":
-            valid_nodes: Iterable[PipelineInfo] = chain(
-                *map(PipelineInfo.from_node, query_res["nodes"])
-            )
-            return [info for info in valid_nodes if info.pipeline_name == pipeline_name]
+            valid_nodes: Iterable[JobInfo] = chain(*map(JobInfo.from_node, query_res["nodes"]))
+            return [info for info in valid_nodes if info.job_name == job_name]
         else:
             raise DagsterGraphQLClientError(repo_connection_status, query_res["message"])
 
     def _core_submit_execution(
         self,
         pipeline_name: str,
         repository_location_name: Optional[str] = None,
@@ -142,32 +140,32 @@
             ),
         )
         tags = validate_tags(tags)
 
         pipeline_or_job = "Job" if is_using_job_op_graph_apis else "Pipeline"
 
         if not repository_location_name or not repository_name:
-            pipeline_info_lst = self._get_repo_locations_and_names_with_pipeline(pipeline_name)
-            if len(pipeline_info_lst) == 0:
+            job_info_lst = self._get_repo_locations_and_names_with_pipeline(pipeline_name)
+            if len(job_info_lst) == 0:
                 raise DagsterGraphQLClientError(
                     f"{pipeline_or_job}NotFoundError",
                     (
                         f"No {'jobs' if is_using_job_op_graph_apis else 'pipelines'} with the name"
                         f" `{pipeline_name}` exist"
                     ),
                 )
-            elif len(pipeline_info_lst) == 1:
-                pipeline_info = pipeline_info_lst[0]
-                repository_location_name = pipeline_info.repository_location_name
-                repository_name = pipeline_info.repository_name
+            elif len(job_info_lst) == 1:
+                job_info = job_info_lst[0]
+                repository_location_name = job_info.repository_location_name
+                repository_name = job_info.repository_name
             else:
                 raise DagsterGraphQLClientError(
                     "Must specify repository_location_name and repository_name since there are"
                     f" multiple {'jobs' if is_using_job_op_graph_apis else 'pipelines'} with the"
-                    f" name {pipeline_name}.\n\tchoose one of: {pipeline_info_lst}"
+                    f" name {pipeline_name}.\n\tchoose one of: {job_info_lst}"
                 )
 
         variables: Dict[str, Any] = {
             "executionParams": {
                 "selector": {
                     "repositoryLocationName": repository_location_name,
                     "repositoryName": repository_name,
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.3.3/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/client/query.py` & `dagster-graphql-1.3.3/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/client/utils.py` & `dagster-graphql-1.3.3/dagster_graphql/client/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,30 +52,30 @@
           `status == ShutdownRepositoryLocationStatus.FAILURE`. Defaults to None.
     """
 
     status: ShutdownRepositoryLocationStatus
     message: Optional[str] = None
 
 
-class PipelineInfo(NamedTuple):
+class JobInfo(NamedTuple):
     repository_location_name: str
     repository_name: str
-    pipeline_name: str
+    job_name: str
 
     @staticmethod
-    def from_node(node: Dict[str, Any]) -> List["PipelineInfo"]:
+    def from_node(node: Dict[str, Any]) -> List["JobInfo"]:
         repo_name = node["name"]
         repo_location_name = node["location"]["name"]
         return [
-            PipelineInfo(
+            JobInfo(
                 repository_location_name=repo_location_name,
                 repository_name=repo_name,
-                pipeline_name=pipeline["name"],
+                job_name=job["name"],
             )
-            for pipeline in node["pipelines"]
+            for job in node["pipelines"]
         ]
 
 
 class InvalidOutputErrorInfo(NamedTuple):
     """This class gives information about an InvalidOutputError from submitting a pipeline for execution
     from GraphQL.
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/events.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         DagsterEventType.PIPELINE_SUCCESS,
     ):
         return GrapheneRunSuccessEvent(pipelineName=pipeline_name, **basic_params)
     elif dagster_event.event_type in (
         DagsterEventType.RUN_FAILURE,
         DagsterEventType.PIPELINE_FAILURE,
     ):
-        data = dagster_event.pipeline_failure_data
+        data = dagster_event.job_failure_data
         return GrapheneRunFailureEvent(
             pipelineName=pipeline_name,
             error=GraphenePythonError(data.error) if (data and data.error) else None,
             **basic_params,
         )
 
     elif dagster_event.event_type == DagsterEventType.ALERT_START:
@@ -365,14 +365,16 @@
     elif dagster_event.event_type == DagsterEventType.LOGS_CAPTURED:
         data = dagster_event.logs_captured_data
         return GrapheneLogsCapturedEvent(
             fileKey=data.file_key,
             logKey=data.file_key,
             stepKeys=data.step_keys,
             externalUrl=data.external_url,
+            externalStdoutUrl=data.external_stdout_url or data.external_url,
+            externalStderrUrl=data.external_stderr_url or data.external_url,
             pid=dagster_event.pid,
             **basic_params,
         )
     elif dagster_event.event_type == DagsterEventType.STEP_WORKER_STARTING:
         data = dagster_event.engine_event_data
         return GrapheneStepWorkerStartingEvent(
             metadataEntries=_to_metadata_entries(data.metadata),
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # re-exports
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey
 from dagster._core.events import EngineEventData
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.captured_log_manager import CapturedLogManager
 from dagster._core.storage.compute_log_manager import ComputeIOType, ComputeLogFileData
-from dagster._core.storage.pipeline_run import DagsterRunStatus
+from dagster._core.storage.dagster_run import DagsterRunStatus
 from dagster._core.workspace.permissions import Permissions
 from dagster._utils.error import serializable_error_info_from_exc_info
 from starlette.concurrency import (
     run_in_threadpool,  # can provide this indirectly if we dont want starlette dep in dagster-graphql
 )
 
 if TYPE_CHECKING:
@@ -94,17 +94,15 @@
     if not record:
         assert_permission(graphene_info, Permissions.TERMINATE_PIPELINE_EXECUTION)
         return GrapheneRunNotFoundError(run_id)
 
     run = record.dagster_run
     graphene_run = GrapheneRun(record)
 
-    location_name = (
-        run.external_pipeline_origin.location_name if run.external_pipeline_origin else None
-    )
+    location_name = run.external_job_origin.location_name if run.external_job_origin else None
 
     if location_name:
         assert_permission_for_location(
             graphene_info, Permissions.TERMINATE_PIPELINE_EXECUTION, location_name
         )
     else:
         assert_permission(graphene_info, Permissions.TERMINATE_PIPELINE_EXECUTION)
@@ -127,15 +125,15 @@
                 instance.run_coordinator.cancel_run(run_id)
         except:
             instance.report_engine_event(
                 (
                     "Exception while attempting to force-terminate run. Run will still be marked as"
                     " canceled."
                 ),
-                pipeline_name=run.pipeline_name,
+                job_name=run.job_name,
                 run_id=run.run_id,
                 engine_event_data=EngineEventData(
                     error=serializable_error_info_from_exc_info(sys.exc_info()),
                 ),
             )
         return _force_mark_as_canceled(instance, run_id)
 
@@ -156,17 +154,15 @@
 
     instance = graphene_info.context.instance
 
     run = instance.get_run_by_id(run_id)
     if not run:
         return GrapheneRunNotFoundError(run_id)
 
-    location_name = (
-        run.external_pipeline_origin.location_name if run.external_pipeline_origin else None
-    )
+    location_name = run.external_job_origin.location_name if run.external_job_origin else None
     if location_name:
         assert_permission_for_location(
             graphene_info, Permissions.DELETE_PIPELINE_RUN, location_name
         )
     else:
         assert_permission(graphene_info, Permissions.DELETE_PIPELINE_RUN)
 
@@ -227,15 +223,15 @@
             cursor=after_cursor,
             limit=chunk_size,
         )
         if not dont_send_past_records:
             yield GraphenePipelineRunLogsSubscriptionSuccess(
                 run=GrapheneRun(record),
                 messages=[
-                    from_event_record(record.event_log_entry, run.pipeline_name)
+                    from_event_record(record.event_log_entry, run.job_name)
                     for record in connection.records
                 ],
                 hasMorePastEvents=connection.has_more,
                 cursor=connection.cursor,
             )
         has_more = connection.has_more
         after_cursor = connection.cursor
@@ -249,15 +245,15 @@
     # watch for live events
     instance.watch_event_logs(run_id, after_cursor, _enqueue)
     try:
         while True:
             event, cursor = await queue.get()
             yield GraphenePipelineRunLogsSubscriptionSuccess(
                 run=GrapheneRun(record),
-                messages=[from_event_record(event, run.pipeline_name)],
+                messages=[from_event_record(event, run.job_name)],
                 hasMorePastEvents=False,
                 cursor=cursor,
             )
     finally:
         instance.end_watch_event_logs(run_id, _enqueue)
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import TYPE_CHECKING, cast
 
 import dagster._check as check
-from dagster._core.definitions.selector import PipelineSelector
+from dagster._core.definitions.selector import JobSubsetSelector
 from dagster._core.execution.plan.resume_retry import ReexecutionStrategy
 from dagster._core.instance import DagsterInstance
-from dagster._core.storage.pipeline_run import DagsterRun, RunsFilter
+from dagster._core.storage.dagster_run import DagsterRun, RunsFilter
 from dagster._core.workspace.permissions import Permissions
 
-from ..external import get_external_pipeline_or_raise
+from ..external import get_external_job_or_raise
 from ..utils import (
     ExecutionMetadata,
     ExecutionParams,
     assert_permission_for_location,
     capture_error,
 )
 from .run_lifecycle import create_valid_pipeline_run
@@ -44,19 +44,19 @@
     if is_reexecuted:
         # required fields for re-execution
         execution_metadata = check.inst_param(
             execution_params.execution_metadata, "execution_metadata", ExecutionMetadata
         )
         check.str_param(execution_metadata.root_run_id, "root_run_id")
         check.str_param(execution_metadata.parent_run_id, "parent_run_id")
-    external_pipeline = get_external_pipeline_or_raise(graphene_info, execution_params.selector)
-    pipeline_run = create_valid_pipeline_run(graphene_info, external_pipeline, execution_params)
+    external_job = get_external_job_or_raise(graphene_info, execution_params.selector)
+    dagster_run = create_valid_pipeline_run(graphene_info, external_job, execution_params)
 
     return graphene_info.context.instance.submit_run(
-        pipeline_run.run_id,
+        dagster_run.run_id,
         workspace=graphene_info.context,
     )
 
 
 def _launch_pipeline_execution(
     graphene_info: "ResolveInfo", execution_params: ExecutionParams, is_reexecuted: bool = False
 ) -> "GrapheneLaunchRunSuccess":
@@ -82,35 +82,35 @@
 
     check.str_param(parent_run_id, "parent_run_id")
 
     instance: DagsterInstance = graphene_info.context.instance
     parent_run = check.not_none(
         instance.get_run_by_id(parent_run_id), f"Could not find parent run with id: {parent_run_id}"
     )
-    origin = check.not_none(parent_run.external_pipeline_origin)
-    selector = PipelineSelector(
+    origin = check.not_none(parent_run.external_job_origin)
+    selector = JobSubsetSelector(
         location_name=origin.external_repository_origin.code_location_origin.location_name,
         repository_name=origin.external_repository_origin.repository_name,
-        pipeline_name=parent_run.pipeline_name,
+        job_name=parent_run.job_name,
         solid_selection=None,
     )
 
     assert_permission_for_location(
         graphene_info,
         Permissions.LAUNCH_PIPELINE_REEXECUTION,
         selector.location_name,
     )
 
     repo_location = graphene_info.context.get_code_location(selector.location_name)
-    external_pipeline = get_external_pipeline_or_raise(graphene_info, selector)
+    external_pipeline = get_external_job_or_raise(graphene_info, selector)
 
     run = instance.create_reexecuted_run(
         parent_run=cast(DagsterRun, parent_run),
         code_location=repo_location,
-        external_pipeline=external_pipeline,
+        external_job=external_pipeline,
         strategy=ReexecutionStrategy(strategy),
         use_parent_run_tags=True,  # inherit whatever tags were set on the parent run at launch time
     )
     graphene_info.context.instance.submit_run(
         run.run_id,
         workspace=graphene_info.context,
     )
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple, cast
 
 import dagster._check as check
 from dagster._core.errors import DagsterRunNotFoundError
 from dagster._core.execution.plan.state import KnownExecutionState
-from dagster._core.host_representation.external import ExternalPipeline
+from dagster._core.host_representation.external import ExternalJob
 from dagster._core.instance import DagsterInstance
-from dagster._core.storage.pipeline_run import DagsterRun, DagsterRunStatus
+from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus
 from dagster._core.storage.tags import RESUME_RETRY_TAG
 from dagster._core.utils import make_new_run_id
 from dagster._utils.merger import merge_dicts
 
 from ..external import ensure_valid_config, get_external_execution_plan_or_raise
 from ..utils import ExecutionParams
 
@@ -54,15 +54,15 @@
 def is_resume_retry(execution_params: ExecutionParams) -> bool:
     check.inst_param(execution_params, "execution_params", ExecutionParams)
     return execution_params.execution_metadata.tags.get(RESUME_RETRY_TAG) == "true"
 
 
 def create_valid_pipeline_run(
     graphene_info: "ResolveInfo",
-    external_pipeline: ExternalPipeline,
+    external_pipeline: ExternalJob,
     execution_params: ExecutionParams,
 ) -> DagsterRun:
     ensure_valid_config(external_pipeline, execution_params.run_config)
 
     step_keys_to_execute, known_state = compute_step_keys_to_execute(
         graphene_info, execution_params
     )
@@ -72,19 +72,19 @@
         external_pipeline=external_pipeline,
         run_config=execution_params.run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
     )
     tags = merge_dicts(external_pipeline.tags, execution_params.execution_metadata.tags)
 
-    pipeline_run = graphene_info.context.instance.create_run(
-        pipeline_snapshot=external_pipeline.pipeline_snapshot,
+    dagster_run = graphene_info.context.instance.create_run(
+        job_snapshot=external_pipeline.job_snapshot,
         execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
-        parent_pipeline_snapshot=external_pipeline.parent_pipeline_snapshot,
-        pipeline_name=execution_params.selector.pipeline_name,
+        parent_job_snapshot=external_pipeline.parent_job_snapshot,
+        job_name=execution_params.selector.job_name,
         run_id=execution_params.execution_metadata.run_id
         if execution_params.execution_metadata.run_id
         else make_new_run_id(),
         asset_selection=frozenset(execution_params.selector.asset_selection)
         if execution_params.selector.asset_selection
         else None,
         solid_selection=execution_params.selector.solid_selection,
@@ -93,12 +93,12 @@
         else None,
         run_config=execution_params.run_config,
         step_keys_to_execute=step_keys_to_execute,
         tags=tags,
         root_run_id=execution_params.execution_metadata.root_run_id,
         parent_run_id=execution_params.execution_metadata.parent_run_id,
         status=DagsterRunStatus.NOT_STARTED,
-        external_pipeline_origin=external_pipeline.get_external_origin(),
-        pipeline_code_origin=external_pipeline.get_python_origin(),
+        external_job_origin=external_pipeline.get_external_origin(),
+        job_code_origin=external_pipeline.get_python_origin(),
     )
 
-    return pipeline_run
+    return dagster_run
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/external.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/external.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import sys
 from typing import TYPE_CHECKING, Mapping, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._config import validate_config_from_snap
-from dagster._core.definitions.selector import PipelineSelector, RepositorySelector
+from dagster._core.definitions.selector import JobSubsetSelector, RepositorySelector
 from dagster._core.execution.plan.state import KnownExecutionState
-from dagster._core.host_representation import ExternalPipeline
+from dagster._core.host_representation import ExternalJob
 from dagster._core.host_representation.external import ExternalExecutionPlan
 from dagster._core.workspace.context import BaseWorkspaceRequestContext, WorkspaceRequestContext
 from dagster._utils.error import serializable_error_info_from_exc_info
 
 from .utils import UserFacingGraphQLError, capture_error
 
 if TYPE_CHECKING:
@@ -21,90 +21,90 @@
         GrapheneRepositoryConnection,
         GrapheneWorkspace,
         GrapheneWorkspaceLocationStatusEntries,
     )
     from dagster_graphql.schema.util import ResolveInfo
 
 
-def get_full_external_pipeline_or_raise(
+def get_full_external_job_or_raise(
     graphene_info: "ResolveInfo",
-    selector: PipelineSelector,
-) -> ExternalPipeline:
-    check.inst_param(selector, "selector", PipelineSelector)
-    return _get_external_pipeline_or_raise(graphene_info, selector, ignore_subset=True)
-
-
-def get_external_pipeline_or_raise(
-    graphene_info: "ResolveInfo", selector: PipelineSelector
-) -> ExternalPipeline:
-    check.inst_param(selector, "selector", PipelineSelector)
-    return _get_external_pipeline_or_raise(graphene_info, selector)
-
-
-def _get_external_pipeline_or_raise(
-    graphene_info: "ResolveInfo", selector: PipelineSelector, ignore_subset: bool = False
-) -> ExternalPipeline:
+    selector: JobSubsetSelector,
+) -> ExternalJob:
+    check.inst_param(selector, "selector", JobSubsetSelector)
+    return _get_external_job_or_raise(graphene_info, selector, ignore_subset=True)
+
+
+def get_external_job_or_raise(
+    graphene_info: "ResolveInfo", selector: JobSubsetSelector
+) -> ExternalJob:
+    check.inst_param(selector, "selector", JobSubsetSelector)
+    return _get_external_job_or_raise(graphene_info, selector)
+
+
+def _get_external_job_or_raise(
+    graphene_info: "ResolveInfo", selector: JobSubsetSelector, ignore_subset: bool = False
+) -> ExternalJob:
     from ..schema.errors import GrapheneInvalidSubsetError, GraphenePipelineNotFoundError
     from ..schema.pipelines.pipeline import GraphenePipeline
 
     ctx = graphene_info.context
     if not ctx.has_external_job(selector):
         raise UserFacingGraphQLError(GraphenePipelineNotFoundError(selector=selector))
     elif ignore_subset:
-        external_pipeline = ctx.get_full_external_job(selector)
+        external_job = ctx.get_full_external_job(selector)
     else:
         code_location = ctx.get_code_location(selector.location_name)
         try:
-            external_pipeline = code_location.get_external_pipeline(selector)
+            external_job = code_location.get_external_job(selector)
         except Exception:
             error_info = serializable_error_info_from_exc_info(sys.exc_info())
             raise UserFacingGraphQLError(
                 GrapheneInvalidSubsetError(
                     message="{message}{cause_message}".format(
                         message=error_info.message,
                         cause_message=f"\n{error_info.cause.message}" if error_info.cause else "",
                     ),
                     pipeline=GraphenePipeline(ctx.get_full_external_job(selector)),
                 )
             )
 
-    return external_pipeline
+    return external_job
 
 
-def ensure_valid_config(external_pipeline: ExternalPipeline, run_config: object) -> object:
+def ensure_valid_config(external_job: ExternalJob, run_config: object) -> object:
     from ..schema.pipelines.config import GrapheneRunConfigValidationInvalid
 
-    check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
+    check.inst_param(external_job, "external_job", ExternalJob)
     # do not type check run_config so that validate_config_from_snap throws
 
     validated_config = validate_config_from_snap(
-        config_schema_snapshot=external_pipeline.config_schema_snapshot,
-        config_type_key=check.not_none(external_pipeline.root_config_key),
+        config_schema_snapshot=external_job.config_schema_snapshot,
+        config_type_key=check.not_none(external_job.root_config_key),
         config_value=run_config,
     )
 
     if not validated_config.success:
         raise UserFacingGraphQLError(
             GrapheneRunConfigValidationInvalid.for_validation_errors(
-                external_pipeline, validated_config.errors
+                external_job, validated_config.errors
             )
         )
 
     return validated_config
 
 
 def get_external_execution_plan_or_raise(
     graphene_info: "ResolveInfo",
-    external_pipeline: ExternalPipeline,
+    external_pipeline: ExternalJob,
     run_config: Mapping[str, object],
     step_keys_to_execute: Optional[Sequence[str]],
     known_state: Optional[KnownExecutionState],
 ) -> ExternalExecutionPlan:
     return graphene_info.context.get_external_execution_plan(
-        external_pipeline=external_pipeline,
+        external_job=external_pipeline,
         run_config=run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
     )
 
 
 @capture_error
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ExternalPartitionSet,
     RepositoryHandle,
 )
 from dagster._core.host_representation.external_data import (
     ExternalPartitionExecutionErrorData,
     ExternalPartitionNamesData,
 )
-from dagster._core.storage.pipeline_run import RunPartitionData, RunsFilter
+from dagster._core.storage.dagster_run import RunPartitionData, RunsFilter
 from dagster._core.storage.tags import (
     PARTITION_NAME_TAG,
     PARTITION_SET_TAG,
     REPOSITORY_LABEL_TAG,
     TagType,
     get_tag_type,
 )
@@ -50,27 +50,27 @@
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
     check.str_param(pipeline_name, "pipeline_name")
     location = graphene_info.context.get_code_location(repository_selector.location_name)
     repository = location.get_repository(repository_selector.repository_name)
     partition_sets = [
         partition_set
         for partition_set in repository.get_external_partition_sets()
-        if partition_set.pipeline_name == pipeline_name
+        if partition_set.job_name == pipeline_name
     ]
 
     return GraphenePartitionSets(
         results=[
             GraphenePartitionSet(
                 external_repository_handle=repository.handle,
                 external_partition_set=partition_set,
             )
             for partition_set in sorted(
                 partition_sets,
                 key=lambda partition_set: (
-                    partition_set.pipeline_name,
+                    partition_set.job_name,
                     partition_set.mode,
                     partition_set.name,
                 ),
             )
         ]
     )
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,95 @@
 from typing import TYPE_CHECKING, Union
 
 import dagster._check as check
 from dagster._core.instance import DagsterInstance
-from dagster._core.storage.pipeline_run import DagsterRun
+from dagster._core.storage.dagster_run import DagsterRun
 
 from dagster_graphql.schema.util import ResolveInfo
 
-from .external import get_external_pipeline_or_raise, get_full_external_pipeline_or_raise
-from .utils import PipelineSelector, UserFacingGraphQLError, capture_error
+from .external import get_external_job_or_raise, get_full_external_job_or_raise
+from .utils import JobSubsetSelector, UserFacingGraphQLError, capture_error
 
 if TYPE_CHECKING:
     from ..schema.pipelines.pipeline import GraphenePipeline
     from ..schema.pipelines.pipeline_ref import GrapheneUnknownPipeline
     from ..schema.pipelines.snapshot import GraphenePipelineSnapshot
 
 
 @capture_error
-def get_pipeline_snapshot_or_error_from_pipeline_selector(
-    graphene_info: ResolveInfo, pipeline_selector: PipelineSelector
+def get_job_snapshot_or_error_from_job_selector(
+    graphene_info: ResolveInfo, job_selector: JobSubsetSelector
 ) -> "GraphenePipelineSnapshot":
     from ..schema.pipelines.snapshot import GraphenePipelineSnapshot
 
-    check.inst_param(pipeline_selector, "pipeline_selector", PipelineSelector)
-    return GraphenePipelineSnapshot(
-        get_full_external_pipeline_or_raise(graphene_info, pipeline_selector)
-    )
+    check.inst_param(job_selector, "pipeline_selector", JobSubsetSelector)
+    return GraphenePipelineSnapshot(get_full_external_job_or_raise(graphene_info, job_selector))
 
 
 @capture_error
-def get_pipeline_snapshot_or_error_from_snapshot_id(
+def get_job_snapshot_or_error_from_snapshot_id(
     graphene_info: ResolveInfo, snapshot_id: str
 ) -> "GraphenePipelineSnapshot":
     check.str_param(snapshot_id, "snapshot_id")
-    return _get_pipeline_snapshot_from_instance(graphene_info.context.instance, snapshot_id)
+    return _get_job_snapshot_from_instance(graphene_info.context.instance, snapshot_id)
 
 
 # extracted this out to test
-def _get_pipeline_snapshot_from_instance(
+def _get_job_snapshot_from_instance(
     instance: DagsterInstance, snapshot_id: str
 ) -> "GraphenePipelineSnapshot":
     from ..schema.errors import GraphenePipelineSnapshotNotFoundError
     from ..schema.pipelines.snapshot import GraphenePipelineSnapshot
 
-    if not instance.has_pipeline_snapshot(snapshot_id):
+    if not instance.has_job_snapshot(snapshot_id):
         raise UserFacingGraphQLError(GraphenePipelineSnapshotNotFoundError(snapshot_id))
 
-    historical_pipeline = instance.get_historical_pipeline(snapshot_id)
+    historical_pipeline = instance.get_historical_job(snapshot_id)
 
     if not historical_pipeline:
         # Either a temporary error or it has been deleted in the interim
         raise UserFacingGraphQLError(GraphenePipelineSnapshotNotFoundError(snapshot_id))
 
     return GraphenePipelineSnapshot(historical_pipeline)
 
 
 @capture_error
-def get_pipeline_or_error(
-    graphene_info: ResolveInfo, selector: PipelineSelector
-) -> "GraphenePipeline":
+def get_job_or_error(graphene_info: ResolveInfo, selector: JobSubsetSelector) -> "GraphenePipeline":
     """Returns a PipelineOrError."""
-    return get_pipeline_from_selector(graphene_info, selector)
+    return get_job_from_selector(graphene_info, selector)
 
 
-def get_pipeline_or_raise(
-    graphene_info: ResolveInfo, selector: PipelineSelector
-) -> "GraphenePipeline":
+def get_job_or_raise(graphene_info: ResolveInfo, selector: JobSubsetSelector) -> "GraphenePipeline":
     """Returns a Pipeline or raises a UserFacingGraphQLError if one cannot be retrieved
     from the selector, e.g., the pipeline is not present in the loaded repository.
     """
-    return get_pipeline_from_selector(graphene_info, selector)
+    return get_job_from_selector(graphene_info, selector)
 
 
-def get_pipeline_reference_or_raise(
-    graphene_info: ResolveInfo, pipeline_run: DagsterRun
+def get_job_reference_or_raise(
+    graphene_info: ResolveInfo, dagster_run: DagsterRun
 ) -> Union["GraphenePipelineSnapshot", "GrapheneUnknownPipeline"]:
     """Returns a PipelineReference or raises a UserFacingGraphQLError if a pipeline
     reference cannot be retrieved based on the run, e.g, a UserFacingGraphQLError that wraps an
     InvalidSubsetError.
     """
     from ..schema.pipelines.pipeline_ref import GrapheneUnknownPipeline
 
-    check.inst_param(pipeline_run, "pipeline_run", DagsterRun)
-    solid_selection = (
-        list(pipeline_run.solids_to_execute) if pipeline_run.solids_to_execute else None
-    )
+    check.inst_param(dagster_run, "pipeline_run", DagsterRun)
+    solid_selection = list(dagster_run.solids_to_execute) if dagster_run.solids_to_execute else None
 
-    if pipeline_run.pipeline_snapshot_id is None:
-        return GrapheneUnknownPipeline(pipeline_run.pipeline_name, solid_selection)
+    if dagster_run.job_snapshot_id is None:
+        return GrapheneUnknownPipeline(dagster_run.job_name, solid_selection)
 
-    return _get_pipeline_snapshot_from_instance(
-        graphene_info.context.instance, pipeline_run.pipeline_snapshot_id
+    return _get_job_snapshot_from_instance(
+        graphene_info.context.instance, dagster_run.job_snapshot_id
     )
 
 
-def get_pipeline_from_selector(
-    graphene_info: ResolveInfo, selector: PipelineSelector
+def get_job_from_selector(
+    graphene_info: ResolveInfo, selector: JobSubsetSelector
 ) -> "GraphenePipeline":
     from ..schema.pipelines.pipeline import GraphenePipeline
 
-    check.inst_param(selector, "selector", PipelineSelector)
+    check.inst_param(selector, "selector", JobSubsetSelector)
 
-    return GraphenePipeline(get_external_pipeline_or_raise(graphene_info, selector))
+    return GraphenePipeline(get_external_job_or_raise(graphene_info, selector))
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_runs.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     cast,
 )
 
 from dagster import (
     AssetKey,
     _check as check,
 )
-from dagster._core.definitions.selector import PipelineSelector
+from dagster._core.definitions.selector import JobSubsetSelector
 from dagster._core.errors import DagsterRunNotFoundError
 from dagster._core.execution.stats import RunStepKeyStatsSnapshot, StepEventStatus
-from dagster._core.storage.pipeline_run import DagsterRunStatus, RunRecord, RunsFilter
+from dagster._core.storage.dagster_run import DagsterRunStatus, RunRecord, RunsFilter
 from dagster._core.storage.tags import TagType, get_tag_type
 
-from .external import ensure_valid_config, get_external_pipeline_or_raise
+from .external import ensure_valid_config, get_external_job_or_raise
 from .utils import capture_error
 
 if TYPE_CHECKING:
     from ..schema.asset_graph import GrapheneAssetLatestInfo, GrapheneAssetNode
     from ..schema.errors import GrapheneRunNotFoundError
     from ..schema.execution import GrapheneExecutionPlan
     from ..schema.logs.events import GrapheneRunStepStats
@@ -329,41 +329,41 @@
         for root_run_id, run_group in run_groups.items()
     ]
 
 
 @capture_error
 def validate_pipeline_config(
     graphene_info: "ResolveInfo",
-    selector: PipelineSelector,
+    selector: JobSubsetSelector,
     run_config: Union[str, Mapping[str, object]],
 ) -> "GraphenePipelineConfigValidationValid":
     from ..schema.pipelines.config import GraphenePipelineConfigValidationValid
 
-    check.inst_param(selector, "selector", PipelineSelector)
+    check.inst_param(selector, "selector", JobSubsetSelector)
 
-    external_pipeline = get_external_pipeline_or_raise(graphene_info, selector)
-    ensure_valid_config(external_pipeline, run_config)
-    return GraphenePipelineConfigValidationValid(pipeline_name=external_pipeline.name)
+    external_job = get_external_job_or_raise(graphene_info, selector)
+    ensure_valid_config(external_job, run_config)
+    return GraphenePipelineConfigValidationValid(pipeline_name=external_job.name)
 
 
 @capture_error
 def get_execution_plan(
     graphene_info: "ResolveInfo",
-    selector: PipelineSelector,
+    selector: JobSubsetSelector,
     run_config: Mapping[str, Any],
 ) -> "GrapheneExecutionPlan":
     from ..schema.execution import GrapheneExecutionPlan
 
-    check.inst_param(selector, "selector", PipelineSelector)
+    check.inst_param(selector, "selector", JobSubsetSelector)
 
-    external_pipeline = get_external_pipeline_or_raise(graphene_info, selector)
-    ensure_valid_config(external_pipeline, run_config)
+    external_job = get_external_job_or_raise(graphene_info, selector)
+    ensure_valid_config(external_job, run_config)
     return GrapheneExecutionPlan(
         graphene_info.context.get_external_execution_plan(
-            external_pipeline=external_pipeline,
+            external_job=external_job,
             run_config=run_config,
             step_keys_to_execute=None,
             known_state=None,
         )
     )
 
 
@@ -399,13 +399,11 @@
     instance = graphene_info.context.instance
     run = instance.get_run_by_id(run_id)
     if not run:
         return GrapheneRunNotFoundError(run_id)
 
     conn = instance.get_records_for_run(run_id, cursor=cursor, limit=limit)
     return GrapheneEventConnection(
-        events=[
-            from_event_record(record.event_log_entry, run.pipeline_name) for record in conn.records
-        ],
+        events=[from_event_record(record.event_log_entry, run.job_name) for record in conn.records],
         cursor=conn.cursor,
         hasMore=conn.has_more,
     )
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Optional, Sequence, Set
 
 import dagster._check as check
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.definitions.selector import (
-    PipelineSelector,
+    JobSubsetSelector,
     RepositorySelector,
     ScheduleSelector,
 )
 from dagster._core.scheduler.instigation import InstigatorState, InstigatorStatus
 from dagster._core.workspace.permissions import Permissions
 from dagster._seven import get_current_datetime_in_utc, get_timestamp_from_utc_datetime
 
@@ -136,27 +136,27 @@
         for schedule in filtered
     ]
 
     return GrapheneSchedules(results=results)
 
 
 def get_schedules_for_pipeline(
-    graphene_info: ResolveInfo, pipeline_selector: PipelineSelector
+    graphene_info: ResolveInfo, pipeline_selector: JobSubsetSelector
 ) -> Sequence["GrapheneSchedule"]:
     from ..schema.schedules import GrapheneSchedule
 
-    check.inst_param(pipeline_selector, "pipeline_selector", PipelineSelector)
+    check.inst_param(pipeline_selector, "pipeline_selector", JobSubsetSelector)
 
     location = graphene_info.context.get_code_location(pipeline_selector.location_name)
     repository = location.get_repository(pipeline_selector.repository_name)
     external_schedules = repository.get_external_schedules()
 
     results = []
     for external_schedule in external_schedules:
-        if external_schedule.pipeline_name != pipeline_selector.pipeline_name:
+        if external_schedule.job_name != pipeline_selector.job_name:
             continue
 
         schedule_state = graphene_info.context.instance.get_instigator_state(
             external_schedule.get_external_origin_id(),
             external_schedule.selector_id,
         )
         results.append(GrapheneSchedule(external_schedule, schedule_state))
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_sensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Optional, Sequence, Set
 
 import dagster._check as check
 from dagster._core.definitions.run_request import InstigatorType
-from dagster._core.definitions.selector import PipelineSelector, RepositorySelector, SensorSelector
+from dagster._core.definitions.selector import JobSubsetSelector, RepositorySelector, SensorSelector
 from dagster._core.scheduler.instigation import (
     InstigatorState,
     InstigatorStatus,
     SensorInstigatorData,
 )
 from dagster._core.workspace.permissions import Permissions
 from dagster._seven import get_current_datetime_in_utc, get_timestamp_from_utc_datetime
@@ -178,28 +178,28 @@
             GrapheneInstigationState(instigator_state=sensor_state)
             for sensor_state in unloadable_states
         ]
     )
 
 
 def get_sensors_for_pipeline(
-    graphene_info: ResolveInfo, pipeline_selector: PipelineSelector
+    graphene_info: ResolveInfo, pipeline_selector: JobSubsetSelector
 ) -> Sequence["GrapheneSensor"]:
     from ..schema.sensors import GrapheneSensor
 
-    check.inst_param(pipeline_selector, "pipeline_selector", PipelineSelector)
+    check.inst_param(pipeline_selector, "pipeline_selector", JobSubsetSelector)
 
     location = graphene_info.context.get_code_location(pipeline_selector.location_name)
     repository = location.get_repository(pipeline_selector.repository_name)
     external_sensors = repository.get_external_sensors()
 
     results = []
     for external_sensor in external_sensors:
-        if pipeline_selector.pipeline_name not in [
-            target.pipeline_name for target in external_sensor.get_external_targets()
+        if pipeline_selector.job_name not in [
+            target.job_name for target in external_sensor.get_external_targets()
         ]:
             continue
 
         sensor_state = graphene_info.context.instance.get_instigator_state(
             external_sensor.get_external_origin_id(),
             external_sensor.selector_id,
         )
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dagster._core.host_representation import ExternalRepository
 from dagster._core.host_representation.external_data import (
     ExternalAssetDependedBy,
     ExternalAssetDependency,
     ExternalAssetNode,
 )
 from dagster._core.scheduler.instigation import InstigatorState, InstigatorType
-from dagster._core.storage.pipeline_run import JobBucket, RunRecord, RunsFilter, TagBucket
+from dagster._core.storage.dagster_run import JobBucket, RunRecord, RunsFilter, TagBucket
 from dagster._core.storage.tags import REPOSITORY_LABEL_TAG, SCHEDULE_NAME_TAG, SENSOR_NAME_TAG
 from dagster._core.workspace.context import WorkspaceRequestContext
 
 
 class RepositoryDataType(Enum):
     JOB_RUNS = "job_runs"
     SCHEDULE_RUNS = "schedule_runs"
@@ -81,25 +81,25 @@
             else:
                 records = []
                 for job_name in job_names:
                     records.extend(
                         list(
                             self._instance.get_run_records(
                                 filters=RunsFilter(
-                                    pipeline_name=job_name,
+                                    job_name=job_name,
                                     tags={
                                         REPOSITORY_LABEL_TAG: self._repository.get_external_origin().get_label(),
                                     },
                                 ),
                                 limit=limit,
                             )
                         )
                     )
             for record in records:
-                fetched[record.dagster_run.pipeline_name].append(record)
+                fetched[record.dagster_run.job_name].append(record)
 
         elif data_type == RepositoryDataType.SCHEDULE_RUNS:
             schedule_names = [
                 schedule.name for schedule in self._repository.get_external_schedules()
             ]
             if self._instance.supports_bucket_queries and len(schedule_names) > 1:
                 records = self._instance.get_run_records(
@@ -349,81 +349,93 @@
     @lru_cache(maxsize=1)
     def _build_cross_repo_deps(
         self,
     ) -> Tuple[
         Dict[AssetKey, ExternalAssetNode],
         Dict[Tuple[str, str], Dict[AssetKey, List[ExternalAssetDependedBy]]],
     ]:
-        """This method constructs a sink asset as an ExternalAssetNode for every asset immediately
-        downstream of a source asset that is defined in another repository as a derived asset.
-
-        In Dagit, sink assets will display as ForeignAssets, which are external from the repository.
+        """For asset X, find all "sink assets" and define them as ExternalAssetNodes. A "sink asset" is
+        any asset that depends on X and exists in other repository. This enables displaying cross-repo
+        dependencies for a source asset in a given repository.
 
         This method also stores a mapping from source asset key to ExternalAssetDependedBy nodes
-        that depend on the asset with that key. When get_cross_repo_dependent_assets is called with a derived
-        asset's asset key and its location, all dependent ExternalAssetDependedBy nodes are returned.
+        that depend on that asset key. When get_cross_repo_dependent_assets is called with
+        a source asset key and its location, all dependent ExternalAssetDependedBy nodes outside of the
+        source asset location are returned.
         """
-        depended_by_assets_by_source_asset: Dict[AssetKey, List[ExternalAssetDependedBy]] = {}
+        depended_by_assets_by_location_by_source_asset: Dict[
+            AssetKey, Dict[Tuple[str, str], List[ExternalAssetDependedBy]]
+        ] = defaultdict(lambda: defaultdict(list))
 
-        map_defined_asset_to_location: Dict[
+        # A mapping containing all derived (non-source) assets and their location
+        map_derived_asset_to_location: Dict[
             AssetKey, Tuple[str, str]
         ] = {}  # key is asset key, value is tuple (location_name, repo_name)
 
-        external_asset_node_by_asset_key: Dict[
-            AssetKey, ExternalAssetNode
-        ] = {}  # only contains derived assets
         for location in self._context.code_locations:
             repositories = location.get_repositories()
             for repo_name, external_repo in repositories.items():
                 asset_nodes = external_repo.get_external_asset_nodes()
                 for asset_node in asset_nodes:
+                    location_tuple = (location.name, repo_name)
                     if not asset_node.op_name:  # is source asset
-                        if asset_node.asset_key not in depended_by_assets_by_source_asset:
-                            depended_by_assets_by_source_asset[asset_node.asset_key] = []
-                        depended_by_assets_by_source_asset[asset_node.asset_key].extend(
-                            asset_node.depended_by
-                        )
-                    else:
-                        map_defined_asset_to_location[asset_node.asset_key] = (
-                            location.name,
-                            repo_name,
-                        )
-                        external_asset_node_by_asset_key[asset_node.asset_key] = asset_node
+                        depended_by_assets_by_location_by_source_asset[asset_node.asset_key][
+                            location_tuple
+                        ].extend(asset_node.depended_by)
+                    else:  # derived asset
+                        map_derived_asset_to_location[asset_node.asset_key] = location_tuple
 
         sink_assets: Dict[AssetKey, ExternalAssetNode] = {}
         external_asset_deps: Dict[
             Tuple[str, str], Dict[AssetKey, List[ExternalAssetDependedBy]]
-        ] = (
-            {}
+        ] = defaultdict(
+            lambda: defaultdict(list)
         )  # nested dict that maps dependedby assets by asset key by location tuple (repo_location.name, repo_name)
 
-        for source_asset, depended_by_assets in depended_by_assets_by_source_asset.items():
-            asset_def_location = map_defined_asset_to_location.get(source_asset, None)
-            if asset_def_location:  # source asset is defined as asset in another repository
-                if asset_def_location not in external_asset_deps:
-                    external_asset_deps[asset_def_location] = {}
-                if source_asset not in external_asset_deps[asset_def_location]:
-                    external_asset_deps[asset_def_location][source_asset] = []
-                external_asset_deps[asset_def_location][source_asset].extend(depended_by_assets)
-                for asset in depended_by_assets:
-                    # SourceAssets defined as ExternalAssetNodes contain no definition data (e.g.
-                    # no output or partition definition data) and no job_names. Dagit displays
-                    # all ExternalAssetNodes with no job_names as foreign assets, so sink assets
-                    # are defined as ExternalAssetNodes with no definition data.
-                    sink_assets[asset.downstream_asset_key] = ExternalAssetNode(
-                        asset_key=asset.downstream_asset_key,
-                        dependencies=[
-                            ExternalAssetDependency(
-                                upstream_asset_key=source_asset,
-                                input_name=asset.input_name,
-                                output_name=asset.output_name,
-                            )
-                        ],
-                        depended_by=[],
+        for (
+            source_asset,
+            depended_by_assets_by_location,
+        ) in depended_by_assets_by_location_by_source_asset.items():
+            all_depended_by_assets = set()
+            for depended_by_assets in depended_by_assets_by_location.values():
+                all_depended_by_assets = all_depended_by_assets | set(depended_by_assets)
+
+            # source_asset_locations contains a list of all locations where the source asset is defined,
+            # including the location where it is defined as a derived asset
+            source_asset_locations = set(depended_by_assets_by_location.keys())
+            if source_asset in map_derived_asset_to_location:
+                source_asset_locations.add(map_derived_asset_to_location[source_asset])
+
+            for source_asset_location in source_asset_locations:
+                # Map each source asset location and asset key to all assets outside of that location
+                # that depend on the source asset
+                external_asset_deps[source_asset_location][source_asset].extend(
+                    list(
+                        all_depended_by_assets
+                        - set(depended_by_assets_by_location[source_asset_location])
                     )
+                )
+
+            for asset in all_depended_by_assets:
+                # SourceAssets defined as ExternalAssetNodes contain no definition data (e.g.
+                # no output or partition definition data) and no job_names. Dagit displays
+                # all ExternalAssetNodes with no job_names as foreign assets, so sink assets
+                # are defined as ExternalAssetNodes with no definition data.
+                sink_assets[asset.downstream_asset_key] = ExternalAssetNode(
+                    asset_key=asset.downstream_asset_key,
+                    dependencies=[
+                        ExternalAssetDependency(
+                            upstream_asset_key=source_asset,
+                            input_name=asset.input_name,
+                            output_name=asset.output_name,
+                        )
+                    ],
+                    depended_by=[],
+                )
+
         return sink_assets, external_asset_deps
 
     def get_sink_asset(self, asset_key: AssetKey) -> ExternalAssetNode:
         sink_assets, _ = self._build_cross_repo_deps()
         return sink_assets[asset_key]
 
     def get_cross_repo_dependent_assets(
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/run_config_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 from typing import TYPE_CHECKING, Mapping, Optional
 
 import dagster._check as check
 from dagster._config import validate_config_from_snap
-from dagster._core.host_representation import RepresentedPipeline
+from dagster._core.host_representation import RepresentedJob
 from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 
 from dagster_graphql.schema.errors import GrapheneModeNotFoundError
 from dagster_graphql.schema.util import ResolveInfo
 
-from .external import get_external_pipeline_or_raise
-from .utils import PipelineSelector, UserFacingGraphQLError, capture_error
+from .external import get_external_job_or_raise
+from .utils import JobSubsetSelector, UserFacingGraphQLError, capture_error
 
 if TYPE_CHECKING:
     from ..schema.pipelines.config import (
         GraphenePipelineConfigValidationValid,
     )
     from ..schema.run_config import GrapheneRunConfigSchema
 
 
 @capture_error
 def resolve_run_config_schema_or_error(
-    graphene_info: ResolveInfo, selector: PipelineSelector, mode: Optional[str] = None
+    graphene_info: ResolveInfo, selector: JobSubsetSelector, mode: Optional[str] = None
 ) -> "GrapheneRunConfigSchema":
     from ..schema.run_config import GrapheneRunConfigSchema
 
-    check.inst_param(selector, "selector", PipelineSelector)
+    check.inst_param(selector, "selector", JobSubsetSelector)
 
     # Mode has been eliminated from the definitions layer, so we perform a "shallow" check for
     # invalid mode. This is temporary and will be removed when the GQL API transitions to
     # job/op/graph.
     if mode and mode != DEFAULT_MODE_NAME:
         return GrapheneModeNotFoundError(selector=selector, mode=mode)
 
-    external_pipeline = get_external_pipeline_or_raise(graphene_info, selector)
+    external_job = get_external_job_or_raise(graphene_info, selector)
 
     return GrapheneRunConfigSchema(
-        represented_pipeline=external_pipeline,
+        represented_job=external_job,
         mode=DEFAULT_MODE_NAME,
     )
 
 
 @capture_error
 def resolve_is_run_config_valid(
     graphene_info: ResolveInfo,
-    represented_pipeline: RepresentedPipeline,
+    represented_pipeline: RepresentedJob,
     mode: str,
     run_config: Mapping[str, object],
 ) -> "GraphenePipelineConfigValidationValid":
     from ..schema.pipelines.config import (
         GraphenePipelineConfigValidationError,
         GraphenePipelineConfigValidationValid,
         GrapheneRunConfigValidationInvalid,
     )
 
-    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedPipeline)
+    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedJob)
     check.str_param(mode, "mode")
     check.dict_param(run_config, "run_config", key_type=str)
 
     mode_def_snap = represented_pipeline.get_mode_def_snap(mode)
 
     if not mode_def_snap.root_config_key:
         # historical pipeline with unknown environment type. blindly pass validation
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.3.3/dagster_graphql/implementation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     TypeVar,
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey
-from dagster._core.definitions.selector import GraphSelector, PipelineSelector
+from dagster._core.definitions.selector import GraphSelector, JobSubsetSelector
 from dagster._core.workspace.context import BaseWorkspaceRequestContext
 from dagster._utils.error import serializable_error_info_from_exc_info
 from typing_extensions import ParamSpec, TypeAlias
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.errors import GrapheneError, GraphenePythonError
     from dagster_graphql.schema.util import ResolveInfo
@@ -141,20 +141,20 @@
         message = "[{cls}] {message}".format(
             cls=error.__class__.__name__,
             message=error.message if hasattr(error, "message") else None,
         )
         super(UserFacingGraphQLError, self).__init__(message)
 
 
-def pipeline_selector_from_graphql(data: Mapping[str, Any]) -> PipelineSelector:
+def pipeline_selector_from_graphql(data: Mapping[str, Any]) -> JobSubsetSelector:
     asset_selection = cast(Optional[Iterable[Dict[str, List[str]]]], data.get("assetSelection"))
-    return PipelineSelector(
+    return JobSubsetSelector(
         location_name=data["repositoryLocationName"],
         repository_name=data["repositoryName"],
-        pipeline_name=data.get("pipelineName") or data.get("jobName"),  # type: ignore
+        job_name=data.get("pipelineName") or data.get("jobName"),  # type: ignore
         solid_selection=data.get("solidSelection"),
         asset_selection=[AssetKey.from_graphql_input(asset_key) for asset_key in asset_selection]
         if asset_selection
         else None,
     )
 
 
@@ -166,35 +166,35 @@
     )
 
 
 class ExecutionParams(
     NamedTuple(
         "_ExecutionParams",
         [
-            ("selector", PipelineSelector),
+            ("selector", JobSubsetSelector),
             ("run_config", Mapping[str, object]),
             ("mode", Optional[str]),
             ("execution_metadata", "ExecutionMetadata"),
             ("step_keys", Optional[Sequence[str]]),
         ],
     )
 ):
     def __new__(
         cls,
-        selector: PipelineSelector,
+        selector: JobSubsetSelector,
         run_config: Optional[Mapping[str, object]],
         mode: Optional[str],
         execution_metadata: "ExecutionMetadata",
         step_keys: Optional[Sequence[str]],
     ):
         check.opt_list_param(step_keys, "step_keys", of_type=str)
 
         return super(ExecutionParams, cls).__new__(
             cls,
-            selector=check.inst_param(selector, "selector", PipelineSelector),
+            selector=check.inst_param(selector, "selector", JobSubsetSelector),
             run_config=check.opt_mapping_param(run_config, "run_config", key_type=str),
             mode=check.opt_str_param(mode, "mode"),
             execution_metadata=check.inst_param(
                 execution_metadata, "execution_metadata", ExecutionMetadata
             ),
             step_keys=step_keys,
         )
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/asset_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.partition import CachingDynamicPartitionsLoader
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.event_api import EventRecordsFilter
 from dagster._core.events import DagsterEventType
 from dagster._core.host_representation import CodeLocation, ExternalRepository
-from dagster._core.host_representation.external import ExternalPipeline
+from dagster._core.host_representation.external import ExternalJob
 from dagster._core.host_representation.external_data import (
     ExternalAssetNode,
     ExternalDynamicPartitionsDefinitionData,
     ExternalMultiPartitionsDefinitionData,
     ExternalPartitionsDefinitionData,
     ExternalStaticPartitionsDefinitionData,
     ExternalTimeWindowPartitionsDefinitionData,
@@ -174,15 +174,15 @@
         name = "MaterializationUpstreamDataVersion"
 
 
 class GrapheneAssetNode(graphene.ObjectType):
     _depended_by_loader: Optional[CrossRepoAssetDependedByLoader]
     _external_asset_node: ExternalAssetNode
     _node_definition_snap: Optional[Union[GraphDefSnap, OpDefSnap]]
-    _external_pipeline: Optional[ExternalPipeline]
+    _external_job: Optional[ExternalJob]
     _external_repository: ExternalRepository
     _latest_materialization_loader: Optional[BatchMaterializationLoader]
     _stale_status_loader: Optional[StaleStatusLoader]
 
     # NOTE: properties/resolvers are listed alphabetically
     assetKey = graphene.NonNull(GrapheneAssetKey)
     assetMaterializations = graphene.Field(
@@ -282,15 +282,15 @@
             stale_status_loader,
             "stale_status_loader",
             StaleStatusLoader,
         )
         self._dynamic_partitions_loader = check.opt_inst_param(
             dynamic_partitions_loader, "dynamic_partitions_loader", CachingDynamicPartitionsLoader
         )
-        self._external_pipeline = None  # lazily loaded
+        self._external_job = None  # lazily loaded
         self._node_definition_snap = None  # lazily loaded
 
         super().__init__(
             id=get_unique_asset_id(
                 external_asset_node.asset_key, repository_location.name, external_repository.name
             ),
             assetKey=external_asset_node.asset_key,
@@ -316,36 +316,36 @@
     def stale_status_loader(self) -> StaleStatusLoader:
         loader = check.not_none(
             self._stale_status_loader,
             "stale_status_loader must exist in order to access data versioning information",
         )
         return loader
 
-    def get_external_pipeline(self) -> ExternalPipeline:
-        if self._external_pipeline is None:
+    def get_external_job(self) -> ExternalJob:
+        if self._external_job is None:
             check.invariant(
                 len(self._external_asset_node.job_names) >= 1,
                 "Asset must be part of at least one job",
             )
-            self._external_pipeline = self._external_repository.get_full_external_job(
+            self._external_job = self._external_repository.get_full_external_job(
                 self._external_asset_node.job_names[0]
             )
-        return self._external_pipeline
+        return self._external_job
 
     def get_node_definition_snap(
         self,
     ) -> Union[GraphDefSnap, OpDefSnap]:
         if self._node_definition_snap is None and len(self._external_asset_node.job_names) > 0:
             node_key = check.not_none(
                 self._external_asset_node.node_definition_name
                 # nodes serialized using an older Dagster version may not have node_definition_name
                 or self._external_asset_node.graph_name
                 or self._external_asset_node.op_name
             )
-            self._node_definition_snap = self.get_external_pipeline().get_node_def_snap(node_key)
+            self._node_definition_snap = self.get_external_job().get_node_def_snap(node_key)
         # weird mypy bug causes mistyped _node_definition_snap
         return check.not_none(self._node_definition_snap)
 
     def get_partition_keys(
         self,
         partitions_def_data: Optional[ExternalPartitionsDefinitionData] = None,
         start_idx: Optional[int] = None,
@@ -382,20 +382,17 @@
                     and end_idx
                     and isinstance(partitions_def_data, ExternalTimeWindowPartitionsDefinitionData)
                 ):
                     return partitions_def_data.get_partitions_definition().get_partition_keys_between_indexes(
                         start_idx, end_idx
                     )
                 else:
-                    return [
-                        partition.name
-                        for partition in partitions_def_data.get_partitions_definition().get_partitions(
-                            dynamic_partitions_store=self._dynamic_partitions_loader
-                        )
-                    ]
+                    return partitions_def_data.get_partitions_definition().get_partition_keys(
+                        dynamic_partitions_store=self._dynamic_partitions_loader
+                    )
             elif isinstance(partitions_def_data, ExternalDynamicPartitionsDefinitionData):
                 return self._dynamic_partitions_loader.get_dynamic_partitions(
                     partitions_def_name=partitions_def_data.name
                 )
             else:
                 raise DagsterInvariantViolationError(
                     f"Unsupported partition definition type {partitions_def_data}"
@@ -419,15 +416,15 @@
         self, node_def_snap: Union[GraphDefSnap, OpDefSnap]
     ) -> Sequence[str]:
         if isinstance(node_def_snap, GraphDefSnap):
             constituent_node_names = [
                 inv.node_def_name
                 for inv in node_def_snap.dep_structure_snapshot.node_invocation_snaps
             ]
-            external_pipeline = self.get_external_pipeline()
+            external_pipeline = self.get_external_job()
             constituent_resource_key_sets = [
                 self.get_required_resource_keys_rec(external_pipeline.get_node_def_snap(name))
                 for name in constituent_node_names
             ]
             return [key for res_key_set in constituent_resource_key_sets for key in res_key_set]
         else:
             return node_def_snap.required_resource_keys
@@ -559,15 +556,15 @@
                 limit=limit,
             )
         ]
 
     def resolve_configField(self, _graphene_info: ResolveInfo) -> Optional[GrapheneConfigTypeField]:
         if self.is_source_asset():
             return None
-        external_pipeline = self.get_external_pipeline()
+        external_pipeline = self.get_external_job()
         node_def_snap = self.get_node_definition_snap()
         return (
             GrapheneConfigTypeField(
                 config_schema_snapshot=external_pipeline.config_schema_snapshot,
                 field_snap=node_def_snap.config_field_snap,
             )
             if node_def_snap.config_field_snap
@@ -882,15 +879,15 @@
         return list(iterate_metadata_entries(self._external_asset_node.metadata))
 
     def resolve_op(
         self, _graphene_info: ResolveInfo
     ) -> Optional[Union[GrapheneSolidDefinition, GrapheneCompositeSolidDefinition]]:
         if self.is_source_asset():
             return None
-        external_pipeline = self.get_external_pipeline()
+        external_pipeline = self.get_external_job()
         node_def_snap = self.get_node_definition_snap()
         if isinstance(node_def_snap, OpDefSnap):
             return GrapheneSolidDefinition(external_pipeline, node_def_snap.name)
 
         if isinstance(node_def_snap, GraphDefSnap):
             return GrapheneCompositeSolidDefinition(external_pipeline, node_def_snap.name)
 
@@ -974,21 +971,21 @@
     ) -> Optional[
         Union[
             "GrapheneListDagsterType", "GrapheneNullableDagsterType", "GrapheneRegularDagsterType"
         ]
     ]:
         if self.is_source_asset():
             return None
-        external_pipeline = self.get_external_pipeline()
+        external_pipeline = self.get_external_job()
         output_name = self.external_asset_node.output_name
         if output_name:
             for output_def in self.get_node_definition_snap().output_def_snaps:
                 if output_def.name == output_name:
                     return to_dagster_type(
-                        external_pipeline.pipeline_snapshot,
+                        external_pipeline.job_snapshot,
                         output_def.dagster_type_key,
                     )
         return None
 
 
 class GrapheneAssetGroup(graphene.ObjectType):
     groupName = graphene.NonNull(graphene.String)
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/backfill.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from typing import TYPE_CHECKING, Optional, Sequence
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.time_window_partitions import (
     TimeWindowPartitionsSubset,
 )
+from dagster._core.execution.asset_backfill import (
+    AssetBackfillStatus,
+    PartitionedAssetBackfillStatus,
+    UnpartitionedAssetBackfillStatus,
+)
 from dagster._core.execution.backfill import (
-    BackfillPartitionsStatus,
     BulkActionStatus,
     PartitionBackfill,
 )
 from dagster._core.host_representation.external import ExternalPartitionSet
-from dagster._core.storage.pipeline_run import RunPartitionData, RunRecord, RunsFilter
+from dagster._core.storage.dagster_run import RunPartitionData, RunRecord, RunsFilter
 from dagster._core.storage.tags import BACKFILL_ID_TAG
 from dagster._core.workspace.permissions import Permissions
 
 from ..implementation.fetch_partition_sets import (
     partition_status_counts_from_run_partition_data,
     partition_statuses_from_run_partition_data,
 )
@@ -109,16 +113,16 @@
         name = "BulkActionStatus"
 
 
 class GrapheneAssetBackfillData(graphene.ObjectType):
     class Meta:
         name = "AssetBackfillData"
 
-    assetPartitionsStatusCounts = non_null_list(
-        "dagster_graphql.schema.partition_sets.GrapheneAssetPartitionsStatusCounts"
+    assetBackfillStatuses = non_null_list(
+        "dagster_graphql.schema.partition_sets.GrapheneAssetBackfillStatus"
     )
     rootAssetTargetedRanges = graphene.List(
         graphene.NonNull("dagster_graphql.schema.partition_sets.GraphenePartitionKeyRange")
     )
     rootAssetTargetedPartitions = graphene.List(graphene.NonNull(graphene.String))
 
 
@@ -291,39 +295,62 @@
             partition_run_data,
             check.not_none(self._backfill_job.get_partition_names(graphene_info.context)),
         )
 
     def resolve_isAssetBackfill(self, _graphene_info: ResolveInfo) -> bool:
         return self._backfill_job.is_asset_backfill
 
-    def resolve_assetBackfillData(self, graphene_info: ResolveInfo) -> GrapheneAssetBackfillData:
+    def resolve_assetBackfillData(
+        self, graphene_info: ResolveInfo
+    ) -> Optional[GrapheneAssetBackfillData]:
         from dagster_graphql.schema.partition_sets import (
             GrapheneAssetPartitionsStatusCounts,
             GraphenePartitionKeyRange,
+            GrapheneUnpartitionedAssetStatus,
         )
 
-        status_counts_by_asset = (
-            self._backfill_job.get_partitions_status_counts_and_totals_by_asset(
-                graphene_info.context
-            )
+        if not self._backfill_job.is_asset_backfill:
+            return None
+
+        status_per_asset = self._backfill_job.get_backfill_status_per_asset_key(
+            graphene_info.context
         )
 
         asset_partition_status_counts = []
 
-        for asset_key, asset_status in status_counts_by_asset.items():
-            (counts_by_status, total_num_partitions) = asset_status
-            asset_partition_status_counts.append(
-                GrapheneAssetPartitionsStatusCounts(
-                    assetKey=asset_key,
-                    numPartitionsTargeted=total_num_partitions,
-                    numPartitionsRequested=counts_by_status[BackfillPartitionsStatus.REQUESTED],
-                    numPartitionsCompleted=counts_by_status[BackfillPartitionsStatus.COMPLETED],
-                    numPartitionsFailed=counts_by_status[BackfillPartitionsStatus.FAILED],
+        for asset_status in status_per_asset:
+            if isinstance(asset_status, PartitionedAssetBackfillStatus):
+                asset_partition_status_counts.append(
+                    GrapheneAssetPartitionsStatusCounts(
+                        assetKey=asset_status.asset_key,
+                        numPartitionsTargeted=asset_status.num_targeted_partitions,
+                        numPartitionsInProgress=asset_status.partitions_counts_by_status[
+                            AssetBackfillStatus.IN_PROGRESS
+                        ],
+                        numPartitionsMaterialized=asset_status.partitions_counts_by_status[
+                            AssetBackfillStatus.MATERIALIZED
+                        ],
+                        numPartitionsFailed=asset_status.partitions_counts_by_status[
+                            AssetBackfillStatus.FAILED
+                        ],
+                    )
+                )
+            else:
+                if not isinstance(asset_status, UnpartitionedAssetBackfillStatus):
+                    check.failed(f"Unexpected asset status type {type(asset_status)}")
+
+                asset_partition_status_counts.append(
+                    GrapheneUnpartitionedAssetStatus(
+                        assetKey=asset_status.asset_key,
+                        inProgress=asset_status.backfill_status is AssetBackfillStatus.IN_PROGRESS,
+                        materialized=asset_status.backfill_status
+                        is AssetBackfillStatus.MATERIALIZED,
+                        failed=asset_status.backfill_status is AssetBackfillStatus.FAILED,
+                    )
                 )
-            )
 
         root_partitions_subset = self._backfill_job.get_target_root_partitions_subset(
             graphene_info.context
         )
 
         if not root_partitions_subset:
             root_targeted_ranges = None
@@ -335,15 +362,15 @@
             ]
             root_targeted_partitions = None
         else:  # Default partitions subset
             root_targeted_ranges = None
             root_targeted_partitions = root_partitions_subset.get_partition_keys()
 
         return GrapheneAssetBackfillData(
-            assetPartitionsStatusCounts=asset_partition_status_counts,
+            assetBackfillStatuses=asset_partition_status_counts,
             rootAssetTargetedRanges=root_targeted_ranges,
             rootAssetTargetedPartitions=root_targeted_partitions,
         )
 
     def resolve_error(self, _graphene_info: ResolveInfo) -> Optional[GraphenePythonError]:
         if self._backfill_job.error:
             return GraphenePythonError(self._backfill_job.error)
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/dagster_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, Optional, Union
 
 import dagster._check as check
 import graphene
-from dagster._core.snap import PipelineSnapshot
+from dagster._core.snap import JobSnapshot
 from dagster._core.snap.dagster_types import DagsterTypeSnap
 from dagster._core.types.dagster_type import DagsterTypeKind
 from typing_extensions import TypeAlias
 
 from dagster_graphql.implementation.events import iterate_metadata_entries
 from dagster_graphql.schema.metadata import GrapheneMetadataEntry
 
@@ -20,25 +20,25 @@
 
 GrapheneDagsterTypeUnion: TypeAlias = Union[
     "GrapheneListDagsterType", "GrapheneNullableDagsterType", "GrapheneRegularDagsterType"
 ]
 
 
 def config_type_for_schema(
-    pipeline_snapshot: PipelineSnapshot, schema_key: Optional[str]
+    pipeline_snapshot: JobSnapshot, schema_key: Optional[str]
 ) -> Optional[GrapheneConfigTypeUnion]:
     return (
         to_config_type(pipeline_snapshot.config_schema_snapshot, schema_key) if schema_key else None
     )
 
 
 def to_dagster_type(
-    pipeline_snapshot: PipelineSnapshot, dagster_type_key: str
+    pipeline_snapshot: JobSnapshot, dagster_type_key: str
 ) -> GrapheneDagsterTypeUnion:
-    check.inst_param(pipeline_snapshot, "pipeline_snapshot", PipelineSnapshot)
+    check.inst_param(pipeline_snapshot, "pipeline_snapshot", JobSnapshot)
     check.str_param(dagster_type_key, "dagster_type_key")
 
     dagster_type_meta: DagsterTypeSnap = (
         pipeline_snapshot.dagster_type_namespace_snapshot.get_dagster_type_snap(dagster_type_key)
     )
 
     base_args: Dict[str, Any] = dict(
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/errors.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,24 +194,24 @@
         name = "PipelineNotFoundError"
 
     pipeline_name = graphene.NonNull(graphene.String)
     repository_name = graphene.NonNull(graphene.String)
     repository_location_name = graphene.NonNull(graphene.String)
 
     def __init__(self, selector):
-        from ..implementation.utils import PipelineSelector
+        from ..implementation.utils import JobSubsetSelector
 
         super().__init__()
-        check.inst_param(selector, "selector", PipelineSelector)
-        self.pipeline_name = selector.pipeline_name
+        check.inst_param(selector, "selector", JobSubsetSelector)
+        self.pipeline_name = selector.job_name
         self.repository_name = selector.repository_name
         self.repository_location_name = selector.location_name
         self.message = (
             "Could not find Pipeline "
-            f"{selector.location_name}.{selector.repository_name}.{selector.pipeline_name}"
+            f"{selector.location_name}.{selector.repository_name}.{selector.job_name}"
         )
 
 
 class GrapheneGraphNotFoundError(graphene.ObjectType):
     class Meta:
         interfaces = (GrapheneError,)
         name = "GraphNotFoundError"
@@ -285,15 +285,15 @@
         name = "PresetNotFoundError"
 
     preset = graphene.NonNull(graphene.String)
 
     def __init__(self, preset, selector):
         super().__init__()
         self.preset = check.str_param(preset, "preset")
-        self.message = f"Preset {preset} not found in pipeline {selector.pipeline_name}."
+        self.message = f"Preset {preset} not found in pipeline {selector.job_name}."
 
 
 class GrapheneConflictingExecutionParamsError(graphene.ObjectType):
     class Meta:
         interfaces = (GrapheneError,)
         name = "ConflictingExecutionParamsError"
 
@@ -310,15 +310,15 @@
         name = "ModeNotFoundError"
 
     mode = graphene.NonNull(graphene.String)
 
     def __init__(self, mode, selector):
         super().__init__()
         self.mode = check.str_param(mode, "mode")
-        self.message = f"Mode {mode} not found in pipeline {selector.pipeline_name}."
+        self.message = f"Mode {mode} not found in pipeline {selector.job_name}."
 
 
 class GrapheneNoModeProvidedError(graphene.ObjectType):
     class Meta:
         interfaces = (GrapheneError,)
         name = "NoModeProvidedError"
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/execution.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/external.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import graphene
 import pendulum
-from dagster._core.storage.pipeline_run import DagsterRunStatus, RunsFilter
+from dagster._core.storage.dagster_run import DagsterRunStatus, RunsFilter
 
 from .pipelines.status import GrapheneRunStatus
 from .runs import GrapheneRunConfigData
 from .util import non_null_list
 
 
 class GrapheneAssetKeyInput(graphene.InputObjectType):
@@ -49,15 +49,15 @@
             statuses = None
 
         updated_after = pendulum.from_timestamp(self.updatedAfter) if self.updatedAfter else None
         created_before = pendulum.from_timestamp(self.createdBefore) if self.createdBefore else None
 
         return RunsFilter(
             run_ids=self.runIds if self.runIds else None,
-            pipeline_name=self.pipelineName,
+            job_name=self.pipelineName,
             tags=tags,
             statuses=statuses,
             snapshot_id=self.snapshotId,
             updated_after=updated_after,
             created_before=created_before,
         )
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/instance.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/instigation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import sys
 import warnings
 from typing import Optional, Union
 
 import dagster._check as check
 import graphene
 import pendulum
-from dagster._core.definitions.run_request import RunRequest
+from dagster._core.definitions.run_request import (
+    AddDynamicPartitionsRequest,
+    DeleteDynamicPartitionsRequest,
+    RunRequest,
+)
 from dagster._core.definitions.schedule_definition import ScheduleExecutionData
 from dagster._core.definitions.selector import ScheduleSelector, SensorSelector
 from dagster._core.definitions.sensor_definition import SensorExecutionData
 from dagster._core.scheduler.instigation import (
     InstigatorState,
     InstigatorTick,
     InstigatorType,
     ScheduleInstigatorData,
     SensorInstigatorData,
     TickStatus,
 )
-from dagster._core.storage.pipeline_run import DagsterRun, RunsFilter
+from dagster._core.storage.dagster_run import DagsterRun, RunsFilter
 from dagster._core.storage.tags import REPOSITORY_LABEL_TAG, TagType, get_tag_type
 from dagster._core.workspace.permissions import Permissions
 from dagster._seven.compat.pendulum import to_timezone
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.yaml_utils import dump_run_config_yaml
 
 from dagster_graphql.schema.asset_key import GrapheneAssetKey
@@ -123,14 +127,45 @@
         name = "InstigationEventConnection"
 
     events = non_null_list(GrapheneInstigationEvent)
     cursor = graphene.NonNull(graphene.String)
     hasMore = graphene.NonNull(graphene.Boolean)
 
 
+class GrapheneDynamicPartitionsRequestType(graphene.Enum):
+    ADD_PARTITIONS = "ADD_PARTITIONS"
+    DELETE_PARTITIONS = "DELETE_PARTITIONS"
+
+    class Meta:
+        name = "DynamicPartitionsRequestType"
+
+
+class GrapheneDynamicPartitionsRequest(graphene.ObjectType):
+    partitionKeys = graphene.List(graphene.NonNull(graphene.String))
+    partitionsDefName = graphene.NonNull(graphene.String)
+    type = graphene.NonNull(GrapheneDynamicPartitionsRequestType)
+
+    class Meta:
+        name = "DynamicPartitionRequest"
+
+    def __init__(
+        self,
+        dynamic_partition_request: Union[
+            AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest
+        ],
+    ):
+        super().__init__(
+            type=GrapheneDynamicPartitionsRequestType.ADD_PARTITIONS
+            if isinstance(dynamic_partition_request, AddDynamicPartitionsRequest)
+            else GrapheneDynamicPartitionsRequestType.DELETE_PARTITIONS,
+            partitionKeys=dynamic_partition_request.partition_keys,
+            partitionsDefName=dynamic_partition_request.partitions_def_name,
+        )
+
+
 class GrapheneInstigationTick(graphene.ObjectType):
     id = graphene.NonNull(graphene.ID)
     status = graphene.NonNull(GrapheneInstigationTickStatus)
     timestamp = graphene.NonNull(graphene.Float)
     runIds = non_null_list(graphene.String)
     runKeys = non_null_list(graphene.String)
     error = graphene.Field(GraphenePythonError)
@@ -263,19 +298,22 @@
             except Exception:
                 schedule_data = serializable_error_info_from_exc_info(sys.exc_info())
 
             return GrapheneTickEvaluation(schedule_data)
 
 
 class GrapheneTickEvaluation(graphene.ObjectType):
+    dynamicPartitionsRequests = graphene.List(graphene.NonNull(GrapheneDynamicPartitionsRequest))
     runRequests = graphene.List(lambda: graphene.NonNull(GrapheneRunRequest))
     skipReason = graphene.String()
     error = graphene.Field(GraphenePythonError)
     cursor = graphene.String()
 
+    _execution_data: Union[ScheduleExecutionData, SensorExecutionData, SerializableErrorInfo]
+
     class Meta:
         name = "TickEvaluation"
 
     def __init__(self, execution_data):
         check.inst_param(
             execution_data,
             "execution_data",
@@ -287,21 +325,33 @@
             else None
         )
         skip_reason = (
             execution_data.skip_message
             if not isinstance(execution_data, SerializableErrorInfo)
             else None
         )
+        self._execution_data = execution_data
         self._run_requests = (
             execution_data.run_requests
             if not isinstance(execution_data, SerializableErrorInfo)
             else None
         )
+        dynamicPartitionsRequests = None
+        if isinstance(execution_data, SensorExecutionData):
+            dynamicPartitionsRequests = [
+                GrapheneDynamicPartitionsRequest(request)
+                for request in execution_data.dynamic_partitions_requests
+            ]
         cursor = execution_data.cursor if isinstance(execution_data, SensorExecutionData) else None
-        super().__init__(skipReason=skip_reason, error=error, cursor=cursor)
+        super().__init__(
+            skipReason=skip_reason,
+            error=error,
+            cursor=cursor,
+            dynamicPartitionsRequests=dynamicPartitionsRequests,
+        )
 
     def resolve_runRequests(self, _graphene_info: ResolveInfo):
         if not self._run_requests:
             return self._run_requests
 
         return [GrapheneRunRequest(run_request) for run_request in self._run_requests]
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/logs/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,20 +293,22 @@
 
 class GrapheneLogsCapturedEvent(graphene.ObjectType):
     class Meta:
         interfaces = (GrapheneMessageEvent,)
         name = "LogsCapturedEvent"
 
     fileKey = graphene.NonNull(graphene.String)
-    # legacy name for compute log file key... required for back-compat reasons, but has been
-    # renamed to fileKey for newer versions of dagit
-    logKey = graphene.NonNull(graphene.String)
     stepKeys = graphene.List(graphene.NonNull(graphene.String))
     externalUrl = graphene.String()
+    externalStdoutUrl = graphene.String()
+    externalStderrUrl = graphene.String()
     pid = graphene.Int()
+    # legacy name for compute log file key... required for back-compat reasons, but has been
+    # renamed to fileKey for newer versions of dagit
+    logKey = graphene.NonNull(graphene.String)
 
 
 def _construct_asset_event_metadata_params(event, metadata):
     metadata_params = {"label": metadata.label, "description": metadata.description}
     metadata_params.update(construct_basic_params(event))
     return metadata_params
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/partition_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dagster._core.host_representation.external_data import (
     ExternalDynamicPartitionsDefinitionData,
     ExternalMultiPartitionsDefinitionData,
     ExternalPartitionsDefinitionData,
     ExternalStaticPartitionsDefinitionData,
     ExternalTimeWindowPartitionsDefinitionData,
 )
-from dagster._core.storage.pipeline_run import RunsFilter
+from dagster._core.storage.dagster_run import RunsFilter
 from dagster._core.storage.tags import PARTITION_NAME_TAG, PARTITION_SET_TAG
 from dagster._utils.merger import merge_dicts
 
 from dagster_graphql.implementation.fetch_partition_sets import (
     get_partition_by_name,
     get_partition_config,
     get_partition_set_partition_runs,
@@ -124,19 +124,35 @@
 
 class GrapheneAssetPartitionsStatusCounts(graphene.ObjectType):
     class Meta:
         name = "AssetPartitionsStatusCounts"
 
     assetKey = graphene.NonNull(GrapheneAssetKey)
     numPartitionsTargeted = graphene.NonNull(graphene.Int)
-    numPartitionsRequested = graphene.NonNull(graphene.Int)
-    numPartitionsCompleted = graphene.NonNull(graphene.Int)
+    numPartitionsInProgress = graphene.NonNull(graphene.Int)
+    numPartitionsMaterialized = graphene.NonNull(graphene.Int)
     numPartitionsFailed = graphene.NonNull(graphene.Int)
 
 
+class GrapheneUnpartitionedAssetStatus(graphene.ObjectType):
+    class Meta:
+        name = "UnpartitionedAssetStatus"
+
+    assetKey = graphene.NonNull(GrapheneAssetKey)
+    inProgress = graphene.NonNull(graphene.Boolean)
+    materialized = graphene.NonNull(graphene.Boolean)
+    failed = graphene.NonNull(graphene.Boolean)
+
+
+class GrapheneAssetBackfillStatus(graphene.Union):
+    class Meta:
+        types = (GrapheneAssetPartitionsStatusCounts, GrapheneUnpartitionedAssetStatus)
+        name = "AssetBackfillStatus"
+
+
 class GraphenePartitionKeyRange(graphene.ObjectType):
     class Meta:
         name = "PartitionKeyRange"
 
     start = graphene.NonNull(graphene.String)
     end = graphene.NonNull(graphene.String)
 
@@ -161,15 +177,20 @@
         limit=graphene.Int(),
     )
     status = graphene.Field(GrapheneRunStatus)
 
     class Meta:
         name = "Partition"
 
-    def __init__(self, external_repository_handle, external_partition_set, partition_name):
+    def __init__(
+        self,
+        external_repository_handle: RepositoryHandle,
+        external_partition_set: ExternalPartitionSet,
+        partition_name: str,
+    ):
         self._external_repository_handle = check.inst_param(
             external_repository_handle, "external_respository_handle", RepositoryHandle
         )
         self._external_partition_set = check.inst_param(
             external_partition_set, "external_partition_set", ExternalPartitionSet
         )
         self._partition_name = check.str_param(partition_name, "partition_name")
@@ -208,15 +229,15 @@
             PARTITION_SET_TAG: self._external_partition_set.name,
             PARTITION_NAME_TAG: self._partition_name,
         }
         if filter is not None:
             selector = filter.to_selector()
             runs_filter = RunsFilter(
                 run_ids=selector.run_ids,
-                pipeline_name=selector.job_name,
+                job_name=selector.job_name,
                 statuses=selector.statuses,
                 tags=merge_dicts(selector.tags, partition_tags),
             )
         else:
             runs_filter = RunsFilter(tags=partition_tags)
 
         return get_runs(graphene_info, runs_filter, cursor=cursor, limit=limit)
@@ -256,25 +277,29 @@
         cursor=graphene.String(),
         limit=graphene.Int(),
     )
 
     class Meta:
         name = "PartitionSet"
 
-    def __init__(self, external_repository_handle, external_partition_set):
+    def __init__(
+        self,
+        external_repository_handle: RepositoryHandle,
+        external_partition_set: ExternalPartitionSet,
+    ):
         self._external_repository_handle = check.inst_param(
             external_repository_handle, "external_respository_handle", RepositoryHandle
         )
         self._external_partition_set = check.inst_param(
             external_partition_set, "external_partition_set", ExternalPartitionSet
         )
 
         super().__init__(
             name=external_partition_set.name,
-            pipeline_name=external_partition_set.pipeline_name,
+            pipeline_name=external_partition_set.job_name,
             solid_selection=external_partition_set.solid_selection,
             mode=external_partition_set.mode,
         )
 
     def resolve_id(self, _graphene_info: ResolveInfo):
         return self._external_partition_set.get_external_origin_id()
 
@@ -290,15 +315,15 @@
             self._external_repository_handle,
             self._external_partition_set,
             cursor=cursor,
             limit=limit,
             reverse=reverse or False,
         )
 
-    def resolve_partition(self, graphene_info: ResolveInfo, partition_name):
+    def resolve_partition(self, graphene_info: ResolveInfo, partition_name: str):
         return get_partition_by_name(
             graphene_info,
             self._external_repository_handle,
             self._external_partition_set,
             partition_name,
         )
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     FieldNotDefinedErrorData,
     FieldsNotDefinedErrorData,
     MissingFieldErrorData,
     MissingFieldsErrorData,
     RuntimeMismatchErrorData,
     SelectorTypeErrorData,
 )
-from dagster._core.host_representation.represented import RepresentedPipeline
+from dagster._core.host_representation.represented import RepresentedJob
 from dagster._utils.error import SerializableErrorInfo
 from graphene.types.generic import GenericScalar
 
 from ..config_types import GrapheneConfigTypeField
 from ..util import non_null_list
 
 
@@ -300,15 +300,15 @@
 
     class Meta:
         interfaces = (GraphenePipelineConfigValidationInvalid,)
         name = "RunConfigValidationInvalid"
 
     @staticmethod
     def for_validation_errors(represented_pipeline, errors):
-        check.inst_param(represented_pipeline, "represented_pipeline", RepresentedPipeline)
+        check.inst_param(represented_pipeline, "represented_pipeline", RepresentedJob)
         check.list_param(errors, "errors", of_type=DagsterEvaluationError)
         return GrapheneRunConfigValidationInvalid(
             pipeline_name=represented_pipeline.name,
             errors=[
                 GraphenePipelineConfigValidationError.from_dagster_error(
                     represented_pipeline.config_schema_snapshot, err
                 )
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/mode.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
     def __init__(self, config_schema_snapshot, pipeline_snapshot_id, mode_def_snap):
         super().__init__()
         self._mode_def_snap = check.inst_param(mode_def_snap, "mode_def_snap", ModeDefSnap)
         self._config_schema_snapshot = check.inst_param(
             config_schema_snapshot, "config_schema_snapshot", ConfigSchemaSnapshot
         )
-        self._pipeline_snapshot_id = pipeline_snapshot_id
+        self._job_snapshot_id = pipeline_snapshot_id
 
     def resolve_id(self, _graphene_info: ResolveInfo):
         return "{pipeline}-{mode}".format(
-            pipeline=self._pipeline_snapshot_id, mode=self._mode_def_snap.name
+            pipeline=self._job_snapshot_id, mode=self._mode_def_snap.name
         )
 
     def resolve_name(self, _graphene_info: ResolveInfo):
         return self._mode_def_snap.name
 
     def resolve_description(self, _graphene_info: ResolveInfo):
         return self._mode_def_snap.description
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import datetime
 from typing import List, Optional, Sequence
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.time_window_partitions import PartitionRangeStatus
 from dagster._core.events import DagsterEventType
-from dagster._core.host_representation.external import ExternalExecutionPlan, ExternalPipeline
+from dagster._core.host_representation.external import ExternalExecutionPlan, ExternalJob
 from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME, ExternalPresetData
-from dagster._core.storage.pipeline_run import (
+from dagster._core.host_representation.represented import RepresentedJob
+from dagster._core.storage.dagster_run import (
+    DagsterRunStatsSnapshot,
     DagsterRunStatus,
-    PipelineRunStatsSnapshot,
     RunRecord,
     RunsFilter,
 )
 from dagster._core.storage.tags import REPOSITORY_LABEL_TAG, TagType, get_tag_type
 from dagster._core.workspace.permissions import Permissions
 from dagster._utils import datetime_as_float
 from dagster._utils.yaml_utils import dump_run_config_yaml
 
 from dagster_graphql.implementation.events import iterate_metadata_entries
 from dagster_graphql.schema.metadata import GrapheneMetadataEntry
 
 from ...implementation.events import from_event_record
 from ...implementation.fetch_assets import get_assets_for_run_id, get_unique_asset_id
-from ...implementation.fetch_pipelines import get_pipeline_reference_or_raise
+from ...implementation.fetch_pipelines import get_job_reference_or_raise
 from ...implementation.fetch_runs import get_runs, get_stats, get_step_stats
 from ...implementation.fetch_schedules import get_schedules_for_pipeline
 from ...implementation.fetch_sensors import get_sensors_for_pipeline
 from ...implementation.loader import BatchRunLoader, RepositoryScopedBatchLoader
 from ...implementation.utils import UserFacingGraphQLError, capture_error
 from ..asset_key import GrapheneAssetKey
 from ..dagster_types import (
@@ -369,28 +370,28 @@
 
     class Meta:
         interfaces = (GraphenePipelineRun,)
         name = "Run"
 
     def __init__(self, record: RunRecord):
         check.inst_param(record, "record", RunRecord)
-        pipeline_run = record.dagster_run
+        dagster_run = record.dagster_run
         super().__init__(
-            runId=pipeline_run.run_id,
-            status=pipeline_run.status.value,
+            runId=dagster_run.run_id,
+            status=dagster_run.status.value,
             mode=DEFAULT_MODE_NAME,
         )
-        self._pipeline_run = pipeline_run
+        self.dagster_run = dagster_run
         self._run_record = record
-        self._run_stats: Optional[PipelineRunStatsSnapshot] = None
+        self._run_stats: Optional[DagsterRunStatsSnapshot] = None
 
     def _get_permission_value(self, permission: Permissions, graphene_info: ResolveInfo) -> bool:
         location_name = (
-            self._pipeline_run.external_pipeline_origin.location_name
-            if self._pipeline_run.external_pipeline_origin
+            self.dagster_run.external_job_origin.location_name
+            if self.dagster_run.external_job_origin
             else None
         )
 
         return (
             graphene_info.context.has_permission_for_location(permission, location_name)
             if location_name
             else graphene_info.context.has_permission(permission)
@@ -402,53 +403,52 @@
     def resolve_hasTerminatePermission(self, graphene_info: ResolveInfo):
         return self._get_permission_value(Permissions.TERMINATE_PIPELINE_EXECUTION, graphene_info)
 
     def resolve_hasDeletePermission(self, graphene_info: ResolveInfo):
         return self._get_permission_value(Permissions.DELETE_PIPELINE_RUN, graphene_info)
 
     def resolve_id(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.run_id
+        return self.dagster_run.run_id
 
     def resolve_repositoryOrigin(self, _graphene_info: ResolveInfo):
         return (
             GrapheneRepositoryOrigin(
-                self._pipeline_run.external_pipeline_origin.external_repository_origin
+                self.dagster_run.external_job_origin.external_repository_origin
             )
-            if self._pipeline_run.external_pipeline_origin
+            if self.dagster_run.external_job_origin
             else None
         )
 
     def resolve_pipeline(self, graphene_info: ResolveInfo):
-        return get_pipeline_reference_or_raise(graphene_info, self._pipeline_run)
+        return get_job_reference_or_raise(graphene_info, self.dagster_run)
 
     def resolve_pipelineName(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.pipeline_name
+        return self.dagster_run.job_name
 
     def resolve_jobName(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.pipeline_name
+        return self.dagster_run.job_name
 
     def resolve_solidSelection(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.solid_selection
+        return self.dagster_run.solid_selection
 
     def resolve_assetSelection(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.asset_selection
+        return self.dagster_run.asset_selection
 
     def resolve_resolvedOpSelection(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.solids_to_execute
+        return self.dagster_run.solids_to_execute
 
     def resolve_pipelineSnapshotId(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.pipeline_snapshot_id
+        return self.dagster_run.job_snapshot_id
 
     def resolve_parentPipelineSnapshotId(self, graphene_info: ResolveInfo):
-        pipeline_snapshot_id = self._pipeline_run.pipeline_snapshot_id
-        if (
-            pipeline_snapshot_id is not None
-            and graphene_info.context.instance.has_pipeline_snapshot(pipeline_snapshot_id)
+        pipeline_snapshot_id = self.dagster_run.job_snapshot_id
+        if pipeline_snapshot_id is not None and graphene_info.context.instance.has_job_snapshot(
+            pipeline_snapshot_id
         ):
-            snapshot = graphene_info.context.instance.get_pipeline_snapshot(pipeline_snapshot_id)
+            snapshot = graphene_info.context.instance.get_job_snapshot(pipeline_snapshot_id)
             if snapshot.lineage_snapshot is not None:
                 return snapshot.lineage_snapshot.parent_snapshot_id
         return None
 
     def resolve_stats(self, graphene_info: ResolveInfo):
         return get_stats(graphene_info, self.run_id)
 
@@ -461,66 +461,63 @@
     def resolve_capturedLogs(self, graphene_info: ResolveInfo, fileKey):
         compute_log_manager = get_compute_log_manager(graphene_info)
         log_key = compute_log_manager.build_log_key_for_run(self.run_id, fileKey)
         log_data = compute_log_manager.get_log_data(log_key)
         return from_captured_log_data(log_data)
 
     def resolve_executionPlan(self, graphene_info: ResolveInfo):
-        if not (
-            self._pipeline_run.execution_plan_snapshot_id
-            and self._pipeline_run.pipeline_snapshot_id
-        ):
+        if not (self.dagster_run.execution_plan_snapshot_id and self.dagster_run.job_snapshot_id):
             return None
 
         instance = graphene_info.context.instance
 
         execution_plan_snapshot = instance.get_execution_plan_snapshot(
-            self._pipeline_run.execution_plan_snapshot_id
+            self.dagster_run.execution_plan_snapshot_id
         )
         return (
             GrapheneExecutionPlan(
                 ExternalExecutionPlan(execution_plan_snapshot=execution_plan_snapshot)
             )
             if execution_plan_snapshot
             else None
         )
 
     def resolve_stepKeysToExecute(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.step_keys_to_execute
+        return self.dagster_run.step_keys_to_execute
 
     def resolve_runConfigYaml(self, _graphene_info: ResolveInfo):
-        return dump_run_config_yaml(self._pipeline_run.run_config)
+        return dump_run_config_yaml(self.dagster_run.run_config)
 
     def resolve_runConfig(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.run_config
+        return self.dagster_run.run_config
 
     def resolve_tags(self, _graphene_info: ResolveInfo):
         return [
             GraphenePipelineTag(key=key, value=value)
-            for key, value in self._pipeline_run.tags.items()
+            for key, value in self.dagster_run.tags.items()
             if get_tag_type(key) != TagType.HIDDEN
         ]
 
     def resolve_rootRunId(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.root_run_id
+        return self.dagster_run.root_run_id
 
     def resolve_parentRunId(self, _graphene_info: ResolveInfo):
-        return self._pipeline_run.parent_run_id
+        return self.dagster_run.parent_run_id
 
     @property
     def run_id(self):
         return self.runId
 
     def resolve_canTerminate(self, _graphene_info: ResolveInfo):
         # short circuit if the pipeline run is in a terminal state
-        if self._pipeline_run.is_finished:
+        if self.dagster_run.is_finished:
             return False
         return (
-            self._pipeline_run.status == DagsterRunStatus.QUEUED
-            or self._pipeline_run.status == DagsterRunStatus.STARTED
+            self.dagster_run.status == DagsterRunStatus.QUEUED
+            or self.dagster_run.status == DagsterRunStatus.STARTED
         )
 
     def resolve_assets(self, graphene_info: ResolveInfo):
         return get_assets_for_run_id(graphene_info, self.run_id)
 
     def resolve_assetMaterializations(self, graphene_info: ResolveInfo):
         # convenience field added for users querying directly via GraphQL
@@ -531,30 +528,30 @@
             )
         ]
 
     def resolve_eventConnection(self, graphene_info: ResolveInfo, afterCursor=None):
         conn = graphene_info.context.instance.get_records_for_run(self.run_id, cursor=afterCursor)
         return GrapheneEventConnection(
             events=[
-                from_event_record(record.event_log_entry, self._pipeline_run.pipeline_name)
+                from_event_record(record.event_log_entry, self.dagster_run.job_name)
                 for record in conn.records
             ],
             cursor=conn.cursor,
             hasMore=conn.has_more,
         )
 
     def _get_run_record(self, instance):
         if not self._run_record:
             self._run_record = instance.get_run_records(RunsFilter(run_ids=[self.run_id]))[0]
         return self._run_record
 
     def resolve_startTime(self, graphene_info: ResolveInfo):
         run_record = self._get_run_record(graphene_info.context.instance)
         # If a user has not migrated in 0.13.15, then run_record will not have start_time and end_time. So it will be necessary to fill this data using the run_stats. Since we potentially make this call multiple times, we cache the result.
-        if run_record.start_time is None and self._pipeline_run.status in STARTED_STATUSES:
+        if run_record.start_time is None and self.dagster_run.status in STARTED_STATUSES:
             # Short-circuit if pipeline failed to start, so it has an end time but no start time
             if run_record.end_time is not None:
                 return run_record.end_time
 
             if self._run_stats is None or self._run_stats.start_time is None:
                 self._run_stats = graphene_info.context.instance.get_run_stats(self.runId)
 
@@ -562,15 +559,15 @@
                 return self._run_stats.end_time
 
             return self._run_stats.start_time
         return run_record.start_time
 
     def resolve_endTime(self, graphene_info: ResolveInfo):
         run_record = self._get_run_record(graphene_info.context.instance)
-        if run_record.end_time is None and self._pipeline_run.status in COMPLETED_STATUSES:
+        if run_record.end_time is None and self.dagster_run.status in COMPLETED_STATUSES:
             if self._run_stats is None or self._run_stats.end_time is None:
                 self._run_stats = graphene_info.context.instance.get_run_stats(self.runId)
             return self._run_stats.end_time
         return run_record.end_time
 
     def resolve_updateTime(self, graphene_info: ResolveInfo):
         run_record = self._get_run_record(graphene_info.context.instance)
@@ -580,15 +577,15 @@
 
 class GrapheneIPipelineSnapshotMixin:
     # Mixin this class to implement IPipelineSnapshot
     #
     # Graphene has some strange properties that make it so that you cannot
     # implement ABCs nor use properties in an overridable way. So the way
     # the mixin works is that the target classes have to have a method
-    # get_represented_pipeline()
+    # get_represented_job()
     #
     name = graphene.NonNull(graphene.String)
     description = graphene.String()
     id = graphene.NonNull(graphene.ID)
     pipeline_snapshot_id = graphene.NonNull(graphene.String)
     dagster_types = non_null_list(GrapheneDagsterType)
     dagster_type_or_error = graphene.Field(
@@ -615,158 +612,158 @@
     sensors = non_null_list(GrapheneSensor)
     parent_snapshot_id = graphene.String()
     graph_name = graphene.NonNull(graphene.String)
 
     class Meta:
         name = "IPipelineSnapshotMixin"
 
-    def get_represented_pipeline(self):
+    def get_represented_job(self) -> RepresentedJob:
         raise NotImplementedError()
 
     def resolve_pipeline_snapshot_id(self, _graphene_info: ResolveInfo):
-        return self.get_represented_pipeline().identifying_pipeline_snapshot_id
+        return self.get_represented_job().identifying_job_snapshot_id
 
     def resolve_id(self, _graphene_info: ResolveInfo):
-        return self.get_represented_pipeline().identifying_pipeline_snapshot_id
+        return self.get_represented_job().identifying_job_snapshot_id
 
     def resolve_name(self, _graphene_info: ResolveInfo):
-        return self.get_represented_pipeline().name
+        return self.get_represented_job().name
 
     def resolve_description(self, _graphene_info: ResolveInfo):
-        return self.get_represented_pipeline().description
+        return self.get_represented_job().description
 
     def resolve_dagster_types(self, _graphene_info: ResolveInfo):
-        represented_pipeline = self.get_represented_pipeline()
+        represented_pipeline = self.get_represented_job()
         return sorted(
             list(
                 map(
-                    lambda dt: to_dagster_type(represented_pipeline.pipeline_snapshot, dt.key),
+                    lambda dt: to_dagster_type(represented_pipeline.job_snapshot, dt.key),
                     [t for t in represented_pipeline.dagster_type_snaps if t.name],
                 )
             ),
             key=lambda dagster_type: dagster_type.name,
         )
 
     @capture_error
     def resolve_dagster_type_or_error(
         self, _graphene_info: ResolveInfo, dagsterTypeName: str
     ) -> GrapheneDagsterTypeUnion:
-        represented_pipeline = self.get_represented_pipeline()
+        represented_pipeline = self.get_represented_job()
 
         if not represented_pipeline.has_dagster_type_named(dagsterTypeName):
             raise UserFacingGraphQLError(
                 GrapheneDagsterTypeNotFoundError(dagster_type_name=dagsterTypeName)
             )
 
         return to_dagster_type(
-            represented_pipeline.pipeline_snapshot,
+            represented_pipeline.job_snapshot,
             represented_pipeline.get_dagster_type_by_name(dagsterTypeName).key,
         )
 
     def resolve_solids(self, _graphene_info: ResolveInfo):
-        represented_pipeline = self.get_represented_pipeline()
+        represented_pipeline = self.get_represented_job()
         return build_solids(
             represented_pipeline,
             represented_pipeline.dep_structure_index,
         )
 
     def resolve_modes(self, _graphene_info: ResolveInfo):
-        represented_pipeline = self.get_represented_pipeline()
+        represented_pipeline = self.get_represented_job()
         return [
             GrapheneMode(
                 represented_pipeline.config_schema_snapshot,
-                represented_pipeline.identifying_pipeline_snapshot_id,
+                represented_pipeline.identifying_job_snapshot_id,
                 mode_def_snap,
             )
             for mode_def_snap in sorted(
                 represented_pipeline.mode_def_snaps, key=lambda item: item.name
             )
         ]
 
     def resolve_solid_handle(
         self, _graphene_info: ResolveInfo, handleID: str
     ) -> Optional[GrapheneSolidHandle]:
-        return build_solid_handles(self.get_represented_pipeline()).get(handleID)
+        return build_solid_handles(self.get_represented_job()).get(handleID)
 
     def resolve_solid_handles(
         self, _graphene_info: ResolveInfo, parentHandleID: Optional[str] = None
     ) -> Sequence[GrapheneSolidHandle]:
-        handles = build_solid_handles(self.get_represented_pipeline())
+        handles = build_solid_handles(self.get_represented_job())
 
         if parentHandleID == "":
             handles = {key: handle for key, handle in handles.items() if not handle.parent}
         elif parentHandleID is not None:
             handles = {
                 key: handle
                 for key, handle in handles.items()
                 if handle.parent and handle.parent.handleID.to_string() == parentHandleID
             }
 
         return [handles[key] for key in sorted(handles)]
 
     def resolve_tags(self, _graphene_info: ResolveInfo):
-        represented_pipeline = self.get_represented_pipeline()
+        represented_pipeline = self.get_represented_job()
         return [
             GraphenePipelineTag(key=key, value=value)
-            for key, value in represented_pipeline.pipeline_snapshot.tags.items()
+            for key, value in represented_pipeline.job_snapshot.tags.items()
         ]
 
     def resolve_metadata_entries(self, _graphene_info: ResolveInfo) -> List[GrapheneMetadataEntry]:
-        represented_pipeline = self.get_represented_pipeline()
-        return list(iterate_metadata_entries(represented_pipeline.pipeline_snapshot.metadata))
+        represented_pipeline = self.get_represented_job()
+        return list(iterate_metadata_entries(represented_pipeline.job_snapshot.metadata))
 
     def resolve_solidSelection(self, _graphene_info: ResolveInfo):
-        return self.get_represented_pipeline().solid_selection
+        return self.get_represented_job().solid_selection
 
     def resolve_runs(
         self, graphene_info: ResolveInfo, cursor: Optional[str] = None, limit: Optional[int] = None
     ) -> Sequence[GrapheneRun]:
-        pipeline = self.get_represented_pipeline()
-        if isinstance(pipeline, ExternalPipeline):
+        pipeline = self.get_represented_job()
+        if isinstance(pipeline, ExternalJob):
             runs_filter = RunsFilter(
-                pipeline_name=pipeline.name,
+                job_name=pipeline.name,
                 tags={
                     REPOSITORY_LABEL_TAG: pipeline.get_external_origin().external_repository_origin.get_label()
                 },
             )
         else:
-            runs_filter = RunsFilter(pipeline_name=pipeline.name)
+            runs_filter = RunsFilter(job_name=pipeline.name)
         return get_runs(graphene_info, runs_filter, cursor, limit)
 
     def resolve_schedules(self, graphene_info: ResolveInfo):
-        represented_pipeline = self.get_represented_pipeline()
-        if not isinstance(represented_pipeline, ExternalPipeline):
+        represented_pipeline = self.get_represented_job()
+        if not isinstance(represented_pipeline, ExternalJob):
             # this is an historical pipeline snapshot, so there are not any associated running
             # schedules
             return []
 
         pipeline_selector = represented_pipeline.handle.to_selector()
         schedules = get_schedules_for_pipeline(graphene_info, pipeline_selector)
         return schedules
 
     def resolve_sensors(self, graphene_info: ResolveInfo):
-        represented_pipeline = self.get_represented_pipeline()
-        if not isinstance(represented_pipeline, ExternalPipeline):
+        represented_pipeline = self.get_represented_job()
+        if not isinstance(represented_pipeline, ExternalJob):
             # this is an historical pipeline snapshot, so there are not any associated running
             # sensors
             return []
 
         pipeline_selector = represented_pipeline.handle.to_selector()
         sensors = get_sensors_for_pipeline(graphene_info, pipeline_selector)
         return sensors
 
     def resolve_parent_snapshot_id(self, _graphene_info: ResolveInfo):
-        lineage_snapshot = self.get_represented_pipeline().pipeline_snapshot.lineage_snapshot
+        lineage_snapshot = self.get_represented_job().job_snapshot.lineage_snapshot
         if lineage_snapshot:
             return lineage_snapshot.parent_snapshot_id
         else:
             return None
 
     def resolve_graph_name(self, _graphene_info: ResolveInfo):
-        return self.get_represented_pipeline().get_graph_name()
+        return self.get_represented_job().get_graph_name()
 
 
 class GrapheneIPipelineSnapshot(graphene.Interface):
     name = graphene.NonNull(graphene.String)
     description = graphene.String()
     pipeline_snapshot_id = graphene.NonNull(graphene.String)
     dagster_types = non_null_list(GrapheneDagsterType)
@@ -810,15 +807,15 @@
         name = "PipelinePreset"
 
     def __init__(self, active_preset_data, pipeline_name):
         super().__init__()
         self._active_preset_data = check.inst_param(
             active_preset_data, "active_preset_data", ExternalPresetData
         )
-        self._pipeline_name = check.str_param(pipeline_name, "pipeline_name")
+        self._job_name = check.str_param(pipeline_name, "pipeline_name")
 
     def resolve_name(self, _graphene_info: ResolveInfo):
         return self._active_preset_data.name
 
     def resolve_solidSelection(self, _graphene_info: ResolveInfo):
         return self._active_preset_data.solid_selection
 
@@ -843,82 +840,78 @@
     isAssetJob = graphene.NonNull(graphene.Boolean)
     repository = graphene.NonNull("dagster_graphql.schema.external.GrapheneRepository")
 
     class Meta:
         interfaces = (GrapheneSolidContainer, GrapheneIPipelineSnapshot)
         name = "Pipeline"
 
-    def __init__(self, external_pipeline, batch_loader=None):
+    def __init__(
+        self, external_job: ExternalJob, batch_loader: Optional[RepositoryScopedBatchLoader] = None
+    ):
         super().__init__()
-        self._external_pipeline = check.inst_param(
-            external_pipeline, "external_pipeline", ExternalPipeline
-        )
+        self._external_job = check.inst_param(external_job, "external_job", ExternalJob)
         # optional run loader, provided by a parent GrapheneRepository object that instantiates
         # multiple pipelines
         self._batch_loader = check.opt_inst_param(
             batch_loader, "batch_loader", RepositoryScopedBatchLoader
         )
 
     def resolve_id(self, _graphene_info: ResolveInfo):
-        return self._external_pipeline.get_external_origin_id()
+        return self._external_job.get_external_origin_id()
 
-    def get_represented_pipeline(self):
-        return self._external_pipeline
+    def get_represented_job(self) -> RepresentedJob:
+        return self._external_job
 
     def resolve_presets(self, _graphene_info: ResolveInfo):
         return [
-            GraphenePipelinePreset(preset, self._external_pipeline.name)
-            for preset in sorted(self._external_pipeline.active_presets, key=lambda item: item.name)
+            GraphenePipelinePreset(preset, self._external_job.name)
+            for preset in sorted(self._external_job.active_presets, key=lambda item: item.name)
         ]
 
     def resolve_isJob(self, _graphene_info: ResolveInfo):
         return True
 
     def resolve_isAssetJob(self, graphene_info: ResolveInfo):
-        handle = self._external_pipeline.repository_handle
+        handle = self._external_job.repository_handle
         location = graphene_info.context.get_code_location(handle.location_name)
         repository = location.get_repository(handle.repository_name)
-        return bool(repository.get_external_asset_nodes(self._external_pipeline.name))
+        return bool(repository.get_external_asset_nodes(self._external_job.name))
 
     def resolve_repository(self, graphene_info: ResolveInfo):
         from ..external import GrapheneRepository
 
-        handle = self._external_pipeline.repository_handle
+        handle = self._external_job.repository_handle
         location = graphene_info.context.get_code_location(handle.location_name)
         return GrapheneRepository(
             graphene_info.context.instance,
             location.get_repository(handle.repository_name),
             location,
         )
 
     def resolve_runs(
         self, graphene_info: ResolveInfo, cursor: Optional[str] = None, limit: Optional[int] = None
     ) -> Sequence[GrapheneRun]:
         # override the implementation to use the batch run loader
         if not cursor and limit and self._batch_loader:
-            records = self._batch_loader.get_run_records_for_job(
-                self._external_pipeline.name, limit
-            )
+            records = self._batch_loader.get_run_records_for_job(self._external_job.name, limit)
             return [GrapheneRun(record) for record in records]
 
         # otherwise, fall back to the default implementation
         return super().resolve_runs(graphene_info, cursor=cursor, limit=limit)
 
 
 class GrapheneJob(GraphenePipeline):
     class Meta:
         interfaces = (GrapheneSolidContainer, GrapheneIPipelineSnapshot)
         name = "Job"
 
     # doesn't inherit from base class
-    def __init__(self, external_pipeline, batch_loader=None):
+    def __init__(self, external_job, batch_loader=None):
         super().__init__()
-        self._external_pipeline = check.inst_param(
-            external_pipeline, "external_pipeline", ExternalPipeline
-        )
+        self._external_job = check.inst_param(external_job, "external_job", ExternalJob)
         # optional run loader, provided by a parent GrapheneRepository object that instantiates
         # multiple pipelines
         self._batch_loader = check.opt_inst_param(
             batch_loader, "batch_loader", RepositoryScopedBatchLoader
         )
 
 
@@ -937,15 +930,15 @@
     solid_handles = graphene.Field(
         non_null_list(GrapheneSolidHandle), parentHandleID=graphene.String()
     )
     modes = non_null_list(GrapheneMode)
 
     def __init__(self, external_pipeline, solid_handle_id=None):
         self._external_pipeline = check.inst_param(
-            external_pipeline, "external_pipeline", ExternalPipeline
+            external_pipeline, "external_pipeline", ExternalJob
         )
         self._solid_handle_id = check.opt_str_param(solid_handle_id, "solid_handle_id")
         super().__init__()
 
     def resolve_id(self, _graphene_info: ResolveInfo):
         if self._solid_handle_id:
             return (
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dagster._check as check
 import graphene
-from dagster._core.storage.pipeline_run import PipelineRunStatsSnapshot
+from dagster._core.storage.dagster_run import DagsterRunStatsSnapshot
 
 from ..errors import GraphenePythonError
 
 
 class GraphenePipelineRunStatsSnapshot(graphene.Interface):
     id = graphene.NonNull(graphene.String)
     runId = graphene.NonNull(graphene.String)
@@ -34,15 +34,15 @@
     endTime = graphene.Field(graphene.Float)
 
     class Meta:
         interfaces = (GraphenePipelineRunStatsSnapshot,)
         name = "RunStatsSnapshot"
 
     def __init__(self, stats):
-        self._stats = check.inst_param(stats, "stats", PipelineRunStatsSnapshot)
+        self._stats = check.inst_param(stats, "stats", DagsterRunStatsSnapshot)
         super().__init__(
             id="stats-" + self._stats.run_id,
             runId=self._stats.run_id,
             stepsSucceeded=self._stats.steps_succeeded,
             stepsFailed=self._stats.steps_failed,
             materializations=self._stats.materializations,
             expectations=self._stats.expectations,
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dagster._check as check
 import graphene
-from dagster._core.host_representation import RepresentedPipeline
+from dagster._core.host_representation import RepresentedJob
 
 from ..errors import (
     GraphenePipelineNotFoundError,
     GraphenePipelineSnapshotNotFoundError,
     GraphenePythonError,
 )
 from ..solids import GrapheneSolidContainer
@@ -13,22 +13,22 @@
 
 
 class GraphenePipelineSnapshot(GrapheneIPipelineSnapshotMixin, graphene.ObjectType):
     class Meta:
         interfaces = (GrapheneSolidContainer, GrapheneIPipelineSnapshot, GraphenePipelineReference)
         name = "PipelineSnapshot"
 
-    def __init__(self, represented_pipeline):
+    def __init__(self, represented_job: RepresentedJob):
         super().__init__()
-        self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+        self._represented_job = check.inst_param(
+            represented_job, "represented_pipeline", RepresentedJob
         )
 
-    def get_represented_pipeline(self):
-        return self._represented_pipeline
+    def get_represented_job(self) -> RepresentedJob:
+        return self._represented_job
 
 
 class GraphenePipelineSnapshotOrError(graphene.Union):
     class Meta:
         types = (
             GraphenePipelineNotFoundError,
             GraphenePipelineSnapshot,
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/resources.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/roots/mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 
 from ...implementation.execution import (
     delete_pipeline_run,
     terminate_pipeline_execution,
     wipe_assets,
 )
-from ...implementation.external import fetch_workspace, get_full_external_pipeline_or_raise
+from ...implementation.external import fetch_workspace, get_full_external_job_or_raise
 from ...implementation.telemetry import log_dagit_telemetry_event
 from ...implementation.utils import (
     ExecutionMetadata,
     ExecutionParams,
     UserFacingGraphQLError,
     assert_permission_for_location,
     capture_error,
@@ -97,15 +97,15 @@
         if selector.solid_selection:
             raise UserFacingGraphQLError(
                 GrapheneConflictingExecutionParamsError(
                     conflicting_param="selector.solid_selection"
                 )
             )
 
-        external_pipeline = get_full_external_pipeline_or_raise(
+        external_pipeline = get_full_external_job_or_raise(
             graphene_info,
             selector,
         )
 
         if not external_pipeline.has_preset(preset_name):
             raise UserFacingGraphQLError(
                 GraphenePresetNotFoundError(preset=preset_name, selector=selector)
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/roots/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 from ...implementation.fetch_backfills import get_backfill, get_backfills
 from ...implementation.fetch_instigators import (
     get_instigator_state_or_error,
     get_unloadable_instigator_states_or_error,
 )
 from ...implementation.fetch_partition_sets import get_partition_set, get_partition_sets_or_error
 from ...implementation.fetch_pipelines import (
-    get_pipeline_or_error,
-    get_pipeline_snapshot_or_error_from_pipeline_selector,
-    get_pipeline_snapshot_or_error_from_snapshot_id,
+    get_job_or_error,
+    get_job_snapshot_or_error_from_job_selector,
+    get_job_snapshot_or_error_from_snapshot_id,
 )
 from ...implementation.fetch_resources import (
     get_resource_or_error,
     get_top_level_resources_or_error,
 )
 from ...implementation.fetch_runs import (
     get_execution_plan,
@@ -497,19 +497,17 @@
         check.invariant(
             not (snapshotId and activePipelineSelector),
             "Must only pass one of snapshotId or activePipelineSelector",
         )
 
         if activePipelineSelector:
             pipeline_selector = pipeline_selector_from_graphql(activePipelineSelector)
-            return get_pipeline_snapshot_or_error_from_pipeline_selector(
-                graphene_info, pipeline_selector
-            )
+            return get_job_snapshot_or_error_from_job_selector(graphene_info, pipeline_selector)
         elif snapshotId:
-            return get_pipeline_snapshot_or_error_from_snapshot_id(graphene_info, snapshotId)
+            return get_job_snapshot_or_error_from_snapshot_id(graphene_info, snapshotId)
         else:
             check.failed(
                 "Must set one of snapshotId or activePipelineSelector",
             )
 
     def resolve_graphOrError(
         self, graphene_info: ResolveInfo, selector: Optional[GrapheneGraphSelector] = None
@@ -600,15 +598,15 @@
     def resolve_unloadableInstigationStatesOrError(
         self, graphene_info: ResolveInfo, instigationType: Optional[GrapheneInstigationType] = None
     ):
         instigation_type = InstigatorType(instigationType) if instigationType else None
         return get_unloadable_instigator_states_or_error(graphene_info, instigation_type)
 
     def resolve_pipelineOrError(self, graphene_info: ResolveInfo, params: GraphenePipelineSelector):
-        return get_pipeline_or_error(
+        return get_job_or_error(
             graphene_info,
             pipeline_selector_from_graphql(params),
         )
 
     def resolve_pipelineRunsOrError(
         self,
         _graphene_info: ResolveInfo,
@@ -773,19 +771,19 @@
                     for asset_node in external_asset_nodes
                     if asset_node.group_name == group_name
                 ]
                 if external_asset_nodes
                 else []
             )
         elif pipeline is not None:
-            pipeline_name = pipeline.pipelineName
+            job_name = pipeline.pipelineName
             repo_sel = RepositorySelector.from_graphql_input(pipeline)
             repo_loc = graphene_info.context.get_code_location(repo_sel.location_name)
             repo = repo_loc.get_repository(repo_sel.repository_name)
-            external_asset_nodes = repo.get_external_asset_nodes(pipeline_name)
+            external_asset_nodes = repo.get_external_asset_nodes(job_name)
             results = (
                 [
                     GrapheneAssetNode(
                         repo_loc,
                         repo,
                         asset_node,
                         dynamic_partitions_loader=dynamic_partitions_loader,
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/run_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Optional
 
 import dagster._check as check
 import graphene
-from dagster._core.host_representation import RepresentedPipeline
+from dagster._core.host_representation import RepresentedJob
+from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 
 from ..implementation.run_config_schema import resolve_is_run_config_valid
 from .config_types import GrapheneConfigType, to_config_type
 from .errors import (
     GrapheneInvalidSubsetError,
     GrapheneModeNotFoundError,
     GraphenePipelineNotFoundError,
@@ -46,48 +47,46 @@
         description = """The run config schema represents the all the config type
         information given a certain execution selection and mode of execution of that
         selection. All config interactions (e.g. checking config validity, fetching
         all config types, fetching in a particular config type) should be done
         through this type """
         name = "RunConfigSchema"
 
-    def __init__(self, represented_pipeline, mode):
+    def __init__(self, represented_job: RepresentedJob, mode: str):
         super().__init__()
-        self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
-        )
+        self._represented_job = check.inst_param(represented_job, "represented_job", RepresentedJob)
         self._mode = check.str_param(mode, "mode")
 
     def resolve_allConfigTypes(self, _graphene_info: ResolveInfo):
         return sorted(
             list(
                 map(
-                    lambda key: to_config_type(
-                        self._represented_pipeline.config_schema_snapshot, key
-                    ),
-                    self._represented_pipeline.config_schema_snapshot.all_config_keys,
+                    lambda key: to_config_type(self._represented_job.config_schema_snapshot, key),
+                    self._represented_job.config_schema_snapshot.all_config_keys,
                 )
             ),
             key=lambda ct: ct.key,
         )
 
     def resolve_rootConfigType(self, _graphene_info: ResolveInfo):
         return to_config_type(
-            self._represented_pipeline.config_schema_snapshot,
-            self._represented_pipeline.get_mode_def_snap(self._mode).root_config_key,
+            self._represented_job.config_schema_snapshot,
+            self._represented_job.get_mode_def_snap(  # type: ignore  # (possible none)
+                self._mode or DEFAULT_MODE_NAME
+            ).root_config_key,
         )
 
     def resolve_isRunConfigValid(
         self,
         graphene_info: ResolveInfo,
         runConfigData: Optional[Any] = None,  # custom scalar (GrapheneRunConfigData)
     ):
         return resolve_is_run_config_valid(
             graphene_info,
-            self._represented_pipeline,
+            self._represented_job,
             self._mode,
             parse_run_config_input(runConfigData or {}, raise_on_error=False),  # type: ignore
         )
 
 
 class GrapheneRunConfigSchemaOrError(graphene.Union):
     class Meta:
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/runs.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/schedules/schedules.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self._schedule_state = self._external_schedule.get_current_instigator_state(schedule_state)
 
         super().__init__(
             name=external_schedule.name,
             cron_schedule=str(
                 external_schedule.cron_schedule
             ),  # can be sequence, coercing to str for now
-            pipeline_name=external_schedule.pipeline_name,
+            pipeline_name=external_schedule.job_name,
             solid_selection=external_schedule.solid_selection,
             mode=external_schedule.mode,
             execution_timezone=(
                 self._external_schedule.execution_timezone
                 if self._external_schedule.execution_timezone
                 else "UTC"
             ),
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/schedules/ticks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import graphene
 from dagster._core.scheduler.instigation import TickStatus
-from dagster._core.storage.pipeline_run import RunsFilter
+from dagster._core.storage.dagster_run import RunsFilter
 
 from ..errors import GraphenePythonError
 from ..instigation import GrapheneInstigationTickStatus
 
 
 class GrapheneScheduleTickSuccessData(graphene.ObjectType):
     run = graphene.Field("dagster_graphql.schema.pipelines.pipeline.GrapheneRun")
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,20 @@
     pipelineName = graphene.NonNull(graphene.String)
     mode = graphene.NonNull(graphene.String)
     solidSelection = graphene.List(graphene.NonNull(graphene.String))
 
     class Meta:
         name = "Target"
 
-    def __init__(self, external_target):
+    def __init__(self, external_target: ExternalTargetData):
         self._external_target = check.inst_param(
             external_target, "external_target", ExternalTargetData
         )
         super().__init__(
-            pipelineName=external_target.pipeline_name,
+            pipelineName=external_target.job_name,
             mode=external_target.mode,
             solidSelection=external_target.solid_selection,
         )
 
 
 class GrapheneSensorMetadata(graphene.ObjectType):
     assetKeys = graphene.List(graphene.NonNull(GrapheneAssetKey))
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/solids.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/solids.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from functools import lru_cache
 from typing import TYPE_CHECKING, List, Mapping, Optional, Sequence, Union
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions import NodeHandle
-from dagster._core.host_representation import RepresentedPipeline
-from dagster._core.host_representation.external import ExternalPipeline
-from dagster._core.host_representation.historical import HistoricalPipeline
+from dagster._core.host_representation import RepresentedJob
+from dagster._core.host_representation.external import ExternalJob
+from dagster._core.host_representation.historical import HistoricalJob
 from dagster._core.snap import DependencyStructureIndex, GraphDefSnap, OpDefSnap
 from dagster._core.snap.node import InputMappingSnap, OutputMappingSnap
-from dagster._core.storage.pipeline_run import RunsFilter
+from dagster._core.storage.dagster_run import RunsFilter
 
 from dagster_graphql.implementation.events import iterate_metadata_entries
 from dagster_graphql.schema.logs.events import GrapheneRunStepStats
 from dagster_graphql.schema.metadata import GrapheneMetadataEntry
 
 from .config_types import GrapheneConfigTypeField
 from .dagster_types import GrapheneDagsterType, GrapheneDagsterTypeUnion, to_dagster_type
@@ -35,38 +35,36 @@
     description = graphene.String()
     type = graphene.NonNull(GrapheneDagsterType)
     metadata_entries = non_null_list(GrapheneMetadataEntry)
 
     class Meta:
         name = "InputDefinition"
 
-    def __init__(
-        self, represented_pipeline: RepresentedPipeline, solid_def_name: str, input_def_name: str
-    ):
-        self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+    def __init__(self, represented_job: RepresentedJob, solid_def_name: str, input_def_name: str):
+        self._represented_job = check.inst_param(
+            represented_job, "represented_pipeline", RepresentedJob
         )
         check.str_param(solid_def_name, "solid_def_name")
         check.str_param(input_def_name, "input_def_name")
-        solid_def_snap = self._represented_pipeline.get_node_def_snap(solid_def_name)
+        solid_def_snap = self._represented_job.get_node_def_snap(solid_def_name)
         self._input_def_snap = solid_def_snap.get_input_snap(input_def_name)
         super().__init__(
             name=self._input_def_snap.name,
             description=self._input_def_snap.description,
         )
 
     def resolve_type(self, _graphene_info: ResolveInfo) -> GrapheneDagsterTypeUnion:
         return to_dagster_type(
-            self._represented_pipeline.pipeline_snapshot, self._input_def_snap.dagster_type_key
+            self._represented_job.job_snapshot, self._input_def_snap.dagster_type_key
         )
 
     def resolve_solid_definition(
         self, _graphene_info: ResolveInfo
     ) -> Union["GrapheneSolidDefinition", "GrapheneCompositeSolidDefinition"]:
-        return build_solid_definition(self._represented_pipeline, self._solid_def_snap.name)
+        return build_solid_definition(self._represented_job, self._solid_def_snap.name)
 
     def resolve_metadata_entries(self, _graphene_info):
         return list(iterate_metadata_entries(self._input_def_snap.metadata))
 
 
 class GrapheneOutputDefinition(graphene.ObjectType):
     solid_definition = graphene.NonNull(lambda: GrapheneSolidDefinition)
@@ -77,21 +75,21 @@
     metadata_entries = non_null_list(GrapheneMetadataEntry)
 
     class Meta:
         name = "OutputDefinition"
 
     def __init__(
         self,
-        represented_pipeline: RepresentedPipeline,
+        represented_pipeline: RepresentedJob,
         solid_def_name: str,
         output_def_name: str,
         is_dynamic: bool,
     ):
         self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+            represented_pipeline, "represented_pipeline", RepresentedJob
         )
         check.str_param(solid_def_name, "solid_def_name")
         check.str_param(output_def_name, "output_def_name")
 
         self._solid_def_snap = represented_pipeline.get_node_def_snap(solid_def_name)
         self._output_def_snap = self._solid_def_snap.get_output_snap(output_def_name)
 
@@ -99,15 +97,15 @@
             name=self._output_def_snap.name,
             description=self._output_def_snap.description,
             is_dynamic=is_dynamic,
         )
 
     def resolve_type(self, _graphene_info) -> GrapheneDagsterTypeUnion:
         return to_dagster_type(
-            self._represented_pipeline.pipeline_snapshot,
+            self._represented_pipeline.job_snapshot,
             self._output_def_snap.dagster_type_key,
         )
 
     def resolve_solid_definition(
         self, _graphene_info
     ) -> Union["GrapheneSolidDefinition", "GrapheneCompositeSolidDefinition"]:
         return build_solid_definition(self._represented_pipeline, self._solid_def_snap.name)
@@ -123,21 +121,21 @@
     is_dynamic_collect = graphene.NonNull(graphene.Boolean)
 
     class Meta:
         name = "Input"
 
     def __init__(
         self,
-        represented_pipeline: RepresentedPipeline,
+        represented_pipeline: RepresentedJob,
         current_dep_structure: DependencyStructureIndex,
         solid_name: str,
         input_name: str,
     ):
         self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+            represented_pipeline, "represented_pipeline", RepresentedJob
         )
         self._current_dep_structure = check.inst_param(
             current_dep_structure, "current_dep_structure", DependencyStructureIndex
         )
         self._solid_name = check.str_param(solid_name, "solid_name")
         self._input_name = check.str_param(input_name, "input_name")
         self._solid_invocation_snap = current_dep_structure.get_invocation(solid_name)
@@ -183,15 +181,15 @@
     depended_by = non_null_list(GrapheneInput)
 
     class Meta:
         name = "Output"
 
     def __init__(self, represented_pipeline, current_dep_structure, solid_name, output_name):
         self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+            represented_pipeline, "represented_pipeline", RepresentedJob
         )
         self._current_dep_structure = check.inst_param(
             current_dep_structure, "current_dep_structure", DependencyStructureIndex
         )
         self._solid_name = check.str_param(solid_name, "solid_name")
         self._output_name = check.str_param(output_name, "output_name")
         self._solid_invocation_snap = current_dep_structure.get_invocation(solid_name)
@@ -239,15 +237,15 @@
         self,
         represented_pipeline,
         current_dep_index,
         solid_def_name,
         input_mapping_snap,
     ):
         self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+            represented_pipeline, "represented_pipeline", RepresentedJob
         )
         self._current_dep_index = check.inst_param(
             current_dep_index, "current_dep_index", DependencyStructureIndex
         )
         self._input_mapping_snap = check.inst_param(
             input_mapping_snap, "input_mapping_snap", InputMappingSnap
         )
@@ -277,15 +275,15 @@
     class Meta:
         name = "OutputMapping"
 
     def __init__(
         self, represented_pipeline, current_dep_index, solid_def_name, output_mapping_snap
     ):
         self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+            represented_pipeline, "represented_pipeline", RepresentedJob
         )
         self._current_dep_index = check.inst_param(
             current_dep_index, "current_dep_index", DependencyStructureIndex
         )
         self._output_mapping_snap = check.inst_param(
             output_mapping_snap, "output_mapping_snap", OutputMappingSnap
         )
@@ -321,30 +319,30 @@
 
     def __init__(self, resource_key):
         super().__init__()
         self.resource_key = resource_key
 
 
 def build_solids(represented_pipeline, current_dep_index):
-    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedPipeline)
+    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedJob)
     return sorted(
         [
             GrapheneSolid(represented_pipeline, solid_name, current_dep_index)
             for solid_name in current_dep_index.node_invocation_names
         ],
         key=lambda solid: solid.name,
     )
 
 
 def _build_solid_handles(
-    represented_pipeline: RepresentedPipeline,
+    represented_pipeline: RepresentedJob,
     current_dep_index: DependencyStructureIndex,
     parent: Optional["GrapheneSolidHandle"] = None,
 ) -> Sequence["GrapheneSolidHandle"]:
-    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedPipeline)
+    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedJob)
     check.opt_inst_param(parent, "parent", GrapheneSolidHandle)
     all_handle: List[GrapheneSolidHandle] = []
     for solid_invocation in current_dep_index.node_invocations:
         solid_name, solid_def_name = solid_invocation.node_name, solid_invocation.node_def_name
         handle = GrapheneSolidHandle(
             solid=GrapheneSolid(represented_pipeline, solid_name, current_dep_index),
             handle=NodeHandle(solid_name, parent.handleID if parent else None),
@@ -361,17 +359,17 @@
         all_handle.append(handle)
 
     return all_handle
 
 
 @lru_cache(maxsize=32)
 def build_solid_handles(
-    represented_pipeline: RepresentedPipeline,
+    represented_pipeline: RepresentedJob,
 ) -> Mapping[str, "GrapheneSolidHandle"]:
-    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedPipeline)
+    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedJob)
     return {
         str(item.handleID): item
         for item in _build_solid_handles(
             represented_pipeline, represented_pipeline.dep_structure_index
         )
     }
 
@@ -385,17 +383,17 @@
     asset_nodes = non_null_list("dagster_graphql.schema.asset_graph.GrapheneAssetNode")
 
     class Meta:
         name = "ISolidDefinition"
 
 
 class ISolidDefinitionMixin:
-    def __init__(self, represented_pipeline: RepresentedPipeline, solid_def_name: str):
+    def __init__(self, represented_pipeline: RepresentedJob, solid_def_name: str):
         self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+            represented_pipeline, "represented_pipeline", RepresentedJob
         )
         check.str_param(solid_def_name, "solid_def_name")
         self._solid_def_snap = represented_pipeline.get_node_def_snap(solid_def_name)
 
     def resolve_metadata(self, _graphene_info):
         return [
             GrapheneMetadataItemDefinition(key=item[0], value=item[1])
@@ -428,18 +426,18 @@
     def resolve_asset_nodes(self, graphene_info: ResolveInfo) -> Sequence["GrapheneAssetNode"]:
         # NOTE: This is a temporary hack. We really should prob be resolving solids against the repo
         # rather than pipeline, that way we would not have to refetch the repo here here in order to
         # access the asset nodes.
         from .asset_graph import GrapheneAssetNode
 
         # This is a workaround for the fact that asset info is not persisted in pipeline snapshots.
-        if isinstance(self._represented_pipeline, HistoricalPipeline):
+        if isinstance(self._represented_pipeline, HistoricalJob):
             return []
         else:
-            assert isinstance(self._represented_pipeline, ExternalPipeline)
+            assert isinstance(self._represented_pipeline, ExternalJob)
             repo_handle = self._represented_pipeline.repository_handle
             origin = repo_handle.code_location_origin
             location = graphene_info.context.get_code_location(origin.location_name)
             ext_repo = location.get_repository(repo_handle.repository_name)
             nodes = [
                 node
                 for node in ext_repo.get_external_asset_nodes()
@@ -452,16 +450,16 @@
     config_field = graphene.Field(GrapheneConfigTypeField)
     required_resources = non_null_list(GrapheneResourceRequirement)
 
     class Meta:
         interfaces = (GrapheneISolidDefinition,)
         name = "SolidDefinition"
 
-    def __init__(self, represented_pipeline: RepresentedPipeline, solid_def_name: str):
-        check.inst_param(represented_pipeline, "represented_pipeline", RepresentedPipeline)
+    def __init__(self, represented_pipeline: RepresentedJob, solid_def_name: str):
+        check.inst_param(represented_pipeline, "represented_pipeline", RepresentedJob)
         _solid_def_snap = represented_pipeline.get_node_def_snap(solid_def_name)
         if not isinstance(_solid_def_snap, OpDefSnap):
             check.failed("Expected SolidDefSnap")
         self._solid_def_snap = _solid_def_snap
         super().__init__(name=solid_def_name, description=self._solid_def_snap.description)
         ISolidDefinitionMixin.__init__(self, represented_pipeline, solid_def_name)
 
@@ -513,20 +511,20 @@
     is_dynamic_mapped = graphene.NonNull(graphene.Boolean)
 
     class Meta:
         name = "Solid"
 
     def __init__(
         self,
-        represented_pipeline: RepresentedPipeline,
+        represented_pipeline: RepresentedJob,
         solid_name: str,
         current_dep_structure: DependencyStructureIndex,
     ):
         self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+            represented_pipeline, "represented_pipeline", RepresentedJob
         )
 
         check.str_param(solid_name, "solid_name")
         self._current_dep_structure = check.inst_param(
             current_dep_structure, "current_dep_structure", DependencyStructureIndex
         )
         self._solid_invocation_snap = current_dep_structure.get_invocation(solid_name)
@@ -613,15 +611,15 @@
 
         if self._solid.get_is_composite():
             return GrapheneSolidStepStatsUnavailableError(
                 message="Step stats are not available for composite solids / subgraphs"
             )
 
         instance = _graphene_info.context.instance
-        runs_filter = RunsFilter(pipeline_name=self._solid.get_pipeline_name())
+        runs_filter = RunsFilter(job_name=self._solid.get_pipeline_name())
         runs = instance.get_runs(runs_filter, limit=limit)
         nodes = []
         for run in runs:
             stats = instance.get_run_step_stats(run.run_id, [str(self.handleID)])
             if len(stats):
                 nodes.append(GrapheneRunStepStats(stats[0]))
         return GrapheneSolidStepStatsConnection(nodes=nodes)
@@ -661,25 +659,27 @@
     )
     modes = non_null_list("dagster_graphql.schema.pipelines.mode.GrapheneMode")
 
     class Meta:
         interfaces = (GrapheneISolidDefinition, GrapheneSolidContainer)
         name = "CompositeSolidDefinition"
 
-    def __init__(self, represented_pipeline: RepresentedPipeline, solid_def_name: str):
+    def __init__(self, represented_pipeline: RepresentedJob, solid_def_name: str):
         self._represented_pipeline = check.inst_param(
-            represented_pipeline, "represented_pipeline", RepresentedPipeline
+            represented_pipeline, "represented_pipeline", RepresentedJob
         )
         self._solid_def_snap = represented_pipeline.get_node_def_snap(solid_def_name)
         self._comp_solid_dep_index = represented_pipeline.get_dep_structure_index(solid_def_name)
         super().__init__(name=solid_def_name, description=self._solid_def_snap.description)
         ISolidDefinitionMixin.__init__(self, represented_pipeline, solid_def_name)
 
     def resolve_id(self, _graphene_info: ResolveInfo) -> str:
-        return f"{self._represented_pipeline.identifying_pipeline_snapshot_id}:{self._solid_def_snap.name}"
+        return (
+            f"{self._represented_pipeline.identifying_job_snapshot_id}:{self._solid_def_snap.name}"
+        )
 
     def resolve_solids(self, _graphene_info: ResolveInfo) -> Sequence[GrapheneSolid]:
         return build_solids(self._represented_pipeline, self._comp_solid_dep_index)
 
     def resolve_output_mappings(
         self, _graphene_info: ResolveInfo
     ) -> Sequence[GrapheneOutputMapping]:
@@ -730,17 +730,17 @@
     def resolve_modes(self, _graphene_info):
         # returns empty list... composite solids don't have modes, this is a vestige of the old
         # pipeline explorer, which expected all solid containers to be pipelines
         return []
 
 
 def build_solid_definition(
-    represented_pipeline: RepresentedPipeline, solid_def_name: str
+    represented_pipeline: RepresentedJob, solid_def_name: str
 ) -> Union[GrapheneSolidDefinition, GrapheneCompositeSolidDefinition]:
-    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedPipeline)
+    check.inst_param(represented_pipeline, "represented_pipeline", RepresentedJob)
     check.str_param(solid_def_name, "solid_def_name")
 
     solid_def_snap = represented_pipeline.get_node_def_snap(solid_def_name)
 
     if isinstance(solid_def_snap, OpDefSnap):
         return GrapheneSolidDefinition(represented_pipeline, solid_def_snap.name)
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/table.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/tags.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/schema/util.py` & `dagster-graphql-1.3.3/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql/test/utils.py` & `dagster-graphql-1.3.3/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.3.3/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.2
+Version: 1.3.3
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.2/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.3.3/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.2/setup.py` & `dagster-graphql-1.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.3.2",
+        "dagster==1.3.3",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
+        "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

